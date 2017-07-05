# Getting started

TODO: Add a description

## How to Build


The generated code has dependencies over external libraries like UniRest. These dependencies are defined in the ```PodFile``` file that comes with the SDK. 
To resolve these dependencies, we use the Cocoapods package manager.
Visit https://guides.cocoapods.org/using/getting-started.html to setup Cocoapods on your system.
Open command prompt and type ```pod --version```. This should display the current version of Cocoapods installed if the installation was successful.

Using command line, navigate to the directory containing the generated files (including ```PodFile```) for the SDK. 
Run the command ```pod install```. This should install all the required dependencies and create the ```pods``` directory in your project directory.

![Installing dependencies using Cocoapods](https://apidocs.io/illustration/objc?step=AddDependencies&workspaceFolder=ClickSend%20REST%20API%20v3-ObjC&workspaceName=ClickSendRESTAPIV3&projectName=ClickSendRESTAPIV3&rootNamespace=ClickSendRESTAPIV3)

Open the project workspace using the (ClickSendRESTAPIV3.xcworkspace) file. Invoke the build process using `Command(⌘)+B` shortcut key or using the `Build` menu as shown below.

![Building SDK using Xcode](https://apidocs.io/illustration/objc?step=BuildSDK&workspaceFolder=ClickSend%20REST%20API%20v3-ObjC&workspaceName=ClickSendRESTAPIV3&projectName=ClickSendRESTAPIV3&rootNamespace=ClickSendRESTAPIV3)


## How to Use

The generated code is a Cocoa Touch Static Library which can be used in any iOS project. The support for these generated libraries go all the way back to iOS 6.

The following section explains how to use the ClickSendRESTAPIV3 library in a new iOS project.     
### 1. Starting a new project
To start a new project, left-click on the ```Create a new Xcode project```.
![Create Test Project - Step 1](https://apidocs.io/illustration/objc?step=Test1&workspaceFolder=ClickSend%20REST%20API%20v3-ObjC&workspaceName=ClickSendRESTAPIV3&projectName=ClickSendRESTAPIV3&rootNamespace=ClickSendRESTAPIV3)

Next, choose **Single View Application** and click ```Next```.
![Create Test Project - Step 2](https://apidocs.io/illustration/objc?step=Test2&workspaceFolder=ClickSend%20REST%20API%20v3-ObjC&workspaceName=ClickSendRESTAPIV3&projectName=ClickSendRESTAPIV3&rootNamespace=ClickSendRESTAPIV3)

Provide **Test-Project** as the product name click ```Next```.
![Create Test Project - Step 3](https://apidocs.io/illustration/objc?step=Test3&workspaceFolder=ClickSend%20REST%20API%20v3-ObjC&workspaceName=ClickSendRESTAPIV3&projectName=ClickSendRESTAPIV3&rootNamespace=ClickSendRESTAPIV3)

Choose the desired location of your project folder and click ```Create```.
![Create Test Project - Step 4](https://apidocs.io/illustration/objc?step=Test4&workspaceFolder=ClickSend%20REST%20API%20v3-ObjC&workspaceName=ClickSendRESTAPIV3&projectName=ClickSendRESTAPIV3&rootNamespace=ClickSendRESTAPIV3)

### 2. Adding the static library dependency
To add this dependency open a terminal and navigate to your project folder. Next, input ```pod init``` and press enter.
![Add dependency - Step 1](https://apidocs.io/illustration/objc?step=Add0&workspaceFolder=ClickSend%20REST%20API%20v3-ObjC&workspaceName=ClickSendRESTAPIV3&projectName=ClickSendRESTAPIV3&rootNamespace=ClickSendRESTAPIV3)

Next, open the newly created ```PodFile``` in your favourite text editor. Add the following line : pod 'ClickSendRESTAPIV3', :path => 'Vendor/ClickSendRESTAPIV3'
![Add dependency - Step 2](https://apidocs.io/illustration/objc?step=Add1&workspaceFolder=ClickSend%20REST%20API%20v3-ObjC&workspaceName=ClickSendRESTAPIV3&projectName=ClickSendRESTAPIV3&rootNamespace=ClickSendRESTAPIV3)

Execute `pod install` from terminal to install the dependecy in your project. This would add the dependency to the newly created test project.
![Add dependency - Step 3](https://apidocs.io/illustration/objc?step=Add2&workspaceFolder=ClickSend%20REST%20API%20v3-ObjC&workspaceName=ClickSendRESTAPIV3&projectName=ClickSendRESTAPIV3&rootNamespace=ClickSendRESTAPIV3)


## How to Test

Unit tests in this SDK can be run using Xcode. 

First build the SDK as shown in the steps above and naivgate to the project directory and open the ClickSendRESTAPIV3.xcworkspace file.

Go to the test explorer in Xcode as shown in the picture below and click on `run tests` from the menu. 
![Run tests](https://apidocs.io/illustration/objc?step=RunTests&workspaceFolder=ClickSend%20REST%20API%20v3-ObjC&workspaceName=ClickSendRESTAPIV3&projectName=ClickSendRESTAPIV3&rootNamespace=ClickSendRESTAPIV3)


## Initialization

### Authentication
In order to setup authentication and initialization of the API client, you need the following information.

| Parameter | Description |
|-----------|-------------|
| basicAuthUserName | The username to use with basic authentication |
| basicAuthPassword | The password to use with basic authentication |



Configuration variables can be set as following.
```Objc
// Configuration parameters and credentials
Configuration_BasicAuthUserName = "Configuration_BasicAuthUserName"; // The username to use with basic authentication
Configuration_BasicAuthPassword = "Configuration_BasicAuthPassword"; // The password to use with basic authentication

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
```objc
Account* account = [[Account alloc]init] ;
```

### <a name="create_a_new_account_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.createANewAccountAsyncWithBody") createANewAccountAsyncWithBody

> **Note:** *Authentication isn't required to create a new account.*


```objc
function createANewAccountAsyncWithBody:(CreateANewAccountRequest*) body
                completionBlock:(CompletedPostCreateANewAccount) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CreateANewAccountRequest* body = (CreateANewAccountRequest*) [APIHelper jsonDeserialize: @"    {        \"username\":\"johndoe1\",        \"user_email\":\"johndoe1@awesome.com\",        \"user_phone\":\"518-481-1001\",        \"user_first_name\":\"John\",        \"user_last_name\":\"Doe\",        \"country\":\"US\",        \"password\":\"pass\",        \"account_name\":\"The Awesome Company\"    }"
                toClass: CreateANewAccountRequest.class];

    [self.account createANewAccountAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CreateANewAccountResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_account_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.updateAccountAsyncWithBody") updateAccountAsyncWithBody

> TODO: Add a method description


```objc
function updateAccountAsyncWithBody:(UpdateAccountRequest*) body
                completionBlock:(CompletedPutUpdateAccount) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    UpdateAccountRequest* body = (UpdateAccountRequest*) [APIHelper jsonDeserialize: @"    {        \"username\":\"johndoe\",        \"user_email\":\"johndoe@awesome.com\",        \"user_phone\":\"518-481-1002\",        \"user_first_name\":\"John\",        \"user_last_name\":\"Doe\",        \"country\":\"AU\",        \"password\":\"pass\",        \"account_name\":\"The Awesome Company\",        \"timezone\": \"Australia/Melbourne\",        \"private_uploads\": 1,        \"setting_sms_hide_your_number\": 0,        \"setting_sms_hide_business_name\": 1    }"
                toClass: UpdateAccountRequest.class];

    [self.account updateAccountAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, UpdateAccountResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_account_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.getAccountWithCompletionBlock") getAccountWithCompletionBlock

> TODO: Add a method description


```objc
function getAccountWithCompletionBlock:(CompletedGetAccount) onCompleted()
```



#### Example Usage

```objc

    [self.account getAccountWithCompletionBlock:  ^(BOOL success, HttpContext* context, GetAccountResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_account_usage_async_with_year"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.getAccountUsageAsyncWithYear") getAccountUsageAsyncWithYear

> TODO: Add a method description


```objc
function getAccountUsageAsyncWithYear:(double) year
                month:(double) month
                type:(NSString*) type
                completionBlock:(CompletedGetAccountUsage) onCompleted(year month : month type : type)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| year |  ``` Required ```  | Your account usage year. |
| month |  ``` Required ```  | Your account usage month. |
| type |  ``` Required ```  | The account type. Value can only be either email or subaccount. |





#### Example Usage

```objc
    // Parameters for the API call
    double year = [@"2016" doubleValue];
    double month = [@"4" doubleValue];
    NSString* type = @"subaccount";

    [self.account getAccountUsageAsyncWithYear: year month : month type : type  completionBlock:^(BOOL success, HttpContext* context, AccountUsageResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_send_account_activation_token_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.updateSendAccountActivationTokenAsyncWithBody") updateSendAccountActivationTokenAsyncWithBody

> TODO: Add a method description


```objc
function updateSendAccountActivationTokenAsyncWithBody:(SendAccountActivationTokenRequest*) body
                completionBlock:(CompletedPutSendAccountActivationToken) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    SendAccountActivationTokenRequest* body = (SendAccountActivationTokenRequest*) [APIHelper jsonDeserialize: @"    {        \"user_phone\":\"352-394-4199\",        \"type\":\"sms\",        \"country\": \"US\"    }"
                toClass: SendAccountActivationTokenRequest.class];

    [self.account updateSendAccountActivationTokenAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, SendAccountActivationTokenResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_verify_new_account_async_with_activation_token"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.updateVerifyNewAccountAsyncWithActivationToken") updateVerifyNewAccountAsyncWithActivationToken

> TODO: Add a method description


```objc
function updateVerifyNewAccountAsyncWithActivationToken:(NSString*) activationToken
                completionBlock:(CompletedPutVerifyNewAccount) onCompleted(activationToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| activationToken |  ``` Required ```  | The ActivationToken to be used to verify an account. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* activationToken = @"1827364";

    [self.account updateVerifyNewAccountAsyncWithActivationToken: activationToken  completionBlock:^(BOOL success, HttpContext* context, VerifyNewAccountResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="account_recharge_controller"></a>![Class: ](https://apidocs.io/img/class.png ".AccountRechargeController") AccountRechargeController

### Get singleton instance
```objc
AccountRecharge* accountRecharge = [[AccountRecharge alloc]init] ;
```

### <a name="get_credit_card_info_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.getCreditCardInfoWithCompletionBlock") getCreditCardInfoWithCompletionBlock

> TODO: Add a method description


```objc
function getCreditCardInfoWithCompletionBlock:(CompletedGetCreditCardInfo) onCompleted()
```



#### Example Usage

```objc

    [self.accountRecharge getCreditCardInfoWithCompletionBlock:  ^(BOOL success, HttpContext* context, GetCreditCardInfoResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_credit_card_info_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.updateCreditCardInfoAsyncWithBody") updateCreditCardInfoAsyncWithBody

> TODO: Add a method description


```objc
function updateCreditCardInfoAsyncWithBody:(UpdateCreditCardInfoRequest*) body
                completionBlock:(CompletedPutUpdateCreditCardInfo) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    UpdateCreditCardInfoRequest* body = [[UpdateCreditCardInfoRequest alloc]init];

    [self.accountRecharge updateCreditCardInfoAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, UpdateCreditCardInfoResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="list_of_packages_async_with_country"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.listOfPackagesAsyncWithCountry") listOfPackagesAsyncWithCountry

> TODO: Add a method description


```objc
function listOfPackagesAsyncWithCountry:(NSString*) country
                completionBlock:(CompletedGetListOfPackages) onCompleted(country)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Optional ```  | Your country. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* country = @"\"AU\"";

    [self.accountRecharge listOfPackagesAsyncWithCountry: country  completionBlock:^(BOOL success, HttpContext* context, ListOfPackagesResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_purchase_a_package_async_with_package_id"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.updatePurchaseAPackageAsyncWithPackageId") updatePurchaseAPackageAsyncWithPackageId

> TODO: Add a method description


```objc
function updatePurchaseAPackageAsyncWithPackageId:(double) packageId
                completionBlock:(CompletedPutPurchaseAPackage) onCompleted(packageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| packageId |  ``` Required ```  | Your package id. |





#### Example Usage

```objc
    // Parameters for the API call
    double packageId = [@"1" doubleValue];

    [self.accountRecharge updatePurchaseAPackageAsyncWithPackageId: packageId  completionBlock:^(BOOL success, HttpContext* context, PurchaseAPackageResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_transactions_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.getTransactionsWithCompletionBlock") getTransactionsWithCompletionBlock

> TODO: Add a method description


```objc
function getTransactionsWithCompletionBlock:(CompletedGetTransactions) onCompleted()
```



#### Example Usage

```objc

    [self.accountRecharge getTransactionsWithCompletionBlock:  ^(BOOL success, HttpContext* context, GetTransactionsResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_a_specific_transaction_async_with_transaction_id"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.getASpecificTransactionAsyncWithTransactionId") getASpecificTransactionAsyncWithTransactionId

> TODO: Add a method description


```objc
function getASpecificTransactionAsyncWithTransactionId:(NSString*) transactionId
                completionBlock:(CompletedGetASpecificTransaction) onCompleted(transactionId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| transactionId |  ``` Required ```  | 1c65-47fa-aea2-3ded9ed57557 (number, required) - Your transction id. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* transactionId = @"transaction_id";

    [self.accountRecharge getASpecificTransactionAsyncWithTransactionId: transactionId  completionBlock:^(BOOL success, HttpContext* context, NSData* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="automation_rules_controller"></a>![Class: ](https://apidocs.io/img/class.png ".AutomationRulesController") AutomationRulesController

### Get singleton instance
```objc
AutomationRules* automationRules = [[AutomationRules alloc]init] ;
```

### <a name="list_rules_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.listRulesWithCompletionBlock") listRulesWithCompletionBlock

> TODO: Add a method description


```objc
function listRulesWithCompletionBlock:(CompletedGetListRules) onCompleted()
```



#### Example Usage

```objc

    [self.automationRules listRulesWithCompletionBlock:  ^(BOOL success, HttpContext* context, ListRulesResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_a_specific_rule_async_with_inbound_rule_id"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.getASpecificRuleAsyncWithInboundRuleId") getASpecificRuleAsyncWithInboundRuleId

> TODO: Add a method description


```objc
function getASpecificRuleAsyncWithInboundRuleId:(double) inboundRuleId
                completionBlock:(CompletedGetASpecificRule) onCompleted(inboundRuleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Inbound Rule ID. |





#### Example Usage

```objc
    // Parameters for the API call
    double inboundRuleId = [@"1" doubleValue];

    [self.automationRules getASpecificRuleAsyncWithInboundRuleId: inboundRuleId  completionBlock:^(BOOL success, HttpContext* context, GetASpecificRuleResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_a_new_rule_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.createANewRuleAsyncWithBody") createANewRuleAsyncWithBody

> TODO: Add a method description


```objc
function createANewRuleAsyncWithBody:(CreateANewRuleRequest*) body
                completionBlock:(CompletedPostCreateANewRule) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CreateANewRuleRequest* body = [[CreateANewRuleRequest alloc]init];

    [self.automationRules createANewRuleAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CreateANewRuleResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_a_rule_async_with_inbound_rule_id"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.updateARuleAsyncWithInboundRuleId") updateARuleAsyncWithInboundRuleId

> TODO: Add a method description


```objc
function updateARuleAsyncWithInboundRuleId:(double) inboundRuleId
                body:(UpdateARuleRequest*) body
                completionBlock:(CompletedPutUpdateARule) onCompleted(inboundRuleId body : body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Inbound Rule ID. |
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    double inboundRuleId = [@"1" doubleValue];
    UpdateARuleRequest* body = (UpdateARuleRequest*) [APIHelper jsonDeserialize: @"{    \"dedicated_number\":\"+61298441484\",    \"rule_name\":\"My Rule\",    \"message_search_type\":3,    \"message_search_term\":\"My Search Term\",    \"action\":\"EMAIL_FIXED\",    \"action_address\":\"john@doe.com\",    \"enabled\":1}"
                toClass: UpdateARuleRequest.class];

    [self.automationRules updateARuleAsyncWithInboundRuleId: inboundRuleId body : body  completionBlock:^(BOOL success, HttpContext* context, UpdateARuleResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="delete_a_rule_async_with_inbound_rule_id"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.deleteARuleAsyncWithInboundRuleId") deleteARuleAsyncWithInboundRuleId

> TODO: Add a method description


```objc
function deleteARuleAsyncWithInboundRuleId:(double) inboundRuleId
                completionBlock:(CompletedDeleteARule) onCompleted(inboundRuleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Inbound Rule ID. |





#### Example Usage

```objc
    // Parameters for the API call
    double inboundRuleId = [@"1" doubleValue];

    [self.automationRules deleteARuleAsyncWithInboundRuleId: inboundRuleId  completionBlock:^(BOOL success, HttpContext* context, DeleteARuleResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="list_rules1_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.listRules1WithCompletionBlock") listRules1WithCompletionBlock

> TODO: Add a method description


```objc
function listRules1WithCompletionBlock:(CompletedGetListRules1) onCompleted()
```



#### Example Usage

```objc

    [self.automationRules listRules1WithCompletionBlock:  ^(BOOL success, HttpContext* context, ListRulesResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_a_specific_rule_async_with_receipt_rule_id"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.getASpecificRuleAsyncWithReceiptRuleId") getASpecificRuleAsyncWithReceiptRuleId

> TODO: Add a method description


```objc
function getASpecificRuleAsyncWithReceiptRuleId:(double) receiptRuleId
                completionBlock:(CompletedGetASpecificRule) onCompleted(receiptRuleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |





#### Example Usage

```objc
    // Parameters for the API call
    double receiptRuleId = [@"2" doubleValue];

    [self.automationRules getASpecificRuleAsyncWithReceiptRuleId: receiptRuleId  completionBlock:^(BOOL success, HttpContext* context, GetASpecificRuleResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_a_new_rule1_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.createANewRule1AsyncWithBody") createANewRule1AsyncWithBody

> TODO: Add a method description


```objc
function createANewRule1AsyncWithBody:(CreateANewRuleRequest24*) body
                completionBlock:(CompletedPostCreateANewRule1) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CreateANewRuleRequest24* body = (CreateANewRuleRequest24*) [APIHelper jsonDeserialize: @"{    \"rule_name\": \"My Rule\",    \"match_type\": 3,    \"action\": \"EMAIL_FIXED\",    \"action_address\": \"john@doe.com\",    \"enabled\": 1}"
                toClass: CreateANewRuleRequest24.class];

    [self.automationRules createANewRule1AsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CreateANewRuleResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_a_rule_async_with_receipt_rule_id"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.updateARuleAsyncWithReceiptRuleId") updateARuleAsyncWithReceiptRuleId

> TODO: Add a method description


```objc
function updateARuleAsyncWithReceiptRuleId:(double) receiptRuleId
                body:(UpdateARuleRequest26*) body
                completionBlock:(CompletedPutUpdateARule) onCompleted(receiptRuleId body : body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    double receiptRuleId = [@"7" doubleValue];
    UpdateARuleRequest26* body = (UpdateARuleRequest26*) [APIHelper jsonDeserialize: @"{    \"rule_name\": \"My Rule\",    \"match_type\": 3,    \"action\": \"EMAIL_FIXED\",    \"action_address\": \"john@doe.com\",    \"enabled\": 1}"
                toClass: UpdateARuleRequest26.class];

    [self.automationRules updateARuleAsyncWithReceiptRuleId: receiptRuleId body : body  completionBlock:^(BOOL success, HttpContext* context, UpdateARuleResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="delete_a_rule_async_with_receipt_rule_id"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.deleteARuleAsyncWithReceiptRuleId") deleteARuleAsyncWithReceiptRuleId

> TODO: Add a method description


```objc
function deleteARuleAsyncWithReceiptRuleId:(double) receiptRuleId
                completionBlock:(CompletedDeleteARule) onCompleted(receiptRuleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |





#### Example Usage

```objc
    // Parameters for the API call
    double receiptRuleId = [@"7" doubleValue];

    [self.automationRules deleteARuleAsyncWithReceiptRuleId: receiptRuleId  completionBlock:^(BOOL success, HttpContext* context, DeleteARuleResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="list_rules2_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.listRules2WithCompletionBlock") listRules2WithCompletionBlock

> TODO: Add a method description


```objc
function listRules2WithCompletionBlock:(CompletedGetListRules2) onCompleted()
```



#### Example Usage

```objc

    [self.automationRules listRules2WithCompletionBlock:  ^(BOOL success, HttpContext* context, ListRulesResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_a_specific_rule1_async_with_receipt_rule_id"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.getASpecificRule1AsyncWithReceiptRuleId") getASpecificRule1AsyncWithReceiptRuleId

> TODO: Add a method description


```objc
function getASpecificRule1AsyncWithReceiptRuleId:(double) receiptRuleId
                completionBlock:(CompletedGetASpecificRule1) onCompleted(receiptRuleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |





#### Example Usage

```objc
    // Parameters for the API call
    double receiptRuleId = [@"2" doubleValue];

    [self.automationRules getASpecificRule1AsyncWithReceiptRuleId: receiptRuleId  completionBlock:^(BOOL success, HttpContext* context, GetASpecificRuleResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_a_new_rule2_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.createANewRule2AsyncWithBody") createANewRule2AsyncWithBody

> TODO: Add a method description


```objc
function createANewRule2AsyncWithBody:(CreateANewRuleRequest24*) body
                completionBlock:(CompletedPostCreateANewRule2) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CreateANewRuleRequest24* body = (CreateANewRuleRequest24*) [APIHelper jsonDeserialize: @"{    \"rule_name\":\"My Rule\",    \"match_type\":3,    \"action\":\"EMAIL_FIXED\",    \"action_address\":\"john@doe.com\",    \"enabled\":1}"
                toClass: CreateANewRuleRequest24.class];

    [self.automationRules createANewRule2AsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CreateANewRuleResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_a_rule1_async_with_receipt_rule_id"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.updateARule1AsyncWithReceiptRuleId") updateARule1AsyncWithReceiptRuleId

> TODO: Add a method description


```objc
function updateARule1AsyncWithReceiptRuleId:(double) receiptRuleId
                body:(UpdateARuleRequest26*) body
                completionBlock:(CompletedPutUpdateARule1) onCompleted(receiptRuleId body : body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    double receiptRuleId = [@"2" doubleValue];
    UpdateARuleRequest26* body = (UpdateARuleRequest26*) [APIHelper jsonDeserialize: @"{    \"rule_name\":\"My Rule\",    \"match_type\":3,    \"action\":\"EMAIL_FIXED\",    \"action_address\":\"john@doe.com\",    \"enabled\":1}"
                toClass: UpdateARuleRequest26.class];

    [self.automationRules updateARule1AsyncWithReceiptRuleId: receiptRuleId body : body  completionBlock:^(BOOL success, HttpContext* context, UpdateARuleResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="delete_a_rule1_async_with_receipt_rule_id"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.deleteARule1AsyncWithReceiptRuleId") deleteARule1AsyncWithReceiptRuleId

> TODO: Add a method description


```objc
function deleteARule1AsyncWithReceiptRuleId:(double) receiptRuleId
                completionBlock:(CompletedDeleteARule1) onCompleted(receiptRuleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |





#### Example Usage

```objc
    // Parameters for the API call
    double receiptRuleId = [@"2" doubleValue];

    [self.automationRules deleteARule1AsyncWithReceiptRuleId: receiptRuleId  completionBlock:^(BOOL success, HttpContext* context, DeleteARuleResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="list_rules3_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.listRules3WithCompletionBlock") listRules3WithCompletionBlock

> TODO: Add a method description


```objc
function listRules3WithCompletionBlock:(CompletedGetListRules3) onCompleted()
```



#### Example Usage

```objc

    [self.automationRules listRules3WithCompletionBlock:  ^(BOOL success, HttpContext* context, ListRulesResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_a_specific_rule1_async_with_inbound_rule_id"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.getASpecificRule1AsyncWithInboundRuleId") getASpecificRule1AsyncWithInboundRuleId

> TODO: Add a method description


```objc
function getASpecificRule1AsyncWithInboundRuleId:(double) inboundRuleId
                completionBlock:(CompletedGetASpecificRule1) onCompleted(inboundRuleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Fax inbound rule id |





#### Example Usage

```objc
    // Parameters for the API call
    double inboundRuleId = [@"14" doubleValue];

    [self.automationRules getASpecificRule1AsyncWithInboundRuleId: inboundRuleId  completionBlock:^(BOOL success, HttpContext* context, GetASpecificRuleResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_a_new_rule3_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.createANewRule3AsyncWithBody") createANewRule3AsyncWithBody

> TODO: Add a method description


```objc
function createANewRule3AsyncWithBody:(CreateANewRuleRequest38*) body
                completionBlock:(CompletedPostCreateANewRule3) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CreateANewRuleRequest38* body = (CreateANewRuleRequest38*) [APIHelper jsonDeserialize: @"    {        \"dedicated_number\":\"+61298441484\",        \"rule_name\":\"Rule Name\",        \"action\":\"EMAIL_FIXED\",        \"action_address\":\"email@domain.com\",        \"enabled\":1    }"
                toClass: CreateANewRuleRequest38.class];

    [self.automationRules createANewRule3AsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CreateANewRuleResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_a_rule1_async_with_inbound_rule_id"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.updateARule1AsyncWithInboundRuleId") updateARule1AsyncWithInboundRuleId

> TODO: Add a method description


```objc
function updateARule1AsyncWithInboundRuleId:(double) inboundRuleId
                body:(UpdateARuleRequest40*) body
                completionBlock:(CompletedPutUpdateARule1) onCompleted(inboundRuleId body : body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Fax inbound rule id |
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    double inboundRuleId = [@"14" doubleValue];
    UpdateARuleRequest40* body = (UpdateARuleRequest40*) [APIHelper jsonDeserialize: @"    {        \"dedicated_number\":\"+61298441484\",        \"rule_name\":\"Rule Name\",        \"action\":\"EMAIL_FIXED\",        \"action_address\":\"email@domain.com\",        \"enabled\":1    }"
                toClass: UpdateARuleRequest40.class];

    [self.automationRules updateARule1AsyncWithInboundRuleId: inboundRuleId body : body  completionBlock:^(BOOL success, HttpContext* context, UpdateARuleResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="delete_a_rule1_async_with_inbound_rule_id"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.deleteARule1AsyncWithInboundRuleId") deleteARule1AsyncWithInboundRuleId

> TODO: Add a method description


```objc
function deleteARule1AsyncWithInboundRuleId:(double) inboundRuleId
                completionBlock:(CompletedDeleteARule1) onCompleted(inboundRuleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Fax inbound rule id |





#### Example Usage

```objc
    // Parameters for the API call
    double inboundRuleId = [@"14" doubleValue];

    [self.automationRules deleteARule1AsyncWithInboundRuleId: inboundRuleId  completionBlock:^(BOOL success, HttpContext* context, DeleteARuleResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="list_rules4_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.listRules4WithCompletionBlock") listRules4WithCompletionBlock

> TODO: Add a method description


```objc
function listRules4WithCompletionBlock:(CompletedGetListRules4) onCompleted()
```



#### Example Usage

```objc

    [self.automationRules listRules4WithCompletionBlock:  ^(BOOL success, HttpContext* context, ListRulesResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_a_specific_rule_async_with_rule_id"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.getASpecificRuleAsyncWithRuleId") getASpecificRuleAsyncWithRuleId

> TODO: Add a method description


```objc
function getASpecificRuleAsyncWithRuleId:(double) ruleId
                completionBlock:(CompletedGetASpecificRule) onCompleted(ruleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |





#### Example Usage

```objc
    // Parameters for the API call
    double ruleId = [@"4" doubleValue];

    [self.automationRules getASpecificRuleAsyncWithRuleId: ruleId  completionBlock:^(BOOL success, HttpContext* context, GetASpecificRuleResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_a_new_rule4_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.createANewRule4AsyncWithBody") createANewRule4AsyncWithBody

> TODO: Add a method description


```objc
function createANewRule4AsyncWithBody:(CreateANewRuleRequest24*) body
                completionBlock:(CompletedPostCreateANewRule4) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CreateANewRuleRequest24* body = (CreateANewRuleRequest24*) [APIHelper jsonDeserialize: @"    {        \"rule_name\":\"My Rule\",        \"match_type\":2,        \"action\":\"EMAIL_FIXED\",        \"action_address\":\"john@doe.com\",        \"enabled\":1    }"
                toClass: CreateANewRuleRequest24.class];

    [self.automationRules createANewRule4AsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CreateANewRuleResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_a_rule_async_with_rule_id"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.updateARuleAsyncWithRuleId") updateARuleAsyncWithRuleId

> TODO: Add a method description


```objc
function updateARuleAsyncWithRuleId:(double) ruleId
                body:(UpdateARuleRequest26*) body
                completionBlock:(CompletedPutUpdateARule) onCompleted(ruleId body : body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    double ruleId = [@"4" doubleValue];
    UpdateARuleRequest26* body = (UpdateARuleRequest26*) [APIHelper jsonDeserialize: @"    {        \"rule_name\":\"My Rule\",        \"match_type\":1,        \"action\":\"EMAIL_FIXED\",        \"action_address\":\"john@doe.com\",        \"enabled\":1    }"
                toClass: UpdateARuleRequest26.class];

    [self.automationRules updateARuleAsyncWithRuleId: ruleId body : body  completionBlock:^(BOOL success, HttpContext* context, UpdateARuleResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="delete_a_rule_async_with_rule_id"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.deleteARuleAsyncWithRuleId") deleteARuleAsyncWithRuleId

> TODO: Add a method description


```objc
function deleteARuleAsyncWithRuleId:(double) ruleId
                completionBlock:(CompletedDeleteARule) onCompleted(ruleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to delete. |





#### Example Usage

```objc
    // Parameters for the API call
    double ruleId = 194.360332572535;

    [self.automationRules deleteARuleAsyncWithRuleId: ruleId  completionBlock:^(BOOL success, HttpContext* context, DeleteARuleResponse49* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="list_rules5_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.listRules5WithCompletionBlock") listRules5WithCompletionBlock

> TODO: Add a method description


```objc
function listRules5WithCompletionBlock:(CompletedGetListRules5) onCompleted()
```



#### Example Usage

```objc

    [self.automationRules listRules5WithCompletionBlock:  ^(BOOL success, HttpContext* context, ListRulesResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_a_specific_rule1_async_with_rule_id"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.getASpecificRule1AsyncWithRuleId") getASpecificRule1AsyncWithRuleId

> TODO: Add a method description


```objc
function getASpecificRule1AsyncWithRuleId:(double) ruleId
                completionBlock:(CompletedGetASpecificRule1) onCompleted(ruleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |





#### Example Usage

```objc
    // Parameters for the API call
    double ruleId = [@"5" doubleValue];

    [self.automationRules getASpecificRule1AsyncWithRuleId: ruleId  completionBlock:^(BOOL success, HttpContext* context, GetASpecificRuleResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_a_new_rule5_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.createANewRule5AsyncWithBody") createANewRule5AsyncWithBody

> TODO: Add a method description


```objc
function createANewRule5AsyncWithBody:(CreateANewRuleRequest24*) body
                completionBlock:(CompletedPostCreateANewRule5) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CreateANewRuleRequest24* body = (CreateANewRuleRequest24*) [APIHelper jsonDeserialize: @"    {        \"rule_name\":\"My Rule\",        \"match_type\": 0,        \"action\":\"URL\",        \"action_address\":\"http://testurl.com\",        \"enabled\":1    }"
                toClass: CreateANewRuleRequest24.class];

    [self.automationRules createANewRule5AsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CreateANewRuleResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_a_rule1_async_with_rule_id"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.updateARule1AsyncWithRuleId") updateARule1AsyncWithRuleId

> TODO: Add a method description


```objc
function updateARule1AsyncWithRuleId:(double) ruleId
                body:(UpdateARuleRequest26*) body
                completionBlock:(CompletedPutUpdateARule1) onCompleted(ruleId body : body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    double ruleId = [@"8" doubleValue];
    UpdateARuleRequest26* body = (UpdateARuleRequest26*) [APIHelper jsonDeserialize: @"    {        \"rule_name\":\"My Rule\",        \"match_type\": 0,        \"action\":\"URL\",        \"action_address\":\"http://testurl.com\",        \"enabled\":1    }"
                toClass: UpdateARuleRequest26.class];

    [self.automationRules updateARule1AsyncWithRuleId: ruleId body : body  completionBlock:^(BOOL success, HttpContext* context, UpdateARuleResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="delete_a_rule1_async_with_rule_id"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.deleteARule1AsyncWithRuleId") deleteARule1AsyncWithRuleId

> TODO: Add a method description


```objc
function deleteARule1AsyncWithRuleId:(double) ruleId
                completionBlock:(CompletedDeleteARule1) onCompleted(ruleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to delete. |





#### Example Usage

```objc
    // Parameters for the API call
    double ruleId = [@"8" doubleValue];

    [self.automationRules deleteARule1AsyncWithRuleId: ruleId  completionBlock:^(BOOL success, HttpContext* context, DeleteARuleResponse56* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="contact_lists_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ContactListsController") ContactListsController

### Get singleton instance
```objc
ContactLists* contactLists = [[ContactLists alloc]init] ;
```

### <a name="get_all_contact_lists_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.getAllContactListsWithCompletionBlock") getAllContactListsWithCompletionBlock

> TODO: Add a method description


```objc
function getAllContactListsWithCompletionBlock:(CompletedGetAllContactLists) onCompleted()
```



#### Example Usage

```objc

    [self.contactLists getAllContactListsWithCompletionBlock:  ^(BOOL success, HttpContext* context, GetAllContactListsResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_a_new_contact_list_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.createANewContactListAsyncWithBody") createANewContactListAsyncWithBody

> TODO: Add a method description


```objc
function createANewContactListAsyncWithBody:(CreateANewContactListRequest*) body
                completionBlock:(CompletedPostCreateANewContactList) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CreateANewContactListRequest* body = (CreateANewContactListRequest*) [APIHelper jsonDeserialize: @"    {        \"list_name\":\"ListCT3QrVL4od\"    }"
                toClass: CreateANewContactListRequest.class];

    [self.contactLists createANewContactListAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CreateANewContactListResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_a_specific_contact_list_async_with_list_id"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.getASpecificContactListAsyncWithListId") getASpecificContactListAsyncWithListId

> TODO: Add a method description


```objc
function getASpecificContactListAsyncWithListId:(double) listId
                completionBlock:(CompletedGetASpecificContactList) onCompleted(listId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |





#### Example Usage

```objc
    // Parameters for the API call
    double listId = [@"437" doubleValue];

    [self.contactLists getASpecificContactListAsyncWithListId: listId  completionBlock:^(BOOL success, HttpContext* context, GetASpecificContactListResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_a_specific_contact_list_async_with_list_id"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.updateASpecificContactListAsyncWithListId") updateASpecificContactListAsyncWithListId

> TODO: Add a method description


```objc
function updateASpecificContactListAsyncWithListId:(double) listId
                body:(UpdateASpecificContactListRequest*) body
                completionBlock:(CompletedPutUpdateASpecificContactList) onCompleted(listId body : body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    double listId = [@"439" doubleValue];
    UpdateASpecificContactListRequest* body = (UpdateASpecificContactListRequest*) [APIHelper jsonDeserialize: @"    {        \"list_name\":\"ListlPJf33ksjP\"    }"
                toClass: UpdateASpecificContactListRequest.class];

    [self.contactLists updateASpecificContactListAsyncWithListId: listId body : body  completionBlock:^(BOOL success, HttpContext* context, UpdateASpecificContactListResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="delete_a_specific_contact_list_async_with_list_id"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.deleteASpecificContactListAsyncWithListId") deleteASpecificContactListAsyncWithListId

> TODO: Add a method description


```objc
function deleteASpecificContactListAsyncWithListId:(double) listId
                completionBlock:(CompletedDeleteASpecificContactList) onCompleted(listId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |





#### Example Usage

```objc
    // Parameters for the API call
    double listId = [@"442" doubleValue];

    [self.contactLists deleteASpecificContactListAsyncWithListId: listId  completionBlock:^(BOOL success, HttpContext* context, DeleteASpecificContactListResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_import_contacts_to_list_async_with_list_id"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.createImportContactsToListAsyncWithListId") createImportContactsToListAsyncWithListId

> TODO: Add a method description


```objc
function createImportContactsToListAsyncWithListId:(double) listId
                body:(ImportContactsToListRequest*) body
                completionBlock:(CompletedPostImportContactsToList) onCompleted(listId body : body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    double listId = [@"437" doubleValue];
    ImportContactsToListRequest* body = (ImportContactsToListRequest*) [APIHelper jsonDeserialize: @"{    \"file_url\":\"http://yourdomain.com/5485EA6144/79E8/import.csv\",    \"field_order\":[        \"phone\",        \"first_name\",        \"last_name\",        \"custom1\",        \"custom2\",        \"custom3\",        \"custom4\",        \"fax_number\",        \"organization_name\",        \"email\",        \"address_line_1\",        \"address_line_2\",        \"address_city\",        \"address_state\",        \"address_postal_code\",        \"address_country\"    ]}"
                toClass: ImportContactsToListRequest.class];

    [self.contactLists createImportContactsToListAsyncWithListId: listId body : body  completionBlock:^(BOOL success, HttpContext* context, ImportContactsToListResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_remove_duplicate_contacts_async_with_list_id"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.updateRemoveDuplicateContactsAsyncWithListId") updateRemoveDuplicateContactsAsyncWithListId

> TODO: Add a method description


```objc
function updateRemoveDuplicateContactsAsyncWithListId:(double) listId
                body:(RemoveDuplicateContactsRequest*) body
                completionBlock:(CompletedPutRemoveDuplicateContacts) onCompleted(listId body : body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id. |
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    double listId = [@"439" doubleValue];
    RemoveDuplicateContactsRequest* body = (RemoveDuplicateContactsRequest*) [APIHelper jsonDeserialize: @"{    \"fields\":[        \"phone_number\",        \"first_name\",        \"last_name\",        \"fax_number\",        \"address_country\"    ]}"
                toClass: RemoveDuplicateContactsRequest.class];

    [self.contactLists updateRemoveDuplicateContactsAsyncWithListId: listId body : body  completionBlock:^(BOOL success, HttpContext* context, RemoveDuplicateContactsResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_list_of_acceptable_import_fields_async_with_list_id"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.getListOfAcceptableImportFieldsAsyncWithListId") getListOfAcceptableImportFieldsAsyncWithListId

> TODO: Add a method description


```objc
function getListOfAcceptableImportFieldsAsyncWithListId:(NSString*) listId
                completionBlock:(CompletedGetListOfAcceptableImportFields) onCompleted(listId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Optional ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* listId = @"list_id";

    [self.contactLists getListOfAcceptableImportFieldsAsyncWithListId: listId  completionBlock:^(BOOL success, HttpContext* context, GetListOfAcceptableImportFieldsResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_show_csv_import_file_preview_async_with_list_id"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.createShowCSVImportFilePreviewAsyncWithListId") createShowCSVImportFilePreviewAsyncWithListId

> Show first row of the csv import file.


```objc
function createShowCSVImportFilePreviewAsyncWithListId:(double) listId
                body:(ShowCSVImportFilePreviewRequest*) body
                completionBlock:(CompletedPostShowCSVImportFilePreview) onCompleted(listId body : body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id. |
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    double listId = [@"439" doubleValue];
    ShowCSVImportFilePreviewRequest* body = (ShowCSVImportFilePreviewRequest*) [APIHelper jsonDeserialize: @"{    \"file_url\":\"http://yourdomain.com/5485EA6144/79E8/import.csv\"}"
                toClass: ShowCSVImportFilePreviewRequest.class];

    [self.contactLists createShowCSVImportFilePreviewAsyncWithListId: listId body : body  completionBlock:^(BOOL success, HttpContext* context, ShowCSVImportFilePreviewResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="contact_suggestions_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ContactSuggestionsController") ContactSuggestionsController

### Get singleton instance
```objc
ContactSuggestions* contactSuggestions = [[ContactSuggestions alloc]init] ;
```

### <a name="list_contact_suggestions_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ContactSuggestionsController.listContactSuggestionsWithCompletionBlock") listContactSuggestionsWithCompletionBlock

> TODO: Add a method description


```objc
function listContactSuggestionsWithCompletionBlock:(CompletedGetListContactSuggestions) onCompleted()
```



#### Example Usage

```objc

    [self.contactSuggestions listContactSuggestionsWithCompletionBlock:  ^(BOOL success, HttpContext* context, ListContactSuggestionsResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="contacts_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ContactsController") ContactsController

### Get singleton instance
```objc
Contacts* contacts = [[Contacts alloc]init] ;
```

### <a name="get_all_contacts_in_a_list_async_with_list_id"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.getAllContactsInAListAsyncWithListId") getAllContactsInAListAsyncWithListId

> TODO: Add a method description


```objc
function getAllContactsInAListAsyncWithListId:(double) listId
                completionBlock:(CompletedGetAllContactsInAList) onCompleted(listId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id where your contacts belong. |





#### Example Usage

```objc
    // Parameters for the API call
    double listId = [@"428" doubleValue];

    [self.contacts getAllContactsInAListAsyncWithListId: listId  completionBlock:^(BOOL success, HttpContext* context, GetAllContactsInAListResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_a_new_contact_async_with_list_id"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.createANewContactAsyncWithListId") createANewContactAsyncWithListId

> TODO: Add a method description


```objc
function createANewContactAsyncWithListId:(double) listId
                body:(CreateANewContactRequest*) body
                completionBlock:(CompletedPostCreateANewContact) onCompleted(listId body : body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id where your contact be associated. |
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    double listId = [@"428" doubleValue];
    CreateANewContactRequest* body = (CreateANewContactRequest*) [APIHelper jsonDeserialize: @"    {        \"phone_number\":\"+16783270696\",        \"first_name\":\"Ellen\",        \"last_name\":\"Diaz\",        \"custom_1\":\"Custom 1\",        \"custom_2\":\"Custom 2\",        \"custom_3\":\"Custom 3\",        \"custom_4\":\"Custom 4\",        \"fax_number\":\"+16783270696\",        \"organization_name\":\"Awesome Organization\",        \"email\":\"ellen@diaz.com\",        \"address_line_1\":\"Block 2\",        \"address_line_2\":\"Cool Bldg.\",        \"address_city\":\"Nevada\",        \"address_state\":\"Las Vegas\",        \"address_postal_code\":\"36063\",        \"address_country\":\"US\"    }"
                toClass: CreateANewContactRequest.class];

    [self.contacts createANewContactAsyncWithListId: listId body : body  completionBlock:^(BOOL success, HttpContext* context, CreateANewContactResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_a_specific_contact_async_with_list_id"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.getASpecificContactAsyncWithListId") getASpecificContactAsyncWithListId

> TODO: Add a method description


```objc
function getASpecificContactAsyncWithListId:(double) listId
                contactId:(double) contactId
                completionBlock:(CompletedGetASpecificContact) onCompleted(listId contactId : contactId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| contactId |  ``` Required ```  | Your contact id you want to access. |





#### Example Usage

```objc
    // Parameters for the API call
    double listId = [@"428" doubleValue];
    double contactId = [@"552802" doubleValue];

    [self.contacts getASpecificContactAsyncWithListId: listId contactId : contactId  completionBlock:^(BOOL success, HttpContext* context, GetASpecificContactResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_a_specific_contact_async_with_list_id"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.updateASpecificContactAsyncWithListId") updateASpecificContactAsyncWithListId

> TODO: Add a method description


```objc
function updateASpecificContactAsyncWithListId:(double) listId
                contactId:(double) contactId
                body:(UpdateASpecificContactRequest*) body
                completionBlock:(CompletedPutUpdateASpecificContact) onCompleted(listId contactId : contactId body : body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| contactId |  ``` Required ```  | Your contact id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    double listId = [@"428" doubleValue];
    double contactId = [@"552802" doubleValue];
    UpdateASpecificContactRequest* body = (UpdateASpecificContactRequest*) [APIHelper jsonDeserialize: @"{        \"phone_number\":\"+16783275492\",        \"first_name\":\"Ellen\",        \"last_name\":\"Diaz\",        \"custom_1\":\"Custom S72oJ9Teba\",        \"custom_2\":\"Custom NvrRJrKWeq\",        \"custom_3\":\"Custom 2ws94p1Dop\",        \"custom_4\":\"Custom Ku0AaIS5xb\",        \"fax_number\":\"+16783276356\",        \"organization_name\":\"Awesome Organization\",        \"email\":\"ellen@diaz.com\",        \"address_line_1\":\"Block 6\",        \"address_line_2\":\"Cool Bldg.\",        \"address_city\":\"Nevada\",        \"address_state\":\"Las Vegas\",        \"address_postal_code\":\"36063\",        \"address_country\":\"US\"    }"
                toClass: UpdateASpecificContactRequest.class];

    [self.contacts updateASpecificContactAsyncWithListId: listId contactId : contactId body : body  completionBlock:^(BOOL success, HttpContext* context, UpdateASpecificContactResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="delete_a_specific_contact_async_with_list_id"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.deleteASpecificContactAsyncWithListId") deleteASpecificContactAsyncWithListId

> TODO: Add a method description


```objc
function deleteASpecificContactAsyncWithListId:(double) listId
                contactId:(double) contactId
                completionBlock:(CompletedDeleteASpecificContact) onCompleted(listId contactId : contactId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| contactId |  ``` Required ```  | Your contact id you want to access. |





#### Example Usage

```objc
    // Parameters for the API call
    double listId = [@"428" doubleValue];
    double contactId = [@"552807" doubleValue];

    [self.contacts deleteASpecificContactAsyncWithListId: listId contactId : contactId  completionBlock:^(BOOL success, HttpContext* context, DeleteASpecificContactResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_remove_opted_out_contacts_async_with_list_id"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.updateRemoveOptedOutContactsAsyncWithListId") updateRemoveOptedOutContactsAsyncWithListId

> TODO: Add a method description


```objc
function updateRemoveOptedOutContactsAsyncWithListId:(double) listId
                optOutListId:(double) optOutListId
                completionBlock:(CompletedPutRemoveOptedOutContacts) onCompleted(listId optOutListId : optOutListId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id. |
| optOutListId |  ``` Required ```  | Your opt out list id. |





#### Example Usage

```objc
    // Parameters for the API call
    double listId = [@"439" doubleValue];
    double optOutListId = [@"512" doubleValue];

    [self.contacts updateRemoveOptedOutContactsAsyncWithListId: listId optOutListId : optOutListId  completionBlock:^(BOOL success, HttpContext* context, RemoveOptedOutContactsResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_transfer_a_contact_async_with_from_list_id"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.updateTransferAContactAsyncWithFromListId") updateTransferAContactAsyncWithFromListId

> Transfers a specific contact to another list.


```objc
function updateTransferAContactAsyncWithFromListId:(double) fromListId
                contactId:(double) contactId
                toListId:(double) toListId
                completionBlock:(CompletedPutTransferAContact) onCompleted(fromListId contactId : contactId toListId : toListId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| fromListId |  ``` Required ```  | From list id. |
| contactId |  ``` Required ```  | Contact ID. |
| toListId |  ``` Required ```  | To list id. |





#### Example Usage

```objc
    // Parameters for the API call
    double fromListId = [@"428" doubleValue];
    double contactId = [@"1" doubleValue];
    double toListId = [@"429" doubleValue];

    [self.contacts updateTransferAContactAsyncWithFromListId: fromListId contactId : contactId toListId : toListId  completionBlock:^(BOOL success, HttpContext* context, TransferAContactResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="countries_controller"></a>![Class: ](https://apidocs.io/img/class.png ".CountriesController") CountriesController

### Get singleton instance
```objc
Countries* countries = [[Countries alloc]init] ;
```

### <a name="get_all_countries_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".CountriesController.getAllCountriesWithCompletionBlock") getAllCountriesWithCompletionBlock

> TODO: Add a method description


```objc
function getAllCountriesWithCompletionBlock:(CompletedGetAllCountries) onCompleted()
```



#### Example Usage

```objc

    [self.countries getAllCountriesWithCompletionBlock:  ^(BOOL success, HttpContext* context, GetAllCountriesResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="delivery_issues_controller"></a>![Class: ](https://apidocs.io/img/class.png ".DeliveryIssuesController") DeliveryIssuesController

### Get singleton instance
```objc
DeliveryIssues* deliveryIssues = [[DeliveryIssues alloc]init] ;
```

### <a name="get_delivery_issues_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".DeliveryIssuesController.getDeliveryIssuesWithCompletionBlock") getDeliveryIssuesWithCompletionBlock

> TODO: Add a method description


```objc
function getDeliveryIssuesWithCompletionBlock:(CompletedGetDeliveryIssues) onCompleted()
```



#### Example Usage

```objc

    [self.deliveryIssues getDeliveryIssuesWithCompletionBlock:  ^(BOOL success, HttpContext* context, GetDeliveryIssuesResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_delivery_issue_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".DeliveryIssuesController.createDeliveryIssueAsyncWithBody") createDeliveryIssueAsyncWithBody

> TODO: Add a method description


```objc
function createDeliveryIssueAsyncWithBody:(CreateDeliveryIssueRequest*) body
                completionBlock:(CompletedPostCreateDeliveryIssue) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CreateDeliveryIssueRequest* body = (CreateDeliveryIssueRequest*) [APIHelper jsonDeserialize: @"{  \"message_id\": \"B388828B\",  \"type\": \"SMS\",  \"description\": \"This is a test\",  \"client_comments\": \"test\",  \"email_address: john_doe@user.com\": \"\",  \"Body\": \"\"}"
                toClass: CreateDeliveryIssueRequest.class];

    [self.deliveryIssues createDeliveryIssueAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CreateDeliveryIssueResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="email_marketing_controller"></a>![Class: ](https://apidocs.io/img/class.png ".EmailMarketingController") EmailMarketingController

### Get singleton instance
```objc
EmailMarketing* emailMarketing = [[EmailMarketing alloc]init] ;
```

### <a name="get_all_allowed_email_addresses_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getAllAllowedEmailAddressesWithCompletionBlock") getAllAllowedEmailAddressesWithCompletionBlock

> TODO: Add a method description


```objc
function getAllAllowedEmailAddressesWithCompletionBlock:(CompletedGetAllAllowedEmailAddresses) onCompleted()
```



#### Example Usage

```objc

    [self.emailMarketing getAllAllowedEmailAddressesWithCompletionBlock:  ^(BOOL success, HttpContext* context, GetAllAllowedEmailAddressesResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_allowed_email_address_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.createAllowedEmailAddressAsyncWithBody") createAllowedEmailAddressAsyncWithBody

> TODO: Add a method description


```objc
function createAllowedEmailAddressAsyncWithBody:(CreateAllowedEmailAddressRequest*) body
                completionBlock:(CompletedPostCreateAllowedEmailAddress) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CreateAllowedEmailAddressRequest* body = (CreateAllowedEmailAddressRequest*) [APIHelper jsonDeserialize: @"{  \"email_address\": \"johndoe1@user.com\",  \"Body\": \"\"}"
                toClass: CreateAllowedEmailAddressRequest.class];

    [self.emailMarketing createAllowedEmailAddressAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CreateAllowedEmailAddressResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_send_verification_token_async_with_email_address_id"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.updateSendVerificationTokenAsyncWithEmailAddressId") updateSendVerificationTokenAsyncWithEmailAddressId

> TODO: Add a method description


```objc
function updateSendVerificationTokenAsyncWithEmailAddressId:(double) emailAddressId
                completionBlock:(CompletedPutSendVerificationToken) onCompleted(emailAddressId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email addess id you want to access. |





#### Example Usage

```objc
    // Parameters for the API call
    double emailAddressId = 152.637159345968;

    [self.emailMarketing updateSendVerificationTokenAsyncWithEmailAddressId: emailAddressId  completionBlock:^(BOOL success, HttpContext* context, SendVerificationTokenResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_verify_allowed_email_address_async_with_email_address_id"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.updateVerifyAllowedEmailAddressAsyncWithEmailAddressId") updateVerifyAllowedEmailAddressAsyncWithEmailAddressId

> TODO: Add a method description


```objc
function updateVerifyAllowedEmailAddressAsyncWithEmailAddressId:(double) emailAddressId
                activationToken:(NSString*) activationToken
                completionBlock:(CompletedPutVerifyAllowedEmailAddress) onCompleted(emailAddressId activationToken : activationToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email address id you want to access. |
| activationToken |  ``` Required ```  | 6E8B-4FDB-99A7-7ED08DF97BCC (required, string) - Your activation token. |





#### Example Usage

```objc
    // Parameters for the API call
    double emailAddressId = [@"5" doubleValue];
    NSString* activationToken = @"3BD73304";

    [self.emailMarketing updateVerifyAllowedEmailAddressAsyncWithEmailAddressId: emailAddressId activationToken : activationToken  completionBlock:^(BOOL success, HttpContext* context, VerifyAllowedEmailAddressResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="delete_allowed_email_address_async_with_email_address_id"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.deleteAllowedEmailAddressAsyncWithEmailAddressId") deleteAllowedEmailAddressAsyncWithEmailAddressId

> TODO: Add a method description


```objc
function deleteAllowedEmailAddressAsyncWithEmailAddressId:(double) emailAddressId
                completionBlock:(CompletedDeleteAllowedEmailAddress) onCompleted(emailAddressId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email address you want to access. |





#### Example Usage

```objc
    // Parameters for the API call
    double emailAddressId = 152.637159345968;

    [self.emailMarketing deleteAllowedEmailAddressAsyncWithEmailAddressId: emailAddressId  completionBlock:^(BOOL success, HttpContext* context, DeleteAllowedEmailAddressResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_specific_allowed_email_address_async_with_email_address_id"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getSpecificAllowedEmailAddressAsyncWithEmailAddressId") getSpecificAllowedEmailAddressAsyncWithEmailAddressId

> TODO: Add a method description


```objc
function getSpecificAllowedEmailAddressAsyncWithEmailAddressId:(double) emailAddressId
                completionBlock:(CompletedGetSpecificAllowedEmailAddress) onCompleted(emailAddressId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email address you want to access. |





#### Example Usage

```objc
    // Parameters for the API call
    double emailAddressId = [@"4" doubleValue];

    [self.emailMarketing getSpecificAllowedEmailAddressAsyncWithEmailAddressId: emailAddressId  completionBlock:^(BOOL success, HttpContext* context, GetSpecificAllowedEmailAddressResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_all_email_campaigns_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getAllEmailCampaignsWithCompletionBlock") getAllEmailCampaignsWithCompletionBlock

> TODO: Add a method description


```objc
function getAllEmailCampaignsWithCompletionBlock:(CompletedGetAllEmailCampaigns) onCompleted()
```



#### Example Usage

```objc

    [self.emailMarketing getAllEmailCampaignsWithCompletionBlock:  ^(BOOL success, HttpContext* context, GetAllEmailCampaignsResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_specific_email_campaign_async_with_email_campaign_id"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getSpecificEmailCampaignAsyncWithEmailCampaignId") getSpecificEmailCampaignAsyncWithEmailCampaignId

> TODO: Add a method description


```objc
function getSpecificEmailCampaignAsyncWithEmailCampaignId:(double) emailCampaignId
                completionBlock:(CompletedGetSpecificEmailCampaign) onCompleted(emailCampaignId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailCampaignId |  ``` Required ```  | The email campaign id you want to access. |





#### Example Usage

```objc
    // Parameters for the API call
    double emailCampaignId = [@"1" doubleValue];

    [self.emailMarketing getSpecificEmailCampaignAsyncWithEmailCampaignId: emailCampaignId  completionBlock:^(BOOL success, HttpContext* context, GetSpecificEmailCampaignResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_email_campaign_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.createEmailCampaignAsyncWithBody") createEmailCampaignAsyncWithBody

> TODO: Add a method description


```objc
function createEmailCampaignAsyncWithBody:(CreateEmailCampaignRequest*) body
                completionBlock:(CompletedPostCreateEmailCampaign) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CreateEmailCampaignRequest* body = (CreateEmailCampaignRequest*) [APIHelper jsonDeserialize: @"{  \"name\" : \"John Doe\",  \"subject\" : \"Lorem Ipsum\",  \"from_email_address_id\" : 2,  \"from_name\" : \"From name\",  \"template_id\" : 31,  \"body\" : \"<p>This is a test</p>\",  \"list_id\" : 456}"
                toClass: CreateEmailCampaignRequest.class];

    [self.emailMarketing createEmailCampaignAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CreateEmailCampaignResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_email_campaign_async_with_email_campaign_id"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.updateEmailCampaignAsyncWithEmailCampaignId") updateEmailCampaignAsyncWithEmailCampaignId

> TODO: Add a method description


```objc
function updateEmailCampaignAsyncWithEmailCampaignId:(double) emailCampaignId
                body:(UpdateEmailCampaignRequest*) body
                completionBlock:(CompletedPutUpdateEmailCampaign) onCompleted(emailCampaignId body : body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailCampaignId |  ``` Required ```  | The email campaign id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    double emailCampaignId = [@"1" doubleValue];
    UpdateEmailCampaignRequest* body = (UpdateEmailCampaignRequest*) [APIHelper jsonDeserialize: @"{  \"name\" : \"John Doe\",  \"subject\" : \"Lorem Ipsum\",  \"from_email_address_id\" : 2,  \"from_name\" : \"From name\",  \"template_id\" : 31,  \"body\" : \"<p>This is a test</p>\",  \"list_id\" : 456}"
                toClass: UpdateEmailCampaignRequest.class];

    [self.emailMarketing updateEmailCampaignAsyncWithEmailCampaignId: emailCampaignId body : body  completionBlock:^(BOOL success, HttpContext* context, UpdateEmailCampaignResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_cancel_email_campaign_async_with_email_campaign_id"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.updateCancelEmailCampaignAsyncWithEmailCampaignId") updateCancelEmailCampaignAsyncWithEmailCampaignId

> TODO: Add a method description


```objc
function updateCancelEmailCampaignAsyncWithEmailCampaignId:(double) emailCampaignId
                completionBlock:(CompletedPutCancelEmailCampaign) onCompleted(emailCampaignId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailCampaignId |  ``` Required ```  | The email campaign id you want to cancel. |





#### Example Usage

```objc
    // Parameters for the API call
    double emailCampaignId = [@"1" doubleValue];

    [self.emailMarketing updateCancelEmailCampaignAsyncWithEmailCampaignId: emailCampaignId  completionBlock:^(BOOL success, HttpContext* context, CancelEmailCampaignResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_calculate_price_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.createCalculatePriceAsyncWithBody") createCalculatePriceAsyncWithBody

> TODO: Add a method description


```objc
function createCalculatePriceAsyncWithBody:(CalculatePriceRequest*) body
                completionBlock:(CompletedPostCalculatePrice) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CalculatePriceRequest* body = (CalculatePriceRequest*) [APIHelper jsonDeserialize: @"{  \"name\" : \"John Doe\",  \"subject\" : \"Lorem Ipsum\",  \"from_email_address_id\" : 2,  \"from_name\" : \"From name\",  \"template_id\" : 31,  \"body\" : \"<p>This is a test</p>\",  \"list_id\" : 456}"
                toClass: CalculatePriceRequest.class];

    [self.emailMarketing createCalculatePriceAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CalculatePriceResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_specific_email_campaign_history_async_with_campaign_id"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getSpecificEmailCampaignHistoryAsyncWithCampaignId") getSpecificEmailCampaignHistoryAsyncWithCampaignId

> TODO: Add a method description


```objc
function getSpecificEmailCampaignHistoryAsyncWithCampaignId:(double) campaignId
                completionBlock:(CompletedGetSpecificEmailCampaignHistory) onCompleted(campaignId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| campaignId |  ``` Required ```  | The email campaign id you want to access. |





#### Example Usage

```objc
    // Parameters for the API call
    double campaignId = [@"77" doubleValue];

    [self.emailMarketing getSpecificEmailCampaignHistoryAsyncWithCampaignId: campaignId  completionBlock:^(BOOL success, HttpContext* context, GetSpecificEmailCampaignHistoryResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_all_email_templates_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getAllEmailTemplatesWithCompletionBlock") getAllEmailTemplatesWithCompletionBlock

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```objc
function getAllEmailTemplatesWithCompletionBlock:(CompletedGetAllEmailTemplates) onCompleted()
```



#### Example Usage

```objc

    [self.emailMarketing getAllEmailTemplatesWithCompletionBlock:  ^(BOOL success, HttpContext* context, GetAllEmailTemplatesResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_specific_email_template_async_with_template_id"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getSpecificEmailTemplateAsyncWithTemplateId") getSpecificEmailTemplateAsyncWithTemplateId

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```objc
function getSpecificEmailTemplateAsyncWithTemplateId:(double) templateId
                completionBlock:(CompletedGetSpecificEmailTemplate) onCompleted(templateId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | The email template id. |





#### Example Usage

```objc
    // Parameters for the API call
    double templateId = [@"291" doubleValue];

    [self.emailMarketing getSpecificEmailTemplateAsyncWithTemplateId: templateId  completionBlock:^(BOOL success, HttpContext* context, GetSpecificEmailTemplateResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_new_email_template_from_master_template_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.createNewEmailTemplateFromMasterTemplateAsyncWithBody") createNewEmailTemplateFromMasterTemplateAsyncWithBody

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```objc
function createNewEmailTemplateFromMasterTemplateAsyncWithBody:(CreateNewEmailTemplateFromMasterTemplateRequest*) body
                completionBlock:(CompletedPostCreateNewEmailTemplateFromMasterTemplate) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CreateNewEmailTemplateFromMasterTemplateRequest* body = (CreateNewEmailTemplateFromMasterTemplateRequest*) [APIHelper jsonDeserialize: @"{  \"template_name\": \"Minions\",  \"template_id_master\": 57}"
                toClass: CreateNewEmailTemplateFromMasterTemplateRequest.class];

    [self.emailMarketing createNewEmailTemplateFromMasterTemplateAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CreateNewEmailTemplateFromMasterTemplateResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_an_email_template_async_with_template_id"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.updateAnEmailTemplateAsyncWithTemplateId") updateAnEmailTemplateAsyncWithTemplateId

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```objc
function updateAnEmailTemplateAsyncWithTemplateId:(double) templateId
                body:(UpdateAnEmailTemplateRequest*) body
                completionBlock:(CompletedPutUpdateAnEmailTemplate) onCompleted(templateId body : body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | The id of the template to be updated. |
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    double templateId = [@"291" doubleValue];
    UpdateAnEmailTemplateRequest* body = (UpdateAnEmailTemplateRequest*) [APIHelper jsonDeserialize: @"    {        \"template_name\":\"Minions\",        \"body\":\"This is a sample content: Sc0KNWgSMG for this template.\"    }"
                toClass: UpdateAnEmailTemplateRequest.class];

    [self.emailMarketing updateAnEmailTemplateAsyncWithTemplateId: templateId body : body  completionBlock:^(BOOL success, HttpContext* context, UpdateAnEmailTemplateResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="delete_email_template_async_with_template_id"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.deleteEmailTemplateAsyncWithTemplateId") deleteEmailTemplateAsyncWithTemplateId

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```objc
function deleteEmailTemplateAsyncWithTemplateId:(double) templateId
                completionBlock:(CompletedDeleteEmailTemplate) onCompleted(templateId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |





#### Example Usage

```objc
    // Parameters for the API call
    double templateId = [@"25" doubleValue];

    [self.emailMarketing deleteEmailTemplateAsyncWithTemplateId: templateId  completionBlock:^(BOOL success, HttpContext* context, DeleteEmailTemplateResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_all_master_email_templates_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getAllMasterEmailTemplatesWithCompletionBlock") getAllMasterEmailTemplatesWithCompletionBlock

> Master templates are templates that you can clone to a User Email Template which lets you edit and save it.


```objc
function getAllMasterEmailTemplatesWithCompletionBlock:(CompletedGetAllMasterEmailTemplates) onCompleted()
```



#### Example Usage

```objc

    [self.emailMarketing getAllMasterEmailTemplatesWithCompletionBlock:  ^(BOOL success, HttpContext* context, GetAllMasterEmailTemplatesResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_specific_master_template_async_with_template_id"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getSpecificMasterTemplateAsyncWithTemplateId") getSpecificMasterTemplateAsyncWithTemplateId

> Master templates are templates that you can clone to a User Email Template which lets you edit and save it.


```objc
function getSpecificMasterTemplateAsyncWithTemplateId:(NSString*) templateId
                completionBlock:(CompletedGetSpecificMasterTemplate) onCompleted(templateId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* templateId = @"25";

    [self.emailMarketing getSpecificMasterTemplateAsyncWithTemplateId: templateId  completionBlock:^(BOOL success, HttpContext* context, GetSpecificMasterTemplateResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_all_master_template_categories_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getAllMasterTemplateCategoriesWithCompletionBlock") getAllMasterTemplateCategoriesWithCompletionBlock

> TODO: Add a method description


```objc
function getAllMasterTemplateCategoriesWithCompletionBlock:(CompletedGetAllMasterTemplateCategories) onCompleted()
```



#### Example Usage

```objc

    [self.emailMarketing getAllMasterTemplateCategoriesWithCompletionBlock:  ^(BOOL success, HttpContext* context, GetAllMasterTemplateCategoriesResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_specific_email_template_category_async_with_category_id"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getSpecificEmailTemplateCategoryAsyncWithCategoryId") getSpecificEmailTemplateCategoryAsyncWithCategoryId

> TODO: Add a method description


```objc
function getSpecificEmailTemplateCategoryAsyncWithCategoryId:(NSString*) categoryId
                completionBlock:(CompletedGetSpecificEmailTemplateCategory) onCompleted(categoryId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| categoryId |  ``` Required ```  | Your category id. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* categoryId = @"25";

    [self.emailMarketing getSpecificEmailTemplateCategoryAsyncWithCategoryId: categoryId  completionBlock:^(BOOL success, HttpContext* context, GetSpecificEmailTemplateCategoryResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_all_templates_for_category_async_with_category_id"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getAllTemplatesForCategoryAsyncWithCategoryId") getAllTemplatesForCategoryAsyncWithCategoryId

> TODO: Add a method description


```objc
function getAllTemplatesForCategoryAsyncWithCategoryId:(NSString*) categoryId
                completionBlock:(CompletedGetAllTemplatesForCategory) onCompleted(categoryId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| categoryId |  ``` Required ```  | Your category id. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* categoryId = @"1";

    [self.emailMarketing getAllTemplatesForCategoryAsyncWithCategoryId: categoryId  completionBlock:^(BOOL success, HttpContext* context, GetAllTemplatesForCategoryResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="upload_image_to_specific_template_async_with_template_id"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.uploadImageToSpecificTemplateAsyncWithTemplateId") uploadImageToSpecificTemplateAsyncWithTemplateId

> TODO: Add a method description


```objc
function uploadImageToSpecificTemplateAsyncWithTemplateId:(NSString*) templateId
                body:(UploadImageToSpecificTemplateRequest*) body
                completionBlock:(CompletedPostUploadImageToSpecificTemplate) onCompleted(templateId body : body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* templateId = @"1";
    UploadImageToSpecificTemplateRequest* body = (UploadImageToSpecificTemplateRequest*) [APIHelper jsonDeserialize: @"{    \"image\": \"image.png\",    \"url\" : \"http://www.downloadimg.from/here.png\"}"
                toClass: UploadImageToSpecificTemplateRequest.class];

    [self.emailMarketing uploadImageToSpecificTemplateAsyncWithTemplateId: templateId body : body  completionBlock:^(BOOL success, HttpContext* context, UploadImageToSpecificTemplateResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="email_to_sms_allowed_address_controller"></a>![Class: ](https://apidocs.io/img/class.png ".EmailToSMSAllowedAddressController") EmailToSMSAllowedAddressController

### Get singleton instance
```objc
EmailToSMSAllowedAddress* emailToSMSAllowedAddress = [[EmailToSMSAllowedAddress alloc]init] ;
```

### <a name="list_of_email_to_sms_allowed_address_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSAllowedAddressController.listOfEmailToSMSAllowedAddressWithCompletionBlock") listOfEmailToSMSAllowedAddressWithCompletionBlock

> Get list of allowed email addresses.


```objc
function listOfEmailToSMSAllowedAddressWithCompletionBlock:(CompletedGetListOfEmailToSMSAllowedAddress) onCompleted()
```



#### Example Usage

```objc

    [self.emailToSMSAllowedAddress listOfEmailToSMSAllowedAddressWithCompletionBlock:  ^(BOOL success, HttpContext* context, ListOfEmailToSMSAllowedAddressResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_email_to_sms_allowed_address_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSAllowedAddressController.createEmailToSMSAllowedAddressAsyncWithBody") createEmailToSMSAllowedAddressAsyncWithBody

> Create an allowed email address.


```objc
function createEmailToSMSAllowedAddressAsyncWithBody:(CreateEmailToSMSAllowedAddressRequest*) body
                completionBlock:(CompletedPostCreateEmailToSMSAllowedAddress) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CreateEmailToSMSAllowedAddressRequest* body = (CreateEmailToSMSAllowedAddressRequest*) [APIHelper jsonDeserialize: @"    {        \"email_address\":\"Cv3p0@gmail.com\",        \"from\":\"+17128845887\"    }"
                toClass: CreateEmailToSMSAllowedAddressRequest.class];

    [self.emailToSMSAllowedAddress createEmailToSMSAllowedAddressAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CreateEmailToSMSAllowedAddressResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_specific_email_to_sms_allowed_address_async_with_email_address_id"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSAllowedAddressController.getSpecificEmailToSMSAllowedAddressAsyncWithEmailAddressId") getSpecificEmailToSMSAllowedAddressAsyncWithEmailAddressId

> Get a specific allowed email address.


```objc
function getSpecificEmailToSMSAllowedAddressAsyncWithEmailAddressId:(double) emailAddressId
                completionBlock:(CompletedGetSpecificEmailToSMSAllowedAddress) onCompleted(emailAddressId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | Your email address id. |





#### Example Usage

```objc
    // Parameters for the API call
    double emailAddressId = [@"113" doubleValue];

    [self.emailToSMSAllowedAddress getSpecificEmailToSMSAllowedAddressAsyncWithEmailAddressId: emailAddressId  completionBlock:^(BOOL success, HttpContext* context, GetSpecificEmailToSMSAllowedAddressResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_email_to_sms_allowed_address_async_with_email_address_id"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSAllowedAddressController.updateEmailToSMSAllowedAddressAsyncWithEmailAddressId") updateEmailToSMSAllowedAddressAsyncWithEmailAddressId

> Update a specific allowed email address.


```objc
function updateEmailToSMSAllowedAddressAsyncWithEmailAddressId:(double) emailAddressId
                body:(UpdateEmailToSMSAllowedAddressRequest*) body
                completionBlock:(CompletedPutUpdateEmailToSMSAllowedAddress) onCompleted(emailAddressId body : body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | Your email address id. |
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    double emailAddressId = [@"107" doubleValue];
    UpdateEmailToSMSAllowedAddressRequest* body = (UpdateEmailToSMSAllowedAddressRequest*) [APIHelper jsonDeserialize: @"    {        \"email_address\":\"pfvRZ@gmail.com\",        \"from\":\"+17128842283\"    }"
                toClass: UpdateEmailToSMSAllowedAddressRequest.class];

    [self.emailToSMSAllowedAddress updateEmailToSMSAllowedAddressAsyncWithEmailAddressId: emailAddressId body : body  completionBlock:^(BOOL success, HttpContext* context, UpdateEmailToSMSAllowedAddressResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="delete_email_to_sms_allowed_address_async_with_email_address_id"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSAllowedAddressController.deleteEmailToSMSAllowedAddressAsyncWithEmailAddressId") deleteEmailToSMSAllowedAddressAsyncWithEmailAddressId

> Delete a specific allowed email address.


```objc
function deleteEmailToSMSAllowedAddressAsyncWithEmailAddressId:(double) emailAddressId
                completionBlock:(CompletedDeleteEmailToSMSAllowedAddress) onCompleted(emailAddressId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | Your email address id. |





#### Example Usage

```objc
    // Parameters for the API call
    double emailAddressId = [@"107" doubleValue];

    [self.emailToSMSAllowedAddress deleteEmailToSMSAllowedAddressAsyncWithEmailAddressId: emailAddressId  completionBlock:^(BOOL success, HttpContext* context, DeleteEmailToSMSAllowedAddressResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="email_to_sms_stripped_strings_controller"></a>![Class: ](https://apidocs.io/img/class.png ".EmailToSMSStrippedStringsController") EmailToSMSStrippedStringsController

### Get singleton instance
```objc
EmailToSMSStrippedStrings* emailToSMSStrippedStrings = [[EmailToSMSStrippedStrings alloc]init] ;
```

### <a name="list_stripped_strings_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSStrippedStringsController.listStrippedStringsWithCompletionBlock") listStrippedStringsWithCompletionBlock

> TODO: Add a method description


```objc
function listStrippedStringsWithCompletionBlock:(CompletedGetListStrippedStrings) onCompleted()
```



#### Example Usage

```objc

    [self.emailToSMSStrippedStrings listStrippedStringsWithCompletionBlock:  ^(BOOL success, HttpContext* context, ListStrippedStringsResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="find_specific_stripped_string_async_with_rule_id"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSStrippedStringsController.findSpecificStrippedStringAsyncWithRuleId") findSpecificStrippedStringAsyncWithRuleId

> TODO: Add a method description


```objc
function findSpecificStrippedStringAsyncWithRuleId:(double) ruleId
                completionBlock:(CompletedGetFindSpecificStrippedString) onCompleted(ruleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |





#### Example Usage

```objc
    // Parameters for the API call
    double ruleId = [@"18" doubleValue];

    [self.emailToSMSStrippedStrings findSpecificStrippedStringAsyncWithRuleId: ruleId  completionBlock:^(BOOL success, HttpContext* context, FindSpecificStrippedStringResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_stripped_string_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSStrippedStringsController.createStrippedStringAsyncWithBody") createStrippedStringAsyncWithBody

> TODO: Add a method description


```objc
function createStrippedStringAsyncWithBody:(CreateStrippedStringRequest*) body
                completionBlock:(CompletedPostCreateStrippedString) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CreateStrippedStringRequest* body = (CreateStrippedStringRequest*) [APIHelper jsonDeserialize: @"{    \"strip_string\" : \"~~~test~~~\"}"
                toClass: CreateStrippedStringRequest.class];

    [self.emailToSMSStrippedStrings createStrippedStringAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CreateStrippedStringResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_stripped_string_async_with_rule_id"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSStrippedStringsController.updateStrippedStringAsyncWithRuleId") updateStrippedStringAsyncWithRuleId

> TODO: Add a method description


```objc
function updateStrippedStringAsyncWithRuleId:(double) ruleId
                body:(UpdateStrippedStringRequest*) body
                completionBlock:(CompletedPutUpdateStrippedString) onCompleted(ruleId body : body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    double ruleId = [@"20" doubleValue];
    UpdateStrippedStringRequest* body = (UpdateStrippedStringRequest*) [APIHelper jsonDeserialize: @"{    \"strip_string\" : \"~~~test1~~~\"}"
                toClass: UpdateStrippedStringRequest.class];

    [self.emailToSMSStrippedStrings updateStrippedStringAsyncWithRuleId: ruleId body : body  completionBlock:^(BOOL success, HttpContext* context, UpdateStrippedStringResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="delete_stripped_string_async_with_rule_id"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSStrippedStringsController.deleteStrippedStringAsyncWithRuleId") deleteStrippedStringAsyncWithRuleId

> TODO: Add a method description


```objc
function deleteStrippedStringAsyncWithRuleId:(double) ruleId
                completionBlock:(CompletedDeleteStrippedString) onCompleted(ruleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |





#### Example Usage

```objc
    // Parameters for the API call
    double ruleId = [@"20" doubleValue];

    [self.emailToSMSStrippedStrings deleteStrippedStringAsyncWithRuleId: ruleId  completionBlock:^(BOOL success, HttpContext* context, DeleteStrippedStringResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="fax_controller"></a>![Class: ](https://apidocs.io/img/class.png ".FaxController") FaxController

### Get singleton instance
```objc
Fax* fax = [[Fax alloc]init] ;
```

### <a name="create_send_fax_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.createSendFaxAsyncWithBody") createSendFaxAsyncWithBody

> **Letter File Options**
> **Use existing URL**
> With this option, you can use an existing URL to a PDF document. For example, you might generate the pdf on your server.
> **Upload File to Our Server**
> With this option, you can use the `/uploads` endpoint to upload the document. The `/uploads` endpoint returns a URL that can be used in the `/fax/send` endpoint.


```objc
function createSendFaxAsyncWithBody:(SendFaxRequest*) body
                completionBlock:(CompletedPostSendFax) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    SendFaxRequest* body = [[SendFaxRequest alloc]init];

    [self.fax createSendFaxAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, SendFaxResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_calculate_price_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.createCalculatePriceAsyncWithBody") createCalculatePriceAsyncWithBody

> TODO: Add a method description


```objc
function createCalculatePriceAsyncWithBody:(CalculatePriceRequest132*) body
                completionBlock:(CompletedPostCalculatePrice) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CalculatePriceRequest132* body = [[CalculatePriceRequest132 alloc]init];

    [self.fax createCalculatePriceAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CalculatePriceResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_fax_history_async_with_date_from"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.getFaxHistoryAsyncWithDateFrom") getFaxHistoryAsyncWithDateFrom

> Get a list of Fax History.


```objc
function getFaxHistoryAsyncWithDateFrom:(NSNumber*) dateFrom
                dateTo:(NSNumber*) dateTo
                q:(NSString*) q
                orderBy:(NSString*) orderBy
                completionBlock:(CompletedGetFaxHistory) onCompleted(dateFrom dateTo : dateTo q : q orderBy : orderBy)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateFrom |  ``` Optional ```  | Customize result by setting from date (timestsamp) |
| dateTo |  ``` Optional ```  | Customize result by setting to date (timestamp) |
| q |  ``` Optional ```  | Custom query |
| orderBy |  ``` Optional ```  | Order result by |





#### Example Usage

```objc
    // Parameters for the API call
    NSNumber* dateFrom = [NSNumber numberWithDouble:[@"1457572619" doubleValue]];
    NSNumber* dateTo = [NSNumber numberWithDouble:[@"1457573000" doubleValue]];
    NSString* q = @"status:Sent,status_code:201";
    NSString* orderBy = @"subject:desc";

    [self.fax getFaxHistoryAsyncWithDateFrom: dateFrom dateTo : dateTo q : q orderBy : orderBy  completionBlock:^(BOOL success, HttpContext* context, GetFaxHistoryResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="list_of_fax_delivery_receipts_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.listOfFaxDeliveryReceiptsWithCompletionBlock") listOfFaxDeliveryReceiptsWithCompletionBlock

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


```objc
function listOfFaxDeliveryReceiptsWithCompletionBlock:(CompletedGetListOfFaxDeliveryReceipts) onCompleted()
```



#### Example Usage

```objc

    [self.fax listOfFaxDeliveryReceiptsWithCompletionBlock:  ^(BOOL success, HttpContext* context, ListOfFaxDeliveryReceiptsResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_a_specific_fax_delivery_receipt_async_with_message_id"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.getASpecificFaxDeliveryReceiptAsyncWithMessageId") getASpecificFaxDeliveryReceiptAsyncWithMessageId

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


```objc
function getASpecificFaxDeliveryReceiptAsyncWithMessageId:(NSString*) messageId
                completionBlock:(CompletedGetASpecificFaxDeliveryReceipt) onCompleted(messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | D2AF-479B-8955-6395D561DEF4" (required, number) - Message ID. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* messageId = @"\"3FAC74F1";

    [self.fax getASpecificFaxDeliveryReceiptAsyncWithMessageId: messageId  completionBlock:^(BOOL success, HttpContext* context, GetASpecificFaxDeliveryReceiptResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_mark_fax_delivery_receipts_as_read_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.updateMarkFaxDeliveryReceiptsAsReadAsyncWithBody") updateMarkFaxDeliveryReceiptsAsReadAsyncWithBody

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


```objc
function updateMarkFaxDeliveryReceiptsAsReadAsyncWithBody:(MarkFaxDeliveryReceiptsAsReadRequest*) body
                completionBlock:(CompletedPutMarkFaxDeliveryReceiptsAsRead) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    MarkFaxDeliveryReceiptsAsReadRequest* body = (MarkFaxDeliveryReceiptsAsReadRequest*) [APIHelper jsonDeserialize: @"{    \"date_before\": 1441958441}"
                toClass: MarkFaxDeliveryReceiptsAsReadRequest.class];

    [self.fax updateMarkFaxDeliveryReceiptsAsReadAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, MarkFaxDeliveryReceiptsAsReadResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="add_a_test_delivery_receipt_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.addATestDeliveryReceiptAsyncWithBody") addATestDeliveryReceiptAsyncWithBody

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


```objc
function addATestDeliveryReceiptAsyncWithBody:(AddATestDeliveryReceiptRequest*) body
                completionBlock:(CompletedPostAddATestDeliveryReceipt) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    AddATestDeliveryReceiptRequest* body = (AddATestDeliveryReceiptRequest*) [APIHelper jsonDeserialize: @"    {        \"url\":\"http://yourUrl.com\"    }"
                toClass: AddATestDeliveryReceiptRequest.class];

    [self.fax addATestDeliveryReceiptAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, AddATestDeliveryReceiptResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="forgot_account_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ForgotAccountController") ForgotAccountController

### Get singleton instance
```objc
ForgotAccount* forgotAccount = [[ForgotAccount alloc]init] ;
```

### <a name="update_forgot_username_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".ForgotAccountController.updateForgotUsernameAsyncWithBody") updateForgotUsernameAsyncWithBody

> TODO: Add a method description


```objc
function updateForgotUsernameAsyncWithBody:(ForgotUsernameRequest*) body
                completionBlock:(CompletedPutForgotUsername) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    ForgotUsernameRequest* body = [[ForgotUsernameRequest alloc]init];

    [self.forgotAccount updateForgotUsernameAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, ForgotUsernameResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_forgot_password_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".ForgotAccountController.updateForgotPasswordAsyncWithBody") updateForgotPasswordAsyncWithBody

> TODO: Add a method description


```objc
function updateForgotPasswordAsyncWithBody:(ForgotPasswordRequest*) body
                completionBlock:(CompletedPutForgotPassword) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    ForgotPasswordRequest* body = (ForgotPasswordRequest*) [APIHelper jsonDeserialize: @"    {        \"username\": \"0F6pKiiuca\"    }"
                toClass: ForgotPasswordRequest.class];

    [self.forgotAccount updateForgotPasswordAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, ForgotPasswordResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_verify_forgot_password_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".ForgotAccountController.updateVerifyForgotPasswordAsyncWithBody") updateVerifyForgotPasswordAsyncWithBody

> TODO: Add a method description


```objc
function updateVerifyForgotPasswordAsyncWithBody:(VerifyForgotPasswordRequest*) body
                completionBlock:(CompletedPutVerifyForgotPassword) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    VerifyForgotPasswordRequest* body = (VerifyForgotPasswordRequest*) [APIHelper jsonDeserialize: @"    {        \"subaccount_id\": 54,        \"activation_token\": \"9C648BAD-EB7F-4E7E-96BC-B433140C4F1F\",        \"password\": \"0F6pKiiuca\"    }"
                toClass: VerifyForgotPasswordRequest.class];

    [self.forgotAccount updateVerifyForgotPasswordAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, VerifyForgotPasswordResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="mms_controller"></a>![Class: ](https://apidocs.io/img/class.png ".MMSController") MMSController

### Get singleton instance
```objc
MMS* mMS = [[MMS alloc]init] ;
```

### <a name="create_send_mms_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.createSendMMSAsyncWithBody") createSendMMSAsyncWithBody

> TODO: Add a method description


```objc
function createSendMMSAsyncWithBody:(SendMMSRequest*) body
                completionBlock:(CompletedPostSendMMS) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    SendMMSRequest* body = [[SendMMSRequest alloc]init];

    [self.mMS createSendMMSAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, SendMMSResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_get_price_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.createGetPriceAsyncWithBody") createGetPriceAsyncWithBody

> TODO: Add a method description


```objc
function createGetPriceAsyncWithBody:(GetPriceRequest*) body
                completionBlock:(CompletedPostGetPrice) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    GetPriceRequest* body = [[GetPriceRequest alloc]init];

    [self.mMS createGetPriceAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, GetPriceResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_mms_history_async_with_q"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.getMMSHistoryAsyncWithQ") getMMSHistoryAsyncWithQ

> TODO: Add a method description


```objc
function getMMSHistoryAsyncWithQ:(NSString*) q
                orderBy:(NSString*) orderBy
                dateFrom:(NSNumber*) dateFrom
                dateTo:(NSNumber*) dateTo
                completionBlock:(CompletedGetMMSHistory) onCompleted(q orderBy : orderBy dateFrom : dateFrom dateTo : dateTo)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| q |  ``` Optional ```  | A custom query. |
| orderBy |  ``` Optional ```  | Sort records by. |
| dateFrom |  ``` Optional ```  | Timestamp (from) used to show records by date. |
| dateTo |  ``` Optional ```  | Timestamp (to) used to show records by date. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* q = @"list_id:429,direction:out";
    NSString* orderBy = @"subject:desc";
    NSNumber* dateFrom = [NSNumber numberWithInteger:[@"1443501617" integerValue]];
    NSNumber* dateTo = [NSNumber numberWithInteger:[@"1443501727" integerValue]];

    [self.mMS getMMSHistoryAsyncWithQ: q orderBy : orderBy dateFrom : dateFrom dateTo : dateTo  completionBlock:^(BOOL success, HttpContext* context, GetMMSHistoryResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_export_mms_history_async_with_filename"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.getExportMMSHistoryAsyncWithFilename") getExportMMSHistoryAsyncWithFilename

> TODO: Add a method description


```objc
function getExportMMSHistoryAsyncWithFilename:(NSString*) filename
                completionBlock:(CompletedGetExportMMSHistory) onCompleted(filename)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | Your export filename. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* filename = @"export.csv";

    [self.mMS getExportMMSHistoryAsyncWithFilename: filename  completionBlock:^(BOOL success, HttpContext* context, ExportMMSHistoryResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_cancel_mms_async_with_message_id"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.updateCancelMMSAsyncWithMessageId") updateCancelMMSAsyncWithMessageId

> TODO: Add a method description


```objc
function updateCancelMMSAsyncWithMessageId:(NSString*) messageId
                completionBlock:(CompletedPutCancelMMS) onCompleted(messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Message ID. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* messageId = @"message_id";

    [self.mMS updateCancelMMSAsyncWithMessageId: messageId  completionBlock:^(BOOL success, HttpContext* context, CancelMMSResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_cancel_all_mms_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.updateCancelAllMMSWithCompletionBlock") updateCancelAllMMSWithCompletionBlock

> TODO: Add a method description


```objc
function updateCancelAllMMSWithCompletionBlock:(CompletedPutCancelAllMMS) onCompleted()
```



#### Example Usage

```objc

    [self.mMS updateCancelAllMMSWithCompletionBlock:  ^(BOOL success, HttpContext* context, CancelAllMMSResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_all_delivery_receipts_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.getAllDeliveryReceiptsWithCompletionBlock") getAllDeliveryReceiptsWithCompletionBlock

> TODO: Add a method description


```objc
function getAllDeliveryReceiptsWithCompletionBlock:(CompletedGetAllDeliveryReceipts) onCompleted()
```



#### Example Usage

```objc

    [self.mMS getAllDeliveryReceiptsWithCompletionBlock:  ^(BOOL success, HttpContext* context, GetAllDeliveryReceiptsResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_delivery_receipt_async_with_message_id"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.getDeliveryReceiptAsyncWithMessageId") getDeliveryReceiptAsyncWithMessageId

> TODO: Add a method description


```objc
function getDeliveryReceiptAsyncWithMessageId:(NSString*) messageId
                completionBlock:(CompletedGetDeliveryReceipt) onCompleted(messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Message ID. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* messageId = @"3E0DC217-7D0F-4C20-A3F2-E3362B938CAF";

    [self.mMS getDeliveryReceiptAsyncWithMessageId: messageId  completionBlock:^(BOOL success, HttpContext* context, GetDeliveryReceiptResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_mark_receipts_as_read_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.updateMarkReceiptsAsReadWithCompletionBlock") updateMarkReceiptsAsReadWithCompletionBlock

> TODO: Add a method description


```objc
function updateMarkReceiptsAsReadWithCompletionBlock:(CompletedPutMarkReceiptsAsRead) onCompleted()
```



#### Example Usage

```objc

    [self.mMS updateMarkReceiptsAsReadWithCompletionBlock:  ^(BOOL success, HttpContext* context, MarkReceiptsAsReadResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_all_inbound_sms_pull_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.getAllInboundSMSPullWithCompletionBlock") getAllInboundSMSPullWithCompletionBlock

> Inbound MMS shares the same rules/settings/endpoints as SMS. Any attachments will be converted to a URL.
> **Push Inbound SMS**
> If you prefer, we can push message replies to your server as they arrive with us.
> Refer to SMS->Inbound SMS in the docs.
> **Pull Inbound SMS**
> Receive SMS by polling your Inbox.
> Refer to SMS->Inbound SMS in the docs.


```objc
function getAllInboundSMSPullWithCompletionBlock:(CompletedGetAllInboundSMSPull) onCompleted()
```



#### Example Usage

```objc

    [self.mMS getAllInboundSMSPullWithCompletionBlock:  ^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="numbers_controller"></a>![Class: ](https://apidocs.io/img/class.png ".NumbersController") NumbersController

### Get singleton instance
```objc
Numbers* numbers = [[Numbers alloc]init] ;
```

### <a name="get_all_dedicated_numbers_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".NumbersController.getAllDedicatedNumbersWithCompletionBlock") getAllDedicatedNumbersWithCompletionBlock

> TODO: Add a method description


```objc
function getAllDedicatedNumbersWithCompletionBlock:(CompletedGetAllDedicatedNumbers) onCompleted()
```



#### Example Usage

```objc

    [self.numbers getAllDedicatedNumbersWithCompletionBlock:  ^(BOOL success, HttpContext* context, GetAllDedicatedNumbersResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_buy_dedicated_number_async_with_dedicated_number"></a>![Method: ](https://apidocs.io/img/method.png ".NumbersController.createBuyDedicatedNumberAsyncWithDedicatedNumber") createBuyDedicatedNumberAsyncWithDedicatedNumber

> TODO: Add a method description


```objc
function createBuyDedicatedNumberAsyncWithDedicatedNumber:(NSString*) dedicatedNumber
                completionBlock:(CompletedPostBuyDedicatedNumber) onCompleted(dedicatedNumber)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dedicatedNumber |  ``` Required ```  | Your phone number in E.164 format. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* dedicatedNumber = @"+12282060576";

    [self.numbers createBuyDedicatedNumberAsyncWithDedicatedNumber: dedicatedNumber  completionBlock:^(BOOL success, HttpContext* context, BuyDedicatedNumberResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="search_dedicated_numbers_by_country_async_with_country"></a>![Method: ](https://apidocs.io/img/method.png ".NumbersController.searchDedicatedNumbersByCountryAsyncWithCountry") searchDedicatedNumbersByCountryAsyncWithCountry

> TODO: Add a method description


```objc
function searchDedicatedNumbersByCountryAsyncWithCountry:(NSString*) country
                search:(NSString*) search
                searchType:(NSNumber*) searchType
                completionBlock:(CompletedGetSearchDedicatedNumbersByCountry) onCompleted(country search : search searchType : searchType)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Required ```  | Your preferred country. |
| search |  ``` Optional ```  | Your search pattern or query. |
| searchType |  ``` Optional ```  | Your strategy for searching, 0 = starts with, 1 = anywhere, 2 = ends with. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* country = @"US";
    NSString* search = @"88";
    NSNumber* searchType = [NSNumber numberWithDouble:[@"1" doubleValue]];

    [self.numbers searchDedicatedNumbersByCountryAsyncWithCountry: country search : search searchType : searchType  completionBlock:^(BOOL success, HttpContext* context, SearchDedicatedNumbersByCountryResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="pricing_controller"></a>![Class: ](https://apidocs.io/img/class.png ".PricingController") PricingController

### Get singleton instance
```objc
Pricing* pricing = [[Pricing alloc]init] ;
```

### <a name="get_country_pricing_async_with_country"></a>![Method: ](https://apidocs.io/img/method.png ".PricingController.getCountryPricingAsyncWithCountry") getCountryPricingAsyncWithCountry

> TODO: Add a method description


```objc
function getCountryPricingAsyncWithCountry:(NSString*) country
                currency:(NSString*) currency
                completionBlock:(CompletedGetCountryPricing) onCompleted(country currency : currency)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Required ```  | Two-letter representation of the country. |
| currency |  ``` Optional ```  | Three-letter representation of the currency. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* country = @"AU";
    NSString* currency = @"AUD";

    [self.pricing getCountryPricingAsyncWithCountry: country currency : currency  completionBlock:^(BOOL success, HttpContext* context, GetCountryPricingResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="post_direct_mail_controller"></a>![Class: ](https://apidocs.io/img/class.png ".PostDirectMailController") PostDirectMailController

### Get singleton instance
```objc
PostDirectMail* postDirectMail = [[PostDirectMail alloc]init] ;
```

### <a name="search_locations_async_with_country"></a>![Method: ](https://apidocs.io/img/method.png ".PostDirectMailController.searchLocationsAsyncWithCountry") searchLocationsAsyncWithCountry

> TODO: Add a method description


```objc
function searchLocationsAsyncWithCountry:(NSString*) country
                query:(NSString*) query
                completionBlock:(CompletedGetSearchLocations) onCompleted(country query : query)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Required ```  | Country code. |
| query |  ``` Required ```  | A postal code or place name. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* country = @"AD";
    NSString* query = @"AD100";

    [self.postDirectMail searchLocationsAsyncWithCountry: country query : query  completionBlock:^(BOOL success, HttpContext* context, SearchLocationsResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_new_campaign_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".PostDirectMailController.createNewCampaignAsyncWithBody") createNewCampaignAsyncWithBody

> Create new direct mail campaign.


```objc
function createNewCampaignAsyncWithBody:(CreateNewCampaignRequest*) body
                completionBlock:(CompletedPostCreateNewCampaign) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CreateNewCampaignRequest* body = [[CreateNewCampaignRequest alloc]init];

    [self.postDirectMail createNewCampaignAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CreateNewCampaignResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_calculate_direct_mail_campaign_price_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".PostDirectMailController.createCalculateDirectMailCampaignPriceAsyncWithBody") createCalculateDirectMailCampaignPriceAsyncWithBody

> Calculate direct mail campaign price.


```objc
function createCalculateDirectMailCampaignPriceAsyncWithBody:(CalculateDirectMailCampaignPriceRequest*) body
                completionBlock:(CompletedPostCalculateDirectMailCampaignPrice) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CalculateDirectMailCampaignPriceRequest* body = [[CalculateDirectMailCampaignPriceRequest alloc]init];

    [self.postDirectMail createCalculateDirectMailCampaignPriceAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CalculateDirectMailCampaignPriceResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="list_direct_mail_campaigns_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".PostDirectMailController.listDirectMailCampaignsWithCompletionBlock") listDirectMailCampaignsWithCompletionBlock

> Get list of direct mail campaigns.


```objc
function listDirectMailCampaignsWithCompletionBlock:(CompletedGetListDirectMailCampaigns) onCompleted()
```



#### Example Usage

```objc

    [self.postDirectMail listDirectMailCampaignsWithCompletionBlock:  ^(BOOL success, HttpContext* context, ListDirectMailCampaignsResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="post_letter_controller"></a>![Class: ](https://apidocs.io/img/class.png ".PostLetterController") PostLetterController

### Get singleton instance
```objc
PostLetter* postLetter = [[PostLetter alloc]init] ;
```

### <a name="create_send_post_letter_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.createSendPostLetterAsyncWithBody") createSendPostLetterAsyncWithBody

> **Supported File Types**
> We support `pdf`, `docx` and `doc` files. Contact us to add support for any other file type. If you're using `docx` or `doc` files, you'll need to convert the file first using our uploads endpoint with the querystring parameter `convert=post` e.g. `POST /uploads?convert=post`. This will return a URL to the converted pdf file that can be used in the `/post/letters/send` endpoint.
> **Letter File Options**
> **Use existing URL**
> With this option, you can use an existing URL to a `pdf` document. For example, you might generate the `pdf` on your server.
> **Upload File to Our Server**
> With this option, you can use the `/uploads` endpoint to upload the document. The `/uploads` endpoint returns a URL that can be used in the `/post/letters/send` endpoint.


```objc
function createSendPostLetterAsyncWithBody:(SendPostLetterRequest*) body
                completionBlock:(CompletedPostSendPostLetter) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    SendPostLetterRequest* body = (SendPostLetterRequest*) [APIHelper jsonDeserialize: @"{  \"file_url\": \"http://server.com/file.pdf\",  \"template_used\": 1,  \"colour\": 1,  \"duplex\": 0,  \"recipients\": [    {      \"address_name\": \"My Home Address\",      \"address_line_1\": \"Address 1\",      \"address_line_2\": \"Address 2\",      \"address_city\": \"CITY\",      \"address_state\": \"State\",      \"address_postal_code\": 123456,      \"address_country\": \"AU\",      \"return_address_id\": 1,      \"schedule\": 1449573604    }  ]}"
                toClass: SendPostLetterRequest.class];

    [self.postLetter createSendPostLetterAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, SendPostLetterResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_calculate_price_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.createCalculatePriceAsyncWithBody") createCalculatePriceAsyncWithBody

> TODO: Add a method description


```objc
function createCalculatePriceAsyncWithBody:(CalculatePriceRequest170*) body
                completionBlock:(CompletedPostCalculatePrice) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CalculatePriceRequest170* body = (CalculatePriceRequest170*) [APIHelper jsonDeserialize: @"{  \"file_url\": \"http://server.com/file.pdf\",  \"template_used\": 1,  \"colour\": 1,  \"duplex\": 0,  \"recipients\": [    \"[]\"  ],  \"Body\": \"\"}"
                toClass: CalculatePriceRequest170.class];

    [self.postLetter createCalculatePriceAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CalculatePriceResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_post_letter_history_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.getPostLetterHistoryWithCompletionBlock") getPostLetterHistoryWithCompletionBlock

> TODO: Add a method description


```objc
function getPostLetterHistoryWithCompletionBlock:(CompletedGetPostLetterHistory) onCompleted()
```



#### Example Usage

```objc

    [self.postLetter getPostLetterHistoryWithCompletionBlock:  ^(BOOL success, HttpContext* context, GetPostLetterHistoryResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_export_post_letter_history_async_with_filename"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.getExportPostLetterHistoryAsyncWithFilename") getExportPostLetterHistoryAsyncWithFilename

> TODO: Add a method description


```objc
function getExportPostLetterHistoryAsyncWithFilename:(NSString*) filename
                completionBlock:(CompletedGetExportPostLetterHistory) onCompleted(filename)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | Filename for the export file. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* filename = @"myexport.csv";

    [self.postLetter getExportPostLetterHistoryAsyncWithFilename: filename  completionBlock:^(BOOL success, HttpContext* context, ExportPostLetterHistoryResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_a_post_return_address_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.createAPostReturnAddressAsyncWithBody") createAPostReturnAddressAsyncWithBody

> TODO: Add a method description


```objc
function createAPostReturnAddressAsyncWithBody:(CreateAPostReturnAddressRequest*) body
                completionBlock:(CompletedPostCreateAPostReturnAddress) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CreateAPostReturnAddressRequest* body = (CreateAPostReturnAddressRequest*) [APIHelper jsonDeserialize: @"{    \"address_name\":\"My Home Address\",    \"address_line_1\":\"Maritime Avenue\",    \"address_line_2\":\"\",    \"address_city\":\"Flynn\",    \"address_state\":\"WA\",    \"address_postal_code\":6302,    \"address_country\":\"Australia\"}"
                toClass: CreateAPostReturnAddressRequest.class];

    [self.postLetter createAPostReturnAddressAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CreateAPostReturnAddressResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_list_of_post_return_addresses_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.getListOfPostReturnAddressesWithCompletionBlock") getListOfPostReturnAddressesWithCompletionBlock

> TODO: Add a method description


```objc
function getListOfPostReturnAddressesWithCompletionBlock:(CompletedGetListOfPostReturnAddresses) onCompleted()
```



#### Example Usage

```objc

    [self.postLetter getListOfPostReturnAddressesWithCompletionBlock:  ^(BOOL success, HttpContext* context, GetListOfPostReturnAddressesResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_post_return_address_async_with_return_address_id"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.getPostReturnAddressAsyncWithReturnAddressId") getPostReturnAddressAsyncWithReturnAddressId

> TODO: Add a method description


```objc
function getPostReturnAddressAsyncWithReturnAddressId:(double) returnAddressId
                completionBlock:(CompletedGetPostReturnAddress) onCompleted(returnAddressId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| returnAddressId |  ``` Required ```  | Your return address id. |





#### Example Usage

```objc
    // Parameters for the API call
    double returnAddressId = [@"14" doubleValue];

    [self.postLetter getPostReturnAddressAsyncWithReturnAddressId: returnAddressId  completionBlock:^(BOOL success, HttpContext* context, GetPostReturnAddressResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_post_return_address_async_with_return_address_id"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.updatePostReturnAddressAsyncWithReturnAddressId") updatePostReturnAddressAsyncWithReturnAddressId

> TODO: Add a method description


```objc
function updatePostReturnAddressAsyncWithReturnAddressId:(double) returnAddressId
                body:(UpdatePostReturnAddressRequest*) body
                completionBlock:(CompletedPutUpdatePostReturnAddress) onCompleted(returnAddressId body : body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| returnAddressId |  ``` Required ```  | Your return address id. |
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    double returnAddressId = [@"14" doubleValue];
    UpdatePostReturnAddressRequest* body = (UpdatePostReturnAddressRequest*) [APIHelper jsonDeserialize: @"{    \"address_name\":\"My Home Address\",    \"address_line_1\":\"Maritime Avenue\",    \"address_line_2\":\"\",    \"address_city\":\"Flynn\",    \"address_state\":\"WA\",    \"address_postal_code\":6302,    \"address_country\":\"Australia\"}"
                toClass: UpdatePostReturnAddressRequest.class];

    [self.postLetter updatePostReturnAddressAsyncWithReturnAddressId: returnAddressId body : body  completionBlock:^(BOOL success, HttpContext* context, UpdatePostReturnAddressResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="delete_post_return_address_async_with_return_address_id"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.deletePostReturnAddressAsyncWithReturnAddressId") deletePostReturnAddressAsyncWithReturnAddressId

> TODO: Add a method description


```objc
function deletePostReturnAddressAsyncWithReturnAddressId:(double) returnAddressId
                completionBlock:(CompletedDeletePostReturnAddress) onCompleted(returnAddressId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| returnAddressId |  ``` Required ```  | Your return address id. |





#### Example Usage

```objc
    // Parameters for the API call
    double returnAddressId = [@"12" doubleValue];

    [self.postLetter deletePostReturnAddressAsyncWithReturnAddressId: returnAddressId  completionBlock:^(BOOL success, HttpContext* context, DeletePostReturnAddressResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="postcards_controller"></a>![Class: ](https://apidocs.io/img/class.png ".PostcardsController") PostcardsController

### Get singleton instance
```objc
Postcards* postcards = [[Postcards alloc]init] ;
```

### <a name="create_send_postcard_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".PostcardsController.createSendPostcardAsyncWithBody") createSendPostcardAsyncWithBody

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


```objc
function createSendPostcardAsyncWithBody:(SendPostcardRequest*) body
                completionBlock:(CompletedPostSendPostcard) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    SendPostcardRequest* body = (SendPostcardRequest*) [APIHelper jsonDeserialize: @"{    \"file_urls\":[         \"https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_front.pdf\",         \"https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_back.pdf\"    ],    \"recipients\":[        {            \"address_name\":\"My Home Address\",            \"address_line_1\":\"Address 1\",            \"address_line_2\":\"\",            \"address_city\":\"City\",            \"address_state\":\"State\",            \"address_postal_code\":\"123456\",            \"address_country\":\"AU\",            \"return_address_id\":1        }    ]}"
                toClass: SendPostcardRequest.class];

    [self.postcards createSendPostcardAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, SendPostcardResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_calculate_pricing_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".PostcardsController.createCalculatePricingAsyncWithBody") createCalculatePricingAsyncWithBody

> For `file_urls` field. You can attach at least 1 and max of 2 PDF file urls.
> - Supply a single pdf with 2 pages (front and back)
> - Supply 2 urls to seperate PDFs


```objc
function createCalculatePricingAsyncWithBody:(CalculatePricingRequest*) body
                completionBlock:(CompletedPostCalculatePricing) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CalculatePricingRequest* body = (CalculatePricingRequest*) [APIHelper jsonDeserialize: @"{    \"file_urls\":[        \"https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_front.pdf\",        \"https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_back.pdf\"    ],    \"recipients\":[        {            \"address_name\":\"My Home Address\",            \"address_line_1\":\"Address 1\",            \"address_line_2\":\"\",            \"address_city\":\"City\",            \"address_state\":\"State\",            \"address_postal_code\":\"123456\",            \"address_country\":\"AU\",            \"return_address_id\":1        }    ]}"
                toClass: CalculatePricingRequest.class];

    [self.postcards createCalculatePricingAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CalculatePricingResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_postcard_history_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".PostcardsController.getPostcardHistoryWithCompletionBlock") getPostcardHistoryWithCompletionBlock

> TODO: Add a method description


```objc
function getPostcardHistoryWithCompletionBlock:(CompletedGetPostcardHistory) onCompleted()
```



#### Example Usage

```objc

    [self.postcards getPostcardHistoryWithCompletionBlock:  ^(BOOL success, HttpContext* context, GetPostcardHistoryResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_export_postcard_history_async_with_filename"></a>![Method: ](https://apidocs.io/img/method.png ".PostcardsController.getExportPostcardHistoryAsyncWithFilename") getExportPostcardHistoryAsyncWithFilename

> TODO: Add a method description


```objc
function getExportPostcardHistoryAsyncWithFilename:(NSString*) filename
                completionBlock:(CompletedGetExportPostcardHistory) onCompleted(filename)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | Filename for the export file. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* filename = @"myexport.csv";

    [self.postcards getExportPostcardHistoryAsyncWithFilename: filename  completionBlock:^(BOOL success, HttpContext* context, ExportPostcardHistoryResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="referral_accounts_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ReferralAccountsController") ReferralAccountsController

### Get singleton instance
```objc
ReferralAccounts* referralAccounts = [[ReferralAccounts alloc]init] ;
```

### <a name="get_list_of_referral_accounts_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ReferralAccountsController.getListOfReferralAccountsWithCompletionBlock") getListOfReferralAccountsWithCompletionBlock

> TODO: Add a method description


```objc
function getListOfReferralAccountsWithCompletionBlock:(CompletedGetListOfReferralAccounts) onCompleted()
```



#### Example Usage

```objc

    [self.referralAccounts getListOfReferralAccountsWithCompletionBlock:  ^(BOOL success, HttpContext* context, GetListOfReferralAccountsResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="reseller_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ResellerController") ResellerController

### Get singleton instance
```objc
Reseller* reseller = [[Reseller alloc]init] ;
```

### <a name="get_reseller_setting_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerController.getResellerSettingWithCompletionBlock") getResellerSettingWithCompletionBlock

> Get reseller setting.


```objc
function getResellerSettingWithCompletionBlock:(CompletedGetResellerSetting) onCompleted()
```



#### Example Usage

```objc

    [self.reseller getResellerSettingWithCompletionBlock:  ^(BOOL success, HttpContext* context, GetResellerSettingResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_reseller_setting_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerController.updateResellerSettingAsyncWithBody") updateResellerSettingAsyncWithBody

> Update a specific reseller setting.


```objc
function updateResellerSettingAsyncWithBody:(UpdateResellerSettingRequest*) body
                completionBlock:(CompletedPutUpdateResellerSetting) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    UpdateResellerSettingRequest* body = (UpdateResellerSettingRequest*) [APIHelper jsonDeserialize: @"    {        \"allow_public_signups\":1,        \"default_margin\":100,        \"default_margin_numbers\":150,        \"trial_balance\":50,        \"subdomain\":\"subdomain\",        \"colour_navigation\":\"#9999FF\",        \"logo_url_light\":\"http://url.com/light\",        \"logo_url_dark\":\"http://url.com/dark\",        \"company_name\":\"MyCompany\"    }"
                toClass: UpdateResellerSettingRequest.class];

    [self.reseller updateResellerSettingAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, UpdateResellerSettingResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_reseller_by_subdomain_async_with_subdomain"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerController.getResellerBySubdomainAsyncWithSubdomain") getResellerBySubdomainAsyncWithSubdomain

> Get reseller setting by subdomin.


```objc
function getResellerBySubdomainAsyncWithSubdomain:(NSString*) subdomain
                completionBlock:(CompletedGetResellerBySubdomain) onCompleted(subdomain)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subdomain |  ``` Required ```  | Subdomain |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* subdomain = @"mysubdomain";

    [self.reseller getResellerBySubdomainAsyncWithSubdomain: subdomain  completionBlock:^(BOOL success, HttpContext* context, ResellerBySubdomainResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="reseller_accounts_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ResellerAccountsController") ResellerAccountsController

### Get singleton instance
```objc
ResellerAccounts* resellerAccounts = [[ResellerAccounts alloc]init] ;
```

### <a name="list_of_reseller_accounts_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.listOfResellerAccountsWithCompletionBlock") listOfResellerAccountsWithCompletionBlock

> Get list of Reseller Accounts


```objc
function listOfResellerAccountsWithCompletionBlock:(CompletedGetListOfResellerAccounts) onCompleted()
```



#### Example Usage

```objc

    [self.resellerAccounts listOfResellerAccountsWithCompletionBlock:  ^(BOOL success, HttpContext* context, ListOfResellerAccountsResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_reseller_account_async_with_client_user_id"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.getResellerAccountAsyncWithClientUserId") getResellerAccountAsyncWithClientUserId

> Get a specific reseller account.


```objc
function getResellerAccountAsyncWithClientUserId:(double) clientUserId
                completionBlock:(CompletedGetResellerAccount) onCompleted(clientUserId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| clientUserId |  ``` Required ```  | The client user id. |





#### Example Usage

```objc
    // Parameters for the API call
    double clientUserId = [@"24" doubleValue];

    [self.resellerAccounts getResellerAccountAsyncWithClientUserId: clientUserId  completionBlock:^(BOOL success, HttpContext* context, GetResellerAccountResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_reseller_account_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.createResellerAccountAsyncWithBody") createResellerAccountAsyncWithBody

> TODO: Add a method description


```objc
function createResellerAccountAsyncWithBody:(CreateResellerAccountRequest*) body
                completionBlock:(CompletedPostCreateResellerAccount) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CreateResellerAccountRequest* body = (CreateResellerAccountRequest*) [APIHelper jsonDeserialize: @"    {        \"username\":\"johndoe2\",        \"user_email\":\"johndoe2@awesome.com\",        \"user_phone\":\"518-481-1002\",        \"user_first_name\":\"John\",        \"user_last_name\":\"Doe\",        \"country\":\"US\",        \"password\":\"pass\",        \"account_name\":\"The Awesome Company\"    }"
                toClass: CreateResellerAccountRequest.class];

    [self.resellerAccounts createResellerAccountAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CreateResellerAccountResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_reseller_account_public_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.createResellerAccountPublicAsyncWithBody") createResellerAccountPublicAsyncWithBody

> TODO: Add a method description


```objc
function createResellerAccountPublicAsyncWithBody:(CreateResellerAccountPublicRequest*) body
                completionBlock:(CompletedPostCreateResellerAccountPublic) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CreateResellerAccountPublicRequest* body = (CreateResellerAccountPublicRequest*) [APIHelper jsonDeserialize: @"{    \"reseller_user_id\":1,    \"username\":\"john_awesome\",    \"user_email\":\"johnis@awesome.com\",    \"user_phone\":\"+61261063270\",    \"user_first_name\":\"John\",    \"user_last_name\":\"Awesome\",    \"country\":\"AU\",    \"password\":\"pass\",    \"account_name\":\"The Awesome Company\"}"
                toClass: CreateResellerAccountPublicRequest.class];

    [self.resellerAccounts createResellerAccountPublicAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CreateResellerAccountPublicResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_reseller_account_async_with_client_user_id"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.updateResellerAccountAsyncWithClientUserId") updateResellerAccountAsyncWithClientUserId

> TODO: Add a method description


```objc
function updateResellerAccountAsyncWithClientUserId:(double) clientUserId
                body:(UpdateResellerAccountRequest*) body
                completionBlock:(CompletedPutUpdateResellerAccount) onCompleted(clientUserId body : body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| clientUserId |  ``` Required ```  | Your client user id. |
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    double clientUserId = [@"24" doubleValue];
    UpdateResellerAccountRequest* body = (UpdateResellerAccountRequest*) [APIHelper jsonDeserialize: @"    {        \"username\":\"johndoe2\",        \"user_email\":\"johndoe2@awesome.com\",        \"user_phone\":\"518-481-1002\",        \"user_first_name\":\"John\",        \"user_last_name\":\"Doe\",        \"country\":\"US\",        \"password\":\"pass\",        \"account_name\":\"The Awesome Company\"    }"
                toClass: UpdateResellerAccountRequest.class];

    [self.resellerAccounts updateResellerAccountAsyncWithClientUserId: clientUserId body : body  completionBlock:^(BOOL success, HttpContext* context, UpdateResellerAccountResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_transfer_credit_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.updateTransferCreditAsyncWithBody") updateTransferCreditAsyncWithBody

> TODO: Add a method description


```objc
function updateTransferCreditAsyncWithBody:(TransferCreditRequest*) body
                completionBlock:(CompletedPutTransferCredit) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    TransferCreditRequest* body = [[TransferCreditRequest alloc]init];

    [self.resellerAccounts updateTransferCreditAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, TransferCreditResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="sdk_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SDKController") SDKController

### Get singleton instance
```objc
SDK* sDK = [[SDK alloc]init] ;
```

### <a name="get_sdk_download_async_with_type"></a>![Method: ](https://apidocs.io/img/method.png ".SDKController.getSDKDownloadAsyncWithType") getSDKDownloadAsyncWithType

> TODO: Add a method description


```objc
function getSDKDownloadAsyncWithType:(NSString*) type
                completionBlock:(CompletedGetSDKDownload) onCompleted(type)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| type |  ``` Required ```  | Supported types. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* type = @"type";

    [self.sDK getSDKDownloadAsyncWithType: type  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="search_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SearchController") SearchController

### Get singleton instance
```objc
Search* search = [[Search alloc]init] ;
```

### <a name="search_contacts_lists_async_with_q"></a>![Method: ](https://apidocs.io/img/method.png ".SearchController.searchContactsListsAsyncWithQ") searchContactsListsAsyncWithQ

> TODO: Add a method description


```objc
function searchContactsListsAsyncWithQ:(NSString*) q
                completionBlock:(CompletedGetSearchContactsLists) onCompleted(q)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| q |  ``` Required ```  | Your keyword or query. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* q = @"Gorne";

    [self.search searchContactsListsAsyncWithQ: q  completionBlock:^(BOOL success, HttpContext* context, SearchContactsListsResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="sms_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SMSController") SMSController

### Get singleton instance
```objc
SMS* sMS = [[SMS alloc]init] ;
```

### <a name="create_send_an_sms_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.createSendAnSMSAsyncWithBody") createSendAnSMSAsyncWithBody

> You can post **up to 1000 messages** with each API call.


```objc
function createSendAnSMSAsyncWithBody:(SendAnSMSRequest*) body
                completionBlock:(CompletedPostSendAnSMS) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    SendAnSMSRequest* body = [[SendAnSMSRequest alloc]init];

    [self.sMS createSendAnSMSAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, SendAnSMSResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_calculate_price_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.createCalculatePriceAsyncWithBody") createCalculatePriceAsyncWithBody

> TODO: Add a method description


```objc
function createCalculatePriceAsyncWithBody:(CalculatePriceRequest205*) body
                completionBlock:(CompletedPostCalculatePrice) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CalculatePriceRequest205* body = [[CalculatePriceRequest205 alloc]init];

    [self.sMS createCalculatePriceAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CalculatePriceResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_all_history_async_with_date_from"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.getAllHistoryAsyncWithDateFrom") getAllHistoryAsyncWithDateFrom

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


```objc
function getAllHistoryAsyncWithDateFrom:(NSNumber*) dateFrom
                dateTo:(NSNumber*) dateTo
                completionBlock:(CompletedGetAllHistory) onCompleted(dateFrom dateTo : dateTo)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateFrom |  ``` Optional ```  | Timestamp (from) used to show records by date. |
| dateTo |  ``` Optional ```  | Timestamp (to) used to show recrods by date. |





#### Example Usage

```objc
    // Parameters for the API call
    NSNumber* dateFrom = [NSNumber numberWithInteger:[@"1449459940" integerValue]];
    NSNumber* dateTo = [NSNumber numberWithInteger:[@"1449659940" integerValue]];

    [self.sMS getAllHistoryAsyncWithDateFrom: dateFrom dateTo : dateTo  completionBlock:^(BOOL success, HttpContext* context, GetAllHistoryResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_export_sms_history_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.getExportSMSHistoryWithCompletionBlock") getExportSMSHistoryWithCompletionBlock

> TODO: Add a method description


```objc
function getExportSMSHistoryWithCompletionBlock:(CompletedGetExportSMSHistory) onCompleted()
```



#### Example Usage

```objc

    [self.sMS getExportSMSHistoryWithCompletionBlock:  ^(BOOL success, HttpContext* context, ExportSMSHistoryResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_all_delivery_receipts_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.getAllDeliveryReceiptsWithCompletionBlock") getAllDeliveryReceiptsWithCompletionBlock

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


```objc
function getAllDeliveryReceiptsWithCompletionBlock:(CompletedGetAllDeliveryReceipts) onCompleted()
```



#### Example Usage

```objc

    [self.sMS getAllDeliveryReceiptsWithCompletionBlock:  ^(BOOL success, HttpContext* context, GetAllDeliveryReceiptsResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_a_specific_delivery_receipt_async_with_message_id"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.getASpecificDeliveryReceiptAsyncWithMessageId") getASpecificDeliveryReceiptAsyncWithMessageId

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


```objc
function getASpecificDeliveryReceiptAsyncWithMessageId:(NSString*) messageId
                completionBlock:(CompletedGetASpecificDeliveryReceipt) onCompleted(messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Your message id. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* messageId = @"88AB118E EB1B 478C 98CE 6C73ABA23F67";

    [self.sMS getASpecificDeliveryReceiptAsyncWithMessageId: messageId  completionBlock:^(BOOL success, HttpContext* context, GetASpecificDeliveryReceiptResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="add_a_test_delivery_receipt_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.addATestDeliveryReceiptAsyncWithBody") addATestDeliveryReceiptAsyncWithBody

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


```objc
function addATestDeliveryReceiptAsyncWithBody:(AddATestDeliveryReceiptRequest*) body
                completionBlock:(CompletedPostAddATestDeliveryReceipt) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    AddATestDeliveryReceiptRequest* body = (AddATestDeliveryReceiptRequest*) [APIHelper jsonDeserialize: @"    {        \"url\":\"http://yourUrl.com\"    }"
                toClass: AddATestDeliveryReceiptRequest.class];

    [self.sMS addATestDeliveryReceiptAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, AddATestDeliveryReceiptResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_mark_delivery_receipts_as_read_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.updateMarkDeliveryReceiptsAsReadAsyncWithBody") updateMarkDeliveryReceiptsAsReadAsyncWithBody

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


```objc
function updateMarkDeliveryReceiptsAsReadAsyncWithBody:(MarkDeliveryReceiptsAsReadRequest*) body
                completionBlock:(CompletedPutMarkDeliveryReceiptsAsRead) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    MarkDeliveryReceiptsAsReadRequest* body = (MarkDeliveryReceiptsAsReadRequest*) [APIHelper jsonDeserialize: @"{    \"date_before\": 1441958441}"
                toClass: MarkDeliveryReceiptsAsReadRequest.class];

    [self.sMS updateMarkDeliveryReceiptsAsReadAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, MarkDeliveryReceiptsAsReadResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_all_inbound_sms_pull_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.getAllInboundSMSPullWithCompletionBlock") getAllInboundSMSPullWithCompletionBlock

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


```objc
function getAllInboundSMSPullWithCompletionBlock:(CompletedGetAllInboundSMSPull) onCompleted()
```



#### Example Usage

```objc

    [self.sMS getAllInboundSMSPullWithCompletionBlock:  ^(BOOL success, HttpContext* context, GetAllInboundSMSPullResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_specific_inbound_pull_async_with_message_id"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.getSpecificInboundPullAsyncWithMessageId") getSpecificInboundPullAsyncWithMessageId

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


```objc
function getSpecificInboundPullAsyncWithMessageId:(NSString*) messageId
                completionBlock:(CompletedGetSpecificInboundPull) onCompleted(messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Message ID. Must be a valid GUID. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* messageId = @"5D420421-8715-4461-A9A2-C8F569E41835";

    [self.sMS getSpecificInboundPullAsyncWithMessageId: messageId  completionBlock:^(BOOL success, HttpContext* context, GetSpecificInboundPullResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="add_a_test_inbound_sms_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.addATestInboundSMSAsyncWithBody") addATestInboundSMSAsyncWithBody

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


```objc
function addATestInboundSMSAsyncWithBody:(AddATestInboundSMSRequest*) body
                completionBlock:(CompletedPostAddATestInboundSMS) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    AddATestInboundSMSRequest* body = (AddATestInboundSMSRequest*) [APIHelper jsonDeserialize: @"    {        \"url\":\"http://yourUrl.com\"    }"
                toClass: AddATestInboundSMSRequest.class];

    [self.sMS addATestInboundSMSAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, AddATestInboundSMSResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_mark_a_specific_inbound_sms_as_read_async_with_message_id"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.updateMarkASpecificInboundSMSAsReadAsyncWithMessageId") updateMarkASpecificInboundSMSAsReadAsyncWithMessageId

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


```objc
function updateMarkASpecificInboundSMSAsReadAsyncWithMessageId:(NSString*) messageId
                completionBlock:(CompletedPutMarkASpecificInboundSMSAsRead) onCompleted(messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | B7CE432193CD-0753597B7293 (string, required) - The message ID you want to mark as read. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* messageId = @"307EF035";

    [self.sMS updateMarkASpecificInboundSMSAsReadAsyncWithMessageId: messageId  completionBlock:^(BOOL success, HttpContext* context, MarkASpecificInboundSMSAsReadResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_mark_all_inbound_sms_as_read_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.updateMarkAllInboundSMSAsReadAsyncWithBody") updateMarkAllInboundSMSAsReadAsyncWithBody

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


```objc
function updateMarkAllInboundSMSAsReadAsyncWithBody:(MarkAllInboundSMSAsReadRequest*) body
                completionBlock:(CompletedPutMarkAllInboundSMSAsRead) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    MarkAllInboundSMSAsReadRequest* body = (MarkAllInboundSMSAsReadRequest*) [APIHelper jsonDeserialize: @"    {        \"date_before\":1442398100    }"
                toClass: MarkAllInboundSMSAsReadRequest.class];

    [self.sMS updateMarkAllInboundSMSAsReadAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, MarkAllInboundSMSAsReadResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_cancel_a_scheduled_message_async_with_message_id"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.updateCancelAScheduledMessageAsyncWithMessageId") updateCancelAScheduledMessageAsyncWithMessageId

> TODO: Add a method description


```objc
function updateCancelAScheduledMessageAsyncWithMessageId:(NSString*) messageId
                completionBlock:(CompletedPutCancelAScheduledMessage) onCompleted(messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | B7CE432193CD-0753597B7293 (string, required) - The message ID you want to cancel. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* messageId = @"307EF035";

    [self.sMS updateCancelAScheduledMessageAsyncWithMessageId: messageId  completionBlock:^(BOOL success, HttpContext* context, CancelAScheduledMessageResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_cancel_all_scheduled_messages_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.updateCancelAllScheduledMessagesWithCompletionBlock") updateCancelAllScheduledMessagesWithCompletionBlock

> TODO: Add a method description


```objc
function updateCancelAllScheduledMessagesWithCompletionBlock:(CompletedPutCancelAllScheduledMessages) onCompleted()
```



#### Example Usage

```objc

    [self.sMS updateCancelAllScheduledMessagesWithCompletionBlock:  ^(BOOL success, HttpContext* context, CancelAllScheduledMessagesResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="sms_campaigns_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SMSCampaignsController") SMSCampaignsController

### Get singleton instance
```objc
SMSCampaigns* sMSCampaigns = [[SMSCampaigns alloc]init] ;
```

### <a name="create_sms_campaign_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.createSMSCampaignAsyncWithBody") createSMSCampaignAsyncWithBody

> You can post to a list with **up to 20000 recipients** with each API call.


```objc
function createSMSCampaignAsyncWithBody:(CreateSMSCampaignRequest*) body
                completionBlock:(CompletedPostCreateSMSCampaign) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CreateSMSCampaignRequest* body = (CreateSMSCampaignRequest*) [APIHelper jsonDeserialize: @"{    \"list_id\":428,    \"name\":\"My Campaign 1\",    \"from\":\"+61353787448\",    \"body\":\"This is my new campaign message.\",    \"schedule\":1444821615}"
                toClass: CreateSMSCampaignRequest.class];

    [self.sMSCampaigns createSMSCampaignAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CreateSMSCampaignResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_calculate_price_for_sms_campaign_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.createCalculatePriceForSMSCampaignAsyncWithBody") createCalculatePriceForSMSCampaignAsyncWithBody

> TODO: Add a method description


```objc
function createCalculatePriceForSMSCampaignAsyncWithBody:(CalculatePriceForSMSCampaignRequest*) body
                completionBlock:(CompletedPostCalculatePriceForSMSCampaign) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CalculatePriceForSMSCampaignRequest* body = (CalculatePriceForSMSCampaignRequest*) [APIHelper jsonDeserialize: @"{    \"list_id\":428,    \"name\":\"My Campaign 1\",    \"from\":\"+61353787448\",    \"body\":\"(First Name), this is your new campaign message.\"}"
                toClass: CalculatePriceForSMSCampaignRequest.class];

    [self.sMSCampaigns createCalculatePriceForSMSCampaignAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CalculatePriceForSMSCampaignResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_an_sms_campaign_async_with_sms_campaign_id"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.updateAnSMSCampaignAsyncWithSmsCampaignId") updateAnSMSCampaignAsyncWithSmsCampaignId

> TODO: Add a method description


```objc
function updateAnSMSCampaignAsyncWithSmsCampaignId:(double) smsCampaignId
                body:(UpdateAnSMSCampaignRequest*) body
                completionBlock:(CompletedPutUpdateAnSMSCampaign) onCompleted(smsCampaignId body : body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| smsCampaignId |  ``` Required ```  | Your SMS Campaign id. |
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    double smsCampaignId = [@"1" doubleValue];
    UpdateAnSMSCampaignRequest* body = (UpdateAnSMSCampaignRequest*) [APIHelper jsonDeserialize: @"{    \"list_id\":428,    \"name\":\"Awesome campaign.\",    \"from\":\"+61353787447\",    \"body\":\"his is an awesome message.\",    \"schedule\":1444821615}"
                toClass: UpdateAnSMSCampaignRequest.class];

    [self.sMSCampaigns updateAnSMSCampaignAsyncWithSmsCampaignId: smsCampaignId body : body  completionBlock:^(BOOL success, HttpContext* context, UpdateAnSMSCampaignResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_sms_campaign_async_with_sms_campaign_id"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.getSMSCampaignAsyncWithSmsCampaignId") getSMSCampaignAsyncWithSmsCampaignId

> TODO: Add a method description


```objc
function getSMSCampaignAsyncWithSmsCampaignId:(double) smsCampaignId
                completionBlock:(CompletedGetSMSCampaign) onCompleted(smsCampaignId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| smsCampaignId |  ``` Required ```  | Your SMS campaign id. |





#### Example Usage

```objc
    // Parameters for the API call
    double smsCampaignId = [@"1" doubleValue];

    [self.sMSCampaigns getSMSCampaignAsyncWithSmsCampaignId: smsCampaignId  completionBlock:^(BOOL success, HttpContext* context, GetSMSCampaignResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_cancel_an_sms_campaign_async_with_sms_campaign_id"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.updateCancelAnSMSCampaignAsyncWithSmsCampaignId") updateCancelAnSMSCampaignAsyncWithSmsCampaignId

> TODO: Add a method description


```objc
function updateCancelAnSMSCampaignAsyncWithSmsCampaignId:(double) smsCampaignId
                completionBlock:(CompletedPutCancelAnSMSCampaign) onCompleted(smsCampaignId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| smsCampaignId |  ``` Required ```  | Your SMS Campaign id. |





#### Example Usage

```objc
    // Parameters for the API call
    double smsCampaignId = [@"1" doubleValue];

    [self.sMSCampaigns updateCancelAnSMSCampaignAsyncWithSmsCampaignId: smsCampaignId  completionBlock:^(BOOL success, HttpContext* context, CancelAnSMSCampaignResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_list_of_sms_campaigns_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.getListOfSMSCampaignsWithCompletionBlock") getListOfSMSCampaignsWithCompletionBlock

> TODO: Add a method description


```objc
function getListOfSMSCampaignsWithCompletionBlock:(CompletedGetListOfSMSCampaigns) onCompleted()
```



#### Example Usage

```objc

    [self.sMSCampaigns getListOfSMSCampaignsWithCompletionBlock:  ^(BOOL success, HttpContext* context, GetListOfSMSCampaignsResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="sms_templates_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SMSTemplatesController") SMSTemplatesController

### Get singleton instance
```objc
SMSTemplates* sMSTemplates = [[SMSTemplates alloc]init] ;
```

### <a name="list_of_templates_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".SMSTemplatesController.listOfTemplatesWithCompletionBlock") listOfTemplatesWithCompletionBlock

> Get list of templates.


```objc
function listOfTemplatesWithCompletionBlock:(CompletedGetListOfTemplates) onCompleted()
```



#### Example Usage

```objc

    [self.sMSTemplates listOfTemplatesWithCompletionBlock:  ^(BOOL success, HttpContext* context, ListOfTemplatesResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_a_template_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".SMSTemplatesController.createATemplateAsyncWithBody") createATemplateAsyncWithBody

> Create new template.


```objc
function createATemplateAsyncWithBody:(CreateATemplateRequest*) body
                completionBlock:(CompletedPostCreateATemplate) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CreateATemplateRequest* body = (CreateATemplateRequest*) [APIHelper jsonDeserialize: @"    {        \"template_name\":\"Template 501916\",        \"body\":\"This is a sample content: H7YI68B3yk for this template.\"    }"
                toClass: CreateATemplateRequest.class];

    [self.sMSTemplates createATemplateAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CreateATemplateResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_a_template_async_with_template_id"></a>![Method: ](https://apidocs.io/img/method.png ".SMSTemplatesController.updateATemplateAsyncWithTemplateId") updateATemplateAsyncWithTemplateId

> TODO: Add a method description


```objc
function updateATemplateAsyncWithTemplateId:(NSString*) templateId
                body:(UpdateATemplateRequest*) body
                completionBlock:(CompletedPutUpdateATemplate) onCompleted(templateId body : body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* templateId = @"25";
    UpdateATemplateRequest* body = (UpdateATemplateRequest*) [APIHelper jsonDeserialize: @"    {        \"template_name\":\"I am updated\",        \"body\":\"This is a sample content: Sc0KNWgSMG for this template.\"    }"
                toClass: UpdateATemplateRequest.class];

    [self.sMSTemplates updateATemplateAsyncWithTemplateId: templateId body : body  completionBlock:^(BOOL success, HttpContext* context, UpdateATemplateResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="delete_a_template_async_with_template_id"></a>![Method: ](https://apidocs.io/img/method.png ".SMSTemplatesController.deleteATemplateAsyncWithTemplateId") deleteATemplateAsyncWithTemplateId

> TODO: Add a method description


```objc
function deleteATemplateAsyncWithTemplateId:(NSString*) templateId
                completionBlock:(CompletedDeleteATemplate) onCompleted(templateId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* templateId = @"25";

    [self.sMSTemplates deleteATemplateAsyncWithTemplateId: templateId  completionBlock:^(BOOL success, HttpContext* context, DeleteATemplateResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="statistics_controller"></a>![Class: ](https://apidocs.io/img/class.png ".StatisticsController") StatisticsController

### Get singleton instance
```objc
Statistics* statistics = [[Statistics alloc]init] ;
```

### <a name="get_sms_statistics_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".StatisticsController.getSMSStatisticsWithCompletionBlock") getSMSStatisticsWithCompletionBlock

> TODO: Add a method description


```objc
function getSMSStatisticsWithCompletionBlock:(CompletedGetSMSStatistics) onCompleted()
```



#### Example Usage

```objc

    [self.statistics getSMSStatisticsWithCompletionBlock:  ^(BOOL success, HttpContext* context, GetSMSStatisticsResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_voice_statistics_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".StatisticsController.getVoiceStatisticsWithCompletionBlock") getVoiceStatisticsWithCompletionBlock

> TODO: Add a method description


```objc
function getVoiceStatisticsWithCompletionBlock:(CompletedGetVoiceStatistics) onCompleted()
```



#### Example Usage

```objc

    [self.statistics getVoiceStatisticsWithCompletionBlock:  ^(BOOL success, HttpContext* context, GetVoiceStatisticsResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="subaccounts_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SubaccountsController") SubaccountsController

### Get singleton instance
```objc
Subaccounts* subaccounts = [[Subaccounts alloc]init] ;
```

### <a name="get_all_subaccounts_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.getAllSubaccountsWithCompletionBlock") getAllSubaccountsWithCompletionBlock

> TODO: Add a method description


```objc
function getAllSubaccountsWithCompletionBlock:(CompletedGetAllSubaccounts) onCompleted()
```



#### Example Usage

```objc

    [self.subaccounts getAllSubaccountsWithCompletionBlock:  ^(BOOL success, HttpContext* context, GetAllSubaccountsResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_a_new_subaccount_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.createANewSubaccountAsyncWithBody") createANewSubaccountAsyncWithBody

> TODO: Add a method description


```objc
function createANewSubaccountAsyncWithBody:(CreateANewSubaccountRequest*) body
                completionBlock:(CompletedPostCreateANewSubaccount) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CreateANewSubaccountRequest* body = (CreateANewSubaccountRequest*) [APIHelper jsonDeserialize: @"    {        \"api_username\":\"nameP99\",        \"password\":\"pass\",        \"email\":\"testvrq@gmail.com\",        \"phone_number\":\"941-751-3278\",        \"first_name\":\"FirstnameeGPqV\",        \"last_name\":\"LastnamePvjJp\"    }"
                toClass: CreateANewSubaccountRequest.class];

    [self.subaccounts createANewSubaccountAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CreateANewSubaccountResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_a_specific_subaccount_async_with_subaccount_id"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.getASpecificSubaccountAsyncWithSubaccountId") getASpecificSubaccountAsyncWithSubaccountId

> TODO: Add a method description


```objc
function getASpecificSubaccountAsyncWithSubaccountId:(double) subaccountId
                completionBlock:(CompletedGetASpecificSubaccount) onCompleted(subaccountId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |





#### Example Usage

```objc
    // Parameters for the API call
    double subaccountId = [@"59" doubleValue];

    [self.subaccounts getASpecificSubaccountAsyncWithSubaccountId: subaccountId  completionBlock:^(BOOL success, HttpContext* context, GetASpecificSubaccountResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_a_specific_subaccount_async_with_subaccount_id"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.updateASpecificSubaccountAsyncWithSubaccountId") updateASpecificSubaccountAsyncWithSubaccountId

> TODO: Add a method description


```objc
function updateASpecificSubaccountAsyncWithSubaccountId:(double) subaccountId
                body:(UpdateASpecificSubaccountRequest*) body
                completionBlock:(CompletedPutUpdateASpecificSubaccount) onCompleted(subaccountId body : body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    double subaccountId = [@"59" doubleValue];
    UpdateASpecificSubaccountRequest* body = (UpdateASpecificSubaccountRequest*) [APIHelper jsonDeserialize: @"    {        \"password\":\"pass\",        \"email\":\"testfP0.updated@gmail.com\",        \"phone_number\":\"+19417519130\",        \"first_name\":\"FirstnameKvdRZUpdated\",        \"last_name\":\"LastnameHUPYGUpdated\",        \"access_users\": 1,        \"access_billing\": 1,        \"access_reporting\": 1,        \"access_contacts\": 1,        \"access_settings\": 1,        \"access_sms\": 1,        \"access_email\": 1,        \"access_voice\": 1,        \"access_fax\": 1,        \"access_post\": 1,        \"access_reseller\": 1,        \"access_mms\": 1,        \"share_campaigns\": 0,        \"notes\": null    }"
                toClass: UpdateASpecificSubaccountRequest.class];

    [self.subaccounts updateASpecificSubaccountAsyncWithSubaccountId: subaccountId body : body  completionBlock:^(BOOL success, HttpContext* context, UpdateASpecificSubaccountResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="delete_a_specific_subaccount_async_with_subaccount_id"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.deleteASpecificSubaccountAsyncWithSubaccountId") deleteASpecificSubaccountAsyncWithSubaccountId

> TODO: Add a method description


```objc
function deleteASpecificSubaccountAsyncWithSubaccountId:(double) subaccountId
                completionBlock:(CompletedDeleteASpecificSubaccount) onCompleted(subaccountId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |





#### Example Usage

```objc
    // Parameters for the API call
    double subaccountId = [@"59" doubleValue];

    [self.subaccounts deleteASpecificSubaccountAsyncWithSubaccountId: subaccountId  completionBlock:^(BOOL success, HttpContext* context, DeleteASpecificSubaccountResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_regenerate_api_key_async_with_subaccount_id"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.updateRegenerateAPIKeyAsyncWithSubaccountId") updateRegenerateAPIKeyAsyncWithSubaccountId

> TODO: Add a method description


```objc
function updateRegenerateAPIKeyAsyncWithSubaccountId:(double) subaccountId
                completionBlock:(CompletedPutRegenerateAPIKey) onCompleted(subaccountId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |





#### Example Usage

```objc
    // Parameters for the API call
    double subaccountId = [@"59" doubleValue];

    [self.subaccounts updateRegenerateAPIKeyAsyncWithSubaccountId: subaccountId  completionBlock:^(BOOL success, HttpContext* context, RegenerateAPIKeyResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="timezones_controller"></a>![Class: ](https://apidocs.io/img/class.png ".TimezonesController") TimezonesController

### Get singleton instance
```objc
Timezones* timezones = [[Timezones alloc]init] ;
```

### <a name="get_timezones_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".TimezonesController.getTimezonesWithCompletionBlock") getTimezonesWithCompletionBlock

> Get supported list of timezones.


```objc
function getTimezonesWithCompletionBlock:(CompletedGetTimezones) onCompleted()
```



#### Example Usage

```objc

    [self.timezones getTimezonesWithCompletionBlock:  ^(BOOL success, HttpContext* context, GetTimezonesResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="transactional_email_controller"></a>![Class: ](https://apidocs.io/img/class.png ".TransactionalEmailController") TransactionalEmailController

### Get singleton instance
```objc
TransactionalEmail* transactionalEmail = [[TransactionalEmail alloc]init] ;
```

### <a name="create_email_send_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".TransactionalEmailController.createEmailSendAsyncWithBody") createEmailSendAsyncWithBody

> TODO: Add a method description


```objc
function createEmailSendAsyncWithBody:(EmailSendRequest*) body
                completionBlock:(CompletedPostEmailSend) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    EmailSendRequest* body = [[EmailSendRequest alloc]init];

    [self.transactionalEmail createEmailSendAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, EmailSendResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_email_price_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".TransactionalEmailController.createEmailPriceAsyncWithBody") createEmailPriceAsyncWithBody

> TODO: Add a method description


```objc
function createEmailPriceAsyncWithBody:(EmailPriceRequest*) body
                completionBlock:(CompletedPostEmailPrice) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    EmailPriceRequest* body = [[EmailPriceRequest alloc]init];

    [self.transactionalEmail createEmailPriceAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, EmailPriceResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_email_history_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".TransactionalEmailController.getEmailHistoryWithCompletionBlock") getEmailHistoryWithCompletionBlock

> TODO: Add a method description


```objc
function getEmailHistoryWithCompletionBlock:(CompletedGetEmailHistory) onCompleted()
```



#### Example Usage

```objc

    [self.transactionalEmail getEmailHistoryWithCompletionBlock:  ^(BOOL success, HttpContext* context, EmailHistoryResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_export_history_async_with_filename"></a>![Method: ](https://apidocs.io/img/method.png ".TransactionalEmailController.getExportHistoryAsyncWithFilename") getExportHistoryAsyncWithFilename

> TODO: Add a method description


```objc
function getExportHistoryAsyncWithFilename:(NSString*) filename
                completionBlock:(CompletedGetExportHistory) onCompleted(filename)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | File name for the export file. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* filename = @"myexport.csv";

    [self.transactionalEmail getExportHistoryAsyncWithFilename: filename  completionBlock:^(BOOL success, HttpContext* context, ExportHistoryResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="add_a_test_delivery_receipt_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".TransactionalEmailController.addATestDeliveryReceiptAsyncWithBody") addATestDeliveryReceiptAsyncWithBody

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


```objc
function addATestDeliveryReceiptAsyncWithBody:(AddATestDeliveryReceiptRequest*) body
                completionBlock:(CompletedPostAddATestDeliveryReceipt) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    AddATestDeliveryReceiptRequest* body = (AddATestDeliveryReceiptRequest*) [APIHelper jsonDeserialize: @"    {        \"url\":\"http://yourUrl.com\"    }"
                toClass: AddATestDeliveryReceiptRequest.class];

    [self.transactionalEmail addATestDeliveryReceiptAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, AddATestDeliveryReceiptResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="uploads_controller"></a>![Class: ](https://apidocs.io/img/class.png ".UploadsController") UploadsController

### Get singleton instance
```objc
Uploads* uploads = [[Uploads alloc]init] ;
```

### <a name="upload_a_file_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".UploadsController.uploadAFileAsyncWithBody") uploadAFileAsyncWithBody

> The `upload` endpoint provides a method for converting files from an unspported format to a format that one of our endpoints can handle.
> Files can be submitted two ways:
> 1. Using `base64` encoding in an `application/json` request. In this case, submit the `base64`-encoded file contents in the `content` field of the request body, and `convert` can be specified either also in the body or as part of the query string.
> 2. Using `multipart/form-data` encoding, in the same way it would be submitted using a HTML form. You may find cURL useful for this. For an example of how to do this, see one of our [SDKs](https://dashboard.clicksend.com/#/libraries-sdk/main). In this case, specify `convert` in the query string.
> Note that `convert` specifies the conversion to take place - that is, what the result should be compatible with - and can be any of `fax`, `mms`, `csv` or `post`.
> All files have 10 minutes expiry.


```objc
function uploadAFileAsyncWithBody:(UploadAFileRequest*) body
                convert:(NSString*) convert
                completionBlock:(CompletedPostUploadAFile) onCompleted(body convert : convert)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |
| convert |  ``` Optional ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    UploadAFileRequest* body = [[UploadAFileRequest alloc]init];
    NSString* convert = @"convert";

    [self.uploads uploadAFileAsyncWithBody: body convert : convert  completionBlock:^(BOOL success, HttpContext* context, UploadAFileResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="voice_controller"></a>![Class: ](https://apidocs.io/img/class.png ".VoiceController") VoiceController

### Get singleton instance
```objc
Voice* voice = [[Voice alloc]init] ;
```

### <a name="create_send_a_voice_call_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.createSendAVoiceCallAsyncWithBody") createSendAVoiceCallAsyncWithBody

> You can post **up to 1000 messages** with each API call.


```objc
function createSendAVoiceCallAsyncWithBody:(SendAVoiceCallRequest*) body
                completionBlock:(CompletedPostSendAVoiceCall) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    SendAVoiceCallRequest* body = [[SendAVoiceCallRequest alloc]init];

    [self.voice createSendAVoiceCallAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, SendAVoiceCallResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="create_calculate_price_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.createCalculatePriceAsyncWithBody") createCalculatePriceAsyncWithBody

> TODO: Add a method description


```objc
function createCalculatePriceAsyncWithBody:(CalculatePriceRequest263*) body
                completionBlock:(CompletedPostCalculatePrice) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    CalculatePriceRequest263* body = [[CalculatePriceRequest263 alloc]init];

    [self.voice createCalculatePriceAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, CalculatePriceResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_voice_languages_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.getVoiceLanguagesWithCompletionBlock") getVoiceLanguagesWithCompletionBlock

> TODO: Add a method description


```objc
function getVoiceLanguagesWithCompletionBlock:(CompletedGetVoiceLanguages) onCompleted()
```



#### Example Usage

```objc

    [self.voice getVoiceLanguagesWithCompletionBlock:  ^(BOOL success, HttpContext* context, VoiceLanguagesResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_voice_history_async_with_date_from"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.getVoiceHistoryAsyncWithDateFrom") getVoiceHistoryAsyncWithDateFrom

> TODO: Add a method description


```objc
function getVoiceHistoryAsyncWithDateFrom:(NSNumber*) dateFrom
                dateTo:(NSNumber*) dateTo
                completionBlock:(CompletedGetVoiceHistory) onCompleted(dateFrom dateTo : dateTo)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateFrom |  ``` Optional ```  | Timestamp (from) used to show records by date. |
| dateTo |  ``` Optional ```  | Timestamp (to) used to show recrods by date. |





#### Example Usage

```objc
    // Parameters for the API call
    NSNumber* dateFrom = [NSNumber numberWithInteger:[@"1443501617" integerValue]];
    NSNumber* dateTo = [NSNumber numberWithInteger:[@"1443501727" integerValue]];

    [self.voice getVoiceHistoryAsyncWithDateFrom: dateFrom dateTo : dateTo  completionBlock:^(BOOL success, HttpContext* context, GetVoiceHistoryResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_export_voice_history_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.getExportVoiceHistoryWithCompletionBlock") getExportVoiceHistoryWithCompletionBlock

> TODO: Add a method description


```objc
function getExportVoiceHistoryWithCompletionBlock:(CompletedGetExportVoiceHistory) onCompleted()
```



#### Example Usage

```objc

    [self.voice getExportVoiceHistoryWithCompletionBlock:  ^(BOOL success, HttpContext* context, ExportVoiceHistoryResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_voice_receipts_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.getVoiceReceiptsWithCompletionBlock") getVoiceReceiptsWithCompletionBlock

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


```objc
function getVoiceReceiptsWithCompletionBlock:(CompletedGetVoiceReceipts) onCompleted()
```



#### Example Usage

```objc

    [self.voice getVoiceReceiptsWithCompletionBlock:  ^(BOOL success, HttpContext* context, GetVoiceReceiptsResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="add_a_test_delivery_receipt_async_with_body"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.addATestDeliveryReceiptAsyncWithBody") addATestDeliveryReceiptAsyncWithBody

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


```objc
function addATestDeliveryReceiptAsyncWithBody:(AddATestDeliveryReceiptRequest*) body
                completionBlock:(CompletedPostAddATestDeliveryReceipt) onCompleted(body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    AddATestDeliveryReceiptRequest* body = (AddATestDeliveryReceiptRequest*) [APIHelper jsonDeserialize: @"    {        \"url\":\"http://yourUrl.com\"    }"
                toClass: AddATestDeliveryReceiptRequest.class];

    [self.voice addATestDeliveryReceiptAsyncWithBody: body  completionBlock:^(BOOL success, HttpContext* context, AddATestDeliveryReceiptResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_specific_voice_receipt_async_with_message_id"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.getSpecificVoiceReceiptAsyncWithMessageId") getSpecificVoiceReceiptAsyncWithMessageId

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


```objc
function getSpecificVoiceReceiptAsyncWithMessageId:(NSString*) messageId
                completionBlock:(CompletedGetSpecificVoiceReceipt) onCompleted(messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | 3055-45F1-9B79-F2C43509FD16 (string, required) - The voice receipt message id. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* messageId = @"28DD2718";

    [self.voice getSpecificVoiceReceiptAsyncWithMessageId: messageId  completionBlock:^(BOOL success, HttpContext* context, GetSpecificVoiceReceiptResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_marked_voice_receipts_as_read_async_with_date_before"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.updateMarkedVoiceReceiptsAsReadAsyncWithDateBefore") updateMarkedVoiceReceiptsAsReadAsyncWithDateBefore

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


```objc
function updateMarkedVoiceReceiptsAsReadAsyncWithDateBefore:(double) dateBefore
                completionBlock:(CompletedPutMarkedVoiceReceiptsAsRead) onCompleted(dateBefore)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateBefore |  ``` Required ```  | An optional timestamp - mark all as read before this timestamp. If not given, all receipts will be marked as read. |





#### Example Usage

```objc
    // Parameters for the API call
    double dateBefore = 16.6672223511465;

    [self.voice updateMarkedVoiceReceiptsAsReadAsyncWithDateBefore: dateBefore  completionBlock:^(BOOL success, HttpContext* context, MarkedVoiceReceiptsAsReadResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_cancel_a_specific_voice_call_async_with_message_id"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.updateCancelASpecificVoiceCallAsyncWithMessageId") updateCancelASpecificVoiceCallAsyncWithMessageId

> TODO: Add a method description


```objc
function updateCancelASpecificVoiceCallAsyncWithMessageId:(NSString*) messageId
                completionBlock:(CompletedPutCancelASpecificVoiceCall) onCompleted(messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Your voice message id. |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* messageId = @"7B5BFC19 06B7 49C1 8DCDFB011600E12B";

    [self.voice updateCancelASpecificVoiceCallAsyncWithMessageId: messageId  completionBlock:^(BOOL success, HttpContext* context, CancelASpecificVoiceCallResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="update_cancel_all_voice_calls_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.updateCancelAllVoiceCallsWithCompletionBlock") updateCancelAllVoiceCallsWithCompletionBlock

> TODO: Add a method description


```objc
function updateCancelAllVoiceCallsWithCompletionBlock:(CompletedPutCancelAllVoiceCalls) onCompleted()
```



#### Example Usage

```objc

    [self.voice updateCancelAllVoiceCallsWithCompletionBlock:  ^(BOOL success, HttpContext* context, CancelAllVoiceCallsResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)



