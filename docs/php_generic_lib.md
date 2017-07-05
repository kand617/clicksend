# Getting started

TODO: Add a description

## How to Build

The generated code has dependencies over external libraries like UniRest. These dependencies are defined in the ```composer.json``` file that comes with the SDK. 
To resolve these dependencies, we use the Composer package manager which requires PHP greater than 5.3.2 installed in your system. 
Visit [https://getcomposer.org/download/](https://getcomposer.org/download/) to download the installer file for Composer and run it in your system. 
Open command prompt and type ```composer --version```. This should display the current version of the Composer installed if the installation was successful.

* Using command line, navigate to the directory containing the generated files (including ```composer.json```) for the SDK. 
* Run the command ```composer install```. This should install all the required dependencies and create the ```vendor``` directory in your project directory.

![Building SDK - Step 1](https://apidocs.io/illustration/php?step=installDependencies&workspaceFolder=ClickSend%20REST%20API%20v3-PHP)

### [For Windows Users Only] Configuring CURL Certificate Path in php.ini

CURL used to include a list of accepted CAs, but no longer bundles ANY CA certs. So by default it will reject all SSL certificates as unverifiable. You will have to get your CA's cert and point curl at it. The steps are as follows:

1. Download the certificate bundle (.pem file) from [https://curl.haxx.se/docs/caextract.html](https://curl.haxx.se/docs/caextract.html) on to your system.
2. Add curl.cainfo = "PATH_TO/cacert.pem" to your php.ini file located in your php installation. “PATH_TO” must be an absolute path containing the .pem file.

```ini
[curl]
; A default value for the CURLOPT_CAINFO option. This is required to be an
; absolute path.
;curl.cainfo =
```

## How to Use

The following section explains how to use the ClickSendRESTAPIV3Lib library in a new project.

### 1. Open Project in an IDE

Open an IDE for PHP like PhpStorm. The basic workflow presented here is also applicable if you prefer using a different editor or IDE.

![Open project in PHPStorm - Step 1](https://apidocs.io/illustration/php?step=openIDE&workspaceFolder=ClickSend%20REST%20API%20v3-PHP)

Click on ```Open``` in PhpStorm to browse to your generated SDK directory and then click ```OK```.

![Open project in PHPStorm - Step 2](https://apidocs.io/illustration/php?step=openProject0&workspaceFolder=ClickSend%20REST%20API%20v3-PHP)     

### 2. Add a new Test Project

Create a new directory by right clicking on the solution name as shown below:

![Add a new project in PHPStorm - Step 1](https://apidocs.io/illustration/php?step=createDirectory&workspaceFolder=ClickSend%20REST%20API%20v3-PHP)

Name the directory as "test"

![Add a new project in PHPStorm - Step 2](https://apidocs.io/illustration/php?step=nameDirectory&workspaceFolder=ClickSend%20REST%20API%20v3-PHP)
   
Add a PHP file to this project

![Add a new project in PHPStorm - Step 3](https://apidocs.io/illustration/php?step=createFile&workspaceFolder=ClickSend%20REST%20API%20v3-PHP)

Name it "testSDK"

![Add a new project in PHPStorm - Step 4](https://apidocs.io/illustration/php?step=nameFile&workspaceFolder=ClickSend%20REST%20API%20v3-PHP)

Depending on your project setup, you might need to include composer's autoloader in your PHP code to enable auto loading of classes.

```PHP
require_once "../vendor/autoload.php";
```

It is important that the path inside require_once correctly points to the file ```autoload.php``` inside the vendor directory created during dependency installations.

![Add a new project in PHPStorm - Step 4](https://apidocs.io/illustration/php?step=projectFiles&workspaceFolder=ClickSend%20REST%20API%20v3-PHP)

After this you can add code to initialize the client library and acquire the instance of a Controller class. Sample code to initialize the client library and using controller methods is given in the subsequent sections.

### 3. Run the Test Project

To run your project you must set the Interpreter for your project. Interpreter is the PHP engine installed on your computer.

Open ```Settings``` from ```File``` menu.

![Run Test Project - Step 1](https://apidocs.io/illustration/php?step=openSettings&workspaceFolder=ClickSend%20REST%20API%20v3-PHP)

Select ```PHP``` from within ```Languages & Frameworks```

![Run Test Project - Step 2](https://apidocs.io/illustration/php?step=setInterpreter0&workspaceFolder=ClickSend%20REST%20API%20v3-PHP)

Browse for Interpreters near the ```Interpreter``` option and choose your interpreter.

![Run Test Project - Step 3](https://apidocs.io/illustration/php?step=setInterpreter1&workspaceFolder=ClickSend%20REST%20API%20v3-PHP)

Once the interpreter is selected, click ```OK```

![Run Test Project - Step 4](https://apidocs.io/illustration/php?step=setInterpreter2&workspaceFolder=ClickSend%20REST%20API%20v3-PHP)

To run your project, right click on your PHP file inside your Test project and click on ```Run```

![Run Test Project - Step 5](https://apidocs.io/illustration/php?step=runProject&workspaceFolder=ClickSend%20REST%20API%20v3-PHP)

## How to Test

Unit tests in this SDK can be run using PHPUnit. 

1. First install the dependencies using composer including the `require-dev` dependencies.
2. Run `vendor\bin\phpunit --verbose` from commandline to execute tests. If you have 
   installed PHPUnit globally, run tests using `phpunit --verbose` instead.

You can change the PHPUnit test configuration in the `phpunit.xml` file.

## Initialization

### Authentication
In order to setup authentication and initialization of the API client, you need the following information.

| Parameter | Description |
|-----------|-------------|
| basicAuthUserName | The username to use with basic authentication |
| basicAuthPassword | The password to use with basic authentication |



API client can be initialized as following.

```php
// Configuration parameters and credentials
$basicAuthUserName = "basicAuthUserName"; // The username to use with basic authentication
$basicAuthPassword = "basicAuthPassword"; // The password to use with basic authentication

$client = new ClickSendRESTAPIV3Lib\ClickSendRESTAPIV3LibClient($basicAuthUserName, $basicAuthPassword);
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

### Get singleton instance

The singleton instance of the ``` AccountController ``` class can be accessed from the API Client.

```php
$account = $client->getAccount();
```

### <a name="create_a_new_account"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.createANewAccount") createANewAccount

> **Note:** *Authentication isn't required to create a new account.*


```php
function createANewAccount($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "    {        \"username\":\"johndoe1\",        \"user_email\":\"johndoe1@awesome.com\",        \"user_phone\":\"518-481-1001\",        \"user_first_name\":\"John\",        \"user_last_name\":\"Doe\",        \"country\":\"US\",        \"password\":\"pass\",        \"account_name\":\"The Awesome Company\"    }";
$body = APIHelper::deserialize($bodyValue);

$result = $account->createANewAccount($body);

```


### <a name="update_account"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.updateAccount") updateAccount

> TODO: Add a method description


```php
function updateAccount($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "    {        \"username\":\"johndoe\",        \"user_email\":\"johndoe@awesome.com\",        \"user_phone\":\"518-481-1002\",        \"user_first_name\":\"John\",        \"user_last_name\":\"Doe\",        \"country\":\"AU\",        \"password\":\"pass\",        \"account_name\":\"The Awesome Company\",        \"timezone\": \"Australia/Melbourne\",        \"private_uploads\": 1,        \"setting_sms_hide_your_number\": 0,        \"setting_sms_hide_business_name\": 1    }";
$body = APIHelper::deserialize($bodyValue);

$result = $account->updateAccount($body);

```


### <a name="get_account"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.getAccount") getAccount

> TODO: Add a method description


```php
function getAccount()
```

#### Example Usage

```php

$result = $account->getAccount();

```


### <a name="get_account_usage"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.getAccountUsage") getAccountUsage

> TODO: Add a method description


```php
function getAccountUsage(
        $year,
        $month,
        $type)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| year |  ``` Required ```  | Your account usage year. |
| month |  ``` Required ```  | Your account usage month. |
| type |  ``` Required ```  | The account type. Value can only be either email or subaccount. |



#### Example Usage

```php
$year = 2016;
$month = 4;
$type = 'subaccount';

$result = $account->getAccountUsage($year, $month, $type);

```


### <a name="update_send_account_activation_token"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.updateSendAccountActivationToken") updateSendAccountActivationToken

> TODO: Add a method description


```php
function updateSendAccountActivationToken($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "    {        \"user_phone\":\"352-394-4199\",        \"type\":\"sms\",        \"country\": \"US\"    }";
$body = APIHelper::deserialize($bodyValue);

$result = $account->updateSendAccountActivationToken($body);

```


### <a name="update_verify_new_account"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.updateVerifyNewAccount") updateVerifyNewAccount

> TODO: Add a method description


```php
function updateVerifyNewAccount($activationToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| activationToken |  ``` Required ```  | The ActivationToken to be used to verify an account. |



#### Example Usage

```php
$activationToken = '1827364';

$result = $account->updateVerifyNewAccount($activationToken);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="account_recharge_controller"></a>![Class: ](https://apidocs.io/img/class.png ".AccountRechargeController") AccountRechargeController

### Get singleton instance

The singleton instance of the ``` AccountRechargeController ``` class can be accessed from the API Client.

```php
$accountRecharge = $client->getAccountRecharge();
```

### <a name="get_credit_card_info"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.getCreditCardInfo") getCreditCardInfo

> TODO: Add a method description


```php
function getCreditCardInfo()
```

#### Example Usage

```php

$result = $accountRecharge->getCreditCardInfo();

```


### <a name="update_credit_card_info"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.updateCreditCardInfo") updateCreditCardInfo

> TODO: Add a method description


```php
function updateCreditCardInfo($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$body = new UpdateCreditCardInfoRequest();

$result = $accountRecharge->updateCreditCardInfo($body);

```


### <a name="list_of_packages"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.listOfPackages") listOfPackages

> TODO: Add a method description


```php
function listOfPackages($country = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Optional ```  | Your country. |



#### Example Usage

```php
$country = '"AU"';

$result = $accountRecharge->listOfPackages($country);

```


### <a name="update_purchase_a_package"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.updatePurchaseAPackage") updatePurchaseAPackage

> TODO: Add a method description


```php
function updatePurchaseAPackage($packageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| packageId |  ``` Required ```  | Your package id. |



#### Example Usage

```php
$packageId = 1;

$result = $accountRecharge->updatePurchaseAPackage($packageId);

```


### <a name="get_transactions"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.getTransactions") getTransactions

> TODO: Add a method description


```php
function getTransactions()
```

#### Example Usage

```php

$result = $accountRecharge->getTransactions();

```


### <a name="get_a_specific_transaction"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.getASpecificTransaction") getASpecificTransaction

> TODO: Add a method description


```php
function getASpecificTransaction($transactionId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| transactionId |  ``` Required ```  | 1c65-47fa-aea2-3ded9ed57557 (number, required) - Your transction id. |



#### Example Usage

```php
$transactionId = 'transaction_id';

$result = $accountRecharge->getASpecificTransaction($transactionId);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="automation_rules_controller"></a>![Class: ](https://apidocs.io/img/class.png ".AutomationRulesController") AutomationRulesController

### Get singleton instance

The singleton instance of the ``` AutomationRulesController ``` class can be accessed from the API Client.

```php
$automationRules = $client->getAutomationRules();
```

### <a name="list_rules"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.listRules") listRules

> TODO: Add a method description


```php
function listRules()
```

#### Example Usage

```php

$result = $automationRules->listRules();

```


### <a name="get_a_specific_rule"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.getASpecificRule") getASpecificRule

> TODO: Add a method description


```php
function getASpecificRule($inboundRuleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Inbound Rule ID. |



#### Example Usage

```php
$inboundRuleId = 1;

$result = $automationRules->getASpecificRule($inboundRuleId);

```


### <a name="create_a_new_rule"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.createANewRule") createANewRule

> TODO: Add a method description


```php
function createANewRule($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$body = new CreateANewRuleRequest();

$result = $automationRules->createANewRule($body);

```


### <a name="update_a_rule"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.updateARule") updateARule

> TODO: Add a method description


```php
function updateARule(
        $inboundRuleId,
        $body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Inbound Rule ID. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$inboundRuleId = 1;
$bodyValue = "{    \"dedicated_number\":\"+61298441484\",    \"rule_name\":\"My Rule\",    \"message_search_type\":3,    \"message_search_term\":\"My Search Term\",    \"action\":\"EMAIL_FIXED\",    \"action_address\":\"john@doe.com\",    \"enabled\":1}";
$body = APIHelper::deserialize($bodyValue);

$result = $automationRules->updateARule($inboundRuleId, $body);

```


### <a name="delete_a_rule"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.deleteARule") deleteARule

> TODO: Add a method description


```php
function deleteARule($inboundRuleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Inbound Rule ID. |



#### Example Usage

```php
$inboundRuleId = 1;

$result = $automationRules->deleteARule($inboundRuleId);

```


### <a name="list_rules1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.listRules1") listRules1

> TODO: Add a method description


```php
function listRules1()
```

#### Example Usage

```php

$result = $automationRules->listRules1();

```


### <a name="get_a_specific_rule1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.getASpecificRule1") getASpecificRule1

> TODO: Add a method description


```php
function getASpecificRule1($receiptRuleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |



#### Example Usage

```php
$receiptRuleId = 2;

$result = $automationRules->getASpecificRule1($receiptRuleId);

```


### <a name="create_a_new_rule1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.createANewRule1") createANewRule1

> TODO: Add a method description


```php
function createANewRule1($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "{    \"rule_name\": \"My Rule\",    \"match_type\": 3,    \"action\": \"EMAIL_FIXED\",    \"action_address\": \"john@doe.com\",    \"enabled\": 1}";
$body = APIHelper::deserialize($bodyValue);

$result = $automationRules->createANewRule1($body);

```


### <a name="update_a_rule1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.updateARule1") updateARule1

> TODO: Add a method description


```php
function updateARule1(
        $receiptRuleId,
        $body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$receiptRuleId = 7;
$bodyValue = "{    \"rule_name\": \"My Rule\",    \"match_type\": 3,    \"action\": \"EMAIL_FIXED\",    \"action_address\": \"john@doe.com\",    \"enabled\": 1}";
$body = APIHelper::deserialize($bodyValue);

$result = $automationRules->updateARule1($receiptRuleId, $body);

```


### <a name="delete_a_rule1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.deleteARule1") deleteARule1

> TODO: Add a method description


```php
function deleteARule1($receiptRuleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |



#### Example Usage

```php
$receiptRuleId = 7;

$result = $automationRules->deleteARule1($receiptRuleId);

```


### <a name="list_rules2"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.listRules2") listRules2

> TODO: Add a method description


```php
function listRules2()
```

#### Example Usage

```php

$result = $automationRules->listRules2();

```


### <a name="get_a_specific_rule11"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.getASpecificRule11") getASpecificRule11

> TODO: Add a method description


```php
function getASpecificRule11($receiptRuleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |



#### Example Usage

```php
$receiptRuleId = 2;

$result = $automationRules->getASpecificRule11($receiptRuleId);

```


### <a name="create_a_new_rule2"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.createANewRule2") createANewRule2

> TODO: Add a method description


```php
function createANewRule2($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "{    \"rule_name\":\"My Rule\",    \"match_type\":3,    \"action\":\"EMAIL_FIXED\",    \"action_address\":\"john@doe.com\",    \"enabled\":1}";
$body = APIHelper::deserialize($bodyValue);

$result = $automationRules->createANewRule2($body);

```


### <a name="update_a_rule11"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.updateARule11") updateARule11

> TODO: Add a method description


```php
function updateARule11(
        $receiptRuleId,
        $body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$receiptRuleId = 2;
$bodyValue = "{    \"rule_name\":\"My Rule\",    \"match_type\":3,    \"action\":\"EMAIL_FIXED\",    \"action_address\":\"john@doe.com\",    \"enabled\":1}";
$body = APIHelper::deserialize($bodyValue);

$result = $automationRules->updateARule11($receiptRuleId, $body);

```


### <a name="delete_a_rule11"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.deleteARule11") deleteARule11

> TODO: Add a method description


```php
function deleteARule11($receiptRuleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |



#### Example Usage

```php
$receiptRuleId = 2;

$result = $automationRules->deleteARule11($receiptRuleId);

```


### <a name="list_rules3"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.listRules3") listRules3

> TODO: Add a method description


```php
function listRules3()
```

#### Example Usage

```php

$result = $automationRules->listRules3();

```


### <a name="get_a_specific_rule111"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.getASpecificRule111") getASpecificRule111

> TODO: Add a method description


```php
function getASpecificRule111($inboundRuleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Fax inbound rule id |



#### Example Usage

```php
$inboundRuleId = 14;

$result = $automationRules->getASpecificRule111($inboundRuleId);

```


### <a name="create_a_new_rule3"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.createANewRule3") createANewRule3

> TODO: Add a method description


```php
function createANewRule3($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "    {        \"dedicated_number\":\"+61298441484\",        \"rule_name\":\"Rule Name\",        \"action\":\"EMAIL_FIXED\",        \"action_address\":\"email@domain.com\",        \"enabled\":1    }";
$body = APIHelper::deserialize($bodyValue);

$result = $automationRules->createANewRule3($body);

```


### <a name="update_a_rule111"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.updateARule111") updateARule111

> TODO: Add a method description


```php
function updateARule111(
        $inboundRuleId,
        $body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Fax inbound rule id |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$inboundRuleId = 14;
$bodyValue = "    {        \"dedicated_number\":\"+61298441484\",        \"rule_name\":\"Rule Name\",        \"action\":\"EMAIL_FIXED\",        \"action_address\":\"email@domain.com\",        \"enabled\":1    }";
$body = APIHelper::deserialize($bodyValue);

$result = $automationRules->updateARule111($inboundRuleId, $body);

```


### <a name="delete_a_rule111"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.deleteARule111") deleteARule111

> TODO: Add a method description


```php
function deleteARule111($inboundRuleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Fax inbound rule id |



#### Example Usage

```php
$inboundRuleId = 14;

$result = $automationRules->deleteARule111($inboundRuleId);

```


### <a name="list_rules4"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.listRules4") listRules4

> TODO: Add a method description


```php
function listRules4()
```

#### Example Usage

```php

$result = $automationRules->listRules4();

```


### <a name="get_a_specific_rule2"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.getASpecificRule2") getASpecificRule2

> TODO: Add a method description


```php
function getASpecificRule2($ruleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |



#### Example Usage

```php
$ruleId = 4;

$result = $automationRules->getASpecificRule2($ruleId);

```


### <a name="create_a_new_rule4"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.createANewRule4") createANewRule4

> TODO: Add a method description


```php
function createANewRule4($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "    {        \"rule_name\":\"My Rule\",        \"match_type\":2,        \"action\":\"EMAIL_FIXED\",        \"action_address\":\"john@doe.com\",        \"enabled\":1    }";
$body = APIHelper::deserialize($bodyValue);

$result = $automationRules->createANewRule4($body);

```


### <a name="update_a_rule2"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.updateARule2") updateARule2

> TODO: Add a method description


```php
function updateARule2(
        $ruleId,
        $body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$ruleId = 4;
$bodyValue = "    {        \"rule_name\":\"My Rule\",        \"match_type\":1,        \"action\":\"EMAIL_FIXED\",        \"action_address\":\"john@doe.com\",        \"enabled\":1    }";
$body = APIHelper::deserialize($bodyValue);

$result = $automationRules->updateARule2($ruleId, $body);

```


### <a name="delete_a_rule2"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.deleteARule2") deleteARule2

> TODO: Add a method description


```php
function deleteARule2($ruleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to delete. |



#### Example Usage

```php
$ruleId = 133.171276018569;

$result = $automationRules->deleteARule2($ruleId);

```


### <a name="list_rules5"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.listRules5") listRules5

> TODO: Add a method description


```php
function listRules5()
```

#### Example Usage

```php

$result = $automationRules->listRules5();

```


### <a name="get_a_specific_rule12"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.getASpecificRule12") getASpecificRule12

> TODO: Add a method description


```php
function getASpecificRule12($ruleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |



#### Example Usage

```php
$ruleId = 5;

$result = $automationRules->getASpecificRule12($ruleId);

```


### <a name="create_a_new_rule5"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.createANewRule5") createANewRule5

> TODO: Add a method description


```php
function createANewRule5($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "    {        \"rule_name\":\"My Rule\",        \"match_type\": 0,        \"action\":\"URL\",        \"action_address\":\"http://testurl.com\",        \"enabled\":1    }";
$body = APIHelper::deserialize($bodyValue);

$result = $automationRules->createANewRule5($body);

```


### <a name="update_a_rule12"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.updateARule12") updateARule12

> TODO: Add a method description


```php
function updateARule12(
        $ruleId,
        $body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$ruleId = 8;
$bodyValue = "    {        \"rule_name\":\"My Rule\",        \"match_type\": 0,        \"action\":\"URL\",        \"action_address\":\"http://testurl.com\",        \"enabled\":1    }";
$body = APIHelper::deserialize($bodyValue);

$result = $automationRules->updateARule12($ruleId, $body);

```


### <a name="delete_a_rule12"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.deleteARule12") deleteARule12

> TODO: Add a method description


```php
function deleteARule12($ruleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to delete. |



#### Example Usage

```php
$ruleId = 8;

$result = $automationRules->deleteARule12($ruleId);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="contact_lists_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ContactListsController") ContactListsController

### Get singleton instance

The singleton instance of the ``` ContactListsController ``` class can be accessed from the API Client.

```php
$contactLists = $client->getContactLists();
```

### <a name="get_all_contact_lists"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.getAllContactLists") getAllContactLists

> TODO: Add a method description


```php
function getAllContactLists()
```

#### Example Usage

```php

$result = $contactLists->getAllContactLists();

```


### <a name="create_a_new_contact_list"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.createANewContactList") createANewContactList

> TODO: Add a method description


```php
function createANewContactList($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "    {        \"list_name\":\"ListCT3QrVL4od\"    }";
$body = APIHelper::deserialize($bodyValue);

$result = $contactLists->createANewContactList($body);

```


### <a name="get_a_specific_contact_list"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.getASpecificContactList") getASpecificContactList

> TODO: Add a method description


```php
function getASpecificContactList($listId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |



#### Example Usage

```php
$listId = 437;

$result = $contactLists->getASpecificContactList($listId);

```


### <a name="update_a_specific_contact_list"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.updateASpecificContactList") updateASpecificContactList

> TODO: Add a method description


```php
function updateASpecificContactList(
        $listId,
        $body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$listId = 439;
$bodyValue = "    {        \"list_name\":\"ListlPJf33ksjP\"    }";
$body = APIHelper::deserialize($bodyValue);

$result = $contactLists->updateASpecificContactList($listId, $body);

```


### <a name="delete_a_specific_contact_list"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.deleteASpecificContactList") deleteASpecificContactList

> TODO: Add a method description


```php
function deleteASpecificContactList($listId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |



#### Example Usage

```php
$listId = 442;

$result = $contactLists->deleteASpecificContactList($listId);

```


### <a name="create_import_contacts_to_list"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.createImportContactsToList") createImportContactsToList

> TODO: Add a method description


```php
function createImportContactsToList(
        $listId,
        $body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$listId = 437;
$bodyValue = "{    \"file_url\":\"http://yourdomain.com/5485EA6144/79E8/import.csv\",    \"field_order\":[        \"phone\",        \"first_name\",        \"last_name\",        \"custom1\",        \"custom2\",        \"custom3\",        \"custom4\",        \"fax_number\",        \"organization_name\",        \"email\",        \"address_line_1\",        \"address_line_2\",        \"address_city\",        \"address_state\",        \"address_postal_code\",        \"address_country\"    ]}";
$body = APIHelper::deserialize($bodyValue);

$result = $contactLists->createImportContactsToList($listId, $body);

```


### <a name="update_remove_duplicate_contacts"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.updateRemoveDuplicateContacts") updateRemoveDuplicateContacts

> TODO: Add a method description


```php
function updateRemoveDuplicateContacts(
        $listId,
        $body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$listId = 439;
$bodyValue = "{    \"fields\":[        \"phone_number\",        \"first_name\",        \"last_name\",        \"fax_number\",        \"address_country\"    ]}";
$body = APIHelper::deserialize($bodyValue);

$result = $contactLists->updateRemoveDuplicateContacts($listId, $body);

```


### <a name="get_list_of_acceptable_import_fields"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.getListOfAcceptableImportFields") getListOfAcceptableImportFields

> TODO: Add a method description


```php
function getListOfAcceptableImportFields($listId = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Optional ```  | TODO: Add a parameter description |



#### Example Usage

```php
$listId = 'list_id';

$result = $contactLists->getListOfAcceptableImportFields($listId);

```


### <a name="create_show_csv_import_file_preview"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.createShowCSVImportFilePreview") createShowCSVImportFilePreview

> Show first row of the csv import file.


```php
function createShowCSVImportFilePreview(
        $listId,
        $body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$listId = 439;
$bodyValue = "{    \"file_url\":\"http://yourdomain.com/5485EA6144/79E8/import.csv\"}";
$body = APIHelper::deserialize($bodyValue);

$result = $contactLists->createShowCSVImportFilePreview($listId, $body);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="contact_suggestions_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ContactSuggestionsController") ContactSuggestionsController

### Get singleton instance

The singleton instance of the ``` ContactSuggestionsController ``` class can be accessed from the API Client.

```php
$contactSuggestions = $client->getContactSuggestions();
```

### <a name="list_contact_suggestions"></a>![Method: ](https://apidocs.io/img/method.png ".ContactSuggestionsController.listContactSuggestions") listContactSuggestions

> TODO: Add a method description


```php
function listContactSuggestions()
```

#### Example Usage

```php

$result = $contactSuggestions->listContactSuggestions();

```


[Back to List of Controllers](#list_of_controllers)

## <a name="contacts_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ContactsController") ContactsController

### Get singleton instance

The singleton instance of the ``` ContactsController ``` class can be accessed from the API Client.

```php
$contacts = $client->getContacts();
```

### <a name="get_all_contacts_in_a_list"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.getAllContactsInAList") getAllContactsInAList

> TODO: Add a method description


```php
function getAllContactsInAList($listId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id where your contacts belong. |



#### Example Usage

```php
$listId = 428;

$result = $contacts->getAllContactsInAList($listId);

```


### <a name="create_a_new_contact"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.createANewContact") createANewContact

> TODO: Add a method description


```php
function createANewContact(
        $listId,
        $body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id where your contact be associated. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$listId = 428;
$bodyValue = "    {        \"phone_number\":\"+16783270696\",        \"first_name\":\"Ellen\",        \"last_name\":\"Diaz\",        \"custom_1\":\"Custom 1\",        \"custom_2\":\"Custom 2\",        \"custom_3\":\"Custom 3\",        \"custom_4\":\"Custom 4\",        \"fax_number\":\"+16783270696\",        \"organization_name\":\"Awesome Organization\",        \"email\":\"ellen@diaz.com\",        \"address_line_1\":\"Block 2\",        \"address_line_2\":\"Cool Bldg.\",        \"address_city\":\"Nevada\",        \"address_state\":\"Las Vegas\",        \"address_postal_code\":\"36063\",        \"address_country\":\"US\"    }";
$body = APIHelper::deserialize($bodyValue);

$result = $contacts->createANewContact($listId, $body);

```


### <a name="get_a_specific_contact"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.getASpecificContact") getASpecificContact

> TODO: Add a method description


```php
function getASpecificContact(
        $listId,
        $contactId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| contactId |  ``` Required ```  | Your contact id you want to access. |



#### Example Usage

```php
$listId = 428;
$contactId = 552802;

$result = $contacts->getASpecificContact($listId, $contactId);

```


### <a name="update_a_specific_contact"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.updateASpecificContact") updateASpecificContact

> TODO: Add a method description


```php
function updateASpecificContact(
        $listId,
        $contactId,
        $body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| contactId |  ``` Required ```  | Your contact id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$listId = 428;
$contactId = 552802;
$bodyValue = "{        \"phone_number\":\"+16783275492\",        \"first_name\":\"Ellen\",        \"last_name\":\"Diaz\",        \"custom_1\":\"Custom S72oJ9Teba\",        \"custom_2\":\"Custom NvrRJrKWeq\",        \"custom_3\":\"Custom 2ws94p1Dop\",        \"custom_4\":\"Custom Ku0AaIS5xb\",        \"fax_number\":\"+16783276356\",        \"organization_name\":\"Awesome Organization\",        \"email\":\"ellen@diaz.com\",        \"address_line_1\":\"Block 6\",        \"address_line_2\":\"Cool Bldg.\",        \"address_city\":\"Nevada\",        \"address_state\":\"Las Vegas\",        \"address_postal_code\":\"36063\",        \"address_country\":\"US\"    }";
$body = APIHelper::deserialize($bodyValue);

$result = $contacts->updateASpecificContact($listId, $contactId, $body);

```


### <a name="delete_a_specific_contact"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.deleteASpecificContact") deleteASpecificContact

> TODO: Add a method description


```php
function deleteASpecificContact(
        $listId,
        $contactId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| contactId |  ``` Required ```  | Your contact id you want to access. |



#### Example Usage

```php
$listId = 428;
$contactId = 552807;

$result = $contacts->deleteASpecificContact($listId, $contactId);

```


### <a name="update_remove_opted_out_contacts"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.updateRemoveOptedOutContacts") updateRemoveOptedOutContacts

> TODO: Add a method description


```php
function updateRemoveOptedOutContacts(
        $listId,
        $optOutListId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id. |
| optOutListId |  ``` Required ```  | Your opt out list id. |



#### Example Usage

```php
$listId = 439;
$optOutListId = 512;

$result = $contacts->updateRemoveOptedOutContacts($listId, $optOutListId);

```


### <a name="update_transfer_a_contact"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.updateTransferAContact") updateTransferAContact

> Transfers a specific contact to another list.


```php
function updateTransferAContact(
        $fromListId,
        $contactId,
        $toListId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| fromListId |  ``` Required ```  | From list id. |
| contactId |  ``` Required ```  | Contact ID. |
| toListId |  ``` Required ```  | To list id. |



#### Example Usage

```php
$fromListId = 428;
$contactId = 1;
$toListId = 429;

$result = $contacts->updateTransferAContact($fromListId, $contactId, $toListId);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="countries_controller"></a>![Class: ](https://apidocs.io/img/class.png ".CountriesController") CountriesController

### Get singleton instance

The singleton instance of the ``` CountriesController ``` class can be accessed from the API Client.

```php
$countries = $client->getCountries();
```

### <a name="get_all_countries"></a>![Method: ](https://apidocs.io/img/method.png ".CountriesController.getAllCountries") getAllCountries

> TODO: Add a method description


```php
function getAllCountries()
```

#### Example Usage

```php

$result = $countries->getAllCountries();

```


[Back to List of Controllers](#list_of_controllers)

## <a name="delivery_issues_controller"></a>![Class: ](https://apidocs.io/img/class.png ".DeliveryIssuesController") DeliveryIssuesController

### Get singleton instance

The singleton instance of the ``` DeliveryIssuesController ``` class can be accessed from the API Client.

```php
$deliveryIssues = $client->getDeliveryIssues();
```

### <a name="get_delivery_issues"></a>![Method: ](https://apidocs.io/img/method.png ".DeliveryIssuesController.getDeliveryIssues") getDeliveryIssues

> TODO: Add a method description


```php
function getDeliveryIssues()
```

#### Example Usage

```php

$result = $deliveryIssues->getDeliveryIssues();

```


### <a name="create_delivery_issue"></a>![Method: ](https://apidocs.io/img/method.png ".DeliveryIssuesController.createDeliveryIssue") createDeliveryIssue

> TODO: Add a method description


```php
function createDeliveryIssue($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "{  \"message_id\": \"B388828B\",  \"type\": \"SMS\",  \"description\": \"This is a test\",  \"client_comments\": \"test\",  \"email_address: john_doe@user.com\": \"\",  \"Body\": \"\"}";
$body = APIHelper::deserialize($bodyValue);

$result = $deliveryIssues->createDeliveryIssue($body);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="email_marketing_controller"></a>![Class: ](https://apidocs.io/img/class.png ".EmailMarketingController") EmailMarketingController

### Get singleton instance

The singleton instance of the ``` EmailMarketingController ``` class can be accessed from the API Client.

```php
$emailMarketing = $client->getEmailMarketing();
```

### <a name="get_all_allowed_email_addresses"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getAllAllowedEmailAddresses") getAllAllowedEmailAddresses

> TODO: Add a method description


```php
function getAllAllowedEmailAddresses()
```

#### Example Usage

```php

$result = $emailMarketing->getAllAllowedEmailAddresses();

```


### <a name="create_allowed_email_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.createAllowedEmailAddress") createAllowedEmailAddress

> TODO: Add a method description


```php
function createAllowedEmailAddress($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "{  \"email_address\": \"johndoe1@user.com\",  \"Body\": \"\"}";
$body = APIHelper::deserialize($bodyValue);

$result = $emailMarketing->createAllowedEmailAddress($body);

```


### <a name="update_send_verification_token"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.updateSendVerificationToken") updateSendVerificationToken

> TODO: Add a method description


```php
function updateSendVerificationToken($emailAddressId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email addess id you want to access. |



#### Example Usage

```php
$emailAddressId = 61.1618398018935;

$result = $emailMarketing->updateSendVerificationToken($emailAddressId);

```


### <a name="update_verify_allowed_email_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.updateVerifyAllowedEmailAddress") updateVerifyAllowedEmailAddress

> TODO: Add a method description


```php
function updateVerifyAllowedEmailAddress(
        $emailAddressId,
        $activationToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email address id you want to access. |
| activationToken |  ``` Required ```  | 6E8B-4FDB-99A7-7ED08DF97BCC (required, string) - Your activation token. |



#### Example Usage

```php
$emailAddressId = 5;
$activationToken = '3BD73304';

$result = $emailMarketing->updateVerifyAllowedEmailAddress($emailAddressId, $activationToken);

```


### <a name="delete_allowed_email_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.deleteAllowedEmailAddress") deleteAllowedEmailAddress

> TODO: Add a method description


```php
function deleteAllowedEmailAddress($emailAddressId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email address you want to access. |



#### Example Usage

```php
$emailAddressId = 61.1618398018935;

$result = $emailMarketing->deleteAllowedEmailAddress($emailAddressId);

```


### <a name="get_specific_allowed_email_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getSpecificAllowedEmailAddress") getSpecificAllowedEmailAddress

> TODO: Add a method description


```php
function getSpecificAllowedEmailAddress($emailAddressId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email address you want to access. |



#### Example Usage

```php
$emailAddressId = 4;

$result = $emailMarketing->getSpecificAllowedEmailAddress($emailAddressId);

```


### <a name="get_all_email_campaigns"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getAllEmailCampaigns") getAllEmailCampaigns

> TODO: Add a method description


```php
function getAllEmailCampaigns()
```

#### Example Usage

```php

$result = $emailMarketing->getAllEmailCampaigns();

```


### <a name="get_specific_email_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getSpecificEmailCampaign") getSpecificEmailCampaign

> TODO: Add a method description


```php
function getSpecificEmailCampaign($emailCampaignId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailCampaignId |  ``` Required ```  | The email campaign id you want to access. |



#### Example Usage

```php
$emailCampaignId = 1;

$result = $emailMarketing->getSpecificEmailCampaign($emailCampaignId);

```


### <a name="create_email_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.createEmailCampaign") createEmailCampaign

> TODO: Add a method description


```php
function createEmailCampaign($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "{  \"name\" : \"John Doe\",  \"subject\" : \"Lorem Ipsum\",  \"from_email_address_id\" : 2,  \"from_name\" : \"From name\",  \"template_id\" : 31,  \"body\" : \"<p>This is a test</p>\",  \"list_id\" : 456}";
$body = APIHelper::deserialize($bodyValue);

$result = $emailMarketing->createEmailCampaign($body);

```


### <a name="update_email_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.updateEmailCampaign") updateEmailCampaign

> TODO: Add a method description


```php
function updateEmailCampaign(
        $emailCampaignId,
        $body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailCampaignId |  ``` Required ```  | The email campaign id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$emailCampaignId = 1;
$bodyValue = "{  \"name\" : \"John Doe\",  \"subject\" : \"Lorem Ipsum\",  \"from_email_address_id\" : 2,  \"from_name\" : \"From name\",  \"template_id\" : 31,  \"body\" : \"<p>This is a test</p>\",  \"list_id\" : 456}";
$body = APIHelper::deserialize($bodyValue);

$result = $emailMarketing->updateEmailCampaign($emailCampaignId, $body);

```


### <a name="update_cancel_email_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.updateCancelEmailCampaign") updateCancelEmailCampaign

> TODO: Add a method description


```php
function updateCancelEmailCampaign($emailCampaignId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailCampaignId |  ``` Required ```  | The email campaign id you want to cancel. |



#### Example Usage

```php
$emailCampaignId = 1;

$result = $emailMarketing->updateCancelEmailCampaign($emailCampaignId);

```


### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.createCalculatePrice") createCalculatePrice

> TODO: Add a method description


```php
function createCalculatePrice($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "{  \"name\" : \"John Doe\",  \"subject\" : \"Lorem Ipsum\",  \"from_email_address_id\" : 2,  \"from_name\" : \"From name\",  \"template_id\" : 31,  \"body\" : \"<p>This is a test</p>\",  \"list_id\" : 456}";
$body = APIHelper::deserialize($bodyValue);

$result = $emailMarketing->createCalculatePrice($body);

```


### <a name="get_specific_email_campaign_history"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getSpecificEmailCampaignHistory") getSpecificEmailCampaignHistory

> TODO: Add a method description


```php
function getSpecificEmailCampaignHistory($campaignId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| campaignId |  ``` Required ```  | The email campaign id you want to access. |



#### Example Usage

```php
$campaignId = 77;

$result = $emailMarketing->getSpecificEmailCampaignHistory($campaignId);

```


### <a name="get_all_email_templates"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getAllEmailTemplates") getAllEmailTemplates

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```php
function getAllEmailTemplates()
```

#### Example Usage

```php

$result = $emailMarketing->getAllEmailTemplates();

```


### <a name="get_specific_email_template"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getSpecificEmailTemplate") getSpecificEmailTemplate

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```php
function getSpecificEmailTemplate($templateId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | The email template id. |



#### Example Usage

```php
$templateId = 291;

$result = $emailMarketing->getSpecificEmailTemplate($templateId);

```


### <a name="create_new_email_template_from_master_template"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.createNewEmailTemplateFromMasterTemplate") createNewEmailTemplateFromMasterTemplate

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```php
function createNewEmailTemplateFromMasterTemplate($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "{  \"template_name\": \"Minions\",  \"template_id_master\": 57}";
$body = APIHelper::deserialize($bodyValue);

$result = $emailMarketing->createNewEmailTemplateFromMasterTemplate($body);

```


### <a name="update_an_email_template"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.updateAnEmailTemplate") updateAnEmailTemplate

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```php
function updateAnEmailTemplate(
        $templateId,
        $body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | The id of the template to be updated. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$templateId = 291;
$bodyValue = "    {        \"template_name\":\"Minions\",        \"body\":\"This is a sample content: Sc0KNWgSMG for this template.\"    }";
$body = APIHelper::deserialize($bodyValue);

$result = $emailMarketing->updateAnEmailTemplate($templateId, $body);

```


### <a name="delete_email_template"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.deleteEmailTemplate") deleteEmailTemplate

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```php
function deleteEmailTemplate($templateId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |



#### Example Usage

```php
$templateId = 25;

$result = $emailMarketing->deleteEmailTemplate($templateId);

```


### <a name="get_all_master_email_templates"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getAllMasterEmailTemplates") getAllMasterEmailTemplates

> Master templates are templates that you can clone to a User Email Template which lets you edit and save it.


```php
function getAllMasterEmailTemplates()
```

#### Example Usage

```php

$result = $emailMarketing->getAllMasterEmailTemplates();

```


### <a name="get_specific_master_template"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getSpecificMasterTemplate") getSpecificMasterTemplate

> Master templates are templates that you can clone to a User Email Template which lets you edit and save it.


```php
function getSpecificMasterTemplate($templateId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |



#### Example Usage

```php
$templateId = '25';

$result = $emailMarketing->getSpecificMasterTemplate($templateId);

```


### <a name="get_all_master_template_categories"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getAllMasterTemplateCategories") getAllMasterTemplateCategories

> TODO: Add a method description


```php
function getAllMasterTemplateCategories()
```

#### Example Usage

```php

$result = $emailMarketing->getAllMasterTemplateCategories();

```


### <a name="get_specific_email_template_category"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getSpecificEmailTemplateCategory") getSpecificEmailTemplateCategory

> TODO: Add a method description


```php
function getSpecificEmailTemplateCategory($categoryId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| categoryId |  ``` Required ```  | Your category id. |



#### Example Usage

```php
$categoryId = '25';

$result = $emailMarketing->getSpecificEmailTemplateCategory($categoryId);

```


### <a name="get_all_templates_for_category"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getAllTemplatesForCategory") getAllTemplatesForCategory

> TODO: Add a method description


```php
function getAllTemplatesForCategory($categoryId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| categoryId |  ``` Required ```  | Your category id. |



#### Example Usage

```php
$categoryId = '1';

$result = $emailMarketing->getAllTemplatesForCategory($categoryId);

```


### <a name="upload_image_to_specific_template"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.uploadImageToSpecificTemplate") uploadImageToSpecificTemplate

> TODO: Add a method description


```php
function uploadImageToSpecificTemplate(
        $templateId,
        $body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$templateId = '1';
$bodyValue = "{    \"image\": \"image.png\",    \"url\" : \"http://www.downloadimg.from/here.png\"}";
$body = APIHelper::deserialize($bodyValue);

$result = $emailMarketing->uploadImageToSpecificTemplate($templateId, $body);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="email_to_sms_allowed_address_controller"></a>![Class: ](https://apidocs.io/img/class.png ".EmailToSMSAllowedAddressController") EmailToSMSAllowedAddressController

### Get singleton instance

The singleton instance of the ``` EmailToSMSAllowedAddressController ``` class can be accessed from the API Client.

```php
$emailToSMSAllowedAddress = $client->getEmailToSMSAllowedAddress();
```

### <a name="list_of_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSAllowedAddressController.listOfEmailToSMSAllowedAddress") listOfEmailToSMSAllowedAddress

> Get list of allowed email addresses.


```php
function listOfEmailToSMSAllowedAddress()
```

#### Example Usage

```php

$result = $emailToSMSAllowedAddress->listOfEmailToSMSAllowedAddress();

```


### <a name="create_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSAllowedAddressController.createEmailToSMSAllowedAddress") createEmailToSMSAllowedAddress

> Create an allowed email address.


```php
function createEmailToSMSAllowedAddress($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "    {        \"email_address\":\"Cv3p0@gmail.com\",        \"from\":\"+17128845887\"    }";
$body = APIHelper::deserialize($bodyValue);

$result = $emailToSMSAllowedAddress->createEmailToSMSAllowedAddress($body);

```


### <a name="get_specific_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSAllowedAddressController.getSpecificEmailToSMSAllowedAddress") getSpecificEmailToSMSAllowedAddress

> Get a specific allowed email address.


```php
function getSpecificEmailToSMSAllowedAddress($emailAddressId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | Your email address id. |



#### Example Usage

```php
$emailAddressId = 113;

$result = $emailToSMSAllowedAddress->getSpecificEmailToSMSAllowedAddress($emailAddressId);

```


### <a name="update_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSAllowedAddressController.updateEmailToSMSAllowedAddress") updateEmailToSMSAllowedAddress

> Update a specific allowed email address.


```php
function updateEmailToSMSAllowedAddress(
        $emailAddressId,
        $body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | Your email address id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$emailAddressId = 107;
$bodyValue = "    {        \"email_address\":\"pfvRZ@gmail.com\",        \"from\":\"+17128842283\"    }";
$body = APIHelper::deserialize($bodyValue);

$result = $emailToSMSAllowedAddress->updateEmailToSMSAllowedAddress($emailAddressId, $body);

```


### <a name="delete_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSAllowedAddressController.deleteEmailToSMSAllowedAddress") deleteEmailToSMSAllowedAddress

> Delete a specific allowed email address.


```php
function deleteEmailToSMSAllowedAddress($emailAddressId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | Your email address id. |



#### Example Usage

```php
$emailAddressId = 107;

$result = $emailToSMSAllowedAddress->deleteEmailToSMSAllowedAddress($emailAddressId);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="email_to_sms_stripped_strings_controller"></a>![Class: ](https://apidocs.io/img/class.png ".EmailToSMSStrippedStringsController") EmailToSMSStrippedStringsController

### Get singleton instance

The singleton instance of the ``` EmailToSMSStrippedStringsController ``` class can be accessed from the API Client.

```php
$emailToSMSStrippedStrings = $client->getEmailToSMSStrippedStrings();
```

### <a name="list_stripped_strings"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSStrippedStringsController.listStrippedStrings") listStrippedStrings

> TODO: Add a method description


```php
function listStrippedStrings()
```

#### Example Usage

```php

$result = $emailToSMSStrippedStrings->listStrippedStrings();

```


### <a name="find_specific_stripped_string"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSStrippedStringsController.findSpecificStrippedString") findSpecificStrippedString

> TODO: Add a method description


```php
function findSpecificStrippedString($ruleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |



#### Example Usage

```php
$ruleId = 18;

$result = $emailToSMSStrippedStrings->findSpecificStrippedString($ruleId);

```


### <a name="create_stripped_string"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSStrippedStringsController.createStrippedString") createStrippedString

> TODO: Add a method description


```php
function createStrippedString($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "{    \"strip_string\" : \"~~~test~~~\"}";
$body = APIHelper::deserialize($bodyValue);

$result = $emailToSMSStrippedStrings->createStrippedString($body);

```


### <a name="update_stripped_string"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSStrippedStringsController.updateStrippedString") updateStrippedString

> TODO: Add a method description


```php
function updateStrippedString(
        $ruleId,
        $body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$ruleId = 20;
$bodyValue = "{    \"strip_string\" : \"~~~test1~~~\"}";
$body = APIHelper::deserialize($bodyValue);

$result = $emailToSMSStrippedStrings->updateStrippedString($ruleId, $body);

```


### <a name="delete_stripped_string"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSStrippedStringsController.deleteStrippedString") deleteStrippedString

> TODO: Add a method description


```php
function deleteStrippedString($ruleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |



#### Example Usage

```php
$ruleId = 20;

$result = $emailToSMSStrippedStrings->deleteStrippedString($ruleId);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="fax_controller"></a>![Class: ](https://apidocs.io/img/class.png ".FaxController") FaxController

### Get singleton instance

The singleton instance of the ``` FaxController ``` class can be accessed from the API Client.

```php
$fax = $client->getFax();
```

### <a name="create_send_fax"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.createSendFax") createSendFax

> **Letter File Options**
> **Use existing URL**
> With this option, you can use an existing URL to a PDF document. For example, you might generate the pdf on your server.
> **Upload File to Our Server**
> With this option, you can use the `/uploads` endpoint to upload the document. The `/uploads` endpoint returns a URL that can be used in the `/fax/send` endpoint.


```php
function createSendFax($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$body = new SendFaxRequest();

$result = $fax->createSendFax($body);

```


### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.createCalculatePrice") createCalculatePrice

> TODO: Add a method description


```php
function createCalculatePrice($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$body = new CalculatePriceRequest132();

$result = $fax->createCalculatePrice($body);

```


### <a name="get_fax_history"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.getFaxHistory") getFaxHistory

> Get a list of Fax History.


```php
function getFaxHistory(
        $dateFrom = null,
        $dateTo = null,
        $q = null,
        $orderBy = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateFrom |  ``` Optional ```  | Customize result by setting from date (timestsamp) |
| dateTo |  ``` Optional ```  | Customize result by setting to date (timestamp) |
| q |  ``` Optional ```  | Custom query |
| orderBy |  ``` Optional ```  | Order result by |



#### Example Usage

```php
$dateFrom = 1457572619;
$dateTo = 1457573000;
$q = 'status:Sent,status_code:201';
$orderBy = 'subject:desc';

$result = $fax->getFaxHistory($dateFrom, $dateTo, $q, $orderBy);

```


### <a name="list_of_fax_delivery_receipts"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.listOfFaxDeliveryReceipts") listOfFaxDeliveryReceipts

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


```php
function listOfFaxDeliveryReceipts()
```

#### Example Usage

```php

$result = $fax->listOfFaxDeliveryReceipts();

```


### <a name="get_a_specific_fax_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.getASpecificFaxDeliveryReceipt") getASpecificFaxDeliveryReceipt

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


```php
function getASpecificFaxDeliveryReceipt($messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | D2AF-479B-8955-6395D561DEF4" (required, number) - Message ID. |



#### Example Usage

```php
$messageId = '"3FAC74F1';

$result = $fax->getASpecificFaxDeliveryReceipt($messageId);

```


### <a name="update_mark_fax_delivery_receipts_as_read"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.updateMarkFaxDeliveryReceiptsAsRead") updateMarkFaxDeliveryReceiptsAsRead

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


```php
function updateMarkFaxDeliveryReceiptsAsRead($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "{    \"date_before\": 1441958441}";
$body = APIHelper::deserialize($bodyValue);

$result = $fax->updateMarkFaxDeliveryReceiptsAsRead($body);

```


### <a name="add_a_test_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.addATestDeliveryReceipt") addATestDeliveryReceipt

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


```php
function addATestDeliveryReceipt($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "    {        \"url\":\"http://yourUrl.com\"    }";
$body = APIHelper::deserialize($bodyValue);

$result = $fax->addATestDeliveryReceipt($body);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="forgot_account_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ForgotAccountController") ForgotAccountController

### Get singleton instance

The singleton instance of the ``` ForgotAccountController ``` class can be accessed from the API Client.

```php
$forgotAccount = $client->getForgotAccount();
```

### <a name="update_forgot_username"></a>![Method: ](https://apidocs.io/img/method.png ".ForgotAccountController.updateForgotUsername") updateForgotUsername

> TODO: Add a method description


```php
function updateForgotUsername($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$body = new ForgotUsernameRequest();

$result = $forgotAccount->updateForgotUsername($body);

```


### <a name="update_forgot_password"></a>![Method: ](https://apidocs.io/img/method.png ".ForgotAccountController.updateForgotPassword") updateForgotPassword

> TODO: Add a method description


```php
function updateForgotPassword($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "    {        \"username\": \"0F6pKiiuca\"    }";
$body = APIHelper::deserialize($bodyValue);

$result = $forgotAccount->updateForgotPassword($body);

```


### <a name="update_verify_forgot_password"></a>![Method: ](https://apidocs.io/img/method.png ".ForgotAccountController.updateVerifyForgotPassword") updateVerifyForgotPassword

> TODO: Add a method description


```php
function updateVerifyForgotPassword($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "    {        \"subaccount_id\": 54,        \"activation_token\": \"9C648BAD-EB7F-4E7E-96BC-B433140C4F1F\",        \"password\": \"0F6pKiiuca\"    }";
$body = APIHelper::deserialize($bodyValue);

$result = $forgotAccount->updateVerifyForgotPassword($body);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="mms_controller"></a>![Class: ](https://apidocs.io/img/class.png ".MMSController") MMSController

### Get singleton instance

The singleton instance of the ``` MMSController ``` class can be accessed from the API Client.

```php
$mMS = $client->getMMS();
```

### <a name="create_send_mms"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.createSendMMS") createSendMMS

> TODO: Add a method description


```php
function createSendMMS($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$body = new SendMMSRequest();

$result = $mMS->createSendMMS($body);

```


### <a name="create_get_price"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.createGetPrice") createGetPrice

> TODO: Add a method description


```php
function createGetPrice($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$body = new GetPriceRequest();

$result = $mMS->createGetPrice($body);

```


### <a name="get_mms_history"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.getMMSHistory") getMMSHistory

> TODO: Add a method description


```php
function getMMSHistory(
        $q = null,
        $orderBy = null,
        $dateFrom = null,
        $dateTo = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| q |  ``` Optional ```  | A custom query. |
| orderBy |  ``` Optional ```  | Sort records by. |
| dateFrom |  ``` Optional ```  | Timestamp (from) used to show records by date. |
| dateTo |  ``` Optional ```  | Timestamp (to) used to show records by date. |



#### Example Usage

```php
$q = 'list_id:429,direction:out';
$orderBy = 'subject:desc';
$dateFrom = 1443501617;
$dateTo = 1443501727;

$result = $mMS->getMMSHistory($q, $orderBy, $dateFrom, $dateTo);

```


### <a name="get_export_mms_history"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.getExportMMSHistory") getExportMMSHistory

> TODO: Add a method description


```php
function getExportMMSHistory($filename)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | Your export filename. |



#### Example Usage

```php
$filename = 'export.csv';

$result = $mMS->getExportMMSHistory($filename);

```


### <a name="update_cancel_mms"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.updateCancelMMS") updateCancelMMS

> TODO: Add a method description


```php
function updateCancelMMS($messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Message ID. |



#### Example Usage

```php
$messageId = 'message_id';

$result = $mMS->updateCancelMMS($messageId);

```


### <a name="update_cancel_all_mms"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.updateCancelAllMMS") updateCancelAllMMS

> TODO: Add a method description


```php
function updateCancelAllMMS()
```

#### Example Usage

```php

$result = $mMS->updateCancelAllMMS();

```


### <a name="get_all_delivery_receipts"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.getAllDeliveryReceipts") getAllDeliveryReceipts

> TODO: Add a method description


```php
function getAllDeliveryReceipts()
```

#### Example Usage

```php

$result = $mMS->getAllDeliveryReceipts();

```


### <a name="get_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.getDeliveryReceipt") getDeliveryReceipt

> TODO: Add a method description


```php
function getDeliveryReceipt($messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Message ID. |



#### Example Usage

```php
$messageId = '3E0DC217-7D0F-4C20-A3F2-E3362B938CAF';

$result = $mMS->getDeliveryReceipt($messageId);

```


### <a name="update_mark_receipts_as_read"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.updateMarkReceiptsAsRead") updateMarkReceiptsAsRead

> TODO: Add a method description


```php
function updateMarkReceiptsAsRead()
```

#### Example Usage

```php

$result = $mMS->updateMarkReceiptsAsRead();

```


### <a name="get_all_inbound_sms_pull"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.getAllInboundSMSPull") getAllInboundSMSPull

> Inbound MMS shares the same rules/settings/endpoints as SMS. Any attachments will be converted to a URL.
> **Push Inbound SMS**
> If you prefer, we can push message replies to your server as they arrive with us.
> Refer to SMS->Inbound SMS in the docs.
> **Pull Inbound SMS**
> Receive SMS by polling your Inbox.
> Refer to SMS->Inbound SMS in the docs.


```php
function getAllInboundSMSPull()
```

#### Example Usage

```php

$result = $mMS->getAllInboundSMSPull();

```


[Back to List of Controllers](#list_of_controllers)

## <a name="numbers_controller"></a>![Class: ](https://apidocs.io/img/class.png ".NumbersController") NumbersController

### Get singleton instance

The singleton instance of the ``` NumbersController ``` class can be accessed from the API Client.

```php
$numbers = $client->getNumbers();
```

### <a name="get_all_dedicated_numbers"></a>![Method: ](https://apidocs.io/img/method.png ".NumbersController.getAllDedicatedNumbers") getAllDedicatedNumbers

> TODO: Add a method description


```php
function getAllDedicatedNumbers()
```

#### Example Usage

```php

$result = $numbers->getAllDedicatedNumbers();

```


### <a name="create_buy_dedicated_number"></a>![Method: ](https://apidocs.io/img/method.png ".NumbersController.createBuyDedicatedNumber") createBuyDedicatedNumber

> TODO: Add a method description


```php
function createBuyDedicatedNumber($dedicatedNumber)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dedicatedNumber |  ``` Required ```  | Your phone number in E.164 format. |



#### Example Usage

```php
$dedicatedNumber = '+12282060576';

$result = $numbers->createBuyDedicatedNumber($dedicatedNumber);

```


### <a name="search_dedicated_numbers_by_country"></a>![Method: ](https://apidocs.io/img/method.png ".NumbersController.searchDedicatedNumbersByCountry") searchDedicatedNumbersByCountry

> TODO: Add a method description


```php
function searchDedicatedNumbersByCountry(
        $country,
        $search = null,
        $searchType = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Required ```  | Your preferred country. |
| search |  ``` Optional ```  | Your search pattern or query. |
| searchType |  ``` Optional ```  | Your strategy for searching, 0 = starts with, 1 = anywhere, 2 = ends with. |



#### Example Usage

```php
$country = 'US';
$search = '88';
$searchType = 1;

$result = $numbers->searchDedicatedNumbersByCountry($country, $search, $searchType);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="pricing_controller"></a>![Class: ](https://apidocs.io/img/class.png ".PricingController") PricingController

### Get singleton instance

The singleton instance of the ``` PricingController ``` class can be accessed from the API Client.

```php
$pricing = $client->getPricing();
```

### <a name="get_country_pricing"></a>![Method: ](https://apidocs.io/img/method.png ".PricingController.getCountryPricing") getCountryPricing

> TODO: Add a method description


```php
function getCountryPricing(
        $country,
        $currency = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Required ```  | Two-letter representation of the country. |
| currency |  ``` Optional ```  | Three-letter representation of the currency. |



#### Example Usage

```php
$country = 'AU';
$currency = 'AUD';

$result = $pricing->getCountryPricing($country, $currency);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="post_direct_mail_controller"></a>![Class: ](https://apidocs.io/img/class.png ".PostDirectMailController") PostDirectMailController

### Get singleton instance

The singleton instance of the ``` PostDirectMailController ``` class can be accessed from the API Client.

```php
$postDirectMail = $client->getPostDirectMail();
```

### <a name="search_locations"></a>![Method: ](https://apidocs.io/img/method.png ".PostDirectMailController.searchLocations") searchLocations

> TODO: Add a method description


```php
function searchLocations(
        $country,
        $query)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Required ```  | Country code. |
| query |  ``` Required ```  | A postal code or place name. |



#### Example Usage

```php
$country = 'AD';
$query = 'AD100';

$result = $postDirectMail->searchLocations($country, $query);

```


### <a name="create_new_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".PostDirectMailController.createNewCampaign") createNewCampaign

> Create new direct mail campaign.


```php
function createNewCampaign($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$body = new CreateNewCampaignRequest();

$result = $postDirectMail->createNewCampaign($body);

```


### <a name="create_calculate_direct_mail_campaign_price"></a>![Method: ](https://apidocs.io/img/method.png ".PostDirectMailController.createCalculateDirectMailCampaignPrice") createCalculateDirectMailCampaignPrice

> Calculate direct mail campaign price.


```php
function createCalculateDirectMailCampaignPrice($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$body = new CalculateDirectMailCampaignPriceRequest();

$result = $postDirectMail->createCalculateDirectMailCampaignPrice($body);

```


### <a name="list_direct_mail_campaigns"></a>![Method: ](https://apidocs.io/img/method.png ".PostDirectMailController.listDirectMailCampaigns") listDirectMailCampaigns

> Get list of direct mail campaigns.


```php
function listDirectMailCampaigns()
```

#### Example Usage

```php

$result = $postDirectMail->listDirectMailCampaigns();

```


[Back to List of Controllers](#list_of_controllers)

## <a name="post_letter_controller"></a>![Class: ](https://apidocs.io/img/class.png ".PostLetterController") PostLetterController

### Get singleton instance

The singleton instance of the ``` PostLetterController ``` class can be accessed from the API Client.

```php
$postLetter = $client->getPostLetter();
```

### <a name="create_send_post_letter"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.createSendPostLetter") createSendPostLetter

> **Supported File Types**
> We support `pdf`, `docx` and `doc` files. Contact us to add support for any other file type. If you're using `docx` or `doc` files, you'll need to convert the file first using our uploads endpoint with the querystring parameter `convert=post` e.g. `POST /uploads?convert=post`. This will return a URL to the converted pdf file that can be used in the `/post/letters/send` endpoint.
> **Letter File Options**
> **Use existing URL**
> With this option, you can use an existing URL to a `pdf` document. For example, you might generate the `pdf` on your server.
> **Upload File to Our Server**
> With this option, you can use the `/uploads` endpoint to upload the document. The `/uploads` endpoint returns a URL that can be used in the `/post/letters/send` endpoint.


```php
function createSendPostLetter($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "{  \"file_url\": \"http://server.com/file.pdf\",  \"template_used\": 1,  \"colour\": 1,  \"duplex\": 0,  \"recipients\": [    {      \"address_name\": \"My Home Address\",      \"address_line_1\": \"Address 1\",      \"address_line_2\": \"Address 2\",      \"address_city\": \"CITY\",      \"address_state\": \"State\",      \"address_postal_code\": 123456,      \"address_country\": \"AU\",      \"return_address_id\": 1,      \"schedule\": 1449573604    }  ]}";
$body = APIHelper::deserialize($bodyValue);

$result = $postLetter->createSendPostLetter($body);

```


### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.createCalculatePrice") createCalculatePrice

> TODO: Add a method description


```php
function createCalculatePrice($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "{  \"file_url\": \"http://server.com/file.pdf\",  \"template_used\": 1,  \"colour\": 1,  \"duplex\": 0,  \"recipients\": [    \"[]\"  ],  \"Body\": \"\"}";
$body = APIHelper::deserialize($bodyValue);

$result = $postLetter->createCalculatePrice($body);

```


### <a name="get_post_letter_history"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.getPostLetterHistory") getPostLetterHistory

> TODO: Add a method description


```php
function getPostLetterHistory()
```

#### Example Usage

```php

$result = $postLetter->getPostLetterHistory();

```


### <a name="get_export_post_letter_history"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.getExportPostLetterHistory") getExportPostLetterHistory

> TODO: Add a method description


```php
function getExportPostLetterHistory($filename)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | Filename for the export file. |



#### Example Usage

```php
$filename = 'myexport.csv';

$result = $postLetter->getExportPostLetterHistory($filename);

```


### <a name="create_a_post_return_address"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.createAPostReturnAddress") createAPostReturnAddress

> TODO: Add a method description


```php
function createAPostReturnAddress($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "{    \"address_name\":\"My Home Address\",    \"address_line_1\":\"Maritime Avenue\",    \"address_line_2\":\"\",    \"address_city\":\"Flynn\",    \"address_state\":\"WA\",    \"address_postal_code\":6302,    \"address_country\":\"Australia\"}";
$body = APIHelper::deserialize($bodyValue);

$result = $postLetter->createAPostReturnAddress($body);

```


### <a name="get_list_of_post_return_addresses"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.getListOfPostReturnAddresses") getListOfPostReturnAddresses

> TODO: Add a method description


```php
function getListOfPostReturnAddresses()
```

#### Example Usage

```php

$result = $postLetter->getListOfPostReturnAddresses();

```


### <a name="get_post_return_address"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.getPostReturnAddress") getPostReturnAddress

> TODO: Add a method description


```php
function getPostReturnAddress($returnAddressId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| returnAddressId |  ``` Required ```  | Your return address id. |



#### Example Usage

```php
$returnAddressId = 14;

$result = $postLetter->getPostReturnAddress($returnAddressId);

```


### <a name="update_post_return_address"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.updatePostReturnAddress") updatePostReturnAddress

> TODO: Add a method description


```php
function updatePostReturnAddress(
        $returnAddressId,
        $body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| returnAddressId |  ``` Required ```  | Your return address id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$returnAddressId = 14;
$bodyValue = "{    \"address_name\":\"My Home Address\",    \"address_line_1\":\"Maritime Avenue\",    \"address_line_2\":\"\",    \"address_city\":\"Flynn\",    \"address_state\":\"WA\",    \"address_postal_code\":6302,    \"address_country\":\"Australia\"}";
$body = APIHelper::deserialize($bodyValue);

$result = $postLetter->updatePostReturnAddress($returnAddressId, $body);

```


### <a name="delete_post_return_address"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.deletePostReturnAddress") deletePostReturnAddress

> TODO: Add a method description


```php
function deletePostReturnAddress($returnAddressId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| returnAddressId |  ``` Required ```  | Your return address id. |



#### Example Usage

```php
$returnAddressId = 12;

$result = $postLetter->deletePostReturnAddress($returnAddressId);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="postcards_controller"></a>![Class: ](https://apidocs.io/img/class.png ".PostcardsController") PostcardsController

### Get singleton instance

The singleton instance of the ``` PostcardsController ``` class can be accessed from the API Client.

```php
$postcards = $client->getPostcards();
```

### <a name="create_send_postcard"></a>![Method: ](https://apidocs.io/img/method.png ".PostcardsController.createSendPostcard") createSendPostcard

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


```php
function createSendPostcard($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "{    \"file_urls\":[         \"https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_front.pdf\",         \"https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_back.pdf\"    ],    \"recipients\":[        {            \"address_name\":\"My Home Address\",            \"address_line_1\":\"Address 1\",            \"address_line_2\":\"\",            \"address_city\":\"City\",            \"address_state\":\"State\",            \"address_postal_code\":\"123456\",            \"address_country\":\"AU\",            \"return_address_id\":1        }    ]}";
$body = APIHelper::deserialize($bodyValue);

$result = $postcards->createSendPostcard($body);

```


### <a name="create_calculate_pricing"></a>![Method: ](https://apidocs.io/img/method.png ".PostcardsController.createCalculatePricing") createCalculatePricing

> For `file_urls` field. You can attach at least 1 and max of 2 PDF file urls.
> - Supply a single pdf with 2 pages (front and back)
> - Supply 2 urls to seperate PDFs


```php
function createCalculatePricing($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "{    \"file_urls\":[        \"https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_front.pdf\",        \"https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_back.pdf\"    ],    \"recipients\":[        {            \"address_name\":\"My Home Address\",            \"address_line_1\":\"Address 1\",            \"address_line_2\":\"\",            \"address_city\":\"City\",            \"address_state\":\"State\",            \"address_postal_code\":\"123456\",            \"address_country\":\"AU\",            \"return_address_id\":1        }    ]}";
$body = APIHelper::deserialize($bodyValue);

$result = $postcards->createCalculatePricing($body);

```


### <a name="get_postcard_history"></a>![Method: ](https://apidocs.io/img/method.png ".PostcardsController.getPostcardHistory") getPostcardHistory

> TODO: Add a method description


```php
function getPostcardHistory()
```

#### Example Usage

```php

$result = $postcards->getPostcardHistory();

```


### <a name="get_export_postcard_history"></a>![Method: ](https://apidocs.io/img/method.png ".PostcardsController.getExportPostcardHistory") getExportPostcardHistory

> TODO: Add a method description


```php
function getExportPostcardHistory($filename)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | Filename for the export file. |



#### Example Usage

```php
$filename = 'myexport.csv';

$result = $postcards->getExportPostcardHistory($filename);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="referral_accounts_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ReferralAccountsController") ReferralAccountsController

### Get singleton instance

The singleton instance of the ``` ReferralAccountsController ``` class can be accessed from the API Client.

```php
$referralAccounts = $client->getReferralAccounts();
```

### <a name="get_list_of_referral_accounts"></a>![Method: ](https://apidocs.io/img/method.png ".ReferralAccountsController.getListOfReferralAccounts") getListOfReferralAccounts

> TODO: Add a method description


```php
function getListOfReferralAccounts()
```

#### Example Usage

```php

$result = $referralAccounts->getListOfReferralAccounts();

```


[Back to List of Controllers](#list_of_controllers)

## <a name="reseller_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ResellerController") ResellerController

### Get singleton instance

The singleton instance of the ``` ResellerController ``` class can be accessed from the API Client.

```php
$reseller = $client->getReseller();
```

### <a name="get_reseller_setting"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerController.getResellerSetting") getResellerSetting

> Get reseller setting.


```php
function getResellerSetting()
```

#### Example Usage

```php

$result = $reseller->getResellerSetting();

```


### <a name="update_reseller_setting"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerController.updateResellerSetting") updateResellerSetting

> Update a specific reseller setting.


```php
function updateResellerSetting($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "    {        \"allow_public_signups\":1,        \"default_margin\":100,        \"default_margin_numbers\":150,        \"trial_balance\":50,        \"subdomain\":\"subdomain\",        \"colour_navigation\":\"#9999FF\",        \"logo_url_light\":\"http://url.com/light\",        \"logo_url_dark\":\"http://url.com/dark\",        \"company_name\":\"MyCompany\"    }";
$body = APIHelper::deserialize($bodyValue);

$result = $reseller->updateResellerSetting($body);

```


### <a name="get_reseller_by_subdomain"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerController.getResellerBySubdomain") getResellerBySubdomain

> Get reseller setting by subdomin.


```php
function getResellerBySubdomain($subdomain)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subdomain |  ``` Required ```  | Subdomain |



#### Example Usage

```php
$subdomain = 'mysubdomain';

$result = $reseller->getResellerBySubdomain($subdomain);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="reseller_accounts_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ResellerAccountsController") ResellerAccountsController

### Get singleton instance

The singleton instance of the ``` ResellerAccountsController ``` class can be accessed from the API Client.

```php
$resellerAccounts = $client->getResellerAccounts();
```

### <a name="list_of_reseller_accounts"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.listOfResellerAccounts") listOfResellerAccounts

> Get list of Reseller Accounts


```php
function listOfResellerAccounts()
```

#### Example Usage

```php

$result = $resellerAccounts->listOfResellerAccounts();

```


### <a name="get_reseller_account"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.getResellerAccount") getResellerAccount

> Get a specific reseller account.


```php
function getResellerAccount($clientUserId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| clientUserId |  ``` Required ```  | The client user id. |



#### Example Usage

```php
$clientUserId = 24;

$result = $resellerAccounts->getResellerAccount($clientUserId);

```


### <a name="create_reseller_account"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.createResellerAccount") createResellerAccount

> TODO: Add a method description


```php
function createResellerAccount($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "    {        \"username\":\"johndoe2\",        \"user_email\":\"johndoe2@awesome.com\",        \"user_phone\":\"518-481-1002\",        \"user_first_name\":\"John\",        \"user_last_name\":\"Doe\",        \"country\":\"US\",        \"password\":\"pass\",        \"account_name\":\"The Awesome Company\"    }";
$body = APIHelper::deserialize($bodyValue);

$result = $resellerAccounts->createResellerAccount($body);

```


### <a name="create_reseller_account_public"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.createResellerAccountPublic") createResellerAccountPublic

> TODO: Add a method description


```php
function createResellerAccountPublic($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "{    \"reseller_user_id\":1,    \"username\":\"john_awesome\",    \"user_email\":\"johnis@awesome.com\",    \"user_phone\":\"+61261063270\",    \"user_first_name\":\"John\",    \"user_last_name\":\"Awesome\",    \"country\":\"AU\",    \"password\":\"pass\",    \"account_name\":\"The Awesome Company\"}";
$body = APIHelper::deserialize($bodyValue);

$result = $resellerAccounts->createResellerAccountPublic($body);

```


### <a name="update_reseller_account"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.updateResellerAccount") updateResellerAccount

> TODO: Add a method description


```php
function updateResellerAccount(
        $clientUserId,
        $body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| clientUserId |  ``` Required ```  | Your client user id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$clientUserId = 24;
$bodyValue = "    {        \"username\":\"johndoe2\",        \"user_email\":\"johndoe2@awesome.com\",        \"user_phone\":\"518-481-1002\",        \"user_first_name\":\"John\",        \"user_last_name\":\"Doe\",        \"country\":\"US\",        \"password\":\"pass\",        \"account_name\":\"The Awesome Company\"    }";
$body = APIHelper::deserialize($bodyValue);

$result = $resellerAccounts->updateResellerAccount($clientUserId, $body);

```


### <a name="update_transfer_credit"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.updateTransferCredit") updateTransferCredit

> TODO: Add a method description


```php
function updateTransferCredit($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$body = new TransferCreditRequest();

$result = $resellerAccounts->updateTransferCredit($body);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="sdk_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SDKController") SDKController

### Get singleton instance

The singleton instance of the ``` SDKController ``` class can be accessed from the API Client.

```php
$sDK = $client->getSDK();
```

### <a name="get_sdk_download"></a>![Method: ](https://apidocs.io/img/method.png ".SDKController.getSDKDownload") getSDKDownload

> TODO: Add a method description


```php
function getSDKDownload($type)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| type |  ``` Required ```  | Supported types. |



#### Example Usage

```php
$type = 'type';

$result = $sDK->getSDKDownload($type);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="search_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SearchController") SearchController

### Get singleton instance

The singleton instance of the ``` SearchController ``` class can be accessed from the API Client.

```php
$search = $client->getSearch();
```

### <a name="search_contacts_lists"></a>![Method: ](https://apidocs.io/img/method.png ".SearchController.searchContactsLists") searchContactsLists

> TODO: Add a method description


```php
function searchContactsLists($q)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| q |  ``` Required ```  | Your keyword or query. |



#### Example Usage

```php
$q = 'Gorne';

$result = $search->searchContactsLists($q);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="sms_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SMSController") SMSController

### Get singleton instance

The singleton instance of the ``` SMSController ``` class can be accessed from the API Client.

```php
$sMS = $client->getSMS();
```

### <a name="create_send_an_sms"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.createSendAnSMS") createSendAnSMS

> You can post **up to 1000 messages** with each API call.


```php
function createSendAnSMS($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$body = new SendAnSMSRequest();

$result = $sMS->createSendAnSMS($body);

```


### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.createCalculatePrice") createCalculatePrice

> TODO: Add a method description


```php
function createCalculatePrice($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$body = new CalculatePriceRequest205();

$result = $sMS->createCalculatePrice($body);

```


### <a name="get_all_history"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.getAllHistory") getAllHistory

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


```php
function getAllHistory(
        $dateFrom = null,
        $dateTo = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateFrom |  ``` Optional ```  | Timestamp (from) used to show records by date. |
| dateTo |  ``` Optional ```  | Timestamp (to) used to show recrods by date. |



#### Example Usage

```php
$dateFrom = 1449459940;
$dateTo = 1449659940;

$result = $sMS->getAllHistory($dateFrom, $dateTo);

```


### <a name="get_export_sms_history"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.getExportSMSHistory") getExportSMSHistory

> TODO: Add a method description


```php
function getExportSMSHistory()
```

#### Example Usage

```php

$result = $sMS->getExportSMSHistory();

```


### <a name="get_all_delivery_receipts"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.getAllDeliveryReceipts") getAllDeliveryReceipts

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


```php
function getAllDeliveryReceipts()
```

#### Example Usage

```php

$result = $sMS->getAllDeliveryReceipts();

```


### <a name="get_a_specific_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.getASpecificDeliveryReceipt") getASpecificDeliveryReceipt

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


```php
function getASpecificDeliveryReceipt($messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Your message id. |



#### Example Usage

```php
$messageId = '88AB118E EB1B 478C 98CE 6C73ABA23F67';

$result = $sMS->getASpecificDeliveryReceipt($messageId);

```


### <a name="add_a_test_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.addATestDeliveryReceipt") addATestDeliveryReceipt

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


```php
function addATestDeliveryReceipt($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "    {        \"url\":\"http://yourUrl.com\"    }";
$body = APIHelper::deserialize($bodyValue);

$result = $sMS->addATestDeliveryReceipt($body);

```


### <a name="update_mark_delivery_receipts_as_read"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.updateMarkDeliveryReceiptsAsRead") updateMarkDeliveryReceiptsAsRead

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


```php
function updateMarkDeliveryReceiptsAsRead($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "{    \"date_before\": 1441958441}";
$body = APIHelper::deserialize($bodyValue);

$result = $sMS->updateMarkDeliveryReceiptsAsRead($body);

```


### <a name="get_all_inbound_sms_pull"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.getAllInboundSMSPull") getAllInboundSMSPull

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


```php
function getAllInboundSMSPull()
```

#### Example Usage

```php

$result = $sMS->getAllInboundSMSPull();

```


### <a name="get_specific_inbound_pull"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.getSpecificInboundPull") getSpecificInboundPull

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


```php
function getSpecificInboundPull($messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Message ID. Must be a valid GUID. |



#### Example Usage

```php
$messageId = '5D420421-8715-4461-A9A2-C8F569E41835';

$result = $sMS->getSpecificInboundPull($messageId);

```


### <a name="add_a_test_inbound_sms"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.addATestInboundSMS") addATestInboundSMS

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


```php
function addATestInboundSMS($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "    {        \"url\":\"http://yourUrl.com\"    }";
$body = APIHelper::deserialize($bodyValue);

$result = $sMS->addATestInboundSMS($body);

```


### <a name="update_mark_a_specific_inbound_sms_as_read"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.updateMarkASpecificInboundSMSAsRead") updateMarkASpecificInboundSMSAsRead

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


```php
function updateMarkASpecificInboundSMSAsRead($messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | B7CE432193CD-0753597B7293 (string, required) - The message ID you want to mark as read. |



#### Example Usage

```php
$messageId = '307EF035';

$result = $sMS->updateMarkASpecificInboundSMSAsRead($messageId);

```


### <a name="update_mark_all_inbound_sms_as_read"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.updateMarkAllInboundSMSAsRead") updateMarkAllInboundSMSAsRead

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


```php
function updateMarkAllInboundSMSAsRead($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "    {        \"date_before\":1442398100    }";
$body = APIHelper::deserialize($bodyValue);

$result = $sMS->updateMarkAllInboundSMSAsRead($body);

```


### <a name="update_cancel_a_scheduled_message"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.updateCancelAScheduledMessage") updateCancelAScheduledMessage

> TODO: Add a method description


```php
function updateCancelAScheduledMessage($messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | B7CE432193CD-0753597B7293 (string, required) - The message ID you want to cancel. |



#### Example Usage

```php
$messageId = '307EF035';

$result = $sMS->updateCancelAScheduledMessage($messageId);

```


### <a name="update_cancel_all_scheduled_messages"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.updateCancelAllScheduledMessages") updateCancelAllScheduledMessages

> TODO: Add a method description


```php
function updateCancelAllScheduledMessages()
```

#### Example Usage

```php

$result = $sMS->updateCancelAllScheduledMessages();

```


[Back to List of Controllers](#list_of_controllers)

## <a name="sms_campaigns_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SMSCampaignsController") SMSCampaignsController

### Get singleton instance

The singleton instance of the ``` SMSCampaignsController ``` class can be accessed from the API Client.

```php
$sMSCampaigns = $client->getSMSCampaigns();
```

### <a name="create_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.createSMSCampaign") createSMSCampaign

> You can post to a list with **up to 20000 recipients** with each API call.


```php
function createSMSCampaign($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "{    \"list_id\":428,    \"name\":\"My Campaign 1\",    \"from\":\"+61353787448\",    \"body\":\"This is my new campaign message.\",    \"schedule\":1444821615}";
$body = APIHelper::deserialize($bodyValue);

$result = $sMSCampaigns->createSMSCampaign($body);

```


### <a name="create_calculate_price_for_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.createCalculatePriceForSMSCampaign") createCalculatePriceForSMSCampaign

> TODO: Add a method description


```php
function createCalculatePriceForSMSCampaign($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "{    \"list_id\":428,    \"name\":\"My Campaign 1\",    \"from\":\"+61353787448\",    \"body\":\"(First Name), this is your new campaign message.\"}";
$body = APIHelper::deserialize($bodyValue);

$result = $sMSCampaigns->createCalculatePriceForSMSCampaign($body);

```


### <a name="update_an_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.updateAnSMSCampaign") updateAnSMSCampaign

> TODO: Add a method description


```php
function updateAnSMSCampaign(
        $smsCampaignId,
        $body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| smsCampaignId |  ``` Required ```  | Your SMS Campaign id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$smsCampaignId = 1;
$bodyValue = "{    \"list_id\":428,    \"name\":\"Awesome campaign.\",    \"from\":\"+61353787447\",    \"body\":\"his is an awesome message.\",    \"schedule\":1444821615}";
$body = APIHelper::deserialize($bodyValue);

$result = $sMSCampaigns->updateAnSMSCampaign($smsCampaignId, $body);

```


### <a name="get_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.getSMSCampaign") getSMSCampaign

> TODO: Add a method description


```php
function getSMSCampaign($smsCampaignId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| smsCampaignId |  ``` Required ```  | Your SMS campaign id. |



#### Example Usage

```php
$smsCampaignId = 1;

$result = $sMSCampaigns->getSMSCampaign($smsCampaignId);

```


### <a name="update_cancel_an_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.updateCancelAnSMSCampaign") updateCancelAnSMSCampaign

> TODO: Add a method description


```php
function updateCancelAnSMSCampaign($smsCampaignId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| smsCampaignId |  ``` Required ```  | Your SMS Campaign id. |



#### Example Usage

```php
$smsCampaignId = 1;

$result = $sMSCampaigns->updateCancelAnSMSCampaign($smsCampaignId);

```


### <a name="get_list_of_sms_campaigns"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.getListOfSMSCampaigns") getListOfSMSCampaigns

> TODO: Add a method description


```php
function getListOfSMSCampaigns()
```

#### Example Usage

```php

$result = $sMSCampaigns->getListOfSMSCampaigns();

```


[Back to List of Controllers](#list_of_controllers)

## <a name="sms_templates_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SMSTemplatesController") SMSTemplatesController

### Get singleton instance

The singleton instance of the ``` SMSTemplatesController ``` class can be accessed from the API Client.

```php
$sMSTemplates = $client->getSMSTemplates();
```

### <a name="list_of_templates"></a>![Method: ](https://apidocs.io/img/method.png ".SMSTemplatesController.listOfTemplates") listOfTemplates

> Get list of templates.


```php
function listOfTemplates()
```

#### Example Usage

```php

$result = $sMSTemplates->listOfTemplates();

```


### <a name="create_a_template"></a>![Method: ](https://apidocs.io/img/method.png ".SMSTemplatesController.createATemplate") createATemplate

> Create new template.


```php
function createATemplate($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "    {        \"template_name\":\"Template 501916\",        \"body\":\"This is a sample content: H7YI68B3yk for this template.\"    }";
$body = APIHelper::deserialize($bodyValue);

$result = $sMSTemplates->createATemplate($body);

```


### <a name="update_a_template"></a>![Method: ](https://apidocs.io/img/method.png ".SMSTemplatesController.updateATemplate") updateATemplate

> TODO: Add a method description


```php
function updateATemplate(
        $templateId,
        $body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$templateId = '25';
$bodyValue = "    {        \"template_name\":\"I am updated\",        \"body\":\"This is a sample content: Sc0KNWgSMG for this template.\"    }";
$body = APIHelper::deserialize($bodyValue);

$result = $sMSTemplates->updateATemplate($templateId, $body);

```


### <a name="delete_a_template"></a>![Method: ](https://apidocs.io/img/method.png ".SMSTemplatesController.deleteATemplate") deleteATemplate

> TODO: Add a method description


```php
function deleteATemplate($templateId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |



#### Example Usage

```php
$templateId = '25';

$result = $sMSTemplates->deleteATemplate($templateId);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="statistics_controller"></a>![Class: ](https://apidocs.io/img/class.png ".StatisticsController") StatisticsController

### Get singleton instance

The singleton instance of the ``` StatisticsController ``` class can be accessed from the API Client.

```php
$statistics = $client->getStatistics();
```

### <a name="get_sms_statistics"></a>![Method: ](https://apidocs.io/img/method.png ".StatisticsController.getSMSStatistics") getSMSStatistics

> TODO: Add a method description


```php
function getSMSStatistics()
```

#### Example Usage

```php

$result = $statistics->getSMSStatistics();

```


### <a name="get_voice_statistics"></a>![Method: ](https://apidocs.io/img/method.png ".StatisticsController.getVoiceStatistics") getVoiceStatistics

> TODO: Add a method description


```php
function getVoiceStatistics()
```

#### Example Usage

```php

$result = $statistics->getVoiceStatistics();

```


[Back to List of Controllers](#list_of_controllers)

## <a name="subaccounts_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SubaccountsController") SubaccountsController

### Get singleton instance

The singleton instance of the ``` SubaccountsController ``` class can be accessed from the API Client.

```php
$subaccounts = $client->getSubaccounts();
```

### <a name="get_all_subaccounts"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.getAllSubaccounts") getAllSubaccounts

> TODO: Add a method description


```php
function getAllSubaccounts()
```

#### Example Usage

```php

$result = $subaccounts->getAllSubaccounts();

```


### <a name="create_a_new_subaccount"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.createANewSubaccount") createANewSubaccount

> TODO: Add a method description


```php
function createANewSubaccount($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "    {        \"api_username\":\"nameP99\",        \"password\":\"pass\",        \"email\":\"testvrq@gmail.com\",        \"phone_number\":\"941-751-3278\",        \"first_name\":\"FirstnameeGPqV\",        \"last_name\":\"LastnamePvjJp\"    }";
$body = APIHelper::deserialize($bodyValue);

$result = $subaccounts->createANewSubaccount($body);

```


### <a name="get_a_specific_subaccount"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.getASpecificSubaccount") getASpecificSubaccount

> TODO: Add a method description


```php
function getASpecificSubaccount($subaccountId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |



#### Example Usage

```php
$subaccountId = 59;

$result = $subaccounts->getASpecificSubaccount($subaccountId);

```


### <a name="update_a_specific_subaccount"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.updateASpecificSubaccount") updateASpecificSubaccount

> TODO: Add a method description


```php
function updateASpecificSubaccount(
        $subaccountId,
        $body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$subaccountId = 59;
$bodyValue = "    {        \"password\":\"pass\",        \"email\":\"testfP0.updated@gmail.com\",        \"phone_number\":\"+19417519130\",        \"first_name\":\"FirstnameKvdRZUpdated\",        \"last_name\":\"LastnameHUPYGUpdated\",        \"access_users\": 1,        \"access_billing\": 1,        \"access_reporting\": 1,        \"access_contacts\": 1,        \"access_settings\": 1,        \"access_sms\": 1,        \"access_email\": 1,        \"access_voice\": 1,        \"access_fax\": 1,        \"access_post\": 1,        \"access_reseller\": 1,        \"access_mms\": 1,        \"share_campaigns\": 0,        \"notes\": null    }";
$body = APIHelper::deserialize($bodyValue);

$result = $subaccounts->updateASpecificSubaccount($subaccountId, $body);

```


### <a name="delete_a_specific_subaccount"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.deleteASpecificSubaccount") deleteASpecificSubaccount

> TODO: Add a method description


```php
function deleteASpecificSubaccount($subaccountId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |



#### Example Usage

```php
$subaccountId = 59;

$result = $subaccounts->deleteASpecificSubaccount($subaccountId);

```


### <a name="update_regenerate_api_key"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.updateRegenerateAPIKey") updateRegenerateAPIKey

> TODO: Add a method description


```php
function updateRegenerateAPIKey($subaccountId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |



#### Example Usage

```php
$subaccountId = 59;

$result = $subaccounts->updateRegenerateAPIKey($subaccountId);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="timezones_controller"></a>![Class: ](https://apidocs.io/img/class.png ".TimezonesController") TimezonesController

### Get singleton instance

The singleton instance of the ``` TimezonesController ``` class can be accessed from the API Client.

```php
$timezones = $client->getTimezones();
```

### <a name="get_timezones"></a>![Method: ](https://apidocs.io/img/method.png ".TimezonesController.getTimezones") getTimezones

> Get supported list of timezones.


```php
function getTimezones()
```

#### Example Usage

```php

$result = $timezones->getTimezones();

```


[Back to List of Controllers](#list_of_controllers)

## <a name="transactional_email_controller"></a>![Class: ](https://apidocs.io/img/class.png ".TransactionalEmailController") TransactionalEmailController

### Get singleton instance

The singleton instance of the ``` TransactionalEmailController ``` class can be accessed from the API Client.

```php
$transactionalEmail = $client->getTransactionalEmail();
```

### <a name="create_email_send"></a>![Method: ](https://apidocs.io/img/method.png ".TransactionalEmailController.createEmailSend") createEmailSend

> TODO: Add a method description


```php
function createEmailSend($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$body = new EmailSendRequest();

$result = $transactionalEmail->createEmailSend($body);

```


### <a name="create_email_price"></a>![Method: ](https://apidocs.io/img/method.png ".TransactionalEmailController.createEmailPrice") createEmailPrice

> TODO: Add a method description


```php
function createEmailPrice($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$body = new EmailPriceRequest();

$result = $transactionalEmail->createEmailPrice($body);

```


### <a name="get_email_history"></a>![Method: ](https://apidocs.io/img/method.png ".TransactionalEmailController.getEmailHistory") getEmailHistory

> TODO: Add a method description


```php
function getEmailHistory()
```

#### Example Usage

```php

$result = $transactionalEmail->getEmailHistory();

```


### <a name="get_export_history"></a>![Method: ](https://apidocs.io/img/method.png ".TransactionalEmailController.getExportHistory") getExportHistory

> TODO: Add a method description


```php
function getExportHistory($filename)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | File name for the export file. |



#### Example Usage

```php
$filename = 'myexport.csv';

$result = $transactionalEmail->getExportHistory($filename);

```


### <a name="add_a_test_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png ".TransactionalEmailController.addATestDeliveryReceipt") addATestDeliveryReceipt

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


```php
function addATestDeliveryReceipt($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "    {        \"url\":\"http://yourUrl.com\"    }";
$body = APIHelper::deserialize($bodyValue);

$result = $transactionalEmail->addATestDeliveryReceipt($body);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="uploads_controller"></a>![Class: ](https://apidocs.io/img/class.png ".UploadsController") UploadsController

### Get singleton instance

The singleton instance of the ``` UploadsController ``` class can be accessed from the API Client.

```php
$uploads = $client->getUploads();
```

### <a name="upload_a_file"></a>![Method: ](https://apidocs.io/img/method.png ".UploadsController.uploadAFile") uploadAFile

> The `upload` endpoint provides a method for converting files from an unspported format to a format that one of our endpoints can handle.
> Files can be submitted two ways:
> 1. Using `base64` encoding in an `application/json` request. In this case, submit the `base64`-encoded file contents in the `content` field of the request body, and `convert` can be specified either also in the body or as part of the query string.
> 2. Using `multipart/form-data` encoding, in the same way it would be submitted using a HTML form. You may find cURL useful for this. For an example of how to do this, see one of our [SDKs](https://dashboard.clicksend.com/#/libraries-sdk/main). In this case, specify `convert` in the query string.
> Note that `convert` specifies the conversion to take place - that is, what the result should be compatible with - and can be any of `fax`, `mms`, `csv` or `post`.
> All files have 10 minutes expiry.


```php
function uploadAFile(
        $body,
        $convert = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |
| convert |  ``` Optional ```  | TODO: Add a parameter description |



#### Example Usage

```php
$body = new UploadAFileRequest();
$convert = 'convert';

$result = $uploads->uploadAFile($body, $convert);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="voice_controller"></a>![Class: ](https://apidocs.io/img/class.png ".VoiceController") VoiceController

### Get singleton instance

The singleton instance of the ``` VoiceController ``` class can be accessed from the API Client.

```php
$voice = $client->getVoice();
```

### <a name="create_send_a_voice_call"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.createSendAVoiceCall") createSendAVoiceCall

> You can post **up to 1000 messages** with each API call.


```php
function createSendAVoiceCall($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$body = new SendAVoiceCallRequest();

$result = $voice->createSendAVoiceCall($body);

```


### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.createCalculatePrice") createCalculatePrice

> TODO: Add a method description


```php
function createCalculatePrice($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$body = new CalculatePriceRequest263();

$result = $voice->createCalculatePrice($body);

```


### <a name="get_voice_languages"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.getVoiceLanguages") getVoiceLanguages

> TODO: Add a method description


```php
function getVoiceLanguages()
```

#### Example Usage

```php

$result = $voice->getVoiceLanguages();

```


### <a name="get_voice_history"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.getVoiceHistory") getVoiceHistory

> TODO: Add a method description


```php
function getVoiceHistory(
        $dateFrom = null,
        $dateTo = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateFrom |  ``` Optional ```  | Timestamp (from) used to show records by date. |
| dateTo |  ``` Optional ```  | Timestamp (to) used to show recrods by date. |



#### Example Usage

```php
$dateFrom = 1443501617;
$dateTo = 1443501727;

$result = $voice->getVoiceHistory($dateFrom, $dateTo);

```


### <a name="get_export_voice_history"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.getExportVoiceHistory") getExportVoiceHistory

> TODO: Add a method description


```php
function getExportVoiceHistory()
```

#### Example Usage

```php

$result = $voice->getExportVoiceHistory();

```


### <a name="get_voice_receipts"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.getVoiceReceipts") getVoiceReceipts

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


```php
function getVoiceReceipts()
```

#### Example Usage

```php

$result = $voice->getVoiceReceipts();

```


### <a name="add_a_test_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.addATestDeliveryReceipt") addATestDeliveryReceipt

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


```php
function addATestDeliveryReceipt($body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$bodyValue = "    {        \"url\":\"http://yourUrl.com\"    }";
$body = APIHelper::deserialize($bodyValue);

$result = $voice->addATestDeliveryReceipt($body);

```


### <a name="get_specific_voice_receipt"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.getSpecificVoiceReceipt") getSpecificVoiceReceipt

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


```php
function getSpecificVoiceReceipt($messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | 3055-45F1-9B79-F2C43509FD16 (string, required) - The voice receipt message id. |



#### Example Usage

```php
$messageId = '28DD2718';

$result = $voice->getSpecificVoiceReceipt($messageId);

```


### <a name="update_marked_voice_receipts_as_read"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.updateMarkedVoiceReceiptsAsRead") updateMarkedVoiceReceiptsAsRead

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


```php
function updateMarkedVoiceReceiptsAsRead($dateBefore)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateBefore |  ``` Required ```  | An optional timestamp - mark all as read before this timestamp. If not given, all receipts will be marked as read. |



#### Example Usage

```php
$dateBefore = 252.201339023747;

$result = $voice->updateMarkedVoiceReceiptsAsRead($dateBefore);

```


### <a name="update_cancel_a_specific_voice_call"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.updateCancelASpecificVoiceCall") updateCancelASpecificVoiceCall

> TODO: Add a method description


```php
function updateCancelASpecificVoiceCall($messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Your voice message id. |



#### Example Usage

```php
$messageId = '7B5BFC19 06B7 49C1 8DCDFB011600E12B';

$result = $voice->updateCancelASpecificVoiceCall($messageId);

```


### <a name="update_cancel_all_voice_calls"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.updateCancelAllVoiceCalls") updateCancelAllVoiceCalls

> TODO: Add a method description


```php
function updateCancelAllVoiceCalls()
```

#### Example Usage

```php

$result = $voice->updateCancelAllVoiceCalls();

```


[Back to List of Controllers](#list_of_controllers)



