# Getting started

TODO: Add a description

## How to Build


You must have Python 2 >=2.7.9 or Python 3 >=3.4 installed on your system to install and run this SDK. This SDK package depends on other Python packages like nose, jsonpickle etc. 
These dependencies are defined in the ```requirements.txt``` file that comes with the SDK.
To resolve these dependencies, you can use the PIP Dependency manager. Install it by following steps at [https://pip.pypa.io/en/stable/installing/](https://pip.pypa.io/en/stable/installing/).

Python and PIP executables should be defined in your PATH. Open command prompt and type ```pip --version```.
This should display the version of the PIP Dependency Manager installed if your installation was successful and the paths are properly defined.

* Using command line, navigate to the directory containing the generated files (including ```requirements.txt```) for the SDK.
* Run the command ```pip install -r requirements.txt```. This should install all the required dependencies.

![Building SDK - Step 1](https://apidocs.io/illustration/python?step=installDependencies&workspaceFolder=ClickSend%20REST%20API%20v3-Python)


## How to Use

The following section explains how to use the Clicksendrestapiv3 SDK package in a new project.

### 1. Open Project in an IDE

Open up a Python IDE like PyCharm. The basic workflow presented here is also applicable if you prefer using a different editor or IDE.

![Open project in PyCharm - Step 1](https://apidocs.io/illustration/python?step=pyCharm)

Click on ```Open``` in PyCharm to browse to your generated SDK directory and then click ```OK```.

![Open project in PyCharm - Step 2](https://apidocs.io/illustration/python?step=openProject0&workspaceFolder=ClickSend%20REST%20API%20v3-Python)     

The project files will be displayed in the side bar as follows:

![Open project in PyCharm - Step 3](https://apidocs.io/illustration/python?step=openProject1&workspaceFolder=ClickSend%20REST%20API%20v3-Python&projectName=clicksendrestapiv3)     

### 2. Add a new Test Project

Create a new directory by right clicking on the solution name as shown below:

![Add a new project in PyCharm - Step 1](https://apidocs.io/illustration/python?step=createDirectory&workspaceFolder=ClickSend%20REST%20API%20v3-Python&projectName=clicksendrestapiv3)

Name the directory as "test"

![Add a new project in PyCharm - Step 2](https://apidocs.io/illustration/python?step=nameDirectory)
   
Add a python file to this project with the name "testsdk"

![Add a new project in PyCharm - Step 3](https://apidocs.io/illustration/python?step=createFile&workspaceFolder=ClickSend%20REST%20API%20v3-Python&projectName=clicksendrestapiv3)

Name it "testsdk"

![Add a new project in PyCharm - Step 4](https://apidocs.io/illustration/python?step=nameFile)

In your python file you will be required to import the generated python library using the following code lines

```Python
from clicksendrestapiv3.clicksendrestapiv_3_client.py import *
```

![Add a new project in PyCharm - Step 4](https://apidocs.io/illustration/python?step=projectFiles&workspaceFolder=ClickSend%20REST%20API%20v3-Python&libraryName=clicksendrestapiv3.clicksendrestapiv_3_client.py&projectName=clicksendrestapiv3)

After this you can write code to instantiate an API client object, get a controller object and  make API calls. Sample code is given in the subsequent sections.

### 3. Run the Test Project

To run the file within your test project, right click on your Python file inside your Test project and click on ```Run```

![Run Test Project - Step 1](https://apidocs.io/illustration/python?step=runProject&workspaceFolder=ClickSend%20REST%20API%20v3-Python&libraryName=clicksendrestapiv3.clicksendrestapiv_3_client.py&projectName=clicksendrestapiv3)


## How to Test

You can test the generated SDK and the server with automatically generated test
cases. unittest is used as the testing framework and nose is used as the test
runner. You can run the tests as follows:

  1. From terminal/cmd navigate to the root directory of the SDK.
  2. Invoke 'pip install -r test-requirements.txt'
  3. Invoke 'nosetests'

## Initialization

### Authentication
In order to setup authentication and initialization of the API client, you need the following information.

| Parameter | Description |
|-----------|-------------|
| basic_auth_user_name | The username to use with basic authentication |
| basic_auth_password | The password to use with basic authentication |



API client can be initialized as following.

```python
# Configuration parameters and credentials
basic_auth_user_name = "basic_auth_user_name" # The username to use with basic authentication
basic_auth_password = "basic_auth_password" # The password to use with basic authentication

client = Clicksendrestapiv3Client(basic_auth_user_name, basic_auth_password)
```

# Class Reference

## <a name="list_of_controllers"></a>List of Controllers

* [AccountController](#account_controller)
* [AccountRechargeController](#account_recharge_controller)
* [AutomationRulesController](#automation_rules_controller)
* [ContactListsController](#contact_lists_controller)
* [ContactSuggestionsController](#contact_suggestions_controller)
* [ContactsController](#contacts_controller)
* [CountriesController](#countries_controller)
* [DeliveryIssuesController](#delivery_issues_controller)
* [EmailMarketingController](#email_marketing_controller)
* [EmailToSMSAllowedAddressController](#email_to_sms_allowed_address_controller)
* [EmailToSMSStrippedStringsController](#email_to_sms_stripped_strings_controller)
* [FaxController](#fax_controller)
* [ForgotAccountController](#forgot_account_controller)
* [MMSController](#mms_controller)
* [NumbersController](#numbers_controller)
* [PricingController](#pricing_controller)
* [PostDirectMailController](#post_direct_mail_controller)
* [PostLetterController](#post_letter_controller)
* [PostcardsController](#postcards_controller)
* [ReferralAccountsController](#referral_accounts_controller)
* [ResellerController](#reseller_controller)
* [ResellerAccountsController](#reseller_accounts_controller)
* [SDKController](#sdk_controller)
* [SearchController](#search_controller)
* [SMSController](#sms_controller)
* [SMSCampaignsController](#sms_campaigns_controller)
* [SMSTemplatesController](#sms_templates_controller)
* [StatisticsController](#statistics_controller)
* [SubaccountsController](#subaccounts_controller)
* [TimezonesController](#timezones_controller)
* [TransactionalEmailController](#transactional_email_controller)
* [UploadsController](#uploads_controller)
* [VoiceController](#voice_controller)

## <a name="account_controller"></a>![Class: ](https://apidocs.io/img/class.png ".AccountController") AccountController

### Get controller instance

An instance of the ``` AccountController ``` class can be accessed from the API Client.

```python
 account_client = client.account
```

### <a name="create_a_new_account"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.create_a_new_account") create_a_new_account

> **Note:** *Authentication isn't required to create a new account.*

```python
def create_a_new_account(self,
                             body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "    {        \"username\":\"johndoe1\",        \"user_email\":\"johndoe1@awesome.com\",        \"user_phone\":\"518-481-1001\",        \"user_first_name\":\"John\",        \"user_last_name\":\"Doe\",        \"country\":\"US\",        \"password\":\"pass\",        \"account_name\":\"The Awesome Company\"    }"
body = json.loads(body_value)

result = account_client.create_a_new_account(body)

```


### <a name="update_account"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.update_account") update_account

> TODO: Add a method description

```python
def update_account(self,
                       body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "    {        \"username\":\"johndoe\",        \"user_email\":\"johndoe@awesome.com\",        \"user_phone\":\"518-481-1002\",        \"user_first_name\":\"John\",        \"user_last_name\":\"Doe\",        \"country\":\"AU\",        \"password\":\"pass\",        \"account_name\":\"The Awesome Company\",        \"timezone\": \"Australia/Melbourne\",        \"private_uploads\": 1,        \"setting_sms_hide_your_number\": 0,        \"setting_sms_hide_business_name\": 1    }"
body = json.loads(body_value)

result = account_client.update_account(body)

```


### <a name="get_account"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.get_account") get_account

> TODO: Add a method description

```python
def get_account(self)
```

#### Example Usage

```python

result = account_client.get_account()

```


### <a name="get_account_usage"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.get_account_usage") get_account_usage

> TODO: Add a method description

```python
def get_account_usage(self,
                          year,
                          month,
                          mtype)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| year |  ``` Required ```  | Your account usage year. |
| month |  ``` Required ```  | Your account usage month. |
| mtype |  ``` Required ```  | The account type. Value can only be either email or subaccount. |



#### Example Usage

```python
year = 2016
month = 4
mtype = 'subaccount'

result = account_client.get_account_usage(year, month, mtype)

```


### <a name="update_send_account_activation_token"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.update_send_account_activation_token") update_send_account_activation_token

> TODO: Add a method description

```python
def update_send_account_activation_token(self,
                                             body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "    {        \"user_phone\":\"352-394-4199\",        \"type\":\"sms\",        \"country\": \"US\"    }"
body = json.loads(body_value)

result = account_client.update_send_account_activation_token(body)

```


### <a name="update_verify_new_account"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.update_verify_new_account") update_verify_new_account

> TODO: Add a method description

```python
def update_verify_new_account(self,
                                  activation_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| activationToken |  ``` Required ```  | The ActivationToken to be used to verify an account. |



#### Example Usage

```python
activation_token = '1827364'

result = account_client.update_verify_new_account(activation_token)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="account_recharge_controller"></a>![Class: ](https://apidocs.io/img/class.png ".AccountRechargeController") AccountRechargeController

### Get controller instance

An instance of the ``` AccountRechargeController ``` class can be accessed from the API Client.

```python
 account_recharge_client = client.account_recharge
```

### <a name="get_credit_card_info"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.get_credit_card_info") get_credit_card_info

> TODO: Add a method description

```python
def get_credit_card_info(self)
```

#### Example Usage

```python

result = account_recharge_client.get_credit_card_info()

```


### <a name="update_credit_card_info"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.update_credit_card_info") update_credit_card_info

> TODO: Add a method description

```python
def update_credit_card_info(self,
                                body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = UpdateCreditCardInfoRequest()

result = account_recharge_client.update_credit_card_info(body)

```


### <a name="list_of_packages"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.list_of_packages") list_of_packages

> TODO: Add a method description

```python
def list_of_packages(self,
                         country=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Optional ```  | Your country. |



#### Example Usage

```python
country = '"AU"'

result = account_recharge_client.list_of_packages(country)

```


### <a name="update_purchase_a_package"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.update_purchase_a_package") update_purchase_a_package

> TODO: Add a method description

```python
def update_purchase_a_package(self,
                                  package_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| packageId |  ``` Required ```  | Your package id. |



#### Example Usage

```python
package_id = 1

result = account_recharge_client.update_purchase_a_package(package_id)

```


### <a name="get_transactions"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.get_transactions") get_transactions

> TODO: Add a method description

```python
def get_transactions(self)
```

#### Example Usage

```python

result = account_recharge_client.get_transactions()

```


### <a name="get_a_specific_transaction"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.get_a_specific_transaction") get_a_specific_transaction

> TODO: Add a method description

```python
def get_a_specific_transaction(self,
                                   transaction_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| transactionId |  ``` Required ```  | 1c65-47fa-aea2-3ded9ed57557 (number, required) - Your transction id. |



#### Example Usage

```python
transaction_id = 'transaction_id'

result = account_recharge_client.get_a_specific_transaction(transaction_id)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="automation_rules_controller"></a>![Class: ](https://apidocs.io/img/class.png ".AutomationRulesController") AutomationRulesController

### Get controller instance

An instance of the ``` AutomationRulesController ``` class can be accessed from the API Client.

```python
 automation_rules_client = client.automation_rules
```

### <a name="list_rules"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.list_rules") list_rules

> TODO: Add a method description

```python
def list_rules(self)
```

#### Example Usage

```python

result = automation_rules_client.list_rules()

```


### <a name="get_a_specific_rule"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.get_a_specific_rule") get_a_specific_rule

> TODO: Add a method description

```python
def get_a_specific_rule(self,
                            inbound_rule_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Inbound Rule ID. |



#### Example Usage

```python
inbound_rule_id = 1

result = automation_rules_client.get_a_specific_rule(inbound_rule_id)

```


### <a name="create_a_new_rule"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.create_a_new_rule") create_a_new_rule

> TODO: Add a method description

```python
def create_a_new_rule(self,
                          body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CreateANewRuleRequest()

result = automation_rules_client.create_a_new_rule(body)

```


### <a name="update_a_rule"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.update_a_rule") update_a_rule

> TODO: Add a method description

```python
def update_a_rule(self,
                      inbound_rule_id,
                      body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Inbound Rule ID. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
inbound_rule_id = 1
body_value = "{    \"dedicated_number\":\"+61298441484\",    \"rule_name\":\"My Rule\",    \"message_search_type\":3,    \"message_search_term\":\"My Search Term\",    \"action\":\"EMAIL_FIXED\",    \"action_address\":\"john@doe.com\",    \"enabled\":1}"
body = json.loads(body_value)

result = automation_rules_client.update_a_rule(inbound_rule_id, body)

```


### <a name="delete_a_rule"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.delete_a_rule") delete_a_rule

> TODO: Add a method description

```python
def delete_a_rule(self,
                      inbound_rule_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Inbound Rule ID. |



#### Example Usage

```python
inbound_rule_id = 1

result = automation_rules_client.delete_a_rule(inbound_rule_id)

```


### <a name="list_rules_1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.list_rules_1") list_rules_1

> TODO: Add a method description

```python
def list_rules_1(self)
```

#### Example Usage

```python

result = automation_rules_client.list_rules_1()

```


### <a name="get_a_specific_rule_1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.get_a_specific_rule_1") get_a_specific_rule_1

> TODO: Add a method description

```python
def get_a_specific_rule_1(self,
                              receipt_rule_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |



#### Example Usage

```python
receipt_rule_id = 2

result = automation_rules_client.get_a_specific_rule_1(receipt_rule_id)

```


### <a name="create_a_new_rule_1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.create_a_new_rule_1") create_a_new_rule_1

> TODO: Add a method description

```python
def create_a_new_rule_1(self,
                            body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "{    \"rule_name\": \"My Rule\",    \"match_type\": 3,    \"action\": \"EMAIL_FIXED\",    \"action_address\": \"john@doe.com\",    \"enabled\": 1}"
body = json.loads(body_value)

result = automation_rules_client.create_a_new_rule_1(body)

```


### <a name="update_a_rule_1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.update_a_rule_1") update_a_rule_1

> TODO: Add a method description

```python
def update_a_rule_1(self,
                        receipt_rule_id,
                        body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
receipt_rule_id = 7
body_value = "{    \"rule_name\": \"My Rule\",    \"match_type\": 3,    \"action\": \"EMAIL_FIXED\",    \"action_address\": \"john@doe.com\",    \"enabled\": 1}"
body = json.loads(body_value)

result = automation_rules_client.update_a_rule_1(receipt_rule_id, body)

```


### <a name="delete_a_rule_1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.delete_a_rule_1") delete_a_rule_1

> TODO: Add a method description

```python
def delete_a_rule_1(self,
                        receipt_rule_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |



#### Example Usage

```python
receipt_rule_id = 7

result = automation_rules_client.delete_a_rule_1(receipt_rule_id)

```


### <a name="list_rules_2"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.list_rules_2") list_rules_2

> TODO: Add a method description

```python
def list_rules_2(self)
```

#### Example Usage

```python

result = automation_rules_client.list_rules_2()

```


### <a name="get_a_specific_rule_11"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.get_a_specific_rule_11") get_a_specific_rule_11

> TODO: Add a method description

```python
def get_a_specific_rule_11(self,
                               receipt_rule_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |



#### Example Usage

```python
receipt_rule_id = 2

result = automation_rules_client.get_a_specific_rule_11(receipt_rule_id)

```


### <a name="create_a_new_rule_2"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.create_a_new_rule_2") create_a_new_rule_2

> TODO: Add a method description

```python
def create_a_new_rule_2(self,
                            body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "{    \"rule_name\":\"My Rule\",    \"match_type\":3,    \"action\":\"EMAIL_FIXED\",    \"action_address\":\"john@doe.com\",    \"enabled\":1}"
body = json.loads(body_value)

result = automation_rules_client.create_a_new_rule_2(body)

```


### <a name="update_a_rule_11"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.update_a_rule_11") update_a_rule_11

> TODO: Add a method description

```python
def update_a_rule_11(self,
                         receipt_rule_id,
                         body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
receipt_rule_id = 2
body_value = "{    \"rule_name\":\"My Rule\",    \"match_type\":3,    \"action\":\"EMAIL_FIXED\",    \"action_address\":\"john@doe.com\",    \"enabled\":1}"
body = json.loads(body_value)

result = automation_rules_client.update_a_rule_11(receipt_rule_id, body)

```


### <a name="delete_a_rule_11"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.delete_a_rule_11") delete_a_rule_11

> TODO: Add a method description

```python
def delete_a_rule_11(self,
                         receipt_rule_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |



#### Example Usage

```python
receipt_rule_id = 2

result = automation_rules_client.delete_a_rule_11(receipt_rule_id)

```


### <a name="list_rules_3"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.list_rules_3") list_rules_3

> TODO: Add a method description

```python
def list_rules_3(self)
```

#### Example Usage

```python

result = automation_rules_client.list_rules_3()

```


### <a name="get_a_specific_rule_111"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.get_a_specific_rule_111") get_a_specific_rule_111

> TODO: Add a method description

```python
def get_a_specific_rule_111(self,
                                inbound_rule_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Fax inbound rule id |



#### Example Usage

```python
inbound_rule_id = 14

result = automation_rules_client.get_a_specific_rule_111(inbound_rule_id)

```


### <a name="create_a_new_rule_3"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.create_a_new_rule_3") create_a_new_rule_3

> TODO: Add a method description

```python
def create_a_new_rule_3(self,
                            body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "    {        \"dedicated_number\":\"+61298441484\",        \"rule_name\":\"Rule Name\",        \"action\":\"EMAIL_FIXED\",        \"action_address\":\"email@domain.com\",        \"enabled\":1    }"
body = json.loads(body_value)

result = automation_rules_client.create_a_new_rule_3(body)

```


### <a name="update_a_rule_111"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.update_a_rule_111") update_a_rule_111

> TODO: Add a method description

```python
def update_a_rule_111(self,
                          inbound_rule_id,
                          body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Fax inbound rule id |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
inbound_rule_id = 14
body_value = "    {        \"dedicated_number\":\"+61298441484\",        \"rule_name\":\"Rule Name\",        \"action\":\"EMAIL_FIXED\",        \"action_address\":\"email@domain.com\",        \"enabled\":1    }"
body = json.loads(body_value)

result = automation_rules_client.update_a_rule_111(inbound_rule_id, body)

```


### <a name="delete_a_rule_111"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.delete_a_rule_111") delete_a_rule_111

> TODO: Add a method description

```python
def delete_a_rule_111(self,
                          inbound_rule_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Fax inbound rule id |



#### Example Usage

```python
inbound_rule_id = 14

result = automation_rules_client.delete_a_rule_111(inbound_rule_id)

```


### <a name="list_rules_4"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.list_rules_4") list_rules_4

> TODO: Add a method description

```python
def list_rules_4(self)
```

#### Example Usage

```python

result = automation_rules_client.list_rules_4()

```


### <a name="get_a_specific_rule_2"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.get_a_specific_rule_2") get_a_specific_rule_2

> TODO: Add a method description

```python
def get_a_specific_rule_2(self,
                              rule_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |



#### Example Usage

```python
rule_id = 4

result = automation_rules_client.get_a_specific_rule_2(rule_id)

```


### <a name="create_a_new_rule_4"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.create_a_new_rule_4") create_a_new_rule_4

> TODO: Add a method description

```python
def create_a_new_rule_4(self,
                            body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "    {        \"rule_name\":\"My Rule\",        \"match_type\":2,        \"action\":\"EMAIL_FIXED\",        \"action_address\":\"john@doe.com\",        \"enabled\":1    }"
body = json.loads(body_value)

result = automation_rules_client.create_a_new_rule_4(body)

```


### <a name="update_a_rule_2"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.update_a_rule_2") update_a_rule_2

> TODO: Add a method description

```python
def update_a_rule_2(self,
                        rule_id,
                        body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
rule_id = 4
body_value = "    {        \"rule_name\":\"My Rule\",        \"match_type\":1,        \"action\":\"EMAIL_FIXED\",        \"action_address\":\"john@doe.com\",        \"enabled\":1    }"
body = json.loads(body_value)

result = automation_rules_client.update_a_rule_2(rule_id, body)

```


### <a name="delete_a_rule_2"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.delete_a_rule_2") delete_a_rule_2

> TODO: Add a method description

```python
def delete_a_rule_2(self,
                        rule_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to delete. |



#### Example Usage

```python
rule_id = 106.478498017638

result = automation_rules_client.delete_a_rule_2(rule_id)

```


### <a name="list_rules_5"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.list_rules_5") list_rules_5

> TODO: Add a method description

```python
def list_rules_5(self)
```

#### Example Usage

```python

result = automation_rules_client.list_rules_5()

```


### <a name="get_a_specific_rule_12"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.get_a_specific_rule_12") get_a_specific_rule_12

> TODO: Add a method description

```python
def get_a_specific_rule_12(self,
                               rule_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |



#### Example Usage

```python
rule_id = 5

result = automation_rules_client.get_a_specific_rule_12(rule_id)

```


### <a name="create_a_new_rule_5"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.create_a_new_rule_5") create_a_new_rule_5

> TODO: Add a method description

```python
def create_a_new_rule_5(self,
                            body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "    {        \"rule_name\":\"My Rule\",        \"match_type\": 0,        \"action\":\"URL\",        \"action_address\":\"http://testurl.com\",        \"enabled\":1    }"
body = json.loads(body_value)

result = automation_rules_client.create_a_new_rule_5(body)

```


### <a name="update_a_rule_12"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.update_a_rule_12") update_a_rule_12

> TODO: Add a method description

```python
def update_a_rule_12(self,
                         rule_id,
                         body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
rule_id = 8
body_value = "    {        \"rule_name\":\"My Rule\",        \"match_type\": 0,        \"action\":\"URL\",        \"action_address\":\"http://testurl.com\",        \"enabled\":1    }"
body = json.loads(body_value)

result = automation_rules_client.update_a_rule_12(rule_id, body)

```


### <a name="delete_a_rule_12"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.delete_a_rule_12") delete_a_rule_12

> TODO: Add a method description

```python
def delete_a_rule_12(self,
                         rule_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to delete. |



#### Example Usage

```python
rule_id = 8

result = automation_rules_client.delete_a_rule_12(rule_id)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="contact_lists_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ContactListsController") ContactListsController

### Get controller instance

An instance of the ``` ContactListsController ``` class can be accessed from the API Client.

```python
 contact_lists_client = client.contact_lists
```

### <a name="get_all_contact_lists"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.get_all_contact_lists") get_all_contact_lists

> TODO: Add a method description

```python
def get_all_contact_lists(self)
```

#### Example Usage

```python

result = contact_lists_client.get_all_contact_lists()

```


### <a name="create_a_new_contact_list"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.create_a_new_contact_list") create_a_new_contact_list

> TODO: Add a method description

```python
def create_a_new_contact_list(self,
                                  body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "    {        \"list_name\":\"ListCT3QrVL4od\"    }"
body = json.loads(body_value)

result = contact_lists_client.create_a_new_contact_list(body)

```


### <a name="get_a_specific_contact_list"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.get_a_specific_contact_list") get_a_specific_contact_list

> TODO: Add a method description

```python
def get_a_specific_contact_list(self,
                                    list_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |



#### Example Usage

```python
list_id = 437

result = contact_lists_client.get_a_specific_contact_list(list_id)

```


### <a name="update_a_specific_contact_list"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.update_a_specific_contact_list") update_a_specific_contact_list

> TODO: Add a method description

```python
def update_a_specific_contact_list(self,
                                       list_id,
                                       body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
list_id = 439
body_value = "    {        \"list_name\":\"ListlPJf33ksjP\"    }"
body = json.loads(body_value)

result = contact_lists_client.update_a_specific_contact_list(list_id, body)

```


### <a name="delete_a_specific_contact_list"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.delete_a_specific_contact_list") delete_a_specific_contact_list

> TODO: Add a method description

```python
def delete_a_specific_contact_list(self,
                                       list_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |



#### Example Usage

```python
list_id = 442

result = contact_lists_client.delete_a_specific_contact_list(list_id)

```


### <a name="create_import_contacts_to_list"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.create_import_contacts_to_list") create_import_contacts_to_list

> TODO: Add a method description

```python
def create_import_contacts_to_list(self,
                                       list_id,
                                       body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
list_id = 437
body_value = "{    \"file_url\":\"http://yourdomain.com/5485EA6144/79E8/import.csv\",    \"field_order\":[        \"phone\",        \"first_name\",        \"last_name\",        \"custom1\",        \"custom2\",        \"custom3\",        \"custom4\",        \"fax_number\",        \"organization_name\",        \"email\",        \"address_line_1\",        \"address_line_2\",        \"address_city\",        \"address_state\",        \"address_postal_code\",        \"address_country\"    ]}"
body = json.loads(body_value)

result = contact_lists_client.create_import_contacts_to_list(list_id, body)

```


### <a name="update_remove_duplicate_contacts"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.update_remove_duplicate_contacts") update_remove_duplicate_contacts

> TODO: Add a method description

```python
def update_remove_duplicate_contacts(self,
                                         list_id,
                                         body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
list_id = 439
body_value = "{    \"fields\":[        \"phone_number\",        \"first_name\",        \"last_name\",        \"fax_number\",        \"address_country\"    ]}"
body = json.loads(body_value)

result = contact_lists_client.update_remove_duplicate_contacts(list_id, body)

```


### <a name="get_list_of_acceptable_import_fields"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.get_list_of_acceptable_import_fields") get_list_of_acceptable_import_fields

> TODO: Add a method description

```python
def get_list_of_acceptable_import_fields(self,
                                             list_id=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Optional ```  | TODO: Add a parameter description |



#### Example Usage

```python
list_id = 'list_id'

result = contact_lists_client.get_list_of_acceptable_import_fields(list_id)

```


### <a name="create_show_csv_import_file_preview"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.create_show_csv_import_file_preview") create_show_csv_import_file_preview

> Show first row of the csv import file.

```python
def create_show_csv_import_file_preview(self,
                                            list_id,
                                            body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
list_id = 439
body_value = "{    \"file_url\":\"http://yourdomain.com/5485EA6144/79E8/import.csv\"}"
body = json.loads(body_value)

result = contact_lists_client.create_show_csv_import_file_preview(list_id, body)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="contact_suggestions_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ContactSuggestionsController") ContactSuggestionsController

### Get controller instance

An instance of the ``` ContactSuggestionsController ``` class can be accessed from the API Client.

```python
 contact_suggestions_client = client.contact_suggestions
```

### <a name="list_contact_suggestions"></a>![Method: ](https://apidocs.io/img/method.png ".ContactSuggestionsController.list_contact_suggestions") list_contact_suggestions

> TODO: Add a method description

```python
def list_contact_suggestions(self)
```

#### Example Usage

```python

result = contact_suggestions_client.list_contact_suggestions()

```


[Back to List of Controllers](#list_of_controllers)

## <a name="contacts_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ContactsController") ContactsController

### Get controller instance

An instance of the ``` ContactsController ``` class can be accessed from the API Client.

```python
 contacts_client = client.contacts
```

### <a name="get_all_contacts_in_a_list"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.get_all_contacts_in_a_list") get_all_contacts_in_a_list

> TODO: Add a method description

```python
def get_all_contacts_in_a_list(self,
                                   list_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id where your contacts belong. |



#### Example Usage

```python
list_id = 428

result = contacts_client.get_all_contacts_in_a_list(list_id)

```


### <a name="create_a_new_contact"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.create_a_new_contact") create_a_new_contact

> TODO: Add a method description

```python
def create_a_new_contact(self,
                             list_id,
                             body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id where your contact be associated. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
list_id = 428
body_value = "    {        \"phone_number\":\"+16783270696\",        \"first_name\":\"Ellen\",        \"last_name\":\"Diaz\",        \"custom_1\":\"Custom 1\",        \"custom_2\":\"Custom 2\",        \"custom_3\":\"Custom 3\",        \"custom_4\":\"Custom 4\",        \"fax_number\":\"+16783270696\",        \"organization_name\":\"Awesome Organization\",        \"email\":\"ellen@diaz.com\",        \"address_line_1\":\"Block 2\",        \"address_line_2\":\"Cool Bldg.\",        \"address_city\":\"Nevada\",        \"address_state\":\"Las Vegas\",        \"address_postal_code\":\"36063\",        \"address_country\":\"US\"    }"
body = json.loads(body_value)

result = contacts_client.create_a_new_contact(list_id, body)

```


### <a name="get_a_specific_contact"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.get_a_specific_contact") get_a_specific_contact

> TODO: Add a method description

```python
def get_a_specific_contact(self,
                               list_id,
                               contact_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| contactId |  ``` Required ```  | Your contact id you want to access. |



#### Example Usage

```python
list_id = 428
contact_id = 552802

result = contacts_client.get_a_specific_contact(list_id, contact_id)

```


### <a name="update_a_specific_contact"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.update_a_specific_contact") update_a_specific_contact

> TODO: Add a method description

```python
def update_a_specific_contact(self,
                                  list_id,
                                  contact_id,
                                  body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| contactId |  ``` Required ```  | Your contact id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
list_id = 428
contact_id = 552802
body_value = "{        \"phone_number\":\"+16783275492\",        \"first_name\":\"Ellen\",        \"last_name\":\"Diaz\",        \"custom_1\":\"Custom S72oJ9Teba\",        \"custom_2\":\"Custom NvrRJrKWeq\",        \"custom_3\":\"Custom 2ws94p1Dop\",        \"custom_4\":\"Custom Ku0AaIS5xb\",        \"fax_number\":\"+16783276356\",        \"organization_name\":\"Awesome Organization\",        \"email\":\"ellen@diaz.com\",        \"address_line_1\":\"Block 6\",        \"address_line_2\":\"Cool Bldg.\",        \"address_city\":\"Nevada\",        \"address_state\":\"Las Vegas\",        \"address_postal_code\":\"36063\",        \"address_country\":\"US\"    }"
body = json.loads(body_value)

result = contacts_client.update_a_specific_contact(list_id, contact_id, body)

```


### <a name="delete_a_specific_contact"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.delete_a_specific_contact") delete_a_specific_contact

> TODO: Add a method description

```python
def delete_a_specific_contact(self,
                                  list_id,
                                  contact_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| contactId |  ``` Required ```  | Your contact id you want to access. |



#### Example Usage

```python
list_id = 428
contact_id = 552807

result = contacts_client.delete_a_specific_contact(list_id, contact_id)

```


### <a name="update_remove_opted_out_contacts"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.update_remove_opted_out_contacts") update_remove_opted_out_contacts

> TODO: Add a method description

```python
def update_remove_opted_out_contacts(self,
                                         list_id,
                                         opt_out_list_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id. |
| optOutListId |  ``` Required ```  | Your opt out list id. |



#### Example Usage

```python
list_id = 439
opt_out_list_id = 512

result = contacts_client.update_remove_opted_out_contacts(list_id, opt_out_list_id)

```


### <a name="update_transfer_a_contact"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.update_transfer_a_contact") update_transfer_a_contact

> Transfers a specific contact to another list.

```python
def update_transfer_a_contact(self,
                                  from_list_id,
                                  contact_id,
                                  to_list_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| fromListId |  ``` Required ```  | From list id. |
| contactId |  ``` Required ```  | Contact ID. |
| toListId |  ``` Required ```  | To list id. |



#### Example Usage

```python
from_list_id = 428
contact_id = 1
to_list_id = 429

result = contacts_client.update_transfer_a_contact(from_list_id, contact_id, to_list_id)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="countries_controller"></a>![Class: ](https://apidocs.io/img/class.png ".CountriesController") CountriesController

### Get controller instance

An instance of the ``` CountriesController ``` class can be accessed from the API Client.

```python
 countries_client = client.countries
```

### <a name="get_all_countries"></a>![Method: ](https://apidocs.io/img/method.png ".CountriesController.get_all_countries") get_all_countries

> TODO: Add a method description

```python
def get_all_countries(self)
```

#### Example Usage

```python

result = countries_client.get_all_countries()

```


[Back to List of Controllers](#list_of_controllers)

## <a name="delivery_issues_controller"></a>![Class: ](https://apidocs.io/img/class.png ".DeliveryIssuesController") DeliveryIssuesController

### Get controller instance

An instance of the ``` DeliveryIssuesController ``` class can be accessed from the API Client.

```python
 delivery_issues_client = client.delivery_issues
```

### <a name="get_delivery_issues"></a>![Method: ](https://apidocs.io/img/method.png ".DeliveryIssuesController.get_delivery_issues") get_delivery_issues

> TODO: Add a method description

```python
def get_delivery_issues(self)
```

#### Example Usage

```python

result = delivery_issues_client.get_delivery_issues()

```


### <a name="create_delivery_issue"></a>![Method: ](https://apidocs.io/img/method.png ".DeliveryIssuesController.create_delivery_issue") create_delivery_issue

> TODO: Add a method description

```python
def create_delivery_issue(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "{  \"message_id\": \"B388828B\",  \"type\": \"SMS\",  \"description\": \"This is a test\",  \"client_comments\": \"test\",  \"email_address: john_doe@user.com\": \"\",  \"Body\": \"\"}"
body = json.loads(body_value)

result = delivery_issues_client.create_delivery_issue(body)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="email_marketing_controller"></a>![Class: ](https://apidocs.io/img/class.png ".EmailMarketingController") EmailMarketingController

### Get controller instance

An instance of the ``` EmailMarketingController ``` class can be accessed from the API Client.

```python
 email_marketing_client = client.email_marketing
```

### <a name="get_all_allowed_email_addresses"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.get_all_allowed_email_addresses") get_all_allowed_email_addresses

> TODO: Add a method description

```python
def get_all_allowed_email_addresses(self)
```

#### Example Usage

```python

result = email_marketing_client.get_all_allowed_email_addresses()

```


### <a name="create_allowed_email_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.create_allowed_email_address") create_allowed_email_address

> TODO: Add a method description

```python
def create_allowed_email_address(self,
                                     body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "{  \"email_address\": \"johndoe1@user.com\",  \"Body\": \"\"}"
body = json.loads(body_value)

result = email_marketing_client.create_allowed_email_address(body)

```


### <a name="update_send_verification_token"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.update_send_verification_token") update_send_verification_token

> TODO: Add a method description

```python
def update_send_verification_token(self,
                                       email_address_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email addess id you want to access. |



#### Example Usage

```python
email_address_id = 156.250606682734

result = email_marketing_client.update_send_verification_token(email_address_id)

```


### <a name="update_verify_allowed_email_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.update_verify_allowed_email_address") update_verify_allowed_email_address

> TODO: Add a method description

```python
def update_verify_allowed_email_address(self,
                                            email_address_id,
                                            activation_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email address id you want to access. |
| activationToken |  ``` Required ```  | 6E8B-4FDB-99A7-7ED08DF97BCC (required, string) - Your activation token. |



#### Example Usage

```python
email_address_id = 5
activation_token = '3BD73304'

result = email_marketing_client.update_verify_allowed_email_address(email_address_id, activation_token)

```


### <a name="delete_allowed_email_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.delete_allowed_email_address") delete_allowed_email_address

> TODO: Add a method description

```python
def delete_allowed_email_address(self,
                                     email_address_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email address you want to access. |



#### Example Usage

```python
email_address_id = 156.250606682734

result = email_marketing_client.delete_allowed_email_address(email_address_id)

```


### <a name="get_specific_allowed_email_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.get_specific_allowed_email_address") get_specific_allowed_email_address

> TODO: Add a method description

```python
def get_specific_allowed_email_address(self,
                                           email_address_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email address you want to access. |



#### Example Usage

```python
email_address_id = 4

result = email_marketing_client.get_specific_allowed_email_address(email_address_id)

```


### <a name="get_all_email_campaigns"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.get_all_email_campaigns") get_all_email_campaigns

> TODO: Add a method description

```python
def get_all_email_campaigns(self)
```

#### Example Usage

```python

result = email_marketing_client.get_all_email_campaigns()

```


### <a name="get_specific_email_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.get_specific_email_campaign") get_specific_email_campaign

> TODO: Add a method description

```python
def get_specific_email_campaign(self,
                                    email_campaign_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailCampaignId |  ``` Required ```  | The email campaign id you want to access. |



#### Example Usage

```python
email_campaign_id = 1

result = email_marketing_client.get_specific_email_campaign(email_campaign_id)

```


### <a name="create_email_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.create_email_campaign") create_email_campaign

> TODO: Add a method description

```python
def create_email_campaign(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "{  \"name\" : \"John Doe\",  \"subject\" : \"Lorem Ipsum\",  \"from_email_address_id\" : 2,  \"from_name\" : \"From name\",  \"template_id\" : 31,  \"body\" : \"<p>This is a test</p>\",  \"list_id\" : 456}"
body = json.loads(body_value)

result = email_marketing_client.create_email_campaign(body)

```


### <a name="update_email_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.update_email_campaign") update_email_campaign

> TODO: Add a method description

```python
def update_email_campaign(self,
                              email_campaign_id,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailCampaignId |  ``` Required ```  | The email campaign id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
email_campaign_id = 1
body_value = "{  \"name\" : \"John Doe\",  \"subject\" : \"Lorem Ipsum\",  \"from_email_address_id\" : 2,  \"from_name\" : \"From name\",  \"template_id\" : 31,  \"body\" : \"<p>This is a test</p>\",  \"list_id\" : 456}"
body = json.loads(body_value)

result = email_marketing_client.update_email_campaign(email_campaign_id, body)

```


### <a name="update_cancel_email_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.update_cancel_email_campaign") update_cancel_email_campaign

> TODO: Add a method description

```python
def update_cancel_email_campaign(self,
                                     email_campaign_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailCampaignId |  ``` Required ```  | The email campaign id you want to cancel. |



#### Example Usage

```python
email_campaign_id = 1

result = email_marketing_client.update_cancel_email_campaign(email_campaign_id)

```


### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.create_calculate_price") create_calculate_price

> TODO: Add a method description

```python
def create_calculate_price(self,
                               body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "{  \"name\" : \"John Doe\",  \"subject\" : \"Lorem Ipsum\",  \"from_email_address_id\" : 2,  \"from_name\" : \"From name\",  \"template_id\" : 31,  \"body\" : \"<p>This is a test</p>\",  \"list_id\" : 456}"
body = json.loads(body_value)

result = email_marketing_client.create_calculate_price(body)

```


### <a name="get_specific_email_campaign_history"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.get_specific_email_campaign_history") get_specific_email_campaign_history

> TODO: Add a method description

```python
def get_specific_email_campaign_history(self,
                                            campaign_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| campaignId |  ``` Required ```  | The email campaign id you want to access. |



#### Example Usage

```python
campaign_id = 77

result = email_marketing_client.get_specific_email_campaign_history(campaign_id)

```


### <a name="get_all_email_templates"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.get_all_email_templates") get_all_email_templates

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.

```python
def get_all_email_templates(self)
```

#### Example Usage

```python

result = email_marketing_client.get_all_email_templates()

```


### <a name="get_specific_email_template"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.get_specific_email_template") get_specific_email_template

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.

```python
def get_specific_email_template(self,
                                    template_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | The email template id. |



#### Example Usage

```python
template_id = 291

result = email_marketing_client.get_specific_email_template(template_id)

```


### <a name="create_new_email_template_from_master_template"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.create_new_email_template_from_master_template") create_new_email_template_from_master_template

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.

```python
def create_new_email_template_from_master_template(self,
                                                       body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "{  \"template_name\": \"Minions\",  \"template_id_master\": 57}"
body = json.loads(body_value)

result = email_marketing_client.create_new_email_template_from_master_template(body)

```


### <a name="update_an_email_template"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.update_an_email_template") update_an_email_template

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.

```python
def update_an_email_template(self,
                                 template_id,
                                 body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | The id of the template to be updated. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
template_id = 291
body_value = "    {        \"template_name\":\"Minions\",        \"body\":\"This is a sample content: Sc0KNWgSMG for this template.\"    }"
body = json.loads(body_value)

result = email_marketing_client.update_an_email_template(template_id, body)

```


### <a name="delete_email_template"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.delete_email_template") delete_email_template

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.

```python
def delete_email_template(self,
                              template_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |



#### Example Usage

```python
template_id = 25

result = email_marketing_client.delete_email_template(template_id)

```


### <a name="get_all_master_email_templates"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.get_all_master_email_templates") get_all_master_email_templates

> Master templates are templates that you can clone to a User Email Template which lets you edit and save it.

```python
def get_all_master_email_templates(self)
```

#### Example Usage

```python

result = email_marketing_client.get_all_master_email_templates()

```


### <a name="get_specific_master_template"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.get_specific_master_template") get_specific_master_template

> Master templates are templates that you can clone to a User Email Template which lets you edit and save it.

```python
def get_specific_master_template(self,
                                     template_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |



#### Example Usage

```python
template_id = '25'

result = email_marketing_client.get_specific_master_template(template_id)

```


### <a name="get_all_master_template_categories"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.get_all_master_template_categories") get_all_master_template_categories

> TODO: Add a method description

```python
def get_all_master_template_categories(self)
```

#### Example Usage

```python

result = email_marketing_client.get_all_master_template_categories()

```


### <a name="get_specific_email_template_category"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.get_specific_email_template_category") get_specific_email_template_category

> TODO: Add a method description

```python
def get_specific_email_template_category(self,
                                             category_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| categoryId |  ``` Required ```  | Your category id. |



#### Example Usage

```python
category_id = '25'

result = email_marketing_client.get_specific_email_template_category(category_id)

```


### <a name="get_all_templates_for_category"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.get_all_templates_for_category") get_all_templates_for_category

> TODO: Add a method description

```python
def get_all_templates_for_category(self,
                                       category_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| categoryId |  ``` Required ```  | Your category id. |



#### Example Usage

```python
category_id = '1'

result = email_marketing_client.get_all_templates_for_category(category_id)

```


### <a name="upload_image_to_specific_template"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.upload_image_to_specific_template") upload_image_to_specific_template

> TODO: Add a method description

```python
def upload_image_to_specific_template(self,
                                          template_id,
                                          body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
template_id = '1'
body_value = "{    \"image\": \"image.png\",    \"url\" : \"http://www.downloadimg.from/here.png\"}"
body = json.loads(body_value)

result = email_marketing_client.upload_image_to_specific_template(template_id, body)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="email_to_sms_allowed_address_controller"></a>![Class: ](https://apidocs.io/img/class.png ".EmailToSMSAllowedAddressController") EmailToSMSAllowedAddressController

### Get controller instance

An instance of the ``` EmailToSMSAllowedAddressController ``` class can be accessed from the API Client.

```python
 email_to_sms_allowed_address_client = client.email_to_sms_allowed_address
```

### <a name="list_of_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSAllowedAddressController.list_of_email_to_sms_allowed_address") list_of_email_to_sms_allowed_address

> Get list of allowed email addresses.

```python
def list_of_email_to_sms_allowed_address(self)
```

#### Example Usage

```python

result = email_to_sms_allowed_address_client.list_of_email_to_sms_allowed_address()

```


### <a name="create_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSAllowedAddressController.create_email_to_sms_allowed_address") create_email_to_sms_allowed_address

> Create an allowed email address.

```python
def create_email_to_sms_allowed_address(self,
                                            body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "    {        \"email_address\":\"Cv3p0@gmail.com\",        \"from\":\"+17128845887\"    }"
body = json.loads(body_value)

result = email_to_sms_allowed_address_client.create_email_to_sms_allowed_address(body)

```


### <a name="get_specific_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSAllowedAddressController.get_specific_email_to_sms_allowed_address") get_specific_email_to_sms_allowed_address

> Get a specific allowed email address.

```python
def get_specific_email_to_sms_allowed_address(self,
                                                  email_address_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | Your email address id. |



#### Example Usage

```python
email_address_id = 113

result = email_to_sms_allowed_address_client.get_specific_email_to_sms_allowed_address(email_address_id)

```


### <a name="update_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSAllowedAddressController.update_email_to_sms_allowed_address") update_email_to_sms_allowed_address

> Update a specific allowed email address.

```python
def update_email_to_sms_allowed_address(self,
                                            email_address_id,
                                            body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | Your email address id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
email_address_id = 107
body_value = "    {        \"email_address\":\"pfvRZ@gmail.com\",        \"from\":\"+17128842283\"    }"
body = json.loads(body_value)

result = email_to_sms_allowed_address_client.update_email_to_sms_allowed_address(email_address_id, body)

```


### <a name="delete_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSAllowedAddressController.delete_email_to_sms_allowed_address") delete_email_to_sms_allowed_address

> Delete a specific allowed email address.

```python
def delete_email_to_sms_allowed_address(self,
                                            email_address_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | Your email address id. |



#### Example Usage

```python
email_address_id = 107

result = email_to_sms_allowed_address_client.delete_email_to_sms_allowed_address(email_address_id)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="email_to_sms_stripped_strings_controller"></a>![Class: ](https://apidocs.io/img/class.png ".EmailToSMSStrippedStringsController") EmailToSMSStrippedStringsController

### Get controller instance

An instance of the ``` EmailToSMSStrippedStringsController ``` class can be accessed from the API Client.

```python
 email_to_sms_stripped_strings_client = client.email_to_sms_stripped_strings
```

### <a name="list_stripped_strings"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSStrippedStringsController.list_stripped_strings") list_stripped_strings

> TODO: Add a method description

```python
def list_stripped_strings(self)
```

#### Example Usage

```python

result = email_to_sms_stripped_strings_client.list_stripped_strings()

```


### <a name="find_specific_stripped_string"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSStrippedStringsController.find_specific_stripped_string") find_specific_stripped_string

> TODO: Add a method description

```python
def find_specific_stripped_string(self,
                                      rule_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |



#### Example Usage

```python
rule_id = 18

result = email_to_sms_stripped_strings_client.find_specific_stripped_string(rule_id)

```


### <a name="create_stripped_string"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSStrippedStringsController.create_stripped_string") create_stripped_string

> TODO: Add a method description

```python
def create_stripped_string(self,
                               body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "{    \"strip_string\" : \"~~~test~~~\"}"
body = json.loads(body_value)

result = email_to_sms_stripped_strings_client.create_stripped_string(body)

```


### <a name="update_stripped_string"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSStrippedStringsController.update_stripped_string") update_stripped_string

> TODO: Add a method description

```python
def update_stripped_string(self,
                               rule_id,
                               body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
rule_id = 20
body_value = "{    \"strip_string\" : \"~~~test1~~~\"}"
body = json.loads(body_value)

result = email_to_sms_stripped_strings_client.update_stripped_string(rule_id, body)

```


### <a name="delete_stripped_string"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSStrippedStringsController.delete_stripped_string") delete_stripped_string

> TODO: Add a method description

```python
def delete_stripped_string(self,
                               rule_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |



#### Example Usage

```python
rule_id = 20

result = email_to_sms_stripped_strings_client.delete_stripped_string(rule_id)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="fax_controller"></a>![Class: ](https://apidocs.io/img/class.png ".FaxController") FaxController

### Get controller instance

An instance of the ``` FaxController ``` class can be accessed from the API Client.

```python
 fax_client = client.fax
```

### <a name="create_send_fax"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.create_send_fax") create_send_fax

> **Letter File Options**
> **Use existing URL**
> With this option, you can use an existing URL to a PDF document. For example, you might generate the pdf on your server.
> **Upload File to Our Server**
> With this option, you can use the `/uploads` endpoint to upload the document. The `/uploads` endpoint returns a URL that can be used in the `/fax/send` endpoint.

```python
def create_send_fax(self,
                        body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = SendFaxRequest()

result = fax_client.create_send_fax(body)

```


### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.create_calculate_price") create_calculate_price

> TODO: Add a method description

```python
def create_calculate_price(self,
                               body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CalculatePriceRequest132()

result = fax_client.create_calculate_price(body)

```


### <a name="get_fax_history"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.get_fax_history") get_fax_history

> Get a list of Fax History.

```python
def get_fax_history(self,
                        date_from=None,
                        date_to=None,
                        q=None,
                        order_by=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateFrom |  ``` Optional ```  | Customize result by setting from date (timestsamp) |
| dateTo |  ``` Optional ```  | Customize result by setting to date (timestamp) |
| q |  ``` Optional ```  | Custom query |
| orderBy |  ``` Optional ```  | Order result by |



#### Example Usage

```python
date_from = 1457572619
date_to = 1457573000
q = 'status:Sent,status_code:201'
order_by = 'subject:desc'

result = fax_client.get_fax_history(date_from, date_to, q, order_by)

```


### <a name="list_of_fax_delivery_receipts"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.list_of_fax_delivery_receipts") list_of_fax_delivery_receipts

> **Push Delivery Receipts**
> If you prefer, we can push message replies to your server as they arrive with us.
> 1. Log into your account.
> 2. Click on 'Fax' then 'Settings' tab.
> 3. Click on the 'Fax Delivery Report Settings' menu.
> 4. Select 'Forward to URL'.
> 5. Enter the URL and click 'Save'.
> The following variables will be posted to the URL specified:
> | Variable | Description |
> |---|---|
> | `timestamp_send` | Timestamp of the original send request in UNIX format. e.g 1439173980
> | `timestamp` | Timestamp of delivery report in UNIX format. e.g 1439173981
> | `message_id` | Message ID, returned when originally sending the message.
> | `status` | Delivered or Undelivered
> | `status_code` | Status code. Refer to 'Fax Delivery Status Codes' in docs.
> | `status_text` | Status text.
> | `error_code` | Error code.
> | `error_text` | Error text.
> | `custom_string` | A custom string used when sending the original message.
> | `user_id` | The user ID of the user who sent the message.
> | `subaccount_id` | The subaccount ID of the user who sent the message.
> | `message_type` | 'fax' (constant).
> **Pull Delivery Receipts**
> Receive delivery reports by polling.
> You can poll our server and retrieve delivery reports at a time that suits you.
> 1. Log into your account.
> 2. Click on 'Fax' then 'Settings' tab.
> 3. Click on the 'Fax Delivery Report Settings' menu.
> 4. Select 'Poll our server' and click 'Save'.

```python
def list_of_fax_delivery_receipts(self)
```

#### Example Usage

```python

result = fax_client.list_of_fax_delivery_receipts()

```


### <a name="get_a_specific_fax_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.get_a_specific_fax_delivery_receipt") get_a_specific_fax_delivery_receipt

> **Push Delivery Receipts**
> If you prefer, we can push message replies to your server as they arrive with us.
> 1. Log into your account.
> 2. Click on 'Fax' then 'Settings' tab.
> 3. Click on the 'Fax Delivery Report Settings' menu.
> 4. Select 'Forward to URL'.
> 5. Enter the URL and click 'Save'.
> The following variables will be posted to the URL specified:
> | Variable | Description |
> |---|---|
> | `timestamp_send` | Timestamp of the original send request in UNIX format. e.g 1439173980
> | `timestamp` | Timestamp of delivery report in UNIX format. e.g 1439173981
> | `message_id` | Message ID, returned when originally sending the message.
> | `status` | Delivered or Undelivered
> | `status_code` | Status code. Refer to 'Fax Delivery Status Codes' in docs.
> | `status_text` | Status text.
> | `error_code` | Error code.
> | `error_text` | Error text.
> | `custom_string` | A custom string used when sending the original message.
> | `user_id` | The user ID of the user who sent the message.
> | `subaccount_id` | The subaccount ID of the user who sent the message.
> | `message_type` | 'fax' (constant).
> **Pull Delivery Receipts**
> Receive delivery reports by polling.
> You can poll our server and retrieve delivery reports at a time that suits you.
> 1. Log into your account.
> 2. Click on 'Fax' then 'Settings' tab.
> 3. Click on the 'Fax Delivery Report Settings' menu.
> 4. Select 'Poll our server' and click 'Save'.

```python
def get_a_specific_fax_delivery_receipt(self,
                                            message_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | D2AF-479B-8955-6395D561DEF4" (required, number) - Message ID. |



#### Example Usage

```python
message_id = '"3FAC74F1'

result = fax_client.get_a_specific_fax_delivery_receipt(message_id)

```


### <a name="update_mark_fax_delivery_receipts_as_read"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.update_mark_fax_delivery_receipts_as_read") update_mark_fax_delivery_receipts_as_read

> **Push Delivery Receipts**
> If you prefer, we can push message replies to your server as they arrive with us.
> 1. Log into your account.
> 2. Click on 'Fax' then 'Settings' tab.
> 3. Click on the 'Fax Delivery Report Settings' menu.
> 4. Select 'Forward to URL'.
> 5. Enter the URL and click 'Save'.
> The following variables will be posted to the URL specified:
> | Variable | Description |
> |---|---|
> | `timestamp_send` | Timestamp of the original send request in UNIX format. e.g 1439173980
> | `timestamp` | Timestamp of delivery report in UNIX format. e.g 1439173981
> | `message_id` | Message ID, returned when originally sending the message.
> | `status` | Delivered or Undelivered
> | `status_code` | Status code. Refer to 'Fax Delivery Status Codes' in docs.
> | `status_text` | Status text.
> | `error_code` | Error code.
> | `error_text` | Error text.
> | `custom_string` | A custom string used when sending the original message.
> | `user_id` | The user ID of the user who sent the message.
> | `subaccount_id` | The subaccount ID of the user who sent the message.
> | `message_type` | 'fax' (constant).
> **Pull Delivery Receipts**
> Receive delivery reports by polling.
> You can poll our server and retrieve delivery reports at a time that suits you.
> 1. Log into your account.
> 2. Click on 'Fax' then 'Settings' tab.
> 3. Click on the 'Fax Delivery Report Settings' menu.
> 4. Select 'Poll our server' and click 'Save'.

```python
def update_mark_fax_delivery_receipts_as_read(self,
                                                  body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "{    \"date_before\": 1441958441}"
body = json.loads(body_value)

result = fax_client.update_mark_fax_delivery_receipts_as_read(body)

```


### <a name="add_a_test_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.add_a_test_delivery_receipt") add_a_test_delivery_receipt

> **Push Delivery Receipts**
> If you prefer, we can push message replies to your server as they arrive with us.
> 1. Log into your account.
> 2. Click on 'Fax' then 'Settings' tab.
> 3. Click on the 'Fax Delivery Report Settings' menu.
> 4. Select 'Forward to URL'.
> 5. Enter the URL and click 'Save'.
> The following variables will be posted to the URL specified:
> | Variable | Description |
> |---|---|
> | `timestamp_send` | Timestamp of the original send request in UNIX format. e.g 1439173980
> | `timestamp` | Timestamp of delivery report in UNIX format. e.g 1439173981
> | `message_id` | Message ID, returned when originally sending the message.
> | `status` | Delivered or Undelivered
> | `status_code` | Status code. Refer to 'Fax Delivery Status Codes' in docs.
> | `status_text` | Status text.
> | `error_code` | Error code.
> | `error_text` | Error text.
> | `custom_string` | A custom string used when sending the original message.
> | `user_id` | The user ID of the user who sent the message.
> | `subaccount_id` | The subaccount ID of the user who sent the message.
> | `message_type` | 'fax' (constant).
> **Pull Delivery Receipts**
> Receive delivery reports by polling.
> You can poll our server and retrieve delivery reports at a time that suits you.
> 1. Log into your account.
> 2. Click on 'Fax' then 'Settings' tab.
> 3. Click on the 'Fax Delivery Report Settings' menu.
> 4. Select 'Poll our server' and click 'Save'.

```python
def add_a_test_delivery_receipt(self,
                                    body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "    {        \"url\":\"http://yourUrl.com\"    }"
body = json.loads(body_value)

result = fax_client.add_a_test_delivery_receipt(body)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="forgot_account_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ForgotAccountController") ForgotAccountController

### Get controller instance

An instance of the ``` ForgotAccountController ``` class can be accessed from the API Client.

```python
 forgot_account_client = client.forgot_account
```

### <a name="update_forgot_username"></a>![Method: ](https://apidocs.io/img/method.png ".ForgotAccountController.update_forgot_username") update_forgot_username

> TODO: Add a method description

```python
def update_forgot_username(self,
                               body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = ForgotUsernameRequest()

result = forgot_account_client.update_forgot_username(body)

```


### <a name="update_forgot_password"></a>![Method: ](https://apidocs.io/img/method.png ".ForgotAccountController.update_forgot_password") update_forgot_password

> TODO: Add a method description

```python
def update_forgot_password(self,
                               body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "    {        \"username\": \"0F6pKiiuca\"    }"
body = json.loads(body_value)

result = forgot_account_client.update_forgot_password(body)

```


### <a name="update_verify_forgot_password"></a>![Method: ](https://apidocs.io/img/method.png ".ForgotAccountController.update_verify_forgot_password") update_verify_forgot_password

> TODO: Add a method description

```python
def update_verify_forgot_password(self,
                                      body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "    {        \"subaccount_id\": 54,        \"activation_token\": \"9C648BAD-EB7F-4E7E-96BC-B433140C4F1F\",        \"password\": \"0F6pKiiuca\"    }"
body = json.loads(body_value)

result = forgot_account_client.update_verify_forgot_password(body)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="mms_controller"></a>![Class: ](https://apidocs.io/img/class.png ".MMSController") MMSController

### Get controller instance

An instance of the ``` MMSController ``` class can be accessed from the API Client.

```python
 mms_client = client.mms
```

### <a name="create_send_mms"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.create_send_mms") create_send_mms

> TODO: Add a method description

```python
def create_send_mms(self,
                        body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = SendMMSRequest()

result = mms_client.create_send_mms(body)

```


### <a name="create_get_price"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.create_get_price") create_get_price

> TODO: Add a method description

```python
def create_get_price(self,
                         body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = GetPriceRequest()

result = mms_client.create_get_price(body)

```


### <a name="get_mms_history"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.get_mms_history") get_mms_history

> TODO: Add a method description

```python
def get_mms_history(self,
                        q=None,
                        order_by=None,
                        date_from=None,
                        date_to=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| q |  ``` Optional ```  | A custom query. |
| orderBy |  ``` Optional ```  | Sort records by. |
| dateFrom |  ``` Optional ```  | Timestamp (from) used to show records by date. |
| dateTo |  ``` Optional ```  | Timestamp (to) used to show records by date. |



#### Example Usage

```python
q = 'list_id:429,direction:out'
order_by = 'subject:desc'
date_from = 1443501617
date_to = 1443501727

result = mms_client.get_mms_history(q, order_by, date_from, date_to)

```


### <a name="get_export_mms_history"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.get_export_mms_history") get_export_mms_history

> TODO: Add a method description

```python
def get_export_mms_history(self,
                               filename)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | Your export filename. |



#### Example Usage

```python
filename = 'export.csv'

result = mms_client.get_export_mms_history(filename)

```


### <a name="update_cancel_mms"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.update_cancel_mms") update_cancel_mms

> TODO: Add a method description

```python
def update_cancel_mms(self,
                          message_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Message ID. |



#### Example Usage

```python
message_id = 'message_id'

result = mms_client.update_cancel_mms(message_id)

```


### <a name="update_cancel_all_mms"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.update_cancel_all_mms") update_cancel_all_mms

> TODO: Add a method description

```python
def update_cancel_all_mms(self)
```

#### Example Usage

```python

result = mms_client.update_cancel_all_mms()

```


### <a name="get_all_delivery_receipts"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.get_all_delivery_receipts") get_all_delivery_receipts

> TODO: Add a method description

```python
def get_all_delivery_receipts(self)
```

#### Example Usage

```python

result = mms_client.get_all_delivery_receipts()

```


### <a name="get_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.get_delivery_receipt") get_delivery_receipt

> TODO: Add a method description

```python
def get_delivery_receipt(self,
                             message_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Message ID. |



#### Example Usage

```python
message_id = '3E0DC217-7D0F-4C20-A3F2-E3362B938CAF'

result = mms_client.get_delivery_receipt(message_id)

```


### <a name="update_mark_receipts_as_read"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.update_mark_receipts_as_read") update_mark_receipts_as_read

> TODO: Add a method description

```python
def update_mark_receipts_as_read(self)
```

#### Example Usage

```python

result = mms_client.update_mark_receipts_as_read()

```


### <a name="get_all_inbound_sms_pull"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.get_all_inbound_sms_pull") get_all_inbound_sms_pull

> Inbound MMS shares the same rules/settings/endpoints as SMS. Any attachments will be converted to a URL.
> **Push Inbound SMS**
> If you prefer, we can push message replies to your server as they arrive with us.
> Refer to SMS->Inbound SMS in the docs.
> **Pull Inbound SMS**
> Receive SMS by polling your Inbox.
> Refer to SMS->Inbound SMS in the docs.

```python
def get_all_inbound_sms_pull(self)
```

#### Example Usage

```python

result = mms_client.get_all_inbound_sms_pull()

```


[Back to List of Controllers](#list_of_controllers)

## <a name="numbers_controller"></a>![Class: ](https://apidocs.io/img/class.png ".NumbersController") NumbersController

### Get controller instance

An instance of the ``` NumbersController ``` class can be accessed from the API Client.

```python
 numbers_client = client.numbers
```

### <a name="get_all_dedicated_numbers"></a>![Method: ](https://apidocs.io/img/method.png ".NumbersController.get_all_dedicated_numbers") get_all_dedicated_numbers

> TODO: Add a method description

```python
def get_all_dedicated_numbers(self)
```

#### Example Usage

```python

result = numbers_client.get_all_dedicated_numbers()

```


### <a name="create_buy_dedicated_number"></a>![Method: ](https://apidocs.io/img/method.png ".NumbersController.create_buy_dedicated_number") create_buy_dedicated_number

> TODO: Add a method description

```python
def create_buy_dedicated_number(self,
                                    dedicated_number)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dedicatedNumber |  ``` Required ```  | Your phone number in E.164 format. |



#### Example Usage

```python
dedicated_number = '+12282060576'

result = numbers_client.create_buy_dedicated_number(dedicated_number)

```


### <a name="search_dedicated_numbers_by_country"></a>![Method: ](https://apidocs.io/img/method.png ".NumbersController.search_dedicated_numbers_by_country") search_dedicated_numbers_by_country

> TODO: Add a method description

```python
def search_dedicated_numbers_by_country(self,
                                            country,
                                            search=None,
                                            search_type=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Required ```  | Your preferred country. |
| search |  ``` Optional ```  | Your search pattern or query. |
| searchType |  ``` Optional ```  | Your strategy for searching, 0 = starts with, 1 = anywhere, 2 = ends with. |



#### Example Usage

```python
country = 'US'
search = '88'
search_type = 1

result = numbers_client.search_dedicated_numbers_by_country(country, search, search_type)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="pricing_controller"></a>![Class: ](https://apidocs.io/img/class.png ".PricingController") PricingController

### Get controller instance

An instance of the ``` PricingController ``` class can be accessed from the API Client.

```python
 pricing_client = client.pricing
```

### <a name="get_country_pricing"></a>![Method: ](https://apidocs.io/img/method.png ".PricingController.get_country_pricing") get_country_pricing

> TODO: Add a method description

```python
def get_country_pricing(self,
                            country,
                            currency=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Required ```  | Two-letter representation of the country. |
| currency |  ``` Optional ```  | Three-letter representation of the currency. |



#### Example Usage

```python
country = 'AU'
currency = 'AUD'

result = pricing_client.get_country_pricing(country, currency)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="post_direct_mail_controller"></a>![Class: ](https://apidocs.io/img/class.png ".PostDirectMailController") PostDirectMailController

### Get controller instance

An instance of the ``` PostDirectMailController ``` class can be accessed from the API Client.

```python
 post_direct_mail_client = client.post_direct_mail
```

### <a name="search_locations"></a>![Method: ](https://apidocs.io/img/method.png ".PostDirectMailController.search_locations") search_locations

> TODO: Add a method description

```python
def search_locations(self,
                         country,
                         query)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Required ```  | Country code. |
| query |  ``` Required ```  | A postal code or place name. |



#### Example Usage

```python
country = 'AD'
query = 'AD100'

result = post_direct_mail_client.search_locations(country, query)

```


### <a name="create_new_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".PostDirectMailController.create_new_campaign") create_new_campaign

> Create new direct mail campaign.

```python
def create_new_campaign(self,
                            body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CreateNewCampaignRequest()

result = post_direct_mail_client.create_new_campaign(body)

```


### <a name="create_calculate_direct_mail_campaign_price"></a>![Method: ](https://apidocs.io/img/method.png ".PostDirectMailController.create_calculate_direct_mail_campaign_price") create_calculate_direct_mail_campaign_price

> Calculate direct mail campaign price.

```python
def create_calculate_direct_mail_campaign_price(self,
                                                    body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CalculateDirectMailCampaignPriceRequest()

result = post_direct_mail_client.create_calculate_direct_mail_campaign_price(body)

```


### <a name="list_direct_mail_campaigns"></a>![Method: ](https://apidocs.io/img/method.png ".PostDirectMailController.list_direct_mail_campaigns") list_direct_mail_campaigns

> Get list of direct mail campaigns.

```python
def list_direct_mail_campaigns(self)
```

#### Example Usage

```python

result = post_direct_mail_client.list_direct_mail_campaigns()

```


[Back to List of Controllers](#list_of_controllers)

## <a name="post_letter_controller"></a>![Class: ](https://apidocs.io/img/class.png ".PostLetterController") PostLetterController

### Get controller instance

An instance of the ``` PostLetterController ``` class can be accessed from the API Client.

```python
 post_letter_client = client.post_letter
```

### <a name="create_send_post_letter"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.create_send_post_letter") create_send_post_letter

> **Supported File Types**
> We support `pdf`, `docx` and `doc` files. Contact us to add support for any other file type. If you're using `docx` or `doc` files, you'll need to convert the file first using our uploads endpoint with the querystring parameter `convert=post` e.g. `POST /uploads?convert=post`. This will return a URL to the converted pdf file that can be used in the `/post/letters/send` endpoint.
> **Letter File Options**
> **Use existing URL**
> With this option, you can use an existing URL to a `pdf` document. For example, you might generate the `pdf` on your server.
> **Upload File to Our Server**
> With this option, you can use the `/uploads` endpoint to upload the document. The `/uploads` endpoint returns a URL that can be used in the `/post/letters/send` endpoint.

```python
def create_send_post_letter(self,
                                body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "{  \"file_url\": \"http://server.com/file.pdf\",  \"template_used\": 1,  \"colour\": 1,  \"duplex\": 0,  \"recipients\": [    {      \"address_name\": \"My Home Address\",      \"address_line_1\": \"Address 1\",      \"address_line_2\": \"Address 2\",      \"address_city\": \"CITY\",      \"address_state\": \"State\",      \"address_postal_code\": 123456,      \"address_country\": \"AU\",      \"return_address_id\": 1,      \"schedule\": 1449573604    }  ]}"
body = json.loads(body_value)

result = post_letter_client.create_send_post_letter(body)

```


### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.create_calculate_price") create_calculate_price

> TODO: Add a method description

```python
def create_calculate_price(self,
                               body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "{  \"file_url\": \"http://server.com/file.pdf\",  \"template_used\": 1,  \"colour\": 1,  \"duplex\": 0,  \"recipients\": [    \"[]\"  ],  \"Body\": \"\"}"
body = json.loads(body_value)

result = post_letter_client.create_calculate_price(body)

```


### <a name="get_post_letter_history"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.get_post_letter_history") get_post_letter_history

> TODO: Add a method description

```python
def get_post_letter_history(self)
```

#### Example Usage

```python

result = post_letter_client.get_post_letter_history()

```


### <a name="get_export_post_letter_history"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.get_export_post_letter_history") get_export_post_letter_history

> TODO: Add a method description

```python
def get_export_post_letter_history(self,
                                       filename)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | Filename for the export file. |



#### Example Usage

```python
filename = 'myexport.csv'

result = post_letter_client.get_export_post_letter_history(filename)

```


### <a name="create_a_post_return_address"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.create_a_post_return_address") create_a_post_return_address

> TODO: Add a method description

```python
def create_a_post_return_address(self,
                                     body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "{    \"address_name\":\"My Home Address\",    \"address_line_1\":\"Maritime Avenue\",    \"address_line_2\":\"\",    \"address_city\":\"Flynn\",    \"address_state\":\"WA\",    \"address_postal_code\":6302,    \"address_country\":\"Australia\"}"
body = json.loads(body_value)

result = post_letter_client.create_a_post_return_address(body)

```


### <a name="get_list_of_post_return_addresses"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.get_list_of_post_return_addresses") get_list_of_post_return_addresses

> TODO: Add a method description

```python
def get_list_of_post_return_addresses(self)
```

#### Example Usage

```python

result = post_letter_client.get_list_of_post_return_addresses()

```


### <a name="get_post_return_address"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.get_post_return_address") get_post_return_address

> TODO: Add a method description

```python
def get_post_return_address(self,
                                return_address_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| returnAddressId |  ``` Required ```  | Your return address id. |



#### Example Usage

```python
return_address_id = 14

result = post_letter_client.get_post_return_address(return_address_id)

```


### <a name="update_post_return_address"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.update_post_return_address") update_post_return_address

> TODO: Add a method description

```python
def update_post_return_address(self,
                                   return_address_id,
                                   body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| returnAddressId |  ``` Required ```  | Your return address id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
return_address_id = 14
body_value = "{    \"address_name\":\"My Home Address\",    \"address_line_1\":\"Maritime Avenue\",    \"address_line_2\":\"\",    \"address_city\":\"Flynn\",    \"address_state\":\"WA\",    \"address_postal_code\":6302,    \"address_country\":\"Australia\"}"
body = json.loads(body_value)

result = post_letter_client.update_post_return_address(return_address_id, body)

```


### <a name="delete_post_return_address"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.delete_post_return_address") delete_post_return_address

> TODO: Add a method description

```python
def delete_post_return_address(self,
                                   return_address_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| returnAddressId |  ``` Required ```  | Your return address id. |



#### Example Usage

```python
return_address_id = 12

result = post_letter_client.delete_post_return_address(return_address_id)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="postcards_controller"></a>![Class: ](https://apidocs.io/img/class.png ".PostcardsController") PostcardsController

### Get controller instance

An instance of the ``` PostcardsController ``` class can be accessed from the API Client.

```python
 postcards_client = client.postcards
```

### <a name="create_send_postcard"></a>![Method: ](https://apidocs.io/img/method.png ".PostcardsController.create_send_postcard") create_send_postcard

> **Supported File Types**
> We support PDF, docx and doc. Contact us to add support for any other file type. If you're using docx or doc files, you'll need to convert the file first using our uploads endpoint with the querystring parameter ?convert=post. e.g. POST /uploads?convert=post. This will return a URL to the converted pdf file that can be used in the /post/postcards/send endpoint.
> **Postcard File Options**
> **Use existing URL**
> With this option, you can use an existing URL to a PDF document. For example, you might generate the pdf on your server.
> For `file_urls` field. You can attach at least 1 and max of 2 PDF file urls.
> - Supply a single pdf with 2 pages (front and back)
> - Supply 2 urls to seperate PDFs
> **Upload File to Our Server**
> With this option, you can use the `/uploads` endpoint to upload the document. The `/uploads` endpoint returns a URL that can be used in the `/post/postcards/send` endpoint.

```python
def create_send_postcard(self,
                             body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "{    \"file_urls\":[         \"https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_front.pdf\",         \"https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_back.pdf\"    ],    \"recipients\":[        {            \"address_name\":\"My Home Address\",            \"address_line_1\":\"Address 1\",            \"address_line_2\":\"\",            \"address_city\":\"City\",            \"address_state\":\"State\",            \"address_postal_code\":\"123456\",            \"address_country\":\"AU\",            \"return_address_id\":1        }    ]}"
body = json.loads(body_value)

result = postcards_client.create_send_postcard(body)

```


### <a name="create_calculate_pricing"></a>![Method: ](https://apidocs.io/img/method.png ".PostcardsController.create_calculate_pricing") create_calculate_pricing

> For `file_urls` field. You can attach at least 1 and max of 2 PDF file urls.
> - Supply a single pdf with 2 pages (front and back)
> - Supply 2 urls to seperate PDFs

```python
def create_calculate_pricing(self,
                                 body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "{    \"file_urls\":[        \"https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_front.pdf\",        \"https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_back.pdf\"    ],    \"recipients\":[        {            \"address_name\":\"My Home Address\",            \"address_line_1\":\"Address 1\",            \"address_line_2\":\"\",            \"address_city\":\"City\",            \"address_state\":\"State\",            \"address_postal_code\":\"123456\",            \"address_country\":\"AU\",            \"return_address_id\":1        }    ]}"
body = json.loads(body_value)

result = postcards_client.create_calculate_pricing(body)

```


### <a name="get_postcard_history"></a>![Method: ](https://apidocs.io/img/method.png ".PostcardsController.get_postcard_history") get_postcard_history

> TODO: Add a method description

```python
def get_postcard_history(self)
```

#### Example Usage

```python

result = postcards_client.get_postcard_history()

```


### <a name="get_export_postcard_history"></a>![Method: ](https://apidocs.io/img/method.png ".PostcardsController.get_export_postcard_history") get_export_postcard_history

> TODO: Add a method description

```python
def get_export_postcard_history(self,
                                    filename)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | Filename for the export file. |



#### Example Usage

```python
filename = 'myexport.csv'

result = postcards_client.get_export_postcard_history(filename)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="referral_accounts_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ReferralAccountsController") ReferralAccountsController

### Get controller instance

An instance of the ``` ReferralAccountsController ``` class can be accessed from the API Client.

```python
 referral_accounts_client = client.referral_accounts
```

### <a name="get_list_of_referral_accounts"></a>![Method: ](https://apidocs.io/img/method.png ".ReferralAccountsController.get_list_of_referral_accounts") get_list_of_referral_accounts

> TODO: Add a method description

```python
def get_list_of_referral_accounts(self)
```

#### Example Usage

```python

result = referral_accounts_client.get_list_of_referral_accounts()

```


[Back to List of Controllers](#list_of_controllers)

## <a name="reseller_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ResellerController") ResellerController

### Get controller instance

An instance of the ``` ResellerController ``` class can be accessed from the API Client.

```python
 reseller_client = client.reseller
```

### <a name="get_reseller_setting"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerController.get_reseller_setting") get_reseller_setting

> Get reseller setting.

```python
def get_reseller_setting(self)
```

#### Example Usage

```python

result = reseller_client.get_reseller_setting()

```


### <a name="update_reseller_setting"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerController.update_reseller_setting") update_reseller_setting

> Update a specific reseller setting.

```python
def update_reseller_setting(self,
                                body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "    {        \"allow_public_signups\":1,        \"default_margin\":100,        \"default_margin_numbers\":150,        \"trial_balance\":50,        \"subdomain\":\"subdomain\",        \"colour_navigation\":\"#9999FF\",        \"logo_url_light\":\"http://url.com/light\",        \"logo_url_dark\":\"http://url.com/dark\",        \"company_name\":\"MyCompany\"    }"
body = json.loads(body_value)

result = reseller_client.update_reseller_setting(body)

```


### <a name="get_reseller_by_subdomain"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerController.get_reseller_by_subdomain") get_reseller_by_subdomain

> Get reseller setting by subdomin.

```python
def get_reseller_by_subdomain(self,
                                  subdomain)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subdomain |  ``` Required ```  | Subdomain |



#### Example Usage

```python
subdomain = 'mysubdomain'

result = reseller_client.get_reseller_by_subdomain(subdomain)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="reseller_accounts_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ResellerAccountsController") ResellerAccountsController

### Get controller instance

An instance of the ``` ResellerAccountsController ``` class can be accessed from the API Client.

```python
 reseller_accounts_client = client.reseller_accounts
```

### <a name="list_of_reseller_accounts"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.list_of_reseller_accounts") list_of_reseller_accounts

> Get list of Reseller Accounts

```python
def list_of_reseller_accounts(self)
```

#### Example Usage

```python

result = reseller_accounts_client.list_of_reseller_accounts()

```


### <a name="get_reseller_account"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.get_reseller_account") get_reseller_account

> Get a specific reseller account.

```python
def get_reseller_account(self,
                             client_user_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| clientUserId |  ``` Required ```  | The client user id. |



#### Example Usage

```python
client_user_id = 24

result = reseller_accounts_client.get_reseller_account(client_user_id)

```


### <a name="create_reseller_account"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.create_reseller_account") create_reseller_account

> TODO: Add a method description

```python
def create_reseller_account(self,
                                body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "    {        \"username\":\"johndoe2\",        \"user_email\":\"johndoe2@awesome.com\",        \"user_phone\":\"518-481-1002\",        \"user_first_name\":\"John\",        \"user_last_name\":\"Doe\",        \"country\":\"US\",        \"password\":\"pass\",        \"account_name\":\"The Awesome Company\"    }"
body = json.loads(body_value)

result = reseller_accounts_client.create_reseller_account(body)

```


### <a name="create_reseller_account_public"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.create_reseller_account_public") create_reseller_account_public

> TODO: Add a method description

```python
def create_reseller_account_public(self,
                                       body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "{    \"reseller_user_id\":1,    \"username\":\"john_awesome\",    \"user_email\":\"johnis@awesome.com\",    \"user_phone\":\"+61261063270\",    \"user_first_name\":\"John\",    \"user_last_name\":\"Awesome\",    \"country\":\"AU\",    \"password\":\"pass\",    \"account_name\":\"The Awesome Company\"}"
body = json.loads(body_value)

result = reseller_accounts_client.create_reseller_account_public(body)

```


### <a name="update_reseller_account"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.update_reseller_account") update_reseller_account

> TODO: Add a method description

```python
def update_reseller_account(self,
                                client_user_id,
                                body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| clientUserId |  ``` Required ```  | Your client user id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
client_user_id = 24
body_value = "    {        \"username\":\"johndoe2\",        \"user_email\":\"johndoe2@awesome.com\",        \"user_phone\":\"518-481-1002\",        \"user_first_name\":\"John\",        \"user_last_name\":\"Doe\",        \"country\":\"US\",        \"password\":\"pass\",        \"account_name\":\"The Awesome Company\"    }"
body = json.loads(body_value)

result = reseller_accounts_client.update_reseller_account(client_user_id, body)

```


### <a name="update_transfer_credit"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.update_transfer_credit") update_transfer_credit

> TODO: Add a method description

```python
def update_transfer_credit(self,
                               body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = TransferCreditRequest()

result = reseller_accounts_client.update_transfer_credit(body)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="sdk_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SDKController") SDKController

### Get controller instance

An instance of the ``` SDKController ``` class can be accessed from the API Client.

```python
 sdk_client = client.sdk
```

### <a name="get_sdk_download"></a>![Method: ](https://apidocs.io/img/method.png ".SDKController.get_sdk_download") get_sdk_download

> TODO: Add a method description

```python
def get_sdk_download(self,
                         mtype)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mtype |  ``` Required ```  | Supported types. |



#### Example Usage

```python
mtype = 'type'

result = sdk_client.get_sdk_download(mtype)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="search_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SearchController") SearchController

### Get controller instance

An instance of the ``` SearchController ``` class can be accessed from the API Client.

```python
 search_client = client.search
```

### <a name="search_contacts_lists"></a>![Method: ](https://apidocs.io/img/method.png ".SearchController.search_contacts_lists") search_contacts_lists

> TODO: Add a method description

```python
def search_contacts_lists(self,
                              q)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| q |  ``` Required ```  | Your keyword or query. |



#### Example Usage

```python
q = 'Gorne'

result = search_client.search_contacts_lists(q)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="sms_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SMSController") SMSController

### Get controller instance

An instance of the ``` SMSController ``` class can be accessed from the API Client.

```python
 sms_client = client.sms
```

### <a name="create_send_an_sms"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.create_send_an_sms") create_send_an_sms

> You can post **up to 1000 messages** with each API call.

```python
def create_send_an_sms(self,
                           body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = SendAnSMSRequest()

result = sms_client.create_send_an_sms(body)

```


### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.create_calculate_price") create_calculate_price

> TODO: Add a method description

```python
def create_calculate_price(self,
                               body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CalculatePriceRequest205()

result = sms_client.create_calculate_price(body)

```


### <a name="get_all_history"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.get_all_history") get_all_history

> **SMS Delivery Status**
> **Status (status field)**
> | Status | Description |
> |---|---|---|
> | `Completed` | Added to delivery queue. Waiting to be sent to the network.|
> | `Sent` | Message sent to the network.|
> | `Cancelled` | Message cancelled.|
> | `Scheduled` | Message scheduled.|
> | `WaitApproval` | Waiting approval by our team. This is temporary and will change to 'Sent' once approved. This only happens for a few messages that are flagged for approval by our automated spam-detection system.|
> **Status Codes (status_code field)**
> | Code | Text | Description |
> |---|---|---|
> | `200` | Sent by network| Temporary success|
> | `201` | Received on handset| Permanent success|
> | `300` | Delivery failure| Permanent failure|
> | `301` | Delivery failure| Permanent failure|
> | `302` | Delivery failure| Temporary failure - supplier routing issue|

```python
def get_all_history(self,
                        date_from=None,
                        date_to=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateFrom |  ``` Optional ```  | Timestamp (from) used to show records by date. |
| dateTo |  ``` Optional ```  | Timestamp (to) used to show recrods by date. |



#### Example Usage

```python
date_from = 1449459940
date_to = 1449659940

result = sms_client.get_all_history(date_from, date_to)

```


### <a name="get_export_sms_history"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.get_export_sms_history") get_export_sms_history

> TODO: Add a method description

```python
def get_export_sms_history(self)
```

#### Example Usage

```python

result = sms_client.get_export_sms_history()

```


### <a name="get_all_delivery_receipts"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.get_all_delivery_receipts") get_all_delivery_receipts

> **Push Delivery Receipts**
> If you prefer, we can push message replies to your server as they arrive with us.
> 1. Log into your account.
> 2. Click on 'SMS' then 'Settings' tab.
> 3. Click on the 'SMS Delivery Report Settings' menu.
> 4. Select 'Forward to URL'.
> 5. Enter the URL and click 'Save'.
> The following variables will be posted to the URL specified:
> | Variable | Description |
> |---|---|
> | `timestamp_send` | Timestamp of the original send request in UNIX format. e.g 1439173980
> | `timestamp` | Timestamp of delivery report in UNIX format. e.g 1439173981
> | `message_id` | Message ID, returned when originally sending the message.
> | `status` | Delivered or Undelivered
> | `status_code` | Status code. Refer to 'SMS Delivery Status Codes' in docs.
> | `status_text` | Status text.
> | `error_code` | Error code.
> | `error_text` | Error text.
> | `custom_string` | A custom string used when sending the original message.
> | `user_id` | The user ID of the user who sent the message.
> | `subaccount_id` | The subaccount ID of the user who sent the message.
> | `message_type` | 'sms' (constant).
> **Pull Delivery Receipts**
> Receive delivery reports by polling.
> You can poll our server and retrieve delivery reports at a time that suits you.
> 1. Log into your account.
> 2. Click on 'SMS' then 'Settings' tab.
> 3. Click on the 'SMS Delivery Report Settings' menu.
> 4. Select 'Poll our server' and click 'Save'.

```python
def get_all_delivery_receipts(self)
```

#### Example Usage

```python

result = sms_client.get_all_delivery_receipts()

```


### <a name="get_a_specific_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.get_a_specific_delivery_receipt") get_a_specific_delivery_receipt

> **Push Delivery Receipts**
> If you prefer, we can push message replies to your server as they arrive with us.
> 1. Log into your account.
> 2. Click on 'SMS' then 'Settings' tab.
> 3. Click on the 'SMS Delivery Report Settings' menu.
> 4. Select 'Forward to URL'.
> 5. Enter the URL and click 'Save'.
> The following variables will be posted to the URL specified:
> | Variable | Description |
> |---|---|
> | `timestamp_send` | Timestamp of the original send request in UNIX format. e.g 1439173980
> | `timestamp` | Timestamp of delivery report in UNIX format. e.g 1439173981
> | `message_id` | Message ID, returned when originally sending the message.
> | `status` | Delivered or Undelivered
> | `status_code` | Status code. Refer to 'SMS Delivery Status Codes' in docs.
> | `status_text` | Status text.
> | `error_code` | Error code.
> | `error_text` | Error text.
> | `custom_string` | A custom string used when sending the original message.
> | `user_id` | The user ID of the user who sent the message.
> | `subaccount_id` | The subaccount ID of the user who sent the message.
> | `message_type` | 'sms' (constant).
> **Pull Delivery Receipts**
> Receive delivery reports by polling.
> You can poll our server and retrieve delivery reports at a time that suits you.
> 1. Log into your account.
> 2. Click on 'SMS' then 'Settings' tab.
> 3. Click on the 'SMS Delivery Report Settings' menu.
> 4. Select 'Poll our server' and click 'Save'.

```python
def get_a_specific_delivery_receipt(self,
                                        message_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Your message id. |



#### Example Usage

```python
message_id = '88AB118E EB1B 478C 98CE 6C73ABA23F67'

result = sms_client.get_a_specific_delivery_receipt(message_id)

```


### <a name="add_a_test_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.add_a_test_delivery_receipt") add_a_test_delivery_receipt

> **Push Delivery Receipts**
> If you prefer, we can push message replies to your server as they arrive with us.
> 1. Log into your account.
> 2. Click on 'SMS' then 'Settings' tab.
> 3. Click on the 'SMS Delivery Report Settings' menu.
> 4. Select 'Forward to URL'.
> 5. Enter the URL and click 'Save'.
> The following variables will be posted to the URL specified:
> | Variable | Description |
> |---|---|
> | `timestamp_send` | Timestamp of the original send request in UNIX format. e.g 1439173980
> | `timestamp` | Timestamp of delivery report in UNIX format. e.g 1439173981
> | `message_id` | Message ID, returned when originally sending the message.
> | `status` | Delivered or Undelivered
> | `status_code` | Status code. Refer to 'SMS Delivery Status Codes' in docs.
> | `status_text` | Status text.
> | `error_code` | Error code.
> | `error_text` | Error text.
> | `custom_string` | A custom string used when sending the original message.
> | `user_id` | The user ID of the user who sent the message.
> | `subaccount_id` | The subaccount ID of the user who sent the message.
> | `message_type` | 'sms' (constant).
> **Pull Delivery Receipts**
> Receive delivery reports by polling.
> You can poll our server and retrieve delivery reports at a time that suits you.
> 1. Log into your account.
> 2. Click on 'SMS' then 'Settings' tab.
> 3. Click on the 'SMS Delivery Report Settings' menu.
> 4. Select 'Poll our server' and click 'Save'.

```python
def add_a_test_delivery_receipt(self,
                                    body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "    {        \"url\":\"http://yourUrl.com\"    }"
body = json.loads(body_value)

result = sms_client.add_a_test_delivery_receipt(body)

```


### <a name="update_mark_delivery_receipts_as_read"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.update_mark_delivery_receipts_as_read") update_mark_delivery_receipts_as_read

> **Push Delivery Receipts**
> If you prefer, we can push message replies to your server as they arrive with us.
> 1. Log into your account.
> 2. Click on 'SMS' then 'Settings' tab.
> 3. Click on the 'SMS Delivery Report Settings' menu.
> 4. Select 'Forward to URL'.
> 5. Enter the URL and click 'Save'.
> The following variables will be posted to the URL specified:
> | Variable | Description |
> |---|---|
> | `timestamp_send` | Timestamp of the original send request in UNIX format. e.g 1439173980
> | `timestamp` | Timestamp of delivery report in UNIX format. e.g 1439173981
> | `message_id` | Message ID, returned when originally sending the message.
> | `status` | Delivered or Undelivered
> | `status_code` | Status code. Refer to 'SMS Delivery Status Codes' in docs.
> | `status_text` | Status text.
> | `error_code` | Error code.
> | `error_text` | Error text.
> | `custom_string` | A custom string used when sending the original message.
> | `user_id` | The user ID of the user who sent the message.
> | `subaccount_id` | The subaccount ID of the user who sent the message.
> | `message_type` | 'sms' (constant).
> **Pull Delivery Receipts**
> Receive delivery reports by polling.
> You can poll our server and retrieve delivery reports at a time that suits you.
> 1. Log into your account.
> 2. Click on 'SMS' then 'Settings' tab.
> 3. Click on the 'SMS Delivery Report Settings' menu.
> 4. Select 'Poll our server' and click 'Save'.

```python
def update_mark_delivery_receipts_as_read(self,
                                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "{    \"date_before\": 1441958441}"
body = json.loads(body_value)

result = sms_client.update_mark_delivery_receipts_as_read(body)

```


### <a name="get_all_inbound_sms_pull"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.get_all_inbound_sms_pull") get_all_inbound_sms_pull

> **Push Inbound SMS**
> If you prefer, we can push message replies to your server as they arrive with us.
> 1. Log into your account.
> 2. Click on 'SMS' then 'Settings' tab.
> 3. Click on the 'Inbound SMS Settings' menu.
> 4. Add a new rule to and select Action: 'URL'.
> 5. Enter the URL and click 'Save'.
> The following variables will be posted to the URL specified:
> | Variable | Description |
> |---|---|
> | `timestamp` | Timestamp in UNIX format. e.g 1439173981
> | `to` | Number that the SMS was sent to (your Dedicated or shared number).
> | `from` | Recipient Mobile Number that sent the reply message.
> | `body` | Inbound message body.
> | `original_body` | Original outgoing SMS message body.
> | `original_message_id` | Original SMS message ID. Returned when originally sending the message.
> | `custom_string` | A custom string used when sending the original message.
> | `user_id` | The user ID of the user who sent the message.
> | `subaccount_id` | The subaccount ID of the user who sent the message.
> Note: HTTP POST is used to send the variables (Not GET/query-string [**More Info**] (http://www.w3schools.com/tags/ref_httpmethods.asp))
> **Pull Inbound SMS**
> Receive SMS by polling your Inbox.
> You can poll our server and retrieve new Messages at a time that suits you.
> 1. Log into your account.
> 2. Click on 'SMS' then 'Settings' tab.
> 3. Click on the 'Inbound SMS Settings' menu.
> 4. Select Action: 'POLL' and click 'Save'.

```python
def get_all_inbound_sms_pull(self)
```

#### Example Usage

```python

result = sms_client.get_all_inbound_sms_pull()

```


### <a name="get_specific_inbound_pull"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.get_specific_inbound_pull") get_specific_inbound_pull

> **Push Inbound SMS**
> If you prefer, we can push message replies to your server as they arrive with us.
> 1. Log into your account.
> 2. Click on 'SMS' then 'Settings' tab.
> 3. Click on the 'Inbound SMS Settings' menu.
> 4. Add a new rule to and select Action: 'URL'.
> 5. Enter the URL and click 'Save'.
> The following variables will be posted to the URL specified:
> | Variable | Description |
> |---|---|
> | `timestamp` | Timestamp in UNIX format. e.g 1439173981
> | `to` | Number that the SMS was sent to (your Dedicated or shared number).
> | `from` | Recipient Mobile Number that sent the reply message.
> | `body` | Inbound message body.
> | `original_body` | Original outgoing SMS message body.
> | `original_message_id` | Original SMS message ID. Returned when originally sending the message.
> | `custom_string` | A custom string used when sending the original message.
> | `user_id` | The user ID of the user who sent the message.
> | `subaccount_id` | The subaccount ID of the user who sent the message.
> Note: HTTP POST is used to send the variables (Not GET/query-string [**More Info**] (http://www.w3schools.com/tags/ref_httpmethods.asp))
> **Pull Inbound SMS**
> Receive SMS by polling your Inbox.
> You can poll our server and retrieve new Messages at a time that suits you.
> 1. Log into your account.
> 2. Click on 'SMS' then 'Settings' tab.
> 3. Click on the 'Inbound SMS Settings' menu.
> 4. Select Action: 'POLL' and click 'Save'.

```python
def get_specific_inbound_pull(self,
                                  message_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Message ID. Must be a valid GUID. |



#### Example Usage

```python
message_id = '5D420421-8715-4461-A9A2-C8F569E41835'

result = sms_client.get_specific_inbound_pull(message_id)

```


### <a name="add_a_test_inbound_sms"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.add_a_test_inbound_sms") add_a_test_inbound_sms

> **Push Inbound SMS**
> If you prefer, we can push message replies to your server as they arrive with us.
> 1. Log into your account.
> 2. Click on 'SMS' then 'Settings' tab.
> 3. Click on the 'Inbound SMS Settings' menu.
> 4. Add a new rule to and select Action: 'URL'.
> 5. Enter the URL and click 'Save'.
> The following variables will be posted to the URL specified:
> | Variable | Description |
> |---|---|
> | `timestamp` | Timestamp in UNIX format. e.g 1439173981
> | `to` | Number that the SMS was sent to (your Dedicated or shared number).
> | `from` | Recipient Mobile Number that sent the reply message.
> | `body` | Inbound message body.
> | `original_body` | Original outgoing SMS message body.
> | `original_message_id` | Original SMS message ID. Returned when originally sending the message.
> | `custom_string` | A custom string used when sending the original message.
> | `user_id` | The user ID of the user who sent the message.
> | `subaccount_id` | The subaccount ID of the user who sent the message.
> Note: HTTP POST is used to send the variables (Not GET/query-string [**More Info**] (http://www.w3schools.com/tags/ref_httpmethods.asp))
> **Pull Inbound SMS**
> Receive SMS by polling your Inbox.
> You can poll our server and retrieve new Messages at a time that suits you.
> 1. Log into your account.
> 2. Click on 'SMS' then 'Settings' tab.
> 3. Click on the 'Inbound SMS Settings' menu.
> 4. Select Action: 'POLL' and click 'Save'.

```python
def add_a_test_inbound_sms(self,
                               body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "    {        \"url\":\"http://yourUrl.com\"    }"
body = json.loads(body_value)

result = sms_client.add_a_test_inbound_sms(body)

```


### <a name="update_mark_a_specific_inbound_sms_as_read"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.update_mark_a_specific_inbound_sms_as_read") update_mark_a_specific_inbound_sms_as_read

> **Push Inbound SMS**
> If you prefer, we can push message replies to your server as they arrive with us.
> 1. Log into your account.
> 2. Click on 'SMS' then 'Settings' tab.
> 3. Click on the 'Inbound SMS Settings' menu.
> 4. Add a new rule to and select Action: 'URL'.
> 5. Enter the URL and click 'Save'.
> The following variables will be posted to the URL specified:
> | Variable | Description |
> |---|---|
> | `timestamp` | Timestamp in UNIX format. e.g 1439173981
> | `to` | Number that the SMS was sent to (your Dedicated or shared number).
> | `from` | Recipient Mobile Number that sent the reply message.
> | `body` | Inbound message body.
> | `original_body` | Original outgoing SMS message body.
> | `original_message_id` | Original SMS message ID. Returned when originally sending the message.
> | `custom_string` | A custom string used when sending the original message.
> | `user_id` | The user ID of the user who sent the message.
> | `subaccount_id` | The subaccount ID of the user who sent the message.
> Note: HTTP POST is used to send the variables (Not GET/query-string [**More Info**] (http://www.w3schools.com/tags/ref_httpmethods.asp))
> **Pull Inbound SMS**
> Receive SMS by polling your Inbox.
> You can poll our server and retrieve new Messages at a time that suits you.
> 1. Log into your account.
> 2. Click on 'SMS' then 'Settings' tab.
> 3. Click on the 'Inbound SMS Settings' menu.
> 4. Select Action: 'POLL' and click 'Save'.

```python
def update_mark_a_specific_inbound_sms_as_read(self,
                                                   message_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | B7CE432193CD-0753597B7293 (string, required) - The message ID you want to mark as read. |



#### Example Usage

```python
message_id = '307EF035'

result = sms_client.update_mark_a_specific_inbound_sms_as_read(message_id)

```


### <a name="update_mark_all_inbound_sms_as_read"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.update_mark_all_inbound_sms_as_read") update_mark_all_inbound_sms_as_read

> **Push Inbound SMS**
> If you prefer, we can push message replies to your server as they arrive with us.
> 1. Log into your account.
> 2. Click on 'SMS' then 'Settings' tab.
> 3. Click on the 'Inbound SMS Settings' menu.
> 4. Add a new rule to and select Action: 'URL'.
> 5. Enter the URL and click 'Save'.
> The following variables will be posted to the URL specified:
> | Variable | Description |
> |---|---|
> | `timestamp` | Timestamp in UNIX format. e.g 1439173981
> | `to` | Number that the SMS was sent to (your Dedicated or shared number).
> | `from` | Recipient Mobile Number that sent the reply message.
> | `body` | Inbound message body.
> | `original_body` | Original outgoing SMS message body.
> | `original_message_id` | Original SMS message ID. Returned when originally sending the message.
> | `custom_string` | A custom string used when sending the original message.
> | `user_id` | The user ID of the user who sent the message.
> | `subaccount_id` | The subaccount ID of the user who sent the message.
> Note: HTTP POST is used to send the variables (Not GET/query-string [**More Info**] (http://www.w3schools.com/tags/ref_httpmethods.asp))
> **Pull Inbound SMS**
> Receive SMS by polling your Inbox.
> You can poll our server and retrieve new Messages at a time that suits you.
> 1. Log into your account.
> 2. Click on 'SMS' then 'Settings' tab.
> 3. Click on the 'Inbound SMS Settings' menu.
> 4. Select Action: 'POLL' and click 'Save'.

```python
def update_mark_all_inbound_sms_as_read(self,
                                            body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "    {        \"date_before\":1442398100    }"
body = json.loads(body_value)

result = sms_client.update_mark_all_inbound_sms_as_read(body)

```


### <a name="update_cancel_a_scheduled_message"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.update_cancel_a_scheduled_message") update_cancel_a_scheduled_message

> TODO: Add a method description

```python
def update_cancel_a_scheduled_message(self,
                                          message_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | B7CE432193CD-0753597B7293 (string, required) - The message ID you want to cancel. |



#### Example Usage

```python
message_id = '307EF035'

result = sms_client.update_cancel_a_scheduled_message(message_id)

```


### <a name="update_cancel_all_scheduled_messages"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.update_cancel_all_scheduled_messages") update_cancel_all_scheduled_messages

> TODO: Add a method description

```python
def update_cancel_all_scheduled_messages(self)
```

#### Example Usage

```python

result = sms_client.update_cancel_all_scheduled_messages()

```


[Back to List of Controllers](#list_of_controllers)

## <a name="sms_campaigns_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SMSCampaignsController") SMSCampaignsController

### Get controller instance

An instance of the ``` SMSCampaignsController ``` class can be accessed from the API Client.

```python
 sms_campaigns_client = client.sms_campaigns
```

### <a name="create_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.create_sms_campaign") create_sms_campaign

> You can post to a list with **up to 20000 recipients** with each API call.

```python
def create_sms_campaign(self,
                            body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "{    \"list_id\":428,    \"name\":\"My Campaign 1\",    \"from\":\"+61353787448\",    \"body\":\"This is my new campaign message.\",    \"schedule\":1444821615}"
body = json.loads(body_value)

result = sms_campaigns_client.create_sms_campaign(body)

```


### <a name="create_calculate_price_for_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.create_calculate_price_for_sms_campaign") create_calculate_price_for_sms_campaign

> TODO: Add a method description

```python
def create_calculate_price_for_sms_campaign(self,
                                                body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "{    \"list_id\":428,    \"name\":\"My Campaign 1\",    \"from\":\"+61353787448\",    \"body\":\"(First Name), this is your new campaign message.\"}"
body = json.loads(body_value)

result = sms_campaigns_client.create_calculate_price_for_sms_campaign(body)

```


### <a name="update_an_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.update_an_sms_campaign") update_an_sms_campaign

> TODO: Add a method description

```python
def update_an_sms_campaign(self,
                               sms_campaign_id,
                               body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| smsCampaignId |  ``` Required ```  | Your SMS Campaign id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
sms_campaign_id = 1
body_value = "{    \"list_id\":428,    \"name\":\"Awesome campaign.\",    \"from\":\"+61353787447\",    \"body\":\"his is an awesome message.\",    \"schedule\":1444821615}"
body = json.loads(body_value)

result = sms_campaigns_client.update_an_sms_campaign(sms_campaign_id, body)

```


### <a name="get_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.get_sms_campaign") get_sms_campaign

> TODO: Add a method description

```python
def get_sms_campaign(self,
                         sms_campaign_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| smsCampaignId |  ``` Required ```  | Your SMS campaign id. |



#### Example Usage

```python
sms_campaign_id = 1

result = sms_campaigns_client.get_sms_campaign(sms_campaign_id)

```


### <a name="update_cancel_an_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.update_cancel_an_sms_campaign") update_cancel_an_sms_campaign

> TODO: Add a method description

```python
def update_cancel_an_sms_campaign(self,
                                      sms_campaign_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| smsCampaignId |  ``` Required ```  | Your SMS Campaign id. |



#### Example Usage

```python
sms_campaign_id = 1

result = sms_campaigns_client.update_cancel_an_sms_campaign(sms_campaign_id)

```


### <a name="get_list_of_sms_campaigns"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.get_list_of_sms_campaigns") get_list_of_sms_campaigns

> TODO: Add a method description

```python
def get_list_of_sms_campaigns(self)
```

#### Example Usage

```python

result = sms_campaigns_client.get_list_of_sms_campaigns()

```


[Back to List of Controllers](#list_of_controllers)

## <a name="sms_templates_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SMSTemplatesController") SMSTemplatesController

### Get controller instance

An instance of the ``` SMSTemplatesController ``` class can be accessed from the API Client.

```python
 sms_templates_client = client.sms_templates
```

### <a name="list_of_templates"></a>![Method: ](https://apidocs.io/img/method.png ".SMSTemplatesController.list_of_templates") list_of_templates

> Get list of templates.

```python
def list_of_templates(self)
```

#### Example Usage

```python

result = sms_templates_client.list_of_templates()

```


### <a name="create_a_template"></a>![Method: ](https://apidocs.io/img/method.png ".SMSTemplatesController.create_a_template") create_a_template

> Create new template.

```python
def create_a_template(self,
                          body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "    {        \"template_name\":\"Template 501916\",        \"body\":\"This is a sample content: H7YI68B3yk for this template.\"    }"
body = json.loads(body_value)

result = sms_templates_client.create_a_template(body)

```


### <a name="update_a_template"></a>![Method: ](https://apidocs.io/img/method.png ".SMSTemplatesController.update_a_template") update_a_template

> TODO: Add a method description

```python
def update_a_template(self,
                          template_id,
                          body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
template_id = '25'
body_value = "    {        \"template_name\":\"I am updated\",        \"body\":\"This is a sample content: Sc0KNWgSMG for this template.\"    }"
body = json.loads(body_value)

result = sms_templates_client.update_a_template(template_id, body)

```


### <a name="delete_a_template"></a>![Method: ](https://apidocs.io/img/method.png ".SMSTemplatesController.delete_a_template") delete_a_template

> TODO: Add a method description

```python
def delete_a_template(self,
                          template_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |



#### Example Usage

```python
template_id = '25'

result = sms_templates_client.delete_a_template(template_id)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="statistics_controller"></a>![Class: ](https://apidocs.io/img/class.png ".StatisticsController") StatisticsController

### Get controller instance

An instance of the ``` StatisticsController ``` class can be accessed from the API Client.

```python
 statistics_client = client.statistics
```

### <a name="get_sms_statistics"></a>![Method: ](https://apidocs.io/img/method.png ".StatisticsController.get_sms_statistics") get_sms_statistics

> TODO: Add a method description

```python
def get_sms_statistics(self)
```

#### Example Usage

```python

result = statistics_client.get_sms_statistics()

```


### <a name="get_voice_statistics"></a>![Method: ](https://apidocs.io/img/method.png ".StatisticsController.get_voice_statistics") get_voice_statistics

> TODO: Add a method description

```python
def get_voice_statistics(self)
```

#### Example Usage

```python

result = statistics_client.get_voice_statistics()

```


[Back to List of Controllers](#list_of_controllers)

## <a name="subaccounts_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SubaccountsController") SubaccountsController

### Get controller instance

An instance of the ``` SubaccountsController ``` class can be accessed from the API Client.

```python
 subaccounts_client = client.subaccounts
```

### <a name="get_all_subaccounts"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.get_all_subaccounts") get_all_subaccounts

> TODO: Add a method description

```python
def get_all_subaccounts(self)
```

#### Example Usage

```python

result = subaccounts_client.get_all_subaccounts()

```


### <a name="create_a_new_subaccount"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.create_a_new_subaccount") create_a_new_subaccount

> TODO: Add a method description

```python
def create_a_new_subaccount(self,
                                body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "    {        \"api_username\":\"nameP99\",        \"password\":\"pass\",        \"email\":\"testvrq@gmail.com\",        \"phone_number\":\"941-751-3278\",        \"first_name\":\"FirstnameeGPqV\",        \"last_name\":\"LastnamePvjJp\"    }"
body = json.loads(body_value)

result = subaccounts_client.create_a_new_subaccount(body)

```


### <a name="get_a_specific_subaccount"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.get_a_specific_subaccount") get_a_specific_subaccount

> TODO: Add a method description

```python
def get_a_specific_subaccount(self,
                                  subaccount_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |



#### Example Usage

```python
subaccount_id = 59

result = subaccounts_client.get_a_specific_subaccount(subaccount_id)

```


### <a name="update_a_specific_subaccount"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.update_a_specific_subaccount") update_a_specific_subaccount

> TODO: Add a method description

```python
def update_a_specific_subaccount(self,
                                     subaccount_id,
                                     body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
subaccount_id = 59
body_value = "    {        \"password\":\"pass\",        \"email\":\"testfP0.updated@gmail.com\",        \"phone_number\":\"+19417519130\",        \"first_name\":\"FirstnameKvdRZUpdated\",        \"last_name\":\"LastnameHUPYGUpdated\",        \"access_users\": 1,        \"access_billing\": 1,        \"access_reporting\": 1,        \"access_contacts\": 1,        \"access_settings\": 1,        \"access_sms\": 1,        \"access_email\": 1,        \"access_voice\": 1,        \"access_fax\": 1,        \"access_post\": 1,        \"access_reseller\": 1,        \"access_mms\": 1,        \"share_campaigns\": 0,        \"notes\": null    }"
body = json.loads(body_value)

result = subaccounts_client.update_a_specific_subaccount(subaccount_id, body)

```


### <a name="delete_a_specific_subaccount"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.delete_a_specific_subaccount") delete_a_specific_subaccount

> TODO: Add a method description

```python
def delete_a_specific_subaccount(self,
                                     subaccount_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |



#### Example Usage

```python
subaccount_id = 59

result = subaccounts_client.delete_a_specific_subaccount(subaccount_id)

```


### <a name="update_regenerate_api_key"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.update_regenerate_api_key") update_regenerate_api_key

> TODO: Add a method description

```python
def update_regenerate_api_key(self,
                                  subaccount_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |



#### Example Usage

```python
subaccount_id = 59

result = subaccounts_client.update_regenerate_api_key(subaccount_id)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="timezones_controller"></a>![Class: ](https://apidocs.io/img/class.png ".TimezonesController") TimezonesController

### Get controller instance

An instance of the ``` TimezonesController ``` class can be accessed from the API Client.

```python
 timezones_client = client.timezones
```

### <a name="get_timezones"></a>![Method: ](https://apidocs.io/img/method.png ".TimezonesController.get_timezones") get_timezones

> Get supported list of timezones.

```python
def get_timezones(self)
```

#### Example Usage

```python

result = timezones_client.get_timezones()

```


[Back to List of Controllers](#list_of_controllers)

## <a name="transactional_email_controller"></a>![Class: ](https://apidocs.io/img/class.png ".TransactionalEmailController") TransactionalEmailController

### Get controller instance

An instance of the ``` TransactionalEmailController ``` class can be accessed from the API Client.

```python
 transactional_email_client = client.transactional_email
```

### <a name="create_email_send"></a>![Method: ](https://apidocs.io/img/method.png ".TransactionalEmailController.create_email_send") create_email_send

> TODO: Add a method description

```python
def create_email_send(self,
                          body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = EmailSendRequest()

result = transactional_email_client.create_email_send(body)

```


### <a name="create_email_price"></a>![Method: ](https://apidocs.io/img/method.png ".TransactionalEmailController.create_email_price") create_email_price

> TODO: Add a method description

```python
def create_email_price(self,
                           body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = EmailPriceRequest()

result = transactional_email_client.create_email_price(body)

```


### <a name="get_email_history"></a>![Method: ](https://apidocs.io/img/method.png ".TransactionalEmailController.get_email_history") get_email_history

> TODO: Add a method description

```python
def get_email_history(self)
```

#### Example Usage

```python

result = transactional_email_client.get_email_history()

```


### <a name="get_export_history"></a>![Method: ](https://apidocs.io/img/method.png ".TransactionalEmailController.get_export_history") get_export_history

> TODO: Add a method description

```python
def get_export_history(self,
                           filename)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | File name for the export file. |



#### Example Usage

```python
filename = 'myexport.csv'

result = transactional_email_client.get_export_history(filename)

```


### <a name="add_a_test_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png ".TransactionalEmailController.add_a_test_delivery_receipt") add_a_test_delivery_receipt

> **Push Delivery Receipts**
> If you prefer, we can push message replies to your server as they arrive with us.
> 1. Log into your account.
> 2. Click on ’Transactional Email’ then ’Settings’ tab.
> 3. Click on the 'Email Delivery Report Settings' menu.
> 4. Select 'Forward to URL'.
> 5. Enter the URL and click 'Save'.
> The following variables will be posted to the URL specified:
> | Variable | Description |
> |---|---|
> | `email` | The sender of the email.
> | `timestamp` | Timestamp in UNIX format. e.g 1439173981.
> | `message_id` | Message ID, returned when originally sending the message.
> | `status` | The email event. |
> List of email events:
> | Code | Description |
> |---|---|
> | `Processed` | This event fires when smtp server receives an individual message and prepares it to be delivered. |
> | `Deferred` | When an email cannot immediately be delivered, but it hasn’t been completely rejected. |
> | `Delivered` | When an email has been accepted at the receiving server. |
> | `Bounce` | If a server cannot or will not deliver a message. Bounces often are caused by outdated or incorrectly entered email addresses. |
> | `Dropped` | There are a number of reasons your email will not even be sent to a recipient for delivery. This event informs your system when an email has been dropped. |
> | `SpamReport` | Most internet service providers provide a feedback loop, sending specific spam complaints to the email service providers. This event fires so that you can react appropriately–or at the very least, never send another email to that address. |

```python
def add_a_test_delivery_receipt(self,
                                    body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "    {        \"url\":\"http://yourUrl.com\"    }"
body = json.loads(body_value)

result = transactional_email_client.add_a_test_delivery_receipt(body)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="uploads_controller"></a>![Class: ](https://apidocs.io/img/class.png ".UploadsController") UploadsController

### Get controller instance

An instance of the ``` UploadsController ``` class can be accessed from the API Client.

```python
 uploads_client = client.uploads
```

### <a name="upload_a_file"></a>![Method: ](https://apidocs.io/img/method.png ".UploadsController.upload_a_file") upload_a_file

> The `upload` endpoint provides a method for converting files from an unspported format to a format that one of our endpoints can handle.
> Files can be submitted two ways:
> 1. Using `base64` encoding in an `application/json` request. In this case, submit the `base64`-encoded file contents in the `content` field of the request body, and `convert` can be specified either also in the body or as part of the query string.
> 2. Using `multipart/form-data` encoding, in the same way it would be submitted using a HTML form. You may find cURL useful for this. For an example of how to do this, see one of our [SDKs](https://dashboard.clicksend.com/#/libraries-sdk/main). In this case, specify `convert` in the query string.
> Note that `convert` specifies the conversion to take place - that is, what the result should be compatible with - and can be any of `fax`, `mms`, `csv` or `post`.
> All files have 10 minutes expiry.

```python
def upload_a_file(self,
                      body,
                      convert=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |
| convert |  ``` Optional ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = UploadAFileRequest()
convert = 'convert'

result = uploads_client.upload_a_file(body, convert)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="voice_controller"></a>![Class: ](https://apidocs.io/img/class.png ".VoiceController") VoiceController

### Get controller instance

An instance of the ``` VoiceController ``` class can be accessed from the API Client.

```python
 voice_client = client.voice
```

### <a name="create_send_a_voice_call"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.create_send_a_voice_call") create_send_a_voice_call

> You can post **up to 1000 messages** with each API call.

```python
def create_send_a_voice_call(self,
                                 body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = SendAVoiceCallRequest()

result = voice_client.create_send_a_voice_call(body)

```


### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.create_calculate_price") create_calculate_price

> TODO: Add a method description

```python
def create_calculate_price(self,
                               body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CalculatePriceRequest263()

result = voice_client.create_calculate_price(body)

```


### <a name="get_voice_languages"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.get_voice_languages") get_voice_languages

> TODO: Add a method description

```python
def get_voice_languages(self)
```

#### Example Usage

```python

result = voice_client.get_voice_languages()

```


### <a name="get_voice_history"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.get_voice_history") get_voice_history

> TODO: Add a method description

```python
def get_voice_history(self,
                          date_from=None,
                          date_to=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateFrom |  ``` Optional ```  | Timestamp (from) used to show records by date. |
| dateTo |  ``` Optional ```  | Timestamp (to) used to show recrods by date. |



#### Example Usage

```python
date_from = 1443501617
date_to = 1443501727

result = voice_client.get_voice_history(date_from, date_to)

```


### <a name="get_export_voice_history"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.get_export_voice_history") get_export_voice_history

> TODO: Add a method description

```python
def get_export_voice_history(self)
```

#### Example Usage

```python

result = voice_client.get_export_voice_history()

```


### <a name="get_voice_receipts"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.get_voice_receipts") get_voice_receipts

> **Push Delivery Receipts**
> If you prefer, we can push message replies to your server as they arrive with us.
> 1. Log into your account.
> 2. Click on 'Voice' then 'Settings' tab.
> 3. Click on the 'Voice Delivery Report Settings' menu.
> 4. Select 'Forward to URL'.
> 5. Enter the URL and click 'Save'.
> The following variables will be posted to the URL specified:
> | Variable | Description |
> |---|---|
> | `timestamp_send` | Timestamp of the original send request in UNIX format. e.g 1439173980
> | `timestamp` | Timestamp of delivery report in UNIX format. e.g 1439173981
> | `message_id` | Message ID, returned when originally sending the message.
> | `status` | Delivered or Undelivered
> | `status_code` | Status code. Refer to 'Voice Delivery Status Codes' in docs.
> | `status_text` | Status text.
> | `error_code` | Error code.
> | `error_text` | Error text.
> | `custom_string` | A custom string used when sending the original message.
> | `user_id` | The user ID of the user who sent the message.
> | `subaccount_id` | The subaccount ID of the user who sent the message.
> | `message_type` | 'voice' (constant).
> | `digits` | Numbers the recipient pressed on their keypad during the call. A blank string will be used if they didn't provide any input.
> **Pull Delivery Receipts**
> Receive delivery reports by polling.
> You can poll our server and retrieve delivery reports at a time that suits you.
> 1. Log into your account.
> 2. Click on 'Voice' then 'Settings' tab.
> 3. Click on the 'Voice Delivery Report Settings' menu.
> 4. Select 'Poll our server' and click 'Save'.

```python
def get_voice_receipts(self)
```

#### Example Usage

```python

result = voice_client.get_voice_receipts()

```


### <a name="add_a_test_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.add_a_test_delivery_receipt") add_a_test_delivery_receipt

> **Push Delivery Receipts**
> If you prefer, we can push message replies to your server as they arrive with us.
> 1. Log into your account.
> 2. Click on 'Voice' then 'Settings' tab.
> 3. Click on the 'Voice Delivery Report Settings' menu.
> 4. Select 'Forward to URL'.
> 5. Enter the URL and click 'Save'.
> The following variables will be posted to the URL specified:
> | Variable | Description |
> |---|---|
> | `timestamp_send` | Timestamp of the original send request in UNIX format. e.g 1439173980
> | `timestamp` | Timestamp of delivery report in UNIX format. e.g 1439173981
> | `message_id` | Message ID, returned when originally sending the message.
> | `status` | Delivered or Undelivered
> | `status_code` | Status code. Refer to 'Voice Delivery Status Codes' in docs.
> | `status_text` | Status text.
> | `error_code` | Error code.
> | `error_text` | Error text.
> | `custom_string` | A custom string used when sending the original message.
> | `user_id` | The user ID of the user who sent the message.
> | `subaccount_id` | The subaccount ID of the user who sent the message.
> | `message_type` | 'voice' (constant).
> | `digits` | Numbers the recipient pressed on their keypad during the call. A blank string will be used if they didn't provide any input.
> **Pull Delivery Receipts**
> Receive delivery reports by polling.
> You can poll our server and retrieve delivery reports at a time that suits you.
> 1. Log into your account.
> 2. Click on 'Voice' then 'Settings' tab.
> 3. Click on the 'Voice Delivery Report Settings' menu.
> 4. Select 'Poll our server' and click 'Save'.

```python
def add_a_test_delivery_receipt(self,
                                    body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body_value = "    {        \"url\":\"http://yourUrl.com\"    }"
body = json.loads(body_value)

result = voice_client.add_a_test_delivery_receipt(body)

```


### <a name="get_specific_voice_receipt"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.get_specific_voice_receipt") get_specific_voice_receipt

> **Push Delivery Receipts**
> If you prefer, we can push message replies to your server as they arrive with us.
> 1. Log into your account.
> 2. Click on 'Voice' then 'Settings' tab.
> 3. Click on the 'Voice Delivery Report Settings' menu.
> 4. Select 'Forward to URL'.
> 5. Enter the URL and click 'Save'.
> The following variables will be posted to the URL specified:
> | Variable | Description |
> |---|---|
> | `timestamp_send` | Timestamp of the original send request in UNIX format. e.g 1439173980
> | `timestamp` | Timestamp of delivery report in UNIX format. e.g 1439173981
> | `message_id` | Message ID, returned when originally sending the message.
> | `status` | Delivered or Undelivered
> | `status_code` | Status code. Refer to 'Voice Delivery Status Codes' in docs.
> | `status_text` | Status text.
> | `error_code` | Error code.
> | `error_text` | Error text.
> | `custom_string` | A custom string used when sending the original message.
> | `user_id` | The user ID of the user who sent the message.
> | `subaccount_id` | The subaccount ID of the user who sent the message.
> | `message_type` | 'voice' (constant).
> | `digits` | Numbers the recipient pressed on their keypad during the call. A blank string will be used if they didn't provide any input.
> **Pull Delivery Receipts**
> Receive delivery reports by polling.
> You can poll our server and retrieve delivery reports at a time that suits you.
> 1. Log into your account.
> 2. Click on 'Voice' then 'Settings' tab.
> 3. Click on the 'Voice Delivery Report Settings' menu.
> 4. Select 'Poll our server' and click 'Save'.

```python
def get_specific_voice_receipt(self,
                                   message_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | 3055-45F1-9B79-F2C43509FD16 (string, required) - The voice receipt message id. |



#### Example Usage

```python
message_id = '28DD2718'

result = voice_client.get_specific_voice_receipt(message_id)

```


### <a name="update_marked_voice_receipts_as_read"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.update_marked_voice_receipts_as_read") update_marked_voice_receipts_as_read

> **Push Delivery Receipts**
> If you prefer, we can push message replies to your server as they arrive with us.
> 1. Log into your account.
> 2. Click on 'Voice' then 'Settings' tab.
> 3. Click on the 'Voice Delivery Report Settings' menu.
> 4. Select 'Forward to URL'.
> 5. Enter the URL and click 'Save'.
> The following variables will be posted to the URL specified:
> | Variable | Description |
> |---|---|
> | `timestamp_send` | Timestamp of the original send request in UNIX format. e.g 1439173980
> | `timestamp` | Timestamp of delivery report in UNIX format. e.g 1439173981
> | `message_id` | Message ID, returned when originally sending the message.
> | `status` | Delivered or Undelivered
> | `status_code` | Status code. Refer to 'Voice Delivery Status Codes' in docs.
> | `status_text` | Status text.
> | `error_code` | Error code.
> | `error_text` | Error text.
> | `custom_string` | A custom string used when sending the original message.
> | `user_id` | The user ID of the user who sent the message.
> | `subaccount_id` | The subaccount ID of the user who sent the message.
> | `message_type` | 'voice' (constant).
> | `digits` | Numbers the recipient pressed on their keypad during the call. A blank string will be used if they didn't provide any input.
> **Pull Delivery Receipts**
> Receive delivery reports by polling.
> You can poll our server and retrieve delivery reports at a time that suits you.
> 1. Log into your account.
> 2. Click on 'Voice' then 'Settings' tab.
> 3. Click on the 'Voice Delivery Report Settings' menu.
> 4. Select 'Poll our server' and click 'Save'.

```python
def update_marked_voice_receipts_as_read(self,
                                             date_before)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateBefore |  ``` Required ```  | An optional timestamp - mark all as read before this timestamp. If not given, all receipts will be marked as read. |



#### Example Usage

```python
date_before = 233.557496461346

result = voice_client.update_marked_voice_receipts_as_read(date_before)

```


### <a name="update_cancel_a_specific_voice_call"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.update_cancel_a_specific_voice_call") update_cancel_a_specific_voice_call

> TODO: Add a method description

```python
def update_cancel_a_specific_voice_call(self,
                                            message_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Your voice message id. |



#### Example Usage

```python
message_id = '7B5BFC19 06B7 49C1 8DCDFB011600E12B'

result = voice_client.update_cancel_a_specific_voice_call(message_id)

```


### <a name="update_cancel_all_voice_calls"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.update_cancel_all_voice_calls") update_cancel_all_voice_calls

> TODO: Add a method description

```python
def update_cancel_all_voice_calls(self)
```

#### Example Usage

```python

result = voice_client.update_cancel_all_voice_calls()

```


[Back to List of Controllers](#list_of_controllers)



