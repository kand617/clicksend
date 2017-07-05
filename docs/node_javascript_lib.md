# Getting started

TODO: Add a description

## How to Build

The generated SDK relies on [Node Package Manager](https://www.npmjs.com/) (NPM) being available to resolve dependencies. If you don't already have NPM installed, please go ahead and follow instructions to install NPM from [here](https://nodejs.org/en/download/).
The SDK also requires Node to be installed. If Node isn't already installed, please install it from [here](https://nodejs.org/en/download/)
> NPM is installed by default when Node is installed

To check if node and npm have been successfully installed, write the following commands in command prompt:
* `node --version`
* `npm -version` 
![Version Check](https://apidocs.io/illustration/nodejs?step=versionCheck&workspaceFolder=ClickSend%20REST%20API%20v3-Node)  

Now use npm to resolve all dependencies by running the following command in the root directory (of the SDK folder):
* `npm install`
![Resolve Dependencies](https://apidocs.io/illustration/nodejs?step=resolveDependency1&workspaceFolder=ClickSend%20REST%20API%20v3-Node)
![Resolve Dependencies](https://apidocs.io/illustration/nodejs?step=resolveDependency2)

This will install all dependencies in the `node_modules` folder. 

Once dependencies are resolved, you will need to move the folder `ClickSendRESTAPIV3Lib ` in to your `node_modules` folder.

## How to Use

The following section explains how to use the library in a new project.

### 1. Open Project Folder
Open an IDE/Text Editor for JavaScript like Sublime Text. The basic workflow presented here is also applicable if you prefer using a different editor or IDE.  
Click on `File` and select `Open Folder`
![Open Folder](https://apidocs.io/illustration/nodejs?step=openFolder)

Select the folder of your SDK and click on `Select Folder` to open it up in Sublime Text. The folder will become visible in the bar on the left.
![Open Project](https://apidocs.io/illustration/nodejs?step=openProject&workspaceFolder=ClickSend%20REST%20API%20v3-Node)


### 2. Creating a Test File
Now right click on the folder name and select the `New File` option to create a new test file.    Save it as `index.js` Now import the generated NodeJS library using the following lines of code:
```JavaScript
var lib = require('lib');
```
Save changes.

![Create new file](https://apidocs.io/illustration/nodejs?step=createNewFile&workspaceFolder=ClickSend%20REST%20API%20v3-Node)
![Save new file](https://apidocs.io/illustration/nodejs?step=saveNewFile&workspaceFolder=ClickSend%20REST%20API%20v3-Node)

### 3. Running The Test File
To run the `index.js` file, open up the command prompt and navigate to the Path where the SDK folder resides. Type the following command to run the file:  
`node index.js`
![Run file](https://apidocs.io/illustration/nodejs?step=runProject&workspaceFolder=ClickSend%20REST%20API%20v3-Node)


## How to Test

These tests use Mocha framework for testing, coupled with Chai for assertions. These dependencies need to be installed for tests to run.
Tests can be run in a number of ways:

### Method 1 
###### (Run all tests)

1. Navigate to the root directory of the SDK folder from command prompt.
2. Type `mocha --recursive` to run all the tests.

### Method 2
###### (Run all tests)

1. Navigate to the `../test/Controllers/` directory from command prompt.
2. Type `mocha *` to run all the tests.

### Method 3
###### (Run specific controller's tests)

1. Navigate to the `../test/Controllers/` directory from command prompt.
2. Type `mocha  ClickSend REST API v3Controller`  to run all the tests in that controller file.

> To increase mocha's default timeout, you can change the `TEST_TIMEOUT` parameter's value in `TestBootstrap.js`.  

![Run Tests](https://apidocs.io/illustration/nodejs?step=runTests&controllerName=ClickSend%20REST%20API%20v3Controller)

## Initialization

### Authentication
In order to setup authentication in the API client, you need the following information.

| Parameter | Description |
|-----------|-------------|
| basicAuthUserName | The username to use with basic authentication |
| basicAuthPassword | The password to use with basic authentication |



API client can be initialized as following:

```JavaScript
var lib = require('lib');

// Configuration parameters and credentials
lib.Configuration.basicAuthUserName = "basicAuthUserName"; // The username to use with basic authentication
lib.Configuration.basicAuthPassword = "basicAuthPassword"; // The password to use with basic authentication

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

```javascript
var controller = lib.AccountController;
```

### <a name="create_a_new_account"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.createANewAccount") createANewAccount

> **Note:** *Authentication isn't required to create a new account.*


```javascript
function createANewAccount(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CreateANewAccountRequest(    {        "username":"johndoe1",        "user_email":"johndoe1@awesome.com",        "user_phone":"518-481-1001",        "user_first_name":"John",        "user_last_name":"Doe",        "country":"US",        "password":"pass",        "account_name":"The Awesome Company"    });

    controller.createANewAccount(body, function(error, response, context) {

    
	});
```



### <a name="update_account"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.updateAccount") updateAccount

> TODO: Add a method description


```javascript
function updateAccount(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new UpdateAccountRequest(    {        "username":"johndoe",        "user_email":"johndoe@awesome.com",        "user_phone":"518-481-1002",        "user_first_name":"John",        "user_last_name":"Doe",        "country":"AU",        "password":"pass",        "account_name":"The Awesome Company",        "timezone": "Australia/Melbourne",        "private_uploads": 1,        "setting_sms_hide_your_number": 0,        "setting_sms_hide_business_name": 1    });

    controller.updateAccount(body, function(error, response, context) {

    
	});
```



### <a name="get_account"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.getAccount") getAccount

> TODO: Add a method description


```javascript
function getAccount(callback)
```

#### Example Usage

```javascript


    controller.getAccount(function(error, response, context) {

    
	});
```



### <a name="get_account_usage"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.getAccountUsage") getAccountUsage

> TODO: Add a method description


```javascript
function getAccountUsage(year, month, type, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| year |  ``` Required ```  | Your account usage year. |
| month |  ``` Required ```  | Your account usage month. |
| type |  ``` Required ```  | The account type. Value can only be either email or subaccount. |



#### Example Usage

```javascript

    var year = 2016;
    var month = 4;
    var type = 'subaccount';

    controller.getAccountUsage(year, month, type, function(error, response, context) {

    
	});
```



### <a name="update_send_account_activation_token"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.updateSendAccountActivationToken") updateSendAccountActivationToken

> TODO: Add a method description


```javascript
function updateSendAccountActivationToken(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new SendAccountActivationTokenRequest(    {        "user_phone":"352-394-4199",        "type":"sms",        "country": "US"    });

    controller.updateSendAccountActivationToken(body, function(error, response, context) {

    
	});
```



### <a name="update_verify_new_account"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.updateVerifyNewAccount") updateVerifyNewAccount

> TODO: Add a method description


```javascript
function updateVerifyNewAccount(activationToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| activationToken |  ``` Required ```  | The ActivationToken to be used to verify an account. |



#### Example Usage

```javascript

    var activationToken = 1827364;

    controller.updateVerifyNewAccount(activationToken, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="account_recharge_controller"></a>![Class: ](https://apidocs.io/img/class.png ".AccountRechargeController") AccountRechargeController

### Get singleton instance

The singleton instance of the ``` AccountRechargeController ``` class can be accessed from the API Client.

```javascript
var controller = lib.AccountRechargeController;
```

### <a name="get_credit_card_info"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.getCreditCardInfo") getCreditCardInfo

> TODO: Add a method description


```javascript
function getCreditCardInfo(callback)
```

#### Example Usage

```javascript


    controller.getCreditCardInfo(function(error, response, context) {

    
	});
```



### <a name="update_credit_card_info"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.updateCreditCardInfo") updateCreditCardInfo

> TODO: Add a method description


```javascript
function updateCreditCardInfo(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new UpdateCreditCardInfoRequest({"key":"value"});

    controller.updateCreditCardInfo(body, function(error, response, context) {

    
	});
```



### <a name="list_of_packages"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.listOfPackages") listOfPackages

> TODO: Add a method description


```javascript
function listOfPackages(country, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Optional ```  | Your country. |



#### Example Usage

```javascript

    var country = '"AU"';

    controller.listOfPackages(country, function(error, response, context) {

    
	});
```



### <a name="update_purchase_a_package"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.updatePurchaseAPackage") updatePurchaseAPackage

> TODO: Add a method description


```javascript
function updatePurchaseAPackage(packageId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| packageId |  ``` Required ```  | Your package id. |



#### Example Usage

```javascript

    var packageId = 1;

    controller.updatePurchaseAPackage(packageId, function(error, response, context) {

    
	});
```



### <a name="get_transactions"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.getTransactions") getTransactions

> TODO: Add a method description


```javascript
function getTransactions(callback)
```

#### Example Usage

```javascript


    controller.getTransactions(function(error, response, context) {

    
	});
```



### <a name="get_a_specific_transaction"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.getASpecificTransaction") getASpecificTransaction

> TODO: Add a method description


```javascript
function getASpecificTransaction(transactionId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| transactionId |  ``` Required ```  | 1c65-47fa-aea2-3ded9ed57557 (number, required) - Your transction id. |



#### Example Usage

```javascript

    var transactionId = transaction_id;

    controller.getASpecificTransaction(transactionId, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="automation_rules_controller"></a>![Class: ](https://apidocs.io/img/class.png ".AutomationRulesController") AutomationRulesController

### Get singleton instance

The singleton instance of the ``` AutomationRulesController ``` class can be accessed from the API Client.

```javascript
var controller = lib.AutomationRulesController;
```

### <a name="list_rules"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.listRules") listRules

> TODO: Add a method description


```javascript
function listRules(callback)
```

#### Example Usage

```javascript


    controller.listRules(function(error, response, context) {

    
	});
```



### <a name="get_a_specific_rule"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.getASpecificRule") getASpecificRule

> TODO: Add a method description


```javascript
function getASpecificRule(inboundRuleId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Inbound Rule ID. |



#### Example Usage

```javascript

    var inboundRuleId = 1;

    controller.getASpecificRule(inboundRuleId, function(error, response, context) {

    
	});
```



### <a name="create_a_new_rule"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.createANewRule") createANewRule

> TODO: Add a method description


```javascript
function createANewRule(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CreateANewRuleRequest({"key":"value"});

    controller.createANewRule(body, function(error, response, context) {

    
	});
```



### <a name="update_a_rule"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.updateARule") updateARule

> TODO: Add a method description


```javascript
function updateARule(inboundRuleId, body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Inbound Rule ID. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var inboundRuleId = 1;
    var body = new UpdateARuleRequest({    "dedicated_number":"+61298441484",    "rule_name":"My Rule",    "message_search_type":3,    "message_search_term":"My Search Term",    "action":"EMAIL_FIXED",    "action_address":"john@doe.com",    "enabled":1});

    controller.updateARule(inboundRuleId, body, function(error, response, context) {

    
	});
```



### <a name="delete_a_rule"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.deleteARule") deleteARule

> TODO: Add a method description


```javascript
function deleteARule(inboundRuleId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Inbound Rule ID. |



#### Example Usage

```javascript

    var inboundRuleId = 1;

    controller.deleteARule(inboundRuleId, function(error, response, context) {

    
	});
```



### <a name="list_rules1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.listRules1") listRules1

> TODO: Add a method description


```javascript
function listRules1(callback)
```

#### Example Usage

```javascript


    controller.listRules1(function(error, response, context) {

    
	});
```



### <a name="get_a_specific_rule1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.getASpecificRule1") getASpecificRule1

> TODO: Add a method description


```javascript
function getASpecificRule1(receiptRuleId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |



#### Example Usage

```javascript

    var receiptRuleId = 2;

    controller.getASpecificRule1(receiptRuleId, function(error, response, context) {

    
	});
```



### <a name="create_a_new_rule1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.createANewRule1") createANewRule1

> TODO: Add a method description


```javascript
function createANewRule1(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CreateANewRuleRequest24({    "rule_name": "My Rule",    "match_type": 3,    "action": "EMAIL_FIXED",    "action_address": "john@doe.com",    "enabled": 1});

    controller.createANewRule1(body, function(error, response, context) {

    
	});
```



### <a name="update_a_rule1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.updateARule1") updateARule1

> TODO: Add a method description


```javascript
function updateARule1(receiptRuleId, body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var receiptRuleId = 7;
    var body = new UpdateARuleRequest26({    "rule_name": "My Rule",    "match_type": 3,    "action": "EMAIL_FIXED",    "action_address": "john@doe.com",    "enabled": 1});

    controller.updateARule1(receiptRuleId, body, function(error, response, context) {

    
	});
```



### <a name="delete_a_rule1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.deleteARule1") deleteARule1

> TODO: Add a method description


```javascript
function deleteARule1(receiptRuleId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |



#### Example Usage

```javascript

    var receiptRuleId = 7;

    controller.deleteARule1(receiptRuleId, function(error, response, context) {

    
	});
```



### <a name="list_rules2"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.listRules2") listRules2

> TODO: Add a method description


```javascript
function listRules2(callback)
```

#### Example Usage

```javascript


    controller.listRules2(function(error, response, context) {

    
	});
```



### <a name="get_a_specific_rule1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.getASpecificRule1") getASpecificRule1

> TODO: Add a method description


```javascript
function getASpecificRule1(receiptRuleId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |



#### Example Usage

```javascript

    var receiptRuleId = 2;

    controller.getASpecificRule1(receiptRuleId, function(error, response, context) {

    
	});
```



### <a name="create_a_new_rule2"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.createANewRule2") createANewRule2

> TODO: Add a method description


```javascript
function createANewRule2(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CreateANewRuleRequest24({    "rule_name":"My Rule",    "match_type":3,    "action":"EMAIL_FIXED",    "action_address":"john@doe.com",    "enabled":1});

    controller.createANewRule2(body, function(error, response, context) {

    
	});
```



### <a name="update_a_rule1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.updateARule1") updateARule1

> TODO: Add a method description


```javascript
function updateARule1(receiptRuleId, body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var receiptRuleId = 2;
    var body = new UpdateARuleRequest26({    "rule_name":"My Rule",    "match_type":3,    "action":"EMAIL_FIXED",    "action_address":"john@doe.com",    "enabled":1});

    controller.updateARule1(receiptRuleId, body, function(error, response, context) {

    
	});
```



### <a name="delete_a_rule1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.deleteARule1") deleteARule1

> TODO: Add a method description


```javascript
function deleteARule1(receiptRuleId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |



#### Example Usage

```javascript

    var receiptRuleId = 2;

    controller.deleteARule1(receiptRuleId, function(error, response, context) {

    
	});
```



### <a name="list_rules3"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.listRules3") listRules3

> TODO: Add a method description


```javascript
function listRules3(callback)
```

#### Example Usage

```javascript


    controller.listRules3(function(error, response, context) {

    
	});
```



### <a name="get_a_specific_rule11"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.getASpecificRule11") getASpecificRule11

> TODO: Add a method description


```javascript
function getASpecificRule11(inboundRuleId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Fax inbound rule id |



#### Example Usage

```javascript

    var inboundRuleId = 14;

    controller.getASpecificRule11(inboundRuleId, function(error, response, context) {

    
	});
```



### <a name="create_a_new_rule3"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.createANewRule3") createANewRule3

> TODO: Add a method description


```javascript
function createANewRule3(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CreateANewRuleRequest38(    {        "dedicated_number":"+61298441484",        "rule_name":"Rule Name",        "action":"EMAIL_FIXED",        "action_address":"email@domain.com",        "enabled":1    });

    controller.createANewRule3(body, function(error, response, context) {

    
	});
```



### <a name="update_a_rule11"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.updateARule11") updateARule11

> TODO: Add a method description


```javascript
function updateARule11(inboundRuleId, body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Fax inbound rule id |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var inboundRuleId = 14;
    var body = new UpdateARuleRequest40(    {        "dedicated_number":"+61298441484",        "rule_name":"Rule Name",        "action":"EMAIL_FIXED",        "action_address":"email@domain.com",        "enabled":1    });

    controller.updateARule11(inboundRuleId, body, function(error, response, context) {

    
	});
```



### <a name="delete_a_rule11"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.deleteARule11") deleteARule11

> TODO: Add a method description


```javascript
function deleteARule11(inboundRuleId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Fax inbound rule id |



#### Example Usage

```javascript

    var inboundRuleId = 14;

    controller.deleteARule11(inboundRuleId, function(error, response, context) {

    
	});
```



### <a name="list_rules4"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.listRules4") listRules4

> TODO: Add a method description


```javascript
function listRules4(callback)
```

#### Example Usage

```javascript


    controller.listRules4(function(error, response, context) {

    
	});
```



### <a name="get_a_specific_rule2"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.getASpecificRule2") getASpecificRule2

> TODO: Add a method description


```javascript
function getASpecificRule2(ruleId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |



#### Example Usage

```javascript

    var ruleId = 4;

    controller.getASpecificRule2(ruleId, function(error, response, context) {

    
	});
```



### <a name="create_a_new_rule4"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.createANewRule4") createANewRule4

> TODO: Add a method description


```javascript
function createANewRule4(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CreateANewRuleRequest24(    {        "rule_name":"My Rule",        "match_type":2,        "action":"EMAIL_FIXED",        "action_address":"john@doe.com",        "enabled":1    });

    controller.createANewRule4(body, function(error, response, context) {

    
	});
```



### <a name="update_a_rule2"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.updateARule2") updateARule2

> TODO: Add a method description


```javascript
function updateARule2(ruleId, body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var ruleId = 4;
    var body = new UpdateARuleRequest26(    {        "rule_name":"My Rule",        "match_type":1,        "action":"EMAIL_FIXED",        "action_address":"john@doe.com",        "enabled":1    });

    controller.updateARule2(ruleId, body, function(error, response, context) {

    
	});
```



### <a name="delete_a_rule2"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.deleteARule2") deleteARule2

> TODO: Add a method description


```javascript
function deleteARule2(ruleId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to delete. |



#### Example Usage

```javascript

    var ruleId = 143.746220794854;

    controller.deleteARule2(ruleId, function(error, response, context) {

    
	});
```



### <a name="list_rules5"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.listRules5") listRules5

> TODO: Add a method description


```javascript
function listRules5(callback)
```

#### Example Usage

```javascript


    controller.listRules5(function(error, response, context) {

    
	});
```



### <a name="get_a_specific_rule12"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.getASpecificRule12") getASpecificRule12

> TODO: Add a method description


```javascript
function getASpecificRule12(ruleId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |



#### Example Usage

```javascript

    var ruleId = 5;

    controller.getASpecificRule12(ruleId, function(error, response, context) {

    
	});
```



### <a name="create_a_new_rule5"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.createANewRule5") createANewRule5

> TODO: Add a method description


```javascript
function createANewRule5(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CreateANewRuleRequest24(    {        "rule_name":"My Rule",        "match_type": 0,        "action":"URL",        "action_address":"http://testurl.com",        "enabled":1    });

    controller.createANewRule5(body, function(error, response, context) {

    
	});
```



### <a name="update_a_rule12"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.updateARule12") updateARule12

> TODO: Add a method description


```javascript
function updateARule12(ruleId, body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var ruleId = 8;
    var body = new UpdateARuleRequest26(    {        "rule_name":"My Rule",        "match_type": 0,        "action":"URL",        "action_address":"http://testurl.com",        "enabled":1    });

    controller.updateARule12(ruleId, body, function(error, response, context) {

    
	});
```



### <a name="delete_a_rule12"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.deleteARule12") deleteARule12

> TODO: Add a method description


```javascript
function deleteARule12(ruleId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to delete. |



#### Example Usage

```javascript

    var ruleId = 8;

    controller.deleteARule12(ruleId, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="contact_lists_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ContactListsController") ContactListsController

### Get singleton instance

The singleton instance of the ``` ContactListsController ``` class can be accessed from the API Client.

```javascript
var controller = lib.ContactListsController;
```

### <a name="get_all_contact_lists"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.getAllContactLists") getAllContactLists

> TODO: Add a method description


```javascript
function getAllContactLists(callback)
```

#### Example Usage

```javascript


    controller.getAllContactLists(function(error, response, context) {

    
	});
```



### <a name="create_a_new_contact_list"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.createANewContactList") createANewContactList

> TODO: Add a method description


```javascript
function createANewContactList(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CreateANewContactListRequest(    {        "list_name":"ListCT3QrVL4od"    });

    controller.createANewContactList(body, function(error, response, context) {

    
	});
```



### <a name="get_a_specific_contact_list"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.getASpecificContactList") getASpecificContactList

> TODO: Add a method description


```javascript
function getASpecificContactList(listId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |



#### Example Usage

```javascript

    var listId = 437;

    controller.getASpecificContactList(listId, function(error, response, context) {

    
	});
```



### <a name="update_a_specific_contact_list"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.updateASpecificContactList") updateASpecificContactList

> TODO: Add a method description


```javascript
function updateASpecificContactList(listId, body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var listId = 439;
    var body = new UpdateASpecificContactListRequest(    {        "list_name":"ListlPJf33ksjP"    });

    controller.updateASpecificContactList(listId, body, function(error, response, context) {

    
	});
```



### <a name="delete_a_specific_contact_list"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.deleteASpecificContactList") deleteASpecificContactList

> TODO: Add a method description


```javascript
function deleteASpecificContactList(listId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |



#### Example Usage

```javascript

    var listId = 442;

    controller.deleteASpecificContactList(listId, function(error, response, context) {

    
	});
```



### <a name="create_import_contacts_to_list"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.createImportContactsToList") createImportContactsToList

> TODO: Add a method description


```javascript
function createImportContactsToList(listId, body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var listId = 437;
    var body = new ImportContactsToListRequest({    "file_url":"http://yourdomain.com/5485EA6144/79E8/import.csv",    "field_order":[        "phone",        "first_name",        "last_name",        "custom1",        "custom2",        "custom3",        "custom4",        "fax_number",        "organization_name",        "email",        "address_line_1",        "address_line_2",        "address_city",        "address_state",        "address_postal_code",        "address_country"    ]});

    controller.createImportContactsToList(listId, body, function(error, response, context) {

    
	});
```



### <a name="update_remove_duplicate_contacts"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.updateRemoveDuplicateContacts") updateRemoveDuplicateContacts

> TODO: Add a method description


```javascript
function updateRemoveDuplicateContacts(listId, body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var listId = 439;
    var body = new RemoveDuplicateContactsRequest({    "fields":[        "phone_number",        "first_name",        "last_name",        "fax_number",        "address_country"    ]});

    controller.updateRemoveDuplicateContacts(listId, body, function(error, response, context) {

    
	});
```



### <a name="get_list_of_acceptable_import_fields"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.getListOfAcceptableImportFields") getListOfAcceptableImportFields

> TODO: Add a method description


```javascript
function getListOfAcceptableImportFields(listId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Optional ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var listId = list_id;

    controller.getListOfAcceptableImportFields(listId, function(error, response, context) {

    
	});
```



### <a name="create_show_csv_import_file_preview"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.createShowCSVImportFilePreview") createShowCSVImportFilePreview

> Show first row of the csv import file.


```javascript
function createShowCSVImportFilePreview(listId, body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var listId = 439;
    var body = new ShowCSVImportFilePreviewRequest({    "file_url":"http://yourdomain.com/5485EA6144/79E8/import.csv"});

    controller.createShowCSVImportFilePreview(listId, body, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="contact_suggestions_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ContactSuggestionsController") ContactSuggestionsController

### Get singleton instance

The singleton instance of the ``` ContactSuggestionsController ``` class can be accessed from the API Client.

```javascript
var controller = lib.ContactSuggestionsController;
```

### <a name="list_contact_suggestions"></a>![Method: ](https://apidocs.io/img/method.png ".ContactSuggestionsController.listContactSuggestions") listContactSuggestions

> TODO: Add a method description


```javascript
function listContactSuggestions(callback)
```

#### Example Usage

```javascript


    controller.listContactSuggestions(function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="contacts_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ContactsController") ContactsController

### Get singleton instance

The singleton instance of the ``` ContactsController ``` class can be accessed from the API Client.

```javascript
var controller = lib.ContactsController;
```

### <a name="get_all_contacts_in_a_list"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.getAllContactsInAList") getAllContactsInAList

> TODO: Add a method description


```javascript
function getAllContactsInAList(listId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id where your contacts belong. |



#### Example Usage

```javascript

    var listId = 428;

    controller.getAllContactsInAList(listId, function(error, response, context) {

    
	});
```



### <a name="create_a_new_contact"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.createANewContact") createANewContact

> TODO: Add a method description


```javascript
function createANewContact(listId, body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id where your contact be associated. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var listId = 428;
    var body = new CreateANewContactRequest(    {        "phone_number":"+16783270696",        "first_name":"Ellen",        "last_name":"Diaz",        "custom_1":"Custom 1",        "custom_2":"Custom 2",        "custom_3":"Custom 3",        "custom_4":"Custom 4",        "fax_number":"+16783270696",        "organization_name":"Awesome Organization",        "email":"ellen@diaz.com",        "address_line_1":"Block 2",        "address_line_2":"Cool Bldg.",        "address_city":"Nevada",        "address_state":"Las Vegas",        "address_postal_code":"36063",        "address_country":"US"    });

    controller.createANewContact(listId, body, function(error, response, context) {

    
	});
```



### <a name="get_a_specific_contact"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.getASpecificContact") getASpecificContact

> TODO: Add a method description


```javascript
function getASpecificContact(listId, contactId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| contactId |  ``` Required ```  | Your contact id you want to access. |



#### Example Usage

```javascript

    var listId = 428;
    var contactId = 552802;

    controller.getASpecificContact(listId, contactId, function(error, response, context) {

    
	});
```



### <a name="update_a_specific_contact"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.updateASpecificContact") updateASpecificContact

> TODO: Add a method description


```javascript
function updateASpecificContact(listId, contactId, body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| contactId |  ``` Required ```  | Your contact id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var listId = 428;
    var contactId = 552802;
    var body = new UpdateASpecificContactRequest({        "phone_number":"+16783275492",        "first_name":"Ellen",        "last_name":"Diaz",        "custom_1":"Custom S72oJ9Teba",        "custom_2":"Custom NvrRJrKWeq",        "custom_3":"Custom 2ws94p1Dop",        "custom_4":"Custom Ku0AaIS5xb",        "fax_number":"+16783276356",        "organization_name":"Awesome Organization",        "email":"ellen@diaz.com",        "address_line_1":"Block 6",        "address_line_2":"Cool Bldg.",        "address_city":"Nevada",        "address_state":"Las Vegas",        "address_postal_code":"36063",        "address_country":"US"    });

    controller.updateASpecificContact(listId, contactId, body, function(error, response, context) {

    
	});
```



### <a name="delete_a_specific_contact"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.deleteASpecificContact") deleteASpecificContact

> TODO: Add a method description


```javascript
function deleteASpecificContact(listId, contactId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| contactId |  ``` Required ```  | Your contact id you want to access. |



#### Example Usage

```javascript

    var listId = 428;
    var contactId = 552807;

    controller.deleteASpecificContact(listId, contactId, function(error, response, context) {

    
	});
```



### <a name="update_remove_opted_out_contacts"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.updateRemoveOptedOutContacts") updateRemoveOptedOutContacts

> TODO: Add a method description


```javascript
function updateRemoveOptedOutContacts(listId, optOutListId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id. |
| optOutListId |  ``` Required ```  | Your opt out list id. |



#### Example Usage

```javascript

    var listId = 439;
    var optOutListId = 512;

    controller.updateRemoveOptedOutContacts(listId, optOutListId, function(error, response, context) {

    
	});
```



### <a name="update_transfer_a_contact"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.updateTransferAContact") updateTransferAContact

> Transfers a specific contact to another list.


```javascript
function updateTransferAContact(fromListId, contactId, toListId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| fromListId |  ``` Required ```  | From list id. |
| contactId |  ``` Required ```  | Contact ID. |
| toListId |  ``` Required ```  | To list id. |



#### Example Usage

```javascript

    var fromListId = 428;
    var contactId = 1;
    var toListId = 429;

    controller.updateTransferAContact(fromListId, contactId, toListId, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="countries_controller"></a>![Class: ](https://apidocs.io/img/class.png ".CountriesController") CountriesController

### Get singleton instance

The singleton instance of the ``` CountriesController ``` class can be accessed from the API Client.

```javascript
var controller = lib.CountriesController;
```

### <a name="get_all_countries"></a>![Method: ](https://apidocs.io/img/method.png ".CountriesController.getAllCountries") getAllCountries

> TODO: Add a method description


```javascript
function getAllCountries(callback)
```

#### Example Usage

```javascript


    controller.getAllCountries(function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="delivery_issues_controller"></a>![Class: ](https://apidocs.io/img/class.png ".DeliveryIssuesController") DeliveryIssuesController

### Get singleton instance

The singleton instance of the ``` DeliveryIssuesController ``` class can be accessed from the API Client.

```javascript
var controller = lib.DeliveryIssuesController;
```

### <a name="get_delivery_issues"></a>![Method: ](https://apidocs.io/img/method.png ".DeliveryIssuesController.getDeliveryIssues") getDeliveryIssues

> TODO: Add a method description


```javascript
function getDeliveryIssues(callback)
```

#### Example Usage

```javascript


    controller.getDeliveryIssues(function(error, response, context) {

    
	});
```



### <a name="create_delivery_issue"></a>![Method: ](https://apidocs.io/img/method.png ".DeliveryIssuesController.createDeliveryIssue") createDeliveryIssue

> TODO: Add a method description


```javascript
function createDeliveryIssue(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CreateDeliveryIssueRequest({  "message_id": "B388828B",  "type": "SMS",  "description": "This is a test",  "client_comments": "test",  "email_address: john_doe@user.com": "",  "Body": ""});

    controller.createDeliveryIssue(body, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="email_marketing_controller"></a>![Class: ](https://apidocs.io/img/class.png ".EmailMarketingController") EmailMarketingController

### Get singleton instance

The singleton instance of the ``` EmailMarketingController ``` class can be accessed from the API Client.

```javascript
var controller = lib.EmailMarketingController;
```

### <a name="get_all_allowed_email_addresses"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getAllAllowedEmailAddresses") getAllAllowedEmailAddresses

> TODO: Add a method description


```javascript
function getAllAllowedEmailAddresses(callback)
```

#### Example Usage

```javascript


    controller.getAllAllowedEmailAddresses(function(error, response, context) {

    
	});
```



### <a name="create_allowed_email_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.createAllowedEmailAddress") createAllowedEmailAddress

> TODO: Add a method description


```javascript
function createAllowedEmailAddress(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CreateAllowedEmailAddressRequest({  "email_address": "johndoe1@user.com",  "Body": ""});

    controller.createAllowedEmailAddress(body, function(error, response, context) {

    
	});
```



### <a name="update_send_verification_token"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.updateSendVerificationToken") updateSendVerificationToken

> TODO: Add a method description


```javascript
function updateSendVerificationToken(emailAddressId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email addess id you want to access. |



#### Example Usage

```javascript

    var emailAddressId = 143.746220794854;

    controller.updateSendVerificationToken(emailAddressId, function(error, response, context) {

    
	});
```



### <a name="update_verify_allowed_email_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.updateVerifyAllowedEmailAddress") updateVerifyAllowedEmailAddress

> TODO: Add a method description


```javascript
function updateVerifyAllowedEmailAddress(emailAddressId, activationToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email address id you want to access. |
| activationToken |  ``` Required ```  | 6E8B-4FDB-99A7-7ED08DF97BCC (required, string) - Your activation token. |



#### Example Usage

```javascript

    var emailAddressId = 5;
    var activationToken = 3BD73304;

    controller.updateVerifyAllowedEmailAddress(emailAddressId, activationToken, function(error, response, context) {

    
	});
```



### <a name="delete_allowed_email_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.deleteAllowedEmailAddress") deleteAllowedEmailAddress

> TODO: Add a method description


```javascript
function deleteAllowedEmailAddress(emailAddressId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email address you want to access. |



#### Example Usage

```javascript

    var emailAddressId = 143.746220794854;

    controller.deleteAllowedEmailAddress(emailAddressId, function(error, response, context) {

    
	});
```



### <a name="get_specific_allowed_email_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getSpecificAllowedEmailAddress") getSpecificAllowedEmailAddress

> TODO: Add a method description


```javascript
function getSpecificAllowedEmailAddress(emailAddressId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email address you want to access. |



#### Example Usage

```javascript

    var emailAddressId = 4;

    controller.getSpecificAllowedEmailAddress(emailAddressId, function(error, response, context) {

    
	});
```



### <a name="get_all_email_campaigns"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getAllEmailCampaigns") getAllEmailCampaigns

> TODO: Add a method description


```javascript
function getAllEmailCampaigns(callback)
```

#### Example Usage

```javascript


    controller.getAllEmailCampaigns(function(error, response, context) {

    
	});
```



### <a name="get_specific_email_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getSpecificEmailCampaign") getSpecificEmailCampaign

> TODO: Add a method description


```javascript
function getSpecificEmailCampaign(emailCampaignId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailCampaignId |  ``` Required ```  | The email campaign id you want to access. |



#### Example Usage

```javascript

    var emailCampaignId = 1;

    controller.getSpecificEmailCampaign(emailCampaignId, function(error, response, context) {

    
	});
```



### <a name="create_email_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.createEmailCampaign") createEmailCampaign

> TODO: Add a method description


```javascript
function createEmailCampaign(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CreateEmailCampaignRequest({  "name" : "John Doe",  "subject" : "Lorem Ipsum",  "from_email_address_id" : 2,  "from_name" : "From name",  "template_id" : 31,  "body" : "<p>This is a test</p>",  "list_id" : 456});

    controller.createEmailCampaign(body, function(error, response, context) {

    
	});
```



### <a name="update_email_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.updateEmailCampaign") updateEmailCampaign

> TODO: Add a method description


```javascript
function updateEmailCampaign(emailCampaignId, body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailCampaignId |  ``` Required ```  | The email campaign id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var emailCampaignId = 1;
    var body = new UpdateEmailCampaignRequest({  "name" : "John Doe",  "subject" : "Lorem Ipsum",  "from_email_address_id" : 2,  "from_name" : "From name",  "template_id" : 31,  "body" : "<p>This is a test</p>",  "list_id" : 456});

    controller.updateEmailCampaign(emailCampaignId, body, function(error, response, context) {

    
	});
```



### <a name="update_cancel_email_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.updateCancelEmailCampaign") updateCancelEmailCampaign

> TODO: Add a method description


```javascript
function updateCancelEmailCampaign(emailCampaignId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailCampaignId |  ``` Required ```  | The email campaign id you want to cancel. |



#### Example Usage

```javascript

    var emailCampaignId = 1;

    controller.updateCancelEmailCampaign(emailCampaignId, function(error, response, context) {

    
	});
```



### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.createCalculatePrice") createCalculatePrice

> TODO: Add a method description


```javascript
function createCalculatePrice(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CalculatePriceRequest({  "name" : "John Doe",  "subject" : "Lorem Ipsum",  "from_email_address_id" : 2,  "from_name" : "From name",  "template_id" : 31,  "body" : "<p>This is a test</p>",  "list_id" : 456});

    controller.createCalculatePrice(body, function(error, response, context) {

    
	});
```



### <a name="get_specific_email_campaign_history"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getSpecificEmailCampaignHistory") getSpecificEmailCampaignHistory

> TODO: Add a method description


```javascript
function getSpecificEmailCampaignHistory(campaignId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| campaignId |  ``` Required ```  | The email campaign id you want to access. |



#### Example Usage

```javascript

    var campaignId = 77;

    controller.getSpecificEmailCampaignHistory(campaignId, function(error, response, context) {

    
	});
```



### <a name="get_all_email_templates"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getAllEmailTemplates") getAllEmailTemplates

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```javascript
function getAllEmailTemplates(callback)
```

#### Example Usage

```javascript


    controller.getAllEmailTemplates(function(error, response, context) {

    
	});
```



### <a name="get_specific_email_template"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getSpecificEmailTemplate") getSpecificEmailTemplate

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```javascript
function getSpecificEmailTemplate(templateId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | The email template id. |



#### Example Usage

```javascript

    var templateId = 291;

    controller.getSpecificEmailTemplate(templateId, function(error, response, context) {

    
	});
```



### <a name="create_new_email_template_from_master_template"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.createNewEmailTemplateFromMasterTemplate") createNewEmailTemplateFromMasterTemplate

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```javascript
function createNewEmailTemplateFromMasterTemplate(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CreateNewEmailTemplateFromMasterTemplateRequest({  "template_name": "Minions",  "template_id_master": 57});

    controller.createNewEmailTemplateFromMasterTemplate(body, function(error, response, context) {

    
	});
```



### <a name="update_an_email_template"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.updateAnEmailTemplate") updateAnEmailTemplate

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```javascript
function updateAnEmailTemplate(templateId, body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | The id of the template to be updated. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var templateId = 291;
    var body = new UpdateAnEmailTemplateRequest(    {        "template_name":"Minions",        "body":"This is a sample content: Sc0KNWgSMG for this template."    });

    controller.updateAnEmailTemplate(templateId, body, function(error, response, context) {

    
	});
```



### <a name="delete_email_template"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.deleteEmailTemplate") deleteEmailTemplate

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```javascript
function deleteEmailTemplate(templateId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |



#### Example Usage

```javascript

    var templateId = 25;

    controller.deleteEmailTemplate(templateId, function(error, response, context) {

    
	});
```



### <a name="get_all_master_email_templates"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getAllMasterEmailTemplates") getAllMasterEmailTemplates

> Master templates are templates that you can clone to a User Email Template which lets you edit and save it.


```javascript
function getAllMasterEmailTemplates(callback)
```

#### Example Usage

```javascript


    controller.getAllMasterEmailTemplates(function(error, response, context) {

    
	});
```



### <a name="get_specific_master_template"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getSpecificMasterTemplate") getSpecificMasterTemplate

> Master templates are templates that you can clone to a User Email Template which lets you edit and save it.


```javascript
function getSpecificMasterTemplate(templateId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |



#### Example Usage

```javascript

    var templateId = 25;

    controller.getSpecificMasterTemplate(templateId, function(error, response, context) {

    
	});
```



### <a name="get_all_master_template_categories"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getAllMasterTemplateCategories") getAllMasterTemplateCategories

> TODO: Add a method description


```javascript
function getAllMasterTemplateCategories(callback)
```

#### Example Usage

```javascript


    controller.getAllMasterTemplateCategories(function(error, response, context) {

    
	});
```



### <a name="get_specific_email_template_category"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getSpecificEmailTemplateCategory") getSpecificEmailTemplateCategory

> TODO: Add a method description


```javascript
function getSpecificEmailTemplateCategory(categoryId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| categoryId |  ``` Required ```  | Your category id. |



#### Example Usage

```javascript

    var categoryId = 25;

    controller.getSpecificEmailTemplateCategory(categoryId, function(error, response, context) {

    
	});
```



### <a name="get_all_templates_for_category"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getAllTemplatesForCategory") getAllTemplatesForCategory

> TODO: Add a method description


```javascript
function getAllTemplatesForCategory(categoryId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| categoryId |  ``` Required ```  | Your category id. |



#### Example Usage

```javascript

    var categoryId = 1;

    controller.getAllTemplatesForCategory(categoryId, function(error, response, context) {

    
	});
```



### <a name="upload_image_to_specific_template"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.uploadImageToSpecificTemplate") uploadImageToSpecificTemplate

> TODO: Add a method description


```javascript
function uploadImageToSpecificTemplate(templateId, body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var templateId = 1;
    var body = new UploadImageToSpecificTemplateRequest({    "image": "image.png",    "url" : "http://www.downloadimg.from/here.png"});

    controller.uploadImageToSpecificTemplate(templateId, body, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="email_to_sms_allowed_address_controller"></a>![Class: ](https://apidocs.io/img/class.png ".EmailToSMSAllowedAddressController") EmailToSMSAllowedAddressController

### Get singleton instance

The singleton instance of the ``` EmailToSMSAllowedAddressController ``` class can be accessed from the API Client.

```javascript
var controller = lib.EmailToSMSAllowedAddressController;
```

### <a name="list_of_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSAllowedAddressController.listOfEmailToSMSAllowedAddress") listOfEmailToSMSAllowedAddress

> Get list of allowed email addresses.


```javascript
function listOfEmailToSMSAllowedAddress(callback)
```

#### Example Usage

```javascript


    controller.listOfEmailToSMSAllowedAddress(function(error, response, context) {

    
	});
```



### <a name="create_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSAllowedAddressController.createEmailToSMSAllowedAddress") createEmailToSMSAllowedAddress

> Create an allowed email address.


```javascript
function createEmailToSMSAllowedAddress(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CreateEmailToSMSAllowedAddressRequest(    {        "email_address":"Cv3p0@gmail.com",        "from":"+17128845887"    });

    controller.createEmailToSMSAllowedAddress(body, function(error, response, context) {

    
	});
```



### <a name="get_specific_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSAllowedAddressController.getSpecificEmailToSMSAllowedAddress") getSpecificEmailToSMSAllowedAddress

> Get a specific allowed email address.


```javascript
function getSpecificEmailToSMSAllowedAddress(emailAddressId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | Your email address id. |



#### Example Usage

```javascript

    var emailAddressId = 113;

    controller.getSpecificEmailToSMSAllowedAddress(emailAddressId, function(error, response, context) {

    
	});
```



### <a name="update_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSAllowedAddressController.updateEmailToSMSAllowedAddress") updateEmailToSMSAllowedAddress

> Update a specific allowed email address.


```javascript
function updateEmailToSMSAllowedAddress(emailAddressId, body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | Your email address id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var emailAddressId = 107;
    var body = new UpdateEmailToSMSAllowedAddressRequest(    {        "email_address":"pfvRZ@gmail.com",        "from":"+17128842283"    });

    controller.updateEmailToSMSAllowedAddress(emailAddressId, body, function(error, response, context) {

    
	});
```



### <a name="delete_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSAllowedAddressController.deleteEmailToSMSAllowedAddress") deleteEmailToSMSAllowedAddress

> Delete a specific allowed email address.


```javascript
function deleteEmailToSMSAllowedAddress(emailAddressId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | Your email address id. |



#### Example Usage

```javascript

    var emailAddressId = 107;

    controller.deleteEmailToSMSAllowedAddress(emailAddressId, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="email_to_sms_stripped_strings_controller"></a>![Class: ](https://apidocs.io/img/class.png ".EmailToSMSStrippedStringsController") EmailToSMSStrippedStringsController

### Get singleton instance

The singleton instance of the ``` EmailToSMSStrippedStringsController ``` class can be accessed from the API Client.

```javascript
var controller = lib.EmailToSMSStrippedStringsController;
```

### <a name="list_stripped_strings"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSStrippedStringsController.listStrippedStrings") listStrippedStrings

> TODO: Add a method description


```javascript
function listStrippedStrings(callback)
```

#### Example Usage

```javascript


    controller.listStrippedStrings(function(error, response, context) {

    
	});
```



### <a name="find_specific_stripped_string"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSStrippedStringsController.findSpecificStrippedString") findSpecificStrippedString

> TODO: Add a method description


```javascript
function findSpecificStrippedString(ruleId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |



#### Example Usage

```javascript

    var ruleId = 18;

    controller.findSpecificStrippedString(ruleId, function(error, response, context) {

    
	});
```



### <a name="create_stripped_string"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSStrippedStringsController.createStrippedString") createStrippedString

> TODO: Add a method description


```javascript
function createStrippedString(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CreateStrippedStringRequest({    "strip_string" : "~~~test~~~"});

    controller.createStrippedString(body, function(error, response, context) {

    
	});
```



### <a name="update_stripped_string"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSStrippedStringsController.updateStrippedString") updateStrippedString

> TODO: Add a method description


```javascript
function updateStrippedString(ruleId, body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var ruleId = 20;
    var body = new UpdateStrippedStringRequest({    "strip_string" : "~~~test1~~~"});

    controller.updateStrippedString(ruleId, body, function(error, response, context) {

    
	});
```



### <a name="delete_stripped_string"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSStrippedStringsController.deleteStrippedString") deleteStrippedString

> TODO: Add a method description


```javascript
function deleteStrippedString(ruleId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |



#### Example Usage

```javascript

    var ruleId = 20;

    controller.deleteStrippedString(ruleId, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="fax_controller"></a>![Class: ](https://apidocs.io/img/class.png ".FaxController") FaxController

### Get singleton instance

The singleton instance of the ``` FaxController ``` class can be accessed from the API Client.

```javascript
var controller = lib.FaxController;
```

### <a name="create_send_fax"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.createSendFax") createSendFax

> **Letter File Options**
> **Use existing URL**
> With this option, you can use an existing URL to a PDF document. For example, you might generate the pdf on your server.
> **Upload File to Our Server**
> With this option, you can use the `/uploads` endpoint to upload the document. The `/uploads` endpoint returns a URL that can be used in the `/fax/send` endpoint.


```javascript
function createSendFax(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new SendFaxRequest({"key":"value"});

    controller.createSendFax(body, function(error, response, context) {

    
	});
```



### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.createCalculatePrice") createCalculatePrice

> TODO: Add a method description


```javascript
function createCalculatePrice(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CalculatePriceRequest132({"key":"value"});

    controller.createCalculatePrice(body, function(error, response, context) {

    
	});
```



### <a name="get_fax_history"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.getFaxHistory") getFaxHistory

> Get a list of Fax History.


```javascript
function getFaxHistory(dateFrom, dateTo, q, orderBy, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateFrom |  ``` Optional ```  | Customize result by setting from date (timestsamp) |
| dateTo |  ``` Optional ```  | Customize result by setting to date (timestamp) |
| q |  ``` Optional ```  | Custom query |
| orderBy |  ``` Optional ```  | Order result by |



#### Example Usage

```javascript

    var dateFrom = 1457572619;
    var dateTo = 1457573000;
    var q = 'status:Sent,status_code:201';
    var orderBy = subject:desc;

    controller.getFaxHistory(dateFrom, dateTo, q, orderBy, function(error, response, context) {

    
	});
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


```javascript
function listOfFaxDeliveryReceipts(callback)
```

#### Example Usage

```javascript


    controller.listOfFaxDeliveryReceipts(function(error, response, context) {

    
	});
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


```javascript
function getASpecificFaxDeliveryReceipt(messageId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | D2AF-479B-8955-6395D561DEF4" (required, number) - Message ID. |



#### Example Usage

```javascript

    var messageId = "3FAC74F1;

    controller.getASpecificFaxDeliveryReceipt(messageId, function(error, response, context) {

    
	});
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


```javascript
function updateMarkFaxDeliveryReceiptsAsRead(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new MarkFaxDeliveryReceiptsAsReadRequest({    "date_before": 1441958441});

    controller.updateMarkFaxDeliveryReceiptsAsRead(body, function(error, response, context) {

    
	});
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


```javascript
function addATestDeliveryReceipt(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new AddATestDeliveryReceiptRequest(    {        "url":"http://yourUrl.com"    });

    controller.addATestDeliveryReceipt(body, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="forgot_account_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ForgotAccountController") ForgotAccountController

### Get singleton instance

The singleton instance of the ``` ForgotAccountController ``` class can be accessed from the API Client.

```javascript
var controller = lib.ForgotAccountController;
```

### <a name="update_forgot_username"></a>![Method: ](https://apidocs.io/img/method.png ".ForgotAccountController.updateForgotUsername") updateForgotUsername

> TODO: Add a method description


```javascript
function updateForgotUsername(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new ForgotUsernameRequest({"key":"value"});

    controller.updateForgotUsername(body, function(error, response, context) {

    
	});
```



### <a name="update_forgot_password"></a>![Method: ](https://apidocs.io/img/method.png ".ForgotAccountController.updateForgotPassword") updateForgotPassword

> TODO: Add a method description


```javascript
function updateForgotPassword(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new ForgotPasswordRequest(    {        "username": "0F6pKiiuca"    });

    controller.updateForgotPassword(body, function(error, response, context) {

    
	});
```



### <a name="update_verify_forgot_password"></a>![Method: ](https://apidocs.io/img/method.png ".ForgotAccountController.updateVerifyForgotPassword") updateVerifyForgotPassword

> TODO: Add a method description


```javascript
function updateVerifyForgotPassword(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new VerifyForgotPasswordRequest(    {        "subaccount_id": 54,        "activation_token": "9C648BAD-EB7F-4E7E-96BC-B433140C4F1F",        "password": "0F6pKiiuca"    });

    controller.updateVerifyForgotPassword(body, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="mms_controller"></a>![Class: ](https://apidocs.io/img/class.png ".MMSController") MMSController

### Get singleton instance

The singleton instance of the ``` MMSController ``` class can be accessed from the API Client.

```javascript
var controller = lib.MMSController;
```

### <a name="create_send_mms"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.createSendMMS") createSendMMS

> TODO: Add a method description


```javascript
function createSendMMS(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new SendMMSRequest({"key":"value"});

    controller.createSendMMS(body, function(error, response, context) {

    
	});
```



### <a name="create_get_price"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.createGetPrice") createGetPrice

> TODO: Add a method description


```javascript
function createGetPrice(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new GetPriceRequest({"key":"value"});

    controller.createGetPrice(body, function(error, response, context) {

    
	});
```



### <a name="get_mms_history"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.getMMSHistory") getMMSHistory

> TODO: Add a method description


```javascript
function getMMSHistory(q, orderBy, dateFrom, dateTo, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| q |  ``` Optional ```  | A custom query. |
| orderBy |  ``` Optional ```  | Sort records by. |
| dateFrom |  ``` Optional ```  | Timestamp (from) used to show records by date. |
| dateTo |  ``` Optional ```  | Timestamp (to) used to show records by date. |



#### Example Usage

```javascript

    var q = 'list_id:429,direction:out';
    var orderBy = subject:desc;
    var dateFrom = 1443501617;
    var dateTo = 1443501727;

    controller.getMMSHistory(q, orderBy, dateFrom, dateTo, function(error, response, context) {

    
	});
```



### <a name="get_export_mms_history"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.getExportMMSHistory") getExportMMSHistory

> TODO: Add a method description


```javascript
function getExportMMSHistory(filename, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | Your export filename. |



#### Example Usage

```javascript

    var filename = 'export.csv';

    controller.getExportMMSHistory(filename, function(error, response, context) {

    
	});
```



### <a name="update_cancel_mms"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.updateCancelMMS") updateCancelMMS

> TODO: Add a method description


```javascript
function updateCancelMMS(messageId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Message ID. |



#### Example Usage

```javascript

    var messageId = message_id;

    controller.updateCancelMMS(messageId, function(error, response, context) {

    
	});
```



### <a name="update_cancel_all_mms"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.updateCancelAllMMS") updateCancelAllMMS

> TODO: Add a method description


```javascript
function updateCancelAllMMS(callback)
```

#### Example Usage

```javascript


    controller.updateCancelAllMMS(function(error, response, context) {

    
	});
```



### <a name="get_all_delivery_receipts"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.getAllDeliveryReceipts") getAllDeliveryReceipts

> TODO: Add a method description


```javascript
function getAllDeliveryReceipts(callback)
```

#### Example Usage

```javascript


    controller.getAllDeliveryReceipts(function(error, response, context) {

    
	});
```



### <a name="get_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.getDeliveryReceipt") getDeliveryReceipt

> TODO: Add a method description


```javascript
function getDeliveryReceipt(messageId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Message ID. |



#### Example Usage

```javascript

    var messageId = 3E0DC217-7D0F-4C20-A3F2-E3362B938CAF;

    controller.getDeliveryReceipt(messageId, function(error, response, context) {

    
	});
```



### <a name="update_mark_receipts_as_read"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.updateMarkReceiptsAsRead") updateMarkReceiptsAsRead

> TODO: Add a method description


```javascript
function updateMarkReceiptsAsRead(callback)
```

#### Example Usage

```javascript


    controller.updateMarkReceiptsAsRead(function(error, response, context) {

    
	});
```



### <a name="get_all_inbound_sms_pull"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.getAllInboundSMSPull") getAllInboundSMSPull

> Inbound MMS shares the same rules/settings/endpoints as SMS. Any attachments will be converted to a URL.
> **Push Inbound SMS**
> If you prefer, we can push message replies to your server as they arrive with us.
> Refer to SMS->Inbound SMS in the docs.
> **Pull Inbound SMS**
> Receive SMS by polling your Inbox.
> Refer to SMS->Inbound SMS in the docs.


```javascript
function getAllInboundSMSPull(callback)
```

#### Example Usage

```javascript


    controller.getAllInboundSMSPull(function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="numbers_controller"></a>![Class: ](https://apidocs.io/img/class.png ".NumbersController") NumbersController

### Get singleton instance

The singleton instance of the ``` NumbersController ``` class can be accessed from the API Client.

```javascript
var controller = lib.NumbersController;
```

### <a name="get_all_dedicated_numbers"></a>![Method: ](https://apidocs.io/img/method.png ".NumbersController.getAllDedicatedNumbers") getAllDedicatedNumbers

> TODO: Add a method description


```javascript
function getAllDedicatedNumbers(callback)
```

#### Example Usage

```javascript


    controller.getAllDedicatedNumbers(function(error, response, context) {

    
	});
```



### <a name="create_buy_dedicated_number"></a>![Method: ](https://apidocs.io/img/method.png ".NumbersController.createBuyDedicatedNumber") createBuyDedicatedNumber

> TODO: Add a method description


```javascript
function createBuyDedicatedNumber(dedicatedNumber, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dedicatedNumber |  ``` Required ```  | Your phone number in E.164 format. |



#### Example Usage

```javascript

    var dedicatedNumber = +12282060576;

    controller.createBuyDedicatedNumber(dedicatedNumber, function(error, response, context) {

    
	});
```



### <a name="search_dedicated_numbers_by_country"></a>![Method: ](https://apidocs.io/img/method.png ".NumbersController.searchDedicatedNumbersByCountry") searchDedicatedNumbersByCountry

> TODO: Add a method description


```javascript
function searchDedicatedNumbersByCountry(country, search, searchType, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Required ```  | Your preferred country. |
| search |  ``` Optional ```  | Your search pattern or query. |
| searchType |  ``` Optional ```  | Your strategy for searching, 0 = starts with, 1 = anywhere, 2 = ends with. |



#### Example Usage

```javascript

    var country = 'US';
    var search = '88';
    var searchType = 1;

    controller.searchDedicatedNumbersByCountry(country, search, searchType, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="pricing_controller"></a>![Class: ](https://apidocs.io/img/class.png ".PricingController") PricingController

### Get singleton instance

The singleton instance of the ``` PricingController ``` class can be accessed from the API Client.

```javascript
var controller = lib.PricingController;
```

### <a name="get_country_pricing"></a>![Method: ](https://apidocs.io/img/method.png ".PricingController.getCountryPricing") getCountryPricing

> TODO: Add a method description


```javascript
function getCountryPricing(country, currency, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Required ```  | Two-letter representation of the country. |
| currency |  ``` Optional ```  | Three-letter representation of the currency. |



#### Example Usage

```javascript

    var country = 'AU';
    var currency = 'AUD';

    controller.getCountryPricing(country, currency, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="post_direct_mail_controller"></a>![Class: ](https://apidocs.io/img/class.png ".PostDirectMailController") PostDirectMailController

### Get singleton instance

The singleton instance of the ``` PostDirectMailController ``` class can be accessed from the API Client.

```javascript
var controller = lib.PostDirectMailController;
```

### <a name="search_locations"></a>![Method: ](https://apidocs.io/img/method.png ".PostDirectMailController.searchLocations") searchLocations

> TODO: Add a method description


```javascript
function searchLocations(country, query, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Required ```  | Country code. |
| query |  ``` Required ```  | A postal code or place name. |



#### Example Usage

```javascript

    var country = 'AD';
    var query = 'AD100';

    controller.searchLocations(country, query, function(error, response, context) {

    
	});
```



### <a name="create_new_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".PostDirectMailController.createNewCampaign") createNewCampaign

> Create new direct mail campaign.


```javascript
function createNewCampaign(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CreateNewCampaignRequest({"key":"value"});

    controller.createNewCampaign(body, function(error, response, context) {

    
	});
```



### <a name="create_calculate_direct_mail_campaign_price"></a>![Method: ](https://apidocs.io/img/method.png ".PostDirectMailController.createCalculateDirectMailCampaignPrice") createCalculateDirectMailCampaignPrice

> Calculate direct mail campaign price.


```javascript
function createCalculateDirectMailCampaignPrice(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CalculateDirectMailCampaignPriceRequest({"key":"value"});

    controller.createCalculateDirectMailCampaignPrice(body, function(error, response, context) {

    
	});
```



### <a name="list_direct_mail_campaigns"></a>![Method: ](https://apidocs.io/img/method.png ".PostDirectMailController.listDirectMailCampaigns") listDirectMailCampaigns

> Get list of direct mail campaigns.


```javascript
function listDirectMailCampaigns(callback)
```

#### Example Usage

```javascript


    controller.listDirectMailCampaigns(function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="post_letter_controller"></a>![Class: ](https://apidocs.io/img/class.png ".PostLetterController") PostLetterController

### Get singleton instance

The singleton instance of the ``` PostLetterController ``` class can be accessed from the API Client.

```javascript
var controller = lib.PostLetterController;
```

### <a name="create_send_post_letter"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.createSendPostLetter") createSendPostLetter

> **Supported File Types**
> We support `pdf`, `docx` and `doc` files. Contact us to add support for any other file type. If you're using `docx` or `doc` files, you'll need to convert the file first using our uploads endpoint with the querystring parameter `convert=post` e.g. `POST /uploads?convert=post`. This will return a URL to the converted pdf file that can be used in the `/post/letters/send` endpoint.
> **Letter File Options**
> **Use existing URL**
> With this option, you can use an existing URL to a `pdf` document. For example, you might generate the `pdf` on your server.
> **Upload File to Our Server**
> With this option, you can use the `/uploads` endpoint to upload the document. The `/uploads` endpoint returns a URL that can be used in the `/post/letters/send` endpoint.


```javascript
function createSendPostLetter(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new SendPostLetterRequest({  "file_url": "http://server.com/file.pdf",  "template_used": 1,  "colour": 1,  "duplex": 0,  "recipients": [    {      "address_name": "My Home Address",      "address_line_1": "Address 1",      "address_line_2": "Address 2",      "address_city": "CITY",      "address_state": "State",      "address_postal_code": 123456,      "address_country": "AU",      "return_address_id": 1,      "schedule": 1449573604    }  ]});

    controller.createSendPostLetter(body, function(error, response, context) {

    
	});
```



### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.createCalculatePrice") createCalculatePrice

> TODO: Add a method description


```javascript
function createCalculatePrice(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CalculatePriceRequest170({  "file_url": "http://server.com/file.pdf",  "template_used": 1,  "colour": 1,  "duplex": 0,  "recipients": [    "[]"  ],  "Body": ""});

    controller.createCalculatePrice(body, function(error, response, context) {

    
	});
```



### <a name="get_post_letter_history"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.getPostLetterHistory") getPostLetterHistory

> TODO: Add a method description


```javascript
function getPostLetterHistory(callback)
```

#### Example Usage

```javascript


    controller.getPostLetterHistory(function(error, response, context) {

    
	});
```



### <a name="get_export_post_letter_history"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.getExportPostLetterHistory") getExportPostLetterHistory

> TODO: Add a method description


```javascript
function getExportPostLetterHistory(filename, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | Filename for the export file. |



#### Example Usage

```javascript

    var filename = 'myexport.csv';

    controller.getExportPostLetterHistory(filename, function(error, response, context) {

    
	});
```



### <a name="create_a_post_return_address"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.createAPostReturnAddress") createAPostReturnAddress

> TODO: Add a method description


```javascript
function createAPostReturnAddress(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CreateAPostReturnAddressRequest({    "address_name":"My Home Address",    "address_line_1":"Maritime Avenue",    "address_line_2":"",    "address_city":"Flynn",    "address_state":"WA",    "address_postal_code":6302,    "address_country":"Australia"});

    controller.createAPostReturnAddress(body, function(error, response, context) {

    
	});
```



### <a name="get_list_of_post_return_addresses"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.getListOfPostReturnAddresses") getListOfPostReturnAddresses

> TODO: Add a method description


```javascript
function getListOfPostReturnAddresses(callback)
```

#### Example Usage

```javascript


    controller.getListOfPostReturnAddresses(function(error, response, context) {

    
	});
```



### <a name="get_post_return_address"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.getPostReturnAddress") getPostReturnAddress

> TODO: Add a method description


```javascript
function getPostReturnAddress(returnAddressId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| returnAddressId |  ``` Required ```  | Your return address id. |



#### Example Usage

```javascript

    var returnAddressId = 14;

    controller.getPostReturnAddress(returnAddressId, function(error, response, context) {

    
	});
```



### <a name="update_post_return_address"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.updatePostReturnAddress") updatePostReturnAddress

> TODO: Add a method description


```javascript
function updatePostReturnAddress(returnAddressId, body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| returnAddressId |  ``` Required ```  | Your return address id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var returnAddressId = 14;
    var body = new UpdatePostReturnAddressRequest({    "address_name":"My Home Address",    "address_line_1":"Maritime Avenue",    "address_line_2":"",    "address_city":"Flynn",    "address_state":"WA",    "address_postal_code":6302,    "address_country":"Australia"});

    controller.updatePostReturnAddress(returnAddressId, body, function(error, response, context) {

    
	});
```



### <a name="delete_post_return_address"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.deletePostReturnAddress") deletePostReturnAddress

> TODO: Add a method description


```javascript
function deletePostReturnAddress(returnAddressId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| returnAddressId |  ``` Required ```  | Your return address id. |



#### Example Usage

```javascript

    var returnAddressId = 12;

    controller.deletePostReturnAddress(returnAddressId, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="postcards_controller"></a>![Class: ](https://apidocs.io/img/class.png ".PostcardsController") PostcardsController

### Get singleton instance

The singleton instance of the ``` PostcardsController ``` class can be accessed from the API Client.

```javascript
var controller = lib.PostcardsController;
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


```javascript
function createSendPostcard(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new SendPostcardRequest({    "file_urls":[         "https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_front.pdf",         "https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_back.pdf"    ],    "recipients":[        {            "address_name":"My Home Address",            "address_line_1":"Address 1",            "address_line_2":"",            "address_city":"City",            "address_state":"State",            "address_postal_code":"123456",            "address_country":"AU",            "return_address_id":1        }    ]});

    controller.createSendPostcard(body, function(error, response, context) {

    
	});
```



### <a name="create_calculate_pricing"></a>![Method: ](https://apidocs.io/img/method.png ".PostcardsController.createCalculatePricing") createCalculatePricing

> For `file_urls` field. You can attach at least 1 and max of 2 PDF file urls.
> - Supply a single pdf with 2 pages (front and back)
> - Supply 2 urls to seperate PDFs


```javascript
function createCalculatePricing(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CalculatePricingRequest({    "file_urls":[        "https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_front.pdf",        "https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_back.pdf"    ],    "recipients":[        {            "address_name":"My Home Address",            "address_line_1":"Address 1",            "address_line_2":"",            "address_city":"City",            "address_state":"State",            "address_postal_code":"123456",            "address_country":"AU",            "return_address_id":1        }    ]});

    controller.createCalculatePricing(body, function(error, response, context) {

    
	});
```



### <a name="get_postcard_history"></a>![Method: ](https://apidocs.io/img/method.png ".PostcardsController.getPostcardHistory") getPostcardHistory

> TODO: Add a method description


```javascript
function getPostcardHistory(callback)
```

#### Example Usage

```javascript


    controller.getPostcardHistory(function(error, response, context) {

    
	});
```



### <a name="get_export_postcard_history"></a>![Method: ](https://apidocs.io/img/method.png ".PostcardsController.getExportPostcardHistory") getExportPostcardHistory

> TODO: Add a method description


```javascript
function getExportPostcardHistory(filename, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | Filename for the export file. |



#### Example Usage

```javascript

    var filename = 'myexport.csv';

    controller.getExportPostcardHistory(filename, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="referral_accounts_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ReferralAccountsController") ReferralAccountsController

### Get singleton instance

The singleton instance of the ``` ReferralAccountsController ``` class can be accessed from the API Client.

```javascript
var controller = lib.ReferralAccountsController;
```

### <a name="get_list_of_referral_accounts"></a>![Method: ](https://apidocs.io/img/method.png ".ReferralAccountsController.getListOfReferralAccounts") getListOfReferralAccounts

> TODO: Add a method description


```javascript
function getListOfReferralAccounts(callback)
```

#### Example Usage

```javascript


    controller.getListOfReferralAccounts(function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="reseller_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ResellerController") ResellerController

### Get singleton instance

The singleton instance of the ``` ResellerController ``` class can be accessed from the API Client.

```javascript
var controller = lib.ResellerController;
```

### <a name="get_reseller_setting"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerController.getResellerSetting") getResellerSetting

> Get reseller setting.


```javascript
function getResellerSetting(callback)
```

#### Example Usage

```javascript


    controller.getResellerSetting(function(error, response, context) {

    
	});
```



### <a name="update_reseller_setting"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerController.updateResellerSetting") updateResellerSetting

> Update a specific reseller setting.


```javascript
function updateResellerSetting(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new UpdateResellerSettingRequest(    {        "allow_public_signups":1,        "default_margin":100,        "default_margin_numbers":150,        "trial_balance":50,        "subdomain":"subdomain",        "colour_navigation":"#9999FF",        "logo_url_light":"http://url.com/light",        "logo_url_dark":"http://url.com/dark",        "company_name":"MyCompany"    });

    controller.updateResellerSetting(body, function(error, response, context) {

    
	});
```



### <a name="get_reseller_by_subdomain"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerController.getResellerBySubdomain") getResellerBySubdomain

> Get reseller setting by subdomin.


```javascript
function getResellerBySubdomain(subdomain, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subdomain |  ``` Required ```  | Subdomain |



#### Example Usage

```javascript

    var subdomain = 'mysubdomain';

    controller.getResellerBySubdomain(subdomain, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="reseller_accounts_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ResellerAccountsController") ResellerAccountsController

### Get singleton instance

The singleton instance of the ``` ResellerAccountsController ``` class can be accessed from the API Client.

```javascript
var controller = lib.ResellerAccountsController;
```

### <a name="list_of_reseller_accounts"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.listOfResellerAccounts") listOfResellerAccounts

> Get list of Reseller Accounts


```javascript
function listOfResellerAccounts(callback)
```

#### Example Usage

```javascript


    controller.listOfResellerAccounts(function(error, response, context) {

    
	});
```



### <a name="get_reseller_account"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.getResellerAccount") getResellerAccount

> Get a specific reseller account.


```javascript
function getResellerAccount(clientUserId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| clientUserId |  ``` Required ```  | The client user id. |



#### Example Usage

```javascript

    var clientUserId = 24;

    controller.getResellerAccount(clientUserId, function(error, response, context) {

    
	});
```



### <a name="create_reseller_account"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.createResellerAccount") createResellerAccount

> TODO: Add a method description


```javascript
function createResellerAccount(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CreateResellerAccountRequest(    {        "username":"johndoe2",        "user_email":"johndoe2@awesome.com",        "user_phone":"518-481-1002",        "user_first_name":"John",        "user_last_name":"Doe",        "country":"US",        "password":"pass",        "account_name":"The Awesome Company"    });

    controller.createResellerAccount(body, function(error, response, context) {

    
	});
```



### <a name="create_reseller_account_public"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.createResellerAccountPublic") createResellerAccountPublic

> TODO: Add a method description


```javascript
function createResellerAccountPublic(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CreateResellerAccountPublicRequest({    "reseller_user_id":1,    "username":"john_awesome",    "user_email":"johnis@awesome.com",    "user_phone":"+61261063270",    "user_first_name":"John",    "user_last_name":"Awesome",    "country":"AU",    "password":"pass",    "account_name":"The Awesome Company"});

    controller.createResellerAccountPublic(body, function(error, response, context) {

    
	});
```



### <a name="update_reseller_account"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.updateResellerAccount") updateResellerAccount

> TODO: Add a method description


```javascript
function updateResellerAccount(clientUserId, body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| clientUserId |  ``` Required ```  | Your client user id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var clientUserId = 24;
    var body = new UpdateResellerAccountRequest(    {        "username":"johndoe2",        "user_email":"johndoe2@awesome.com",        "user_phone":"518-481-1002",        "user_first_name":"John",        "user_last_name":"Doe",        "country":"US",        "password":"pass",        "account_name":"The Awesome Company"    });

    controller.updateResellerAccount(clientUserId, body, function(error, response, context) {

    
	});
```



### <a name="update_transfer_credit"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.updateTransferCredit") updateTransferCredit

> TODO: Add a method description


```javascript
function updateTransferCredit(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new TransferCreditRequest({"key":"value"});

    controller.updateTransferCredit(body, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="sdk_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SDKController") SDKController

### Get singleton instance

The singleton instance of the ``` SDKController ``` class can be accessed from the API Client.

```javascript
var controller = lib.SDKController;
```

### <a name="get_sdk_download"></a>![Method: ](https://apidocs.io/img/method.png ".SDKController.getSDKDownload") getSDKDownload

> TODO: Add a method description


```javascript
function getSDKDownload(type, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| type |  ``` Required ```  | Supported types. |



#### Example Usage

```javascript

    var type = 'type';

    controller.getSDKDownload(type, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="search_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SearchController") SearchController

### Get singleton instance

The singleton instance of the ``` SearchController ``` class can be accessed from the API Client.

```javascript
var controller = lib.SearchController;
```

### <a name="search_contacts_lists"></a>![Method: ](https://apidocs.io/img/method.png ".SearchController.searchContactsLists") searchContactsLists

> TODO: Add a method description


```javascript
function searchContactsLists(q, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| q |  ``` Required ```  | Your keyword or query. |



#### Example Usage

```javascript

    var q = 'Gorne';

    controller.searchContactsLists(q, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="sms_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SMSController") SMSController

### Get singleton instance

The singleton instance of the ``` SMSController ``` class can be accessed from the API Client.

```javascript
var controller = lib.SMSController;
```

### <a name="create_send_an_sms"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.createSendAnSMS") createSendAnSMS

> You can post **up to 1000 messages** with each API call.


```javascript
function createSendAnSMS(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new SendAnSMSRequest({"key":"value"});

    controller.createSendAnSMS(body, function(error, response, context) {

    
	});
```



### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.createCalculatePrice") createCalculatePrice

> TODO: Add a method description


```javascript
function createCalculatePrice(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CalculatePriceRequest205({"key":"value"});

    controller.createCalculatePrice(body, function(error, response, context) {

    
	});
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


```javascript
function getAllHistory(dateFrom, dateTo, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateFrom |  ``` Optional ```  | Timestamp (from) used to show records by date. |
| dateTo |  ``` Optional ```  | Timestamp (to) used to show recrods by date. |



#### Example Usage

```javascript

    var dateFrom = 1449459940;
    var dateTo = 1449659940;

    controller.getAllHistory(dateFrom, dateTo, function(error, response, context) {

    
	});
```



### <a name="get_export_sms_history"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.getExportSMSHistory") getExportSMSHistory

> TODO: Add a method description


```javascript
function getExportSMSHistory(callback)
```

#### Example Usage

```javascript


    controller.getExportSMSHistory(function(error, response, context) {

    
	});
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


```javascript
function getAllDeliveryReceipts(callback)
```

#### Example Usage

```javascript


    controller.getAllDeliveryReceipts(function(error, response, context) {

    
	});
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


```javascript
function getASpecificDeliveryReceipt(messageId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Your message id. |



#### Example Usage

```javascript

    var messageId = 88AB118E EB1B 478C 98CE 6C73ABA23F67;

    controller.getASpecificDeliveryReceipt(messageId, function(error, response, context) {

    
	});
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


```javascript
function addATestDeliveryReceipt(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new AddATestDeliveryReceiptRequest(    {        "url":"http://yourUrl.com"    });

    controller.addATestDeliveryReceipt(body, function(error, response, context) {

    
	});
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


```javascript
function updateMarkDeliveryReceiptsAsRead(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new MarkDeliveryReceiptsAsReadRequest({    "date_before": 1441958441});

    controller.updateMarkDeliveryReceiptsAsRead(body, function(error, response, context) {

    
	});
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


```javascript
function getAllInboundSMSPull(callback)
```

#### Example Usage

```javascript


    controller.getAllInboundSMSPull(function(error, response, context) {

    
	});
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


```javascript
function getSpecificInboundPull(messageId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Message ID. Must be a valid GUID. |



#### Example Usage

```javascript

    var messageId = 5D420421-8715-4461-A9A2-C8F569E41835;

    controller.getSpecificInboundPull(messageId, function(error, response, context) {

    
	});
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


```javascript
function addATestInboundSMS(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new AddATestInboundSMSRequest(    {        "url":"http://yourUrl.com"    });

    controller.addATestInboundSMS(body, function(error, response, context) {

    
	});
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


```javascript
function updateMarkASpecificInboundSMSAsRead(messageId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | B7CE432193CD-0753597B7293 (string, required) - The message ID you want to mark as read. |



#### Example Usage

```javascript

    var messageId = 307EF035;

    controller.updateMarkASpecificInboundSMSAsRead(messageId, function(error, response, context) {

    
	});
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


```javascript
function updateMarkAllInboundSMSAsRead(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new MarkAllInboundSMSAsReadRequest(    {        "date_before":1442398100    });

    controller.updateMarkAllInboundSMSAsRead(body, function(error, response, context) {

    
	});
```



### <a name="update_cancel_a_scheduled_message"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.updateCancelAScheduledMessage") updateCancelAScheduledMessage

> TODO: Add a method description


```javascript
function updateCancelAScheduledMessage(messageId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | B7CE432193CD-0753597B7293 (string, required) - The message ID you want to cancel. |



#### Example Usage

```javascript

    var messageId = 307EF035;

    controller.updateCancelAScheduledMessage(messageId, function(error, response, context) {

    
	});
```



### <a name="update_cancel_all_scheduled_messages"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.updateCancelAllScheduledMessages") updateCancelAllScheduledMessages

> TODO: Add a method description


```javascript
function updateCancelAllScheduledMessages(callback)
```

#### Example Usage

```javascript


    controller.updateCancelAllScheduledMessages(function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="sms_campaigns_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SMSCampaignsController") SMSCampaignsController

### Get singleton instance

The singleton instance of the ``` SMSCampaignsController ``` class can be accessed from the API Client.

```javascript
var controller = lib.SMSCampaignsController;
```

### <a name="create_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.createSMSCampaign") createSMSCampaign

> You can post to a list with **up to 20000 recipients** with each API call.


```javascript
function createSMSCampaign(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CreateSMSCampaignRequest({    "list_id":428,    "name":"My Campaign 1",    "from":"+61353787448",    "body":"This is my new campaign message.",    "schedule":1444821615});

    controller.createSMSCampaign(body, function(error, response, context) {

    
	});
```



### <a name="create_calculate_price_for_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.createCalculatePriceForSMSCampaign") createCalculatePriceForSMSCampaign

> TODO: Add a method description


```javascript
function createCalculatePriceForSMSCampaign(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CalculatePriceForSMSCampaignRequest({    "list_id":428,    "name":"My Campaign 1",    "from":"+61353787448",    "body":"(First Name), this is your new campaign message."});

    controller.createCalculatePriceForSMSCampaign(body, function(error, response, context) {

    
	});
```



### <a name="update_an_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.updateAnSMSCampaign") updateAnSMSCampaign

> TODO: Add a method description


```javascript
function updateAnSMSCampaign(smsCampaignId, body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| smsCampaignId |  ``` Required ```  | Your SMS Campaign id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var smsCampaignId = 1;
    var body = new UpdateAnSMSCampaignRequest({    "list_id":428,    "name":"Awesome campaign.",    "from":"+61353787447",    "body":"his is an awesome message.",    "schedule":1444821615});

    controller.updateAnSMSCampaign(smsCampaignId, body, function(error, response, context) {

    
	});
```



### <a name="get_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.getSMSCampaign") getSMSCampaign

> TODO: Add a method description


```javascript
function getSMSCampaign(smsCampaignId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| smsCampaignId |  ``` Required ```  | Your SMS campaign id. |



#### Example Usage

```javascript

    var smsCampaignId = 1;

    controller.getSMSCampaign(smsCampaignId, function(error, response, context) {

    
	});
```



### <a name="update_cancel_an_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.updateCancelAnSMSCampaign") updateCancelAnSMSCampaign

> TODO: Add a method description


```javascript
function updateCancelAnSMSCampaign(smsCampaignId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| smsCampaignId |  ``` Required ```  | Your SMS Campaign id. |



#### Example Usage

```javascript

    var smsCampaignId = 1;

    controller.updateCancelAnSMSCampaign(smsCampaignId, function(error, response, context) {

    
	});
```



### <a name="get_list_of_sms_campaigns"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.getListOfSMSCampaigns") getListOfSMSCampaigns

> TODO: Add a method description


```javascript
function getListOfSMSCampaigns(callback)
```

#### Example Usage

```javascript


    controller.getListOfSMSCampaigns(function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="sms_templates_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SMSTemplatesController") SMSTemplatesController

### Get singleton instance

The singleton instance of the ``` SMSTemplatesController ``` class can be accessed from the API Client.

```javascript
var controller = lib.SMSTemplatesController;
```

### <a name="list_of_templates"></a>![Method: ](https://apidocs.io/img/method.png ".SMSTemplatesController.listOfTemplates") listOfTemplates

> Get list of templates.


```javascript
function listOfTemplates(callback)
```

#### Example Usage

```javascript


    controller.listOfTemplates(function(error, response, context) {

    
	});
```



### <a name="create_a_template"></a>![Method: ](https://apidocs.io/img/method.png ".SMSTemplatesController.createATemplate") createATemplate

> Create new template.


```javascript
function createATemplate(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CreateATemplateRequest(    {        "template_name":"Template 501916",        "body":"This is a sample content: H7YI68B3yk for this template."    });

    controller.createATemplate(body, function(error, response, context) {

    
	});
```



### <a name="update_a_template"></a>![Method: ](https://apidocs.io/img/method.png ".SMSTemplatesController.updateATemplate") updateATemplate

> TODO: Add a method description


```javascript
function updateATemplate(templateId, body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var templateId = 25;
    var body = new UpdateATemplateRequest(    {        "template_name":"I am updated",        "body":"This is a sample content: Sc0KNWgSMG for this template."    });

    controller.updateATemplate(templateId, body, function(error, response, context) {

    
	});
```



### <a name="delete_a_template"></a>![Method: ](https://apidocs.io/img/method.png ".SMSTemplatesController.deleteATemplate") deleteATemplate

> TODO: Add a method description


```javascript
function deleteATemplate(templateId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |



#### Example Usage

```javascript

    var templateId = 25;

    controller.deleteATemplate(templateId, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="statistics_controller"></a>![Class: ](https://apidocs.io/img/class.png ".StatisticsController") StatisticsController

### Get singleton instance

The singleton instance of the ``` StatisticsController ``` class can be accessed from the API Client.

```javascript
var controller = lib.StatisticsController;
```

### <a name="get_sms_statistics"></a>![Method: ](https://apidocs.io/img/method.png ".StatisticsController.getSMSStatistics") getSMSStatistics

> TODO: Add a method description


```javascript
function getSMSStatistics(callback)
```

#### Example Usage

```javascript


    controller.getSMSStatistics(function(error, response, context) {

    
	});
```



### <a name="get_voice_statistics"></a>![Method: ](https://apidocs.io/img/method.png ".StatisticsController.getVoiceStatistics") getVoiceStatistics

> TODO: Add a method description


```javascript
function getVoiceStatistics(callback)
```

#### Example Usage

```javascript


    controller.getVoiceStatistics(function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="subaccounts_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SubaccountsController") SubaccountsController

### Get singleton instance

The singleton instance of the ``` SubaccountsController ``` class can be accessed from the API Client.

```javascript
var controller = lib.SubaccountsController;
```

### <a name="get_all_subaccounts"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.getAllSubaccounts") getAllSubaccounts

> TODO: Add a method description


```javascript
function getAllSubaccounts(callback)
```

#### Example Usage

```javascript


    controller.getAllSubaccounts(function(error, response, context) {

    
	});
```



### <a name="create_a_new_subaccount"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.createANewSubaccount") createANewSubaccount

> TODO: Add a method description


```javascript
function createANewSubaccount(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CreateANewSubaccountRequest(    {        "api_username":"nameP99",        "password":"pass",        "email":"testvrq@gmail.com",        "phone_number":"941-751-3278",        "first_name":"FirstnameeGPqV",        "last_name":"LastnamePvjJp"    });

    controller.createANewSubaccount(body, function(error, response, context) {

    
	});
```



### <a name="get_a_specific_subaccount"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.getASpecificSubaccount") getASpecificSubaccount

> TODO: Add a method description


```javascript
function getASpecificSubaccount(subaccountId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |



#### Example Usage

```javascript

    var subaccountId = 59;

    controller.getASpecificSubaccount(subaccountId, function(error, response, context) {

    
	});
```



### <a name="update_a_specific_subaccount"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.updateASpecificSubaccount") updateASpecificSubaccount

> TODO: Add a method description


```javascript
function updateASpecificSubaccount(subaccountId, body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var subaccountId = 59;
    var body = new UpdateASpecificSubaccountRequest(    {        "password":"pass",        "email":"testfP0.updated@gmail.com",        "phone_number":"+19417519130",        "first_name":"FirstnameKvdRZUpdated",        "last_name":"LastnameHUPYGUpdated",        "access_users": 1,        "access_billing": 1,        "access_reporting": 1,        "access_contacts": 1,        "access_settings": 1,        "access_sms": 1,        "access_email": 1,        "access_voice": 1,        "access_fax": 1,        "access_post": 1,        "access_reseller": 1,        "access_mms": 1,        "share_campaigns": 0,        "notes": null    });

    controller.updateASpecificSubaccount(subaccountId, body, function(error, response, context) {

    
	});
```



### <a name="delete_a_specific_subaccount"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.deleteASpecificSubaccount") deleteASpecificSubaccount

> TODO: Add a method description


```javascript
function deleteASpecificSubaccount(subaccountId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |



#### Example Usage

```javascript

    var subaccountId = 59;

    controller.deleteASpecificSubaccount(subaccountId, function(error, response, context) {

    
	});
```



### <a name="update_regenerate_api_key"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.updateRegenerateAPIKey") updateRegenerateAPIKey

> TODO: Add a method description


```javascript
function updateRegenerateAPIKey(subaccountId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |



#### Example Usage

```javascript

    var subaccountId = 59;

    controller.updateRegenerateAPIKey(subaccountId, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="timezones_controller"></a>![Class: ](https://apidocs.io/img/class.png ".TimezonesController") TimezonesController

### Get singleton instance

The singleton instance of the ``` TimezonesController ``` class can be accessed from the API Client.

```javascript
var controller = lib.TimezonesController;
```

### <a name="get_timezones"></a>![Method: ](https://apidocs.io/img/method.png ".TimezonesController.getTimezones") getTimezones

> Get supported list of timezones.


```javascript
function getTimezones(callback)
```

#### Example Usage

```javascript


    controller.getTimezones(function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="transactional_email_controller"></a>![Class: ](https://apidocs.io/img/class.png ".TransactionalEmailController") TransactionalEmailController

### Get singleton instance

The singleton instance of the ``` TransactionalEmailController ``` class can be accessed from the API Client.

```javascript
var controller = lib.TransactionalEmailController;
```

### <a name="create_email_send"></a>![Method: ](https://apidocs.io/img/method.png ".TransactionalEmailController.createEmailSend") createEmailSend

> TODO: Add a method description


```javascript
function createEmailSend(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new EmailSendRequest({"key":"value"});

    controller.createEmailSend(body, function(error, response, context) {

    
	});
```



### <a name="create_email_price"></a>![Method: ](https://apidocs.io/img/method.png ".TransactionalEmailController.createEmailPrice") createEmailPrice

> TODO: Add a method description


```javascript
function createEmailPrice(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new EmailPriceRequest({"key":"value"});

    controller.createEmailPrice(body, function(error, response, context) {

    
	});
```



### <a name="get_email_history"></a>![Method: ](https://apidocs.io/img/method.png ".TransactionalEmailController.getEmailHistory") getEmailHistory

> TODO: Add a method description


```javascript
function getEmailHistory(callback)
```

#### Example Usage

```javascript


    controller.getEmailHistory(function(error, response, context) {

    
	});
```



### <a name="get_export_history"></a>![Method: ](https://apidocs.io/img/method.png ".TransactionalEmailController.getExportHistory") getExportHistory

> TODO: Add a method description


```javascript
function getExportHistory(filename, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | File name for the export file. |



#### Example Usage

```javascript

    var filename = 'myexport.csv';

    controller.getExportHistory(filename, function(error, response, context) {

    
	});
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


```javascript
function addATestDeliveryReceipt(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new AddATestDeliveryReceiptRequest(    {        "url":"http://yourUrl.com"    });

    controller.addATestDeliveryReceipt(body, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="uploads_controller"></a>![Class: ](https://apidocs.io/img/class.png ".UploadsController") UploadsController

### Get singleton instance

The singleton instance of the ``` UploadsController ``` class can be accessed from the API Client.

```javascript
var controller = lib.UploadsController;
```

### <a name="upload_a_file"></a>![Method: ](https://apidocs.io/img/method.png ".UploadsController.uploadAFile") uploadAFile

> The `upload` endpoint provides a method for converting files from an unspported format to a format that one of our endpoints can handle.
> Files can be submitted two ways:
> 1. Using `base64` encoding in an `application/json` request. In this case, submit the `base64`-encoded file contents in the `content` field of the request body, and `convert` can be specified either also in the body or as part of the query string.
> 2. Using `multipart/form-data` encoding, in the same way it would be submitted using a HTML form. You may find cURL useful for this. For an example of how to do this, see one of our [SDKs](https://dashboard.clicksend.com/#/libraries-sdk/main). In this case, specify `convert` in the query string.
> Note that `convert` specifies the conversion to take place - that is, what the result should be compatible with - and can be any of `fax`, `mms`, `csv` or `post`.
> All files have 10 minutes expiry.


```javascript
function uploadAFile(body, convert, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |
| convert |  ``` Optional ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new UploadAFileRequest({"key":"value"});
    var convert = 'convert';

    controller.uploadAFile(body, convert, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="voice_controller"></a>![Class: ](https://apidocs.io/img/class.png ".VoiceController") VoiceController

### Get singleton instance

The singleton instance of the ``` VoiceController ``` class can be accessed from the API Client.

```javascript
var controller = lib.VoiceController;
```

### <a name="create_send_a_voice_call"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.createSendAVoiceCall") createSendAVoiceCall

> You can post **up to 1000 messages** with each API call.


```javascript
function createSendAVoiceCall(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new SendAVoiceCallRequest({"key":"value"});

    controller.createSendAVoiceCall(body, function(error, response, context) {

    
	});
```



### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.createCalculatePrice") createCalculatePrice

> TODO: Add a method description


```javascript
function createCalculatePrice(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CalculatePriceRequest263({"key":"value"});

    controller.createCalculatePrice(body, function(error, response, context) {

    
	});
```



### <a name="get_voice_languages"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.getVoiceLanguages") getVoiceLanguages

> TODO: Add a method description


```javascript
function getVoiceLanguages(callback)
```

#### Example Usage

```javascript


    controller.getVoiceLanguages(function(error, response, context) {

    
	});
```



### <a name="get_voice_history"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.getVoiceHistory") getVoiceHistory

> TODO: Add a method description


```javascript
function getVoiceHistory(dateFrom, dateTo, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateFrom |  ``` Optional ```  | Timestamp (from) used to show records by date. |
| dateTo |  ``` Optional ```  | Timestamp (to) used to show recrods by date. |



#### Example Usage

```javascript

    var dateFrom = 1443501617;
    var dateTo = 1443501727;

    controller.getVoiceHistory(dateFrom, dateTo, function(error, response, context) {

    
	});
```



### <a name="get_export_voice_history"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.getExportVoiceHistory") getExportVoiceHistory

> TODO: Add a method description


```javascript
function getExportVoiceHistory(callback)
```

#### Example Usage

```javascript


    controller.getExportVoiceHistory(function(error, response, context) {

    
	});
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


```javascript
function getVoiceReceipts(callback)
```

#### Example Usage

```javascript


    controller.getVoiceReceipts(function(error, response, context) {

    
	});
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


```javascript
function addATestDeliveryReceipt(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new AddATestDeliveryReceiptRequest(    {        "url":"http://yourUrl.com"    });

    controller.addATestDeliveryReceipt(body, function(error, response, context) {

    
	});
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


```javascript
function getSpecificVoiceReceipt(messageId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | 3055-45F1-9B79-F2C43509FD16 (string, required) - The voice receipt message id. |



#### Example Usage

```javascript

    var messageId = 28DD2718;

    controller.getSpecificVoiceReceipt(messageId, function(error, response, context) {

    
	});
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


```javascript
function updateMarkedVoiceReceiptsAsRead(dateBefore, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateBefore |  ``` Required ```  | An optional timestamp - mark all as read before this timestamp. If not given, all receipts will be marked as read. |



#### Example Usage

```javascript

    var dateBefore = 193.51832945995;

    controller.updateMarkedVoiceReceiptsAsRead(dateBefore, function(error, response, context) {

    
	});
```



### <a name="update_cancel_a_specific_voice_call"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.updateCancelASpecificVoiceCall") updateCancelASpecificVoiceCall

> TODO: Add a method description


```javascript
function updateCancelASpecificVoiceCall(messageId, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Your voice message id. |



#### Example Usage

```javascript

    var messageId = 7B5BFC19 06B7 49C1 8DCDFB011600E12B;

    controller.updateCancelASpecificVoiceCall(messageId, function(error, response, context) {

    
	});
```



### <a name="update_cancel_all_voice_calls"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.updateCancelAllVoiceCalls") updateCancelAllVoiceCalls

> TODO: Add a method description


```javascript
function updateCancelAllVoiceCalls(callback)
```

#### Example Usage

```javascript


    controller.updateCancelAllVoiceCalls(function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)



