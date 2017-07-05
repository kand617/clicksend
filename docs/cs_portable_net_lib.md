# Getting started

TODO: Add a description

## How to Build

The generated code uses a few NuGet Packages e.g., Newtonsoft.Json, UniRest,
and Microsoft Base Class Library. The reference to these packages is already
added as in the packages.config file. If the automatic NuGet package restore
is enabled, these dependencies will be installed automatically. Therefore,
you will need internet access for build.

1. Open the solution (ClickSendRESTAPIV3Tests.sln) file.
2. Invoke the build process using `Ctrl+Shift+B` shortcut key or using the `Build` menu as shown below.

![Building SDK using Visual Studio](https://apidocs.io/illustration/cs?step=buildSDK&workspaceFolder=ClickSend%20REST%20API%20v3-CSharp&workspaceName=ClickSendRESTAPIV3Tests&projectName=ClickSendRESTAPIV3.Tests)

## How to Use

The build process generates a portable class library, which can be used like a normal class library. The generated library is compatible with Windows Forms, Windows RT, Windows Phone 8,
Silverlight 5, Xamarin iOS, Xamarin Android and Mono. More information on how to use can be found at the [MSDN Portable Class Libraries documentation](http://msdn.microsoft.com/en-us/library/vstudio/gg597391%28v=vs.100%29.aspx).

The following section explains how to use the ClickSendRESTAPIV3Tests library in a new console project.

### 1. Starting a new project

For starting a new project, right click on the current solution from the *solution explorer* and choose  ``` Add -> New Project ```.

![Add a new project in the existing solution using Visual Studio](https://apidocs.io/illustration/cs?step=addProject&workspaceFolder=ClickSend%20REST%20API%20v3-CSharp&workspaceName=ClickSendRESTAPIV3Tests&projectName=ClickSendRESTAPIV3.Tests)

Next, choose "Console Application", provide a ``` TestConsoleProject ``` as the project name and click ``` OK ```.

![Create a new console project using Visual Studio](https://apidocs.io/illustration/cs?step=createProject&workspaceFolder=ClickSend%20REST%20API%20v3-CSharp&workspaceName=ClickSendRESTAPIV3Tests&projectName=ClickSendRESTAPIV3.Tests)

### 2. Set as startup project

The new console project is the entry point for the eventual execution. This requires us to set the ``` TestConsoleProject ``` as the start-up project. To do this, right-click on the  ``` TestConsoleProject ``` and choose  ``` Set as StartUp Project ``` form the context menu.

![Set the new cosole project as the start up project](https://apidocs.io/illustration/cs?step=setStartup&workspaceFolder=ClickSend%20REST%20API%20v3-CSharp&workspaceName=ClickSendRESTAPIV3Tests&projectName=ClickSendRESTAPIV3.Tests)

### 3. Add reference of the library project

In order to use the ClickSendRESTAPIV3Tests library in the new project, first we must add a projet reference to the ``` TestConsoleProject ```. First, right click on the ``` References ``` node in the *solution explorer* and click ``` Add Reference... ```.

![Open references of the TestConsoleProject](https://apidocs.io/illustration/cs?step=addReference&workspaceFolder=ClickSend%20REST%20API%20v3-CSharp&workspaceName=ClickSendRESTAPIV3Tests&projectName=ClickSendRESTAPIV3.Tests)

Next, a window will be displayed where we must set the ``` checkbox ``` on ``` ClickSendRESTAPIV3.Tests ``` and click ``` OK ```. By doing this, we have added a reference of the ```ClickSendRESTAPIV3.Tests``` project into the new ``` TestConsoleProject ```.

![Add a reference to the TestConsoleProject](https://apidocs.io/illustration/cs?step=createReference&workspaceFolder=ClickSend%20REST%20API%20v3-CSharp&workspaceName=ClickSendRESTAPIV3Tests&projectName=ClickSendRESTAPIV3.Tests)

### 4. Write sample code

Once the ``` TestConsoleProject ``` is created, a file named ``` Program.cs ``` will be visible in the *solution explorer* with an empty ``` Main ``` method. This is the entry point for the execution of the entire solution.
Here, you can add code to initialize the client library and acquire the instance of a *Controller* class. Sample code to initialize the client library and using controller methods is given in the subsequent sections.

![Add a reference to the TestConsoleProject](https://apidocs.io/illustration/cs?step=addCode&workspaceFolder=ClickSend%20REST%20API%20v3-CSharp&workspaceName=ClickSendRESTAPIV3Tests&projectName=ClickSendRESTAPIV3.Tests)

## How to Test

The generated SDK also contain one or more Tests, which are contained in the Tests project.
In order to invoke these test cases, you will need *NUnit 3.0 Test Adapter Extension for Visual Studio*.
Once the SDK is complied, the test cases should appear in the Test Explorer window.
Here, you can click *Run All* to execute these test cases.

## Initialization

### Authentication
In order to setup authentication and initialization of the API client, you need the following information.

| Parameter | Description |
|-----------|-------------|
| basicAuthUserName | The username to use with basic authentication |
| basicAuthPassword | The password to use with basic authentication |



API client can be initialized as following.

```csharp
// Configuration parameters and credentials
string basicAuthUserName = "basicAuthUserName"; // The username to use with basic authentication
string basicAuthPassword = "basicAuthPassword"; // The password to use with basic authentication

ClickSendRESTAPIV3TestsClient client = new ClickSendRESTAPIV3TestsClient(basicAuthUserName, basicAuthPassword);
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

## <a name="account_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.AccountController") AccountController

### Get singleton instance

The singleton instance of the ``` AccountController ``` class can be accessed from the API Client.

```csharp
AccountController account = client.Account;
```

### <a name="create_a_new_member"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AccountController.CreateANewMember") CreateANewMember

> **Note:** *Authentication isn't required to create a new account.*


```csharp
Task<CreateANewAccountResponse> CreateANewMember(CreateANewAccountRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new CreateANewAccountRequest();

CreateANewAccountResponse result = await account.CreateANewMember(body);

```


### <a name="update_account"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AccountController.UpdateAccount") UpdateAccount

> TODO: Add a method description


```csharp
Task<UpdateAccountResponse> UpdateAccount(UpdateAccountRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "    {        \"username\":\"johndoe\",        \"user_email\":\"johndoe@awesome.com\",        \"user_phone\":\"518-481-1002\",        \"user_first_name\":\"John\",        \"user_last_name\":\"Doe\",        \"country\":\"AU\",        \"password\":\"pass\",        \"account_name\":\"The Awesome Company\",        \"timezone\": \"Australia/Melbourne\",        \"private_uploads\": 1,        \"setting_sms_hide_your_number\": 0,        \"setting_sms_hide_business_name\": 1    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<UpdateAccountRequest>(bodyValue);

UpdateAccountResponse result = await account.UpdateAccount(body);

```


### <a name="get_account"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AccountController.GetAccount") GetAccount

> TODO: Add a method description


```csharp
Task<GetAccountResponse> GetAccount()
```

#### Example Usage

```csharp

GetAccountResponse result = await account.GetAccount();

```


### <a name="get_account_usage"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AccountController.GetAccountUsage") GetAccountUsage

> TODO: Add a method description


```csharp
Task<AccountUsageResponse> GetAccountUsage(double year, double month, string type)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| year |  ``` Required ```  | Your account usage year. |
| month |  ``` Required ```  | Your account usage month. |
| type |  ``` Required ```  | The account type. Value can only be either email or subaccount. |


#### Example Usage

```csharp
double year = 2016;
double month = 4;
string type = "subaccount";

AccountUsageResponse result = await account.GetAccountUsage(year, month, type);

```


### <a name="update_send_account_activation_token"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AccountController.UpdateSendAccountActivationToken") UpdateSendAccountActivationToken

> TODO: Add a method description


```csharp
Task<SendAccountActivationTokenResponse> UpdateSendAccountActivationToken(SendAccountActivationTokenRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "    {        \"user_phone\":\"352-394-4199\",        \"type\":\"sms\",        \"country\": \"US\"    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<SendAccountActivationTokenRequest>(bodyValue);

SendAccountActivationTokenResponse result = await account.UpdateSendAccountActivationToken(body);

```


### <a name="update_verify_new_account"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AccountController.UpdateVerifyNewAccount") UpdateVerifyNewAccount

> TODO: Add a method description


```csharp
Task<VerifyNewAccountResponse> UpdateVerifyNewAccount(string activationToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| activationToken |  ``` Required ```  | The ActivationToken to be used to verify an account. |


#### Example Usage

```csharp
string activationToken = "1827364";

VerifyNewAccountResponse result = await account.UpdateVerifyNewAccount(activationToken);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="account_recharge_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.AccountRechargeController") AccountRechargeController

### Get singleton instance

The singleton instance of the ``` AccountRechargeController ``` class can be accessed from the API Client.

```csharp
AccountRechargeController accountRecharge = client.AccountRecharge;
```

### <a name="get_credit_card_info"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AccountRechargeController.GetCreditCardInfo") GetCreditCardInfo

> TODO: Add a method description


```csharp
Task<GetCreditCardInfoResponse> GetCreditCardInfo()
```

#### Example Usage

```csharp

GetCreditCardInfoResponse result = await accountRecharge.GetCreditCardInfo();

```


### <a name="update_credit_card_info"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AccountRechargeController.UpdateCreditCardInfo") UpdateCreditCardInfo

> TODO: Add a method description


```csharp
Task<UpdateCreditCardInfoResponse> UpdateCreditCardInfo(UpdateCreditCardInfoRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new UpdateCreditCardInfoRequest();

UpdateCreditCardInfoResponse result = await accountRecharge.UpdateCreditCardInfo(body);

```


### <a name="list_of_packages"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AccountRechargeController.ListOfPackages") ListOfPackages

> TODO: Add a method description


```csharp
Task<ListOfPackagesResponse> ListOfPackages(string country = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Optional ```  | Your country. |


#### Example Usage

```csharp
string country = "\"AU\"";

ListOfPackagesResponse result = await accountRecharge.ListOfPackages(country);

```


### <a name="update_purchase_a_package"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AccountRechargeController.UpdatePurchaseAPackage") UpdatePurchaseAPackage

> TODO: Add a method description


```csharp
Task<PurchaseAPackageResponse> UpdatePurchaseAPackage(double packageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| packageId |  ``` Required ```  | Your package id. |


#### Example Usage

```csharp
double packageId = 1;

PurchaseAPackageResponse result = await accountRecharge.UpdatePurchaseAPackage(packageId);

```


### <a name="get_transactions"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AccountRechargeController.GetTransactions") GetTransactions

> TODO: Add a method description


```csharp
Task<GetTransactionsResponse> GetTransactions()
```

#### Example Usage

```csharp

GetTransactionsResponse result = await accountRecharge.GetTransactions();

```


### <a name="get_a_specific_transaction"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AccountRechargeController.GetASpecificTransaction") GetASpecificTransaction

> TODO: Add a method description


```csharp
Task<Stream> GetASpecificTransaction(string transactionId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| transactionId |  ``` Required ```  | 1c65-47fa-aea2-3ded9ed57557 (number, required) - Your transction id. |


#### Example Usage

```csharp
string transactionId = "transaction_id";

Stream result = await accountRecharge.GetASpecificTransaction(transactionId);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="automation_rules_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController") AutomationRulesController

### Get singleton instance

The singleton instance of the ``` AutomationRulesController ``` class can be accessed from the API Client.

```csharp
AutomationRulesController automationRules = client.AutomationRules;
```

### <a name="list_rules"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.ListRules") ListRules

> TODO: Add a method description


```csharp
Task<ListRulesResponse> ListRules()
```

#### Example Usage

```csharp

ListRulesResponse result = await automationRules.ListRules();

```


### <a name="get_a_specific_rule"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.GetASpecificRule") GetASpecificRule

> TODO: Add a method description


```csharp
Task<GetASpecificRuleResponse> GetASpecificRule(double inboundRuleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Inbound Rule ID. |


#### Example Usage

```csharp
double inboundRuleId = 1;

GetASpecificRuleResponse result = await automationRules.GetASpecificRule(inboundRuleId);

```


### <a name="create_a_new_rule"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.CreateANewRule") CreateANewRule

> TODO: Add a method description


```csharp
Task<CreateANewRuleResponse> CreateANewRule(CreateANewRuleRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new CreateANewRuleRequest();

CreateANewRuleResponse result = await automationRules.CreateANewRule(body);

```


### <a name="update_a_rule"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.UpdateARule") UpdateARule

> TODO: Add a method description


```csharp
Task<UpdateARuleResponse> UpdateARule(double inboundRuleId, UpdateARuleRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Inbound Rule ID. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
double inboundRuleId = 1;
string bodyValue = "{    \"dedicated_number\":\"+61298441484\",    \"rule_name\":\"My Rule\",    \"message_search_type\":3,    \"message_search_term\":\"My Search Term\",    \"action\":\"EMAIL_FIXED\",    \"action_address\":\"john@doe.com\",    \"enabled\":1}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<UpdateARuleRequest>(bodyValue);

UpdateARuleResponse result = await automationRules.UpdateARule(inboundRuleId, body);

```


### <a name="delete_a_rule"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.DeleteARule") DeleteARule

> TODO: Add a method description


```csharp
Task<DeleteARuleResponse> DeleteARule(double inboundRuleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Inbound Rule ID. |


#### Example Usage

```csharp
double inboundRuleId = 1;

DeleteARuleResponse result = await automationRules.DeleteARule(inboundRuleId);

```


### <a name="list_rules1"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.ListRules1") ListRules1

> TODO: Add a method description


```csharp
Task<ListRulesResponse> ListRules1()
```

#### Example Usage

```csharp

ListRulesResponse result = await automationRules.ListRules1();

```


### <a name="get_a_specific_rule1"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.GetASpecificRule1") GetASpecificRule1

> TODO: Add a method description


```csharp
Task<GetASpecificRuleResponse> GetASpecificRule1(double receiptRuleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |


#### Example Usage

```csharp
double receiptRuleId = 2;

GetASpecificRuleResponse result = await automationRules.GetASpecificRule1(receiptRuleId);

```


### <a name="create_a_new_rule1"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.CreateANewRule1") CreateANewRule1

> TODO: Add a method description


```csharp
Task<CreateANewRuleResponse> CreateANewRule1(CreateANewRuleRequest24 body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "{    \"rule_name\": \"My Rule\",    \"match_type\": 3,    \"action\": \"EMAIL_FIXED\",    \"action_address\": \"john@doe.com\",    \"enabled\": 1}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<CreateANewRuleRequest24>(bodyValue);

CreateANewRuleResponse result = await automationRules.CreateANewRule1(body);

```


### <a name="update_a_rule1"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.UpdateARule1") UpdateARule1

> TODO: Add a method description


```csharp
Task<UpdateARuleResponse> UpdateARule1(double receiptRuleId, UpdateARuleRequest26 body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
double receiptRuleId = 7;
string bodyValue = "{    \"rule_name\": \"My Rule\",    \"match_type\": 3,    \"action\": \"EMAIL_FIXED\",    \"action_address\": \"john@doe.com\",    \"enabled\": 1}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<UpdateARuleRequest26>(bodyValue);

UpdateARuleResponse result = await automationRules.UpdateARule1(receiptRuleId, body);

```


### <a name="delete_a_rule1"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.DeleteARule1") DeleteARule1

> TODO: Add a method description


```csharp
Task<DeleteARuleResponse> DeleteARule1(double receiptRuleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |


#### Example Usage

```csharp
double receiptRuleId = 7;

DeleteARuleResponse result = await automationRules.DeleteARule1(receiptRuleId);

```


### <a name="list_rules2"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.ListRules2") ListRules2

> TODO: Add a method description


```csharp
Task<ListRulesResponse> ListRules2()
```

#### Example Usage

```csharp

ListRulesResponse result = await automationRules.ListRules2();

```


### <a name="get_a_specific_rule1"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.GetASpecificRule1") GetASpecificRule1

> TODO: Add a method description


```csharp
Task<GetASpecificRuleResponse> GetASpecificRule1(double receiptRuleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |


#### Example Usage

```csharp
double receiptRuleId = 2;

GetASpecificRuleResponse result = await automationRules.GetASpecificRule1(receiptRuleId);

```


### <a name="create_a_new_rule2"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.CreateANewRule2") CreateANewRule2

> TODO: Add a method description


```csharp
Task<CreateANewRuleResponse> CreateANewRule2(CreateANewRuleRequest24 body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "{    \"rule_name\":\"My Rule\",    \"match_type\":3,    \"action\":\"EMAIL_FIXED\",    \"action_address\":\"john@doe.com\",    \"enabled\":1}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<CreateANewRuleRequest24>(bodyValue);

CreateANewRuleResponse result = await automationRules.CreateANewRule2(body);

```


### <a name="update_a_rule1"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.UpdateARule1") UpdateARule1

> TODO: Add a method description


```csharp
Task<UpdateARuleResponse> UpdateARule1(double receiptRuleId, UpdateARuleRequest26 body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
double receiptRuleId = 2;
string bodyValue = "{    \"rule_name\":\"My Rule\",    \"match_type\":3,    \"action\":\"EMAIL_FIXED\",    \"action_address\":\"john@doe.com\",    \"enabled\":1}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<UpdateARuleRequest26>(bodyValue);

UpdateARuleResponse result = await automationRules.UpdateARule1(receiptRuleId, body);

```


### <a name="delete_a_rule1"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.DeleteARule1") DeleteARule1

> TODO: Add a method description


```csharp
Task<DeleteARuleResponse> DeleteARule1(double receiptRuleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |


#### Example Usage

```csharp
double receiptRuleId = 2;

DeleteARuleResponse result = await automationRules.DeleteARule1(receiptRuleId);

```


### <a name="list_rules3"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.ListRules3") ListRules3

> TODO: Add a method description


```csharp
Task<ListRulesResponse> ListRules3()
```

#### Example Usage

```csharp

ListRulesResponse result = await automationRules.ListRules3();

```


### <a name="get_a_specific_rule11"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.GetASpecificRule11") GetASpecificRule11

> TODO: Add a method description


```csharp
Task<GetASpecificRuleResponse> GetASpecificRule11(double inboundRuleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Fax inbound rule id |


#### Example Usage

```csharp
double inboundRuleId = 14;

GetASpecificRuleResponse result = await automationRules.GetASpecificRule11(inboundRuleId);

```


### <a name="create_a_new_rule3"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.CreateANewRule3") CreateANewRule3

> TODO: Add a method description


```csharp
Task<CreateANewRuleResponse> CreateANewRule3(CreateANewRuleRequest38 body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "    {        \"dedicated_number\":\"+61298441484\",        \"rule_name\":\"Rule Name\",        \"action\":\"EMAIL_FIXED\",        \"action_address\":\"email@domain.com\",        \"enabled\":1    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<CreateANewRuleRequest38>(bodyValue);

CreateANewRuleResponse result = await automationRules.CreateANewRule3(body);

```


### <a name="update_a_rule11"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.UpdateARule11") UpdateARule11

> TODO: Add a method description


```csharp
Task<UpdateARuleResponse> UpdateARule11(double inboundRuleId, UpdateARuleRequest40 body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Fax inbound rule id |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
double inboundRuleId = 14;
string bodyValue = "    {        \"dedicated_number\":\"+61298441484\",        \"rule_name\":\"Rule Name\",        \"action\":\"EMAIL_FIXED\",        \"action_address\":\"email@domain.com\",        \"enabled\":1    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<UpdateARuleRequest40>(bodyValue);

UpdateARuleResponse result = await automationRules.UpdateARule11(inboundRuleId, body);

```


### <a name="delete_a_rule11"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.DeleteARule11") DeleteARule11

> TODO: Add a method description


```csharp
Task<DeleteARuleResponse> DeleteARule11(double inboundRuleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Fax inbound rule id |


#### Example Usage

```csharp
double inboundRuleId = 14;

DeleteARuleResponse result = await automationRules.DeleteARule11(inboundRuleId);

```


### <a name="list_rules4"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.ListRules4") ListRules4

> TODO: Add a method description


```csharp
Task<ListRulesResponse> ListRules4()
```

#### Example Usage

```csharp

ListRulesResponse result = await automationRules.ListRules4();

```


### <a name="get_a_specific_rule2"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.GetASpecificRule2") GetASpecificRule2

> TODO: Add a method description


```csharp
Task<GetASpecificRuleResponse> GetASpecificRule2(double ruleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |


#### Example Usage

```csharp
double ruleId = 4;

GetASpecificRuleResponse result = await automationRules.GetASpecificRule2(ruleId);

```


### <a name="create_a_new_rule4"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.CreateANewRule4") CreateANewRule4

> TODO: Add a method description


```csharp
Task<CreateANewRuleResponse> CreateANewRule4(CreateANewRuleRequest24 body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "    {        \"rule_name\":\"My Rule\",        \"match_type\":2,        \"action\":\"EMAIL_FIXED\",        \"action_address\":\"john@doe.com\",        \"enabled\":1    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<CreateANewRuleRequest24>(bodyValue);

CreateANewRuleResponse result = await automationRules.CreateANewRule4(body);

```


### <a name="update_a_rule2"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.UpdateARule2") UpdateARule2

> TODO: Add a method description


```csharp
Task<UpdateARuleResponse> UpdateARule2(double ruleId, UpdateARuleRequest26 body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
double ruleId = 4;
string bodyValue = "    {        \"rule_name\":\"My Rule\",        \"match_type\":1,        \"action\":\"EMAIL_FIXED\",        \"action_address\":\"john@doe.com\",        \"enabled\":1    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<UpdateARuleRequest26>(bodyValue);

UpdateARuleResponse result = await automationRules.UpdateARule2(ruleId, body);

```


### <a name="delete_a_rule2"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.DeleteARule2") DeleteARule2

> TODO: Add a method description


```csharp
Task<DeleteARuleResponse49> DeleteARule2(double ruleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to delete. |


#### Example Usage

```csharp
double ruleId = 100.923311291692;

DeleteARuleResponse49 result = await automationRules.DeleteARule2(ruleId);

```


### <a name="list_rules5"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.ListRules5") ListRules5

> TODO: Add a method description


```csharp
Task<ListRulesResponse> ListRules5()
```

#### Example Usage

```csharp

ListRulesResponse result = await automationRules.ListRules5();

```


### <a name="get_a_specific_rule12"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.GetASpecificRule12") GetASpecificRule12

> TODO: Add a method description


```csharp
Task<GetASpecificRuleResponse> GetASpecificRule12(double ruleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |


#### Example Usage

```csharp
double ruleId = 5;

GetASpecificRuleResponse result = await automationRules.GetASpecificRule12(ruleId);

```


### <a name="create_a_new_rule5"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.CreateANewRule5") CreateANewRule5

> TODO: Add a method description


```csharp
Task<CreateANewRuleResponse> CreateANewRule5(CreateANewRuleRequest24 body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "    {        \"rule_name\":\"My Rule\",        \"match_type\": 0,        \"action\":\"URL\",        \"action_address\":\"http://testurl.com\",        \"enabled\":1    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<CreateANewRuleRequest24>(bodyValue);

CreateANewRuleResponse result = await automationRules.CreateANewRule5(body);

```


### <a name="update_a_rule12"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.UpdateARule12") UpdateARule12

> TODO: Add a method description


```csharp
Task<UpdateARuleResponse> UpdateARule12(double ruleId, UpdateARuleRequest26 body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
double ruleId = 8;
string bodyValue = "    {        \"rule_name\":\"My Rule\",        \"match_type\": 0,        \"action\":\"URL\",        \"action_address\":\"http://testurl.com\",        \"enabled\":1    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<UpdateARuleRequest26>(bodyValue);

UpdateARuleResponse result = await automationRules.UpdateARule12(ruleId, body);

```


### <a name="delete_a_rule12"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.AutomationRulesController.DeleteARule12") DeleteARule12

> TODO: Add a method description


```csharp
Task<DeleteARuleResponse56> DeleteARule12(double ruleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to delete. |


#### Example Usage

```csharp
double ruleId = 8;

DeleteARuleResponse56 result = await automationRules.DeleteARule12(ruleId);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="contact_lists_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.ContactListsController") ContactListsController

### Get singleton instance

The singleton instance of the ``` ContactListsController ``` class can be accessed from the API Client.

```csharp
ContactListsController contactLists = client.ContactLists;
```

### <a name="get_all_contact_lists"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ContactListsController.GetAllContactLists") GetAllContactLists

> TODO: Add a method description


```csharp
Task<GetAllContactListsResponse> GetAllContactLists()
```

#### Example Usage

```csharp

GetAllContactListsResponse result = await contactLists.GetAllContactLists();

```


### <a name="create_a_new_contact_list"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ContactListsController.CreateANewContactList") CreateANewContactList

> TODO: Add a method description


```csharp
Task<CreateANewContactListResponse> CreateANewContactList(CreateANewContactListRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "    {        \"list_name\":\"ListCT3QrVL4od\"    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<CreateANewContactListRequest>(bodyValue);

CreateANewContactListResponse result = await contactLists.CreateANewContactList(body);

```


### <a name="get_a_specific_contact_list"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ContactListsController.GetASpecificContactList") GetASpecificContactList

> TODO: Add a method description


```csharp
Task<GetASpecificContactListResponse> GetASpecificContactList(double listId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |


#### Example Usage

```csharp
double listId = 437;

GetASpecificContactListResponse result = await contactLists.GetASpecificContactList(listId);

```


### <a name="update_a_specific_contact_list"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ContactListsController.UpdateASpecificContactList") UpdateASpecificContactList

> TODO: Add a method description


```csharp
Task<UpdateASpecificContactListResponse> UpdateASpecificContactList(double listId, UpdateASpecificContactListRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
double listId = 439;
string bodyValue = "    {        \"list_name\":\"ListlPJf33ksjP\"    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<UpdateASpecificContactListRequest>(bodyValue);

UpdateASpecificContactListResponse result = await contactLists.UpdateASpecificContactList(listId, body);

```


### <a name="delete_a_specific_contact_list"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ContactListsController.DeleteASpecificContactList") DeleteASpecificContactList

> TODO: Add a method description


```csharp
Task<DeleteASpecificContactListResponse> DeleteASpecificContactList(double listId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |


#### Example Usage

```csharp
double listId = 442;

DeleteASpecificContactListResponse result = await contactLists.DeleteASpecificContactList(listId);

```


### <a name="create_import_contacts_to_list"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ContactListsController.CreateImportContactsToList") CreateImportContactsToList

> TODO: Add a method description


```csharp
Task<ImportContactsToListResponse> CreateImportContactsToList(double listId, ImportContactsToListRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
double listId = 437;
string bodyValue = "{    \"file_url\":\"http://yourdomain.com/5485EA6144/79E8/import.csv\",    \"field_order\":[        \"phone\",        \"first_name\",        \"last_name\",        \"custom1\",        \"custom2\",        \"custom3\",        \"custom4\",        \"fax_number\",        \"organization_name\",        \"email\",        \"address_line_1\",        \"address_line_2\",        \"address_city\",        \"address_state\",        \"address_postal_code\",        \"address_country\"    ]}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<ImportContactsToListRequest>(bodyValue);

ImportContactsToListResponse result = await contactLists.CreateImportContactsToList(listId, body);

```


### <a name="update_remove_duplicate_contacts"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ContactListsController.UpdateRemoveDuplicateContacts") UpdateRemoveDuplicateContacts

> TODO: Add a method description


```csharp
Task<RemoveDuplicateContactsResponse> UpdateRemoveDuplicateContacts(double listId, RemoveDuplicateContactsRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
double listId = 439;
string bodyValue = "{    \"fields\":[        \"phone_number\",        \"first_name\",        \"last_name\",        \"fax_number\",        \"address_country\"    ]}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<RemoveDuplicateContactsRequest>(bodyValue);

RemoveDuplicateContactsResponse result = await contactLists.UpdateRemoveDuplicateContacts(listId, body);

```


### <a name="get_list_of_acceptable_import_fields"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ContactListsController.GetListOfAcceptableImportFields") GetListOfAcceptableImportFields

> TODO: Add a method description


```csharp
Task<GetListOfAcceptableImportFieldsResponse> GetListOfAcceptableImportFields(string listId = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Optional ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string listId = "list_id";

GetListOfAcceptableImportFieldsResponse result = await contactLists.GetListOfAcceptableImportFields(listId);

```


### <a name="create_show_csv_import_file_preview"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ContactListsController.CreateShowCSVImportFilePreview") CreateShowCSVImportFilePreview

> Show first row of the csv import file.


```csharp
Task<ShowCSVImportFilePreviewResponse> CreateShowCSVImportFilePreview(double listId, ShowCSVImportFilePreviewRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
double listId = 439;
string bodyValue = "{    \"file_url\":\"http://yourdomain.com/5485EA6144/79E8/import.csv\"}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<ShowCSVImportFilePreviewRequest>(bodyValue);

ShowCSVImportFilePreviewResponse result = await contactLists.CreateShowCSVImportFilePreview(listId, body);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="contact_suggestions_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.ContactSuggestionsController") ContactSuggestionsController

### Get singleton instance

The singleton instance of the ``` ContactSuggestionsController ``` class can be accessed from the API Client.

```csharp
ContactSuggestionsController contactSuggestions = client.ContactSuggestions;
```

### <a name="list_contact_suggestions"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ContactSuggestionsController.ListContactSuggestions") ListContactSuggestions

> TODO: Add a method description


```csharp
Task<ListContactSuggestionsResponse> ListContactSuggestions()
```

#### Example Usage

```csharp

ListContactSuggestionsResponse result = await contactSuggestions.ListContactSuggestions();

```


[Back to List of Controllers](#list_of_controllers)

## <a name="contacts_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.ContactsController") ContactsController

### Get singleton instance

The singleton instance of the ``` ContactsController ``` class can be accessed from the API Client.

```csharp
ContactsController contacts = client.Contacts;
```

### <a name="get_all_contacts_in_a_list"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ContactsController.GetAllContactsInAList") GetAllContactsInAList

> TODO: Add a method description


```csharp
Task<GetAllContactsInAListResponse> GetAllContactsInAList(double listId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id where your contacts belong. |


#### Example Usage

```csharp
double listId = 428;

GetAllContactsInAListResponse result = await contacts.GetAllContactsInAList(listId);

```


### <a name="create_a_new_contact"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ContactsController.CreateANewContact") CreateANewContact

> TODO: Add a method description


```csharp
Task<CreateANewContactResponse> CreateANewContact(double listId, CreateANewContactRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id where your contact be associated. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
double listId = 428;
string bodyValue = "    {        \"phone_number\":\"+16783270696\",        \"first_name\":\"Ellen\",        \"last_name\":\"Diaz\",        \"custom_1\":\"Custom 1\",        \"custom_2\":\"Custom 2\",        \"custom_3\":\"Custom 3\",        \"custom_4\":\"Custom 4\",        \"fax_number\":\"+16783270696\",        \"organization_name\":\"Awesome Organization\",        \"email\":\"ellen@diaz.com\",        \"address_line_1\":\"Block 2\",        \"address_line_2\":\"Cool Bldg.\",        \"address_city\":\"Nevada\",        \"address_state\":\"Las Vegas\",        \"address_postal_code\":\"36063\",        \"address_country\":\"US\"    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<CreateANewContactRequest>(bodyValue);

CreateANewContactResponse result = await contacts.CreateANewContact(listId, body);

```


### <a name="get_a_specific_contact"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ContactsController.GetASpecificContact") GetASpecificContact

> TODO: Add a method description


```csharp
Task<GetASpecificContactResponse> GetASpecificContact(double listId, double contactId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| contactId |  ``` Required ```  | Your contact id you want to access. |


#### Example Usage

```csharp
double listId = 428;
double contactId = 552802;

GetASpecificContactResponse result = await contacts.GetASpecificContact(listId, contactId);

```


### <a name="update_a_specific_contact"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ContactsController.UpdateASpecificContact") UpdateASpecificContact

> TODO: Add a method description


```csharp
Task<UpdateASpecificContactResponse> UpdateASpecificContact(double listId, double contactId, UpdateASpecificContactRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| contactId |  ``` Required ```  | Your contact id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
double listId = 428;
double contactId = 552802;
string bodyValue = "{        \"phone_number\":\"+16783275492\",        \"first_name\":\"Ellen\",        \"last_name\":\"Diaz\",        \"custom_1\":\"Custom S72oJ9Teba\",        \"custom_2\":\"Custom NvrRJrKWeq\",        \"custom_3\":\"Custom 2ws94p1Dop\",        \"custom_4\":\"Custom Ku0AaIS5xb\",        \"fax_number\":\"+16783276356\",        \"organization_name\":\"Awesome Organization\",        \"email\":\"ellen@diaz.com\",        \"address_line_1\":\"Block 6\",        \"address_line_2\":\"Cool Bldg.\",        \"address_city\":\"Nevada\",        \"address_state\":\"Las Vegas\",        \"address_postal_code\":\"36063\",        \"address_country\":\"US\"    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<UpdateASpecificContactRequest>(bodyValue);

UpdateASpecificContactResponse result = await contacts.UpdateASpecificContact(listId, contactId, body);

```


### <a name="delete_a_specific_contact"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ContactsController.DeleteASpecificContact") DeleteASpecificContact

> TODO: Add a method description


```csharp
Task<DeleteASpecificContactResponse> DeleteASpecificContact(double listId, double contactId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| contactId |  ``` Required ```  | Your contact id you want to access. |


#### Example Usage

```csharp
double listId = 428;
double contactId = 552807;

DeleteASpecificContactResponse result = await contacts.DeleteASpecificContact(listId, contactId);

```


### <a name="update_remove_opted_out_contacts"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ContactsController.UpdateRemoveOptedOutContacts") UpdateRemoveOptedOutContacts

> TODO: Add a method description


```csharp
Task<RemoveOptedOutContactsResponse> UpdateRemoveOptedOutContacts(double listId, double optOutListId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id. |
| optOutListId |  ``` Required ```  | Your opt out list id. |


#### Example Usage

```csharp
double listId = 439;
double optOutListId = 512;

RemoveOptedOutContactsResponse result = await contacts.UpdateRemoveOptedOutContacts(listId, optOutListId);

```


### <a name="update_transfer_a_contact"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ContactsController.UpdateTransferAContact") UpdateTransferAContact

> Transfers a specific contact to another list.


```csharp
Task<TransferAContactResponse> UpdateTransferAContact(double fromListId, double contactId, double toListId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| fromListId |  ``` Required ```  | From list id. |
| contactId |  ``` Required ```  | Contact ID. |
| toListId |  ``` Required ```  | To list id. |


#### Example Usage

```csharp
double fromListId = 428;
double contactId = 1;
double toListId = 429;

TransferAContactResponse result = await contacts.UpdateTransferAContact(fromListId, contactId, toListId);

```


### <a name="get_hello_contact"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ContactsController.GetHelloContact") GetHelloContact

> TODO: Add a method description


```csharp
Task GetHelloContact()
```

#### Example Usage

```csharp

await contacts.GetHelloContact();

```


[Back to List of Controllers](#list_of_controllers)

## <a name="countries_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.CountriesController") CountriesController

### Get singleton instance

The singleton instance of the ``` CountriesController ``` class can be accessed from the API Client.

```csharp
CountriesController countries = client.Countries;
```

### <a name="get_all_countries"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.CountriesController.GetAllCountries") GetAllCountries

> TODO: Add a method description


```csharp
Task<GetAllCountriesResponse> GetAllCountries()
```

#### Example Usage

```csharp

GetAllCountriesResponse result = await countries.GetAllCountries();

```


[Back to List of Controllers](#list_of_controllers)

## <a name="delivery_issues_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.DeliveryIssuesController") DeliveryIssuesController

### Get singleton instance

The singleton instance of the ``` DeliveryIssuesController ``` class can be accessed from the API Client.

```csharp
DeliveryIssuesController deliveryIssues = client.DeliveryIssues;
```

### <a name="get_delivery_issues"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.DeliveryIssuesController.GetDeliveryIssues") GetDeliveryIssues

> TODO: Add a method description


```csharp
Task<GetDeliveryIssuesResponse> GetDeliveryIssues()
```

#### Example Usage

```csharp

GetDeliveryIssuesResponse result = await deliveryIssues.GetDeliveryIssues();

```


### <a name="create_delivery_issue"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.DeliveryIssuesController.CreateDeliveryIssue") CreateDeliveryIssue

> TODO: Add a method description


```csharp
Task<CreateDeliveryIssueResponse> CreateDeliveryIssue(CreateDeliveryIssueRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "{  \"message_id\": \"B388828B\",  \"type\": \"SMS\",  \"description\": \"This is a test\",  \"client_comments\": \"test\",  \"email_address: john_doe@user.com\": \"\",  \"Body\": \"\"}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<CreateDeliveryIssueRequest>(bodyValue);

CreateDeliveryIssueResponse result = await deliveryIssues.CreateDeliveryIssue(body);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="email_marketing_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.EmailMarketingController") EmailMarketingController

### Get singleton instance

The singleton instance of the ``` EmailMarketingController ``` class can be accessed from the API Client.

```csharp
EmailMarketingController emailMarketing = client.EmailMarketing;
```

### <a name="get_all_allowed_email_addresses"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailMarketingController.GetAllAllowedEmailAddresses") GetAllAllowedEmailAddresses

> TODO: Add a method description


```csharp
Task<GetAllAllowedEmailAddressesResponse> GetAllAllowedEmailAddresses()
```

#### Example Usage

```csharp

GetAllAllowedEmailAddressesResponse result = await emailMarketing.GetAllAllowedEmailAddresses();

```


### <a name="create_allowed_email_address"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailMarketingController.CreateAllowedEmailAddress") CreateAllowedEmailAddress

> TODO: Add a method description


```csharp
Task<CreateAllowedEmailAddressResponse> CreateAllowedEmailAddress(CreateAllowedEmailAddressRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "{  \"email_address\": \"johndoe1@user.com\",  \"Body\": \"\"}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<CreateAllowedEmailAddressRequest>(bodyValue);

CreateAllowedEmailAddressResponse result = await emailMarketing.CreateAllowedEmailAddress(body);

```


### <a name="update_send_verification_token"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailMarketingController.UpdateSendVerificationToken") UpdateSendVerificationToken

> TODO: Add a method description


```csharp
Task<SendVerificationTokenResponse> UpdateSendVerificationToken(double emailAddressId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email addess id you want to access. |


#### Example Usage

```csharp
double emailAddressId = 59.2001380651259;

SendVerificationTokenResponse result = await emailMarketing.UpdateSendVerificationToken(emailAddressId);

```


### <a name="update_verify_allowed_email_address"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailMarketingController.UpdateVerifyAllowedEmailAddress") UpdateVerifyAllowedEmailAddress

> TODO: Add a method description


```csharp
Task<VerifyAllowedEmailAddressResponse> UpdateVerifyAllowedEmailAddress(double emailAddressId, string activationToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email address id you want to access. |
| activationToken |  ``` Required ```  | 6E8B-4FDB-99A7-7ED08DF97BCC (required, string) - Your activation token. |


#### Example Usage

```csharp
double emailAddressId = 5;
string activationToken = "3BD73304";

VerifyAllowedEmailAddressResponse result = await emailMarketing.UpdateVerifyAllowedEmailAddress(emailAddressId, activationToken);

```


### <a name="delete_allowed_email_address"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailMarketingController.DeleteAllowedEmailAddress") DeleteAllowedEmailAddress

> TODO: Add a method description


```csharp
Task<DeleteAllowedEmailAddressResponse> DeleteAllowedEmailAddress(double emailAddressId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email address you want to access. |


#### Example Usage

```csharp
double emailAddressId = 59.2001380651259;

DeleteAllowedEmailAddressResponse result = await emailMarketing.DeleteAllowedEmailAddress(emailAddressId);

```


### <a name="get_specific_allowed_email_address"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailMarketingController.GetSpecificAllowedEmailAddress") GetSpecificAllowedEmailAddress

> TODO: Add a method description


```csharp
Task<GetSpecificAllowedEmailAddressResponse> GetSpecificAllowedEmailAddress(double emailAddressId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email address you want to access. |


#### Example Usage

```csharp
double emailAddressId = 4;

GetSpecificAllowedEmailAddressResponse result = await emailMarketing.GetSpecificAllowedEmailAddress(emailAddressId);

```


### <a name="get_all_email_campaigns"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailMarketingController.GetAllEmailCampaigns") GetAllEmailCampaigns

> TODO: Add a method description


```csharp
Task<GetAllEmailCampaignsResponse> GetAllEmailCampaigns()
```

#### Example Usage

```csharp

GetAllEmailCampaignsResponse result = await emailMarketing.GetAllEmailCampaigns();

```


### <a name="get_specific_email_campaign"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailMarketingController.GetSpecificEmailCampaign") GetSpecificEmailCampaign

> TODO: Add a method description


```csharp
Task<GetSpecificEmailCampaignResponse> GetSpecificEmailCampaign(double emailCampaignId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailCampaignId |  ``` Required ```  | The email campaign id you want to access. |


#### Example Usage

```csharp
double emailCampaignId = 1;

GetSpecificEmailCampaignResponse result = await emailMarketing.GetSpecificEmailCampaign(emailCampaignId);

```


### <a name="create_email_campaign"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailMarketingController.CreateEmailCampaign") CreateEmailCampaign

> TODO: Add a method description


```csharp
Task<CreateEmailCampaignResponse> CreateEmailCampaign(CreateEmailCampaignRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "{  \"name\" : \"John Doe\",  \"subject\" : \"Lorem Ipsum\",  \"from_email_address_id\" : 2,  \"from_name\" : \"From name\",  \"template_id\" : 31,  \"body\" : \"<p>This is a test</p>\",  \"list_id\" : 456}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<CreateEmailCampaignRequest>(bodyValue);

CreateEmailCampaignResponse result = await emailMarketing.CreateEmailCampaign(body);

```


### <a name="update_email_campaign"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailMarketingController.UpdateEmailCampaign") UpdateEmailCampaign

> TODO: Add a method description


```csharp
Task<UpdateEmailCampaignResponse> UpdateEmailCampaign(double emailCampaignId, UpdateEmailCampaignRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailCampaignId |  ``` Required ```  | The email campaign id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
double emailCampaignId = 1;
string bodyValue = "{  \"name\" : \"John Doe\",  \"subject\" : \"Lorem Ipsum\",  \"from_email_address_id\" : 2,  \"from_name\" : \"From name\",  \"template_id\" : 31,  \"body\" : \"<p>This is a test</p>\",  \"list_id\" : 456}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<UpdateEmailCampaignRequest>(bodyValue);

UpdateEmailCampaignResponse result = await emailMarketing.UpdateEmailCampaign(emailCampaignId, body);

```


### <a name="update_cancel_email_campaign"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailMarketingController.UpdateCancelEmailCampaign") UpdateCancelEmailCampaign

> TODO: Add a method description


```csharp
Task<CancelEmailCampaignResponse> UpdateCancelEmailCampaign(double emailCampaignId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailCampaignId |  ``` Required ```  | The email campaign id you want to cancel. |


#### Example Usage

```csharp
double emailCampaignId = 1;

CancelEmailCampaignResponse result = await emailMarketing.UpdateCancelEmailCampaign(emailCampaignId);

```


### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailMarketingController.CreateCalculatePrice") CreateCalculatePrice

> TODO: Add a method description


```csharp
Task<CalculatePriceResponse> CreateCalculatePrice(CalculatePriceRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "{  \"name\" : \"John Doe\",  \"subject\" : \"Lorem Ipsum\",  \"from_email_address_id\" : 2,  \"from_name\" : \"From name\",  \"template_id\" : 31,  \"body\" : \"<p>This is a test</p>\",  \"list_id\" : 456}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<CalculatePriceRequest>(bodyValue);

CalculatePriceResponse result = await emailMarketing.CreateCalculatePrice(body);

```


### <a name="get_specific_email_campaign_history"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailMarketingController.GetSpecificEmailCampaignHistory") GetSpecificEmailCampaignHistory

> TODO: Add a method description


```csharp
Task<GetSpecificEmailCampaignHistoryResponse> GetSpecificEmailCampaignHistory(double campaignId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| campaignId |  ``` Required ```  | The email campaign id you want to access. |


#### Example Usage

```csharp
double campaignId = 77;

GetSpecificEmailCampaignHistoryResponse result = await emailMarketing.GetSpecificEmailCampaignHistory(campaignId);

```


### <a name="get_all_email_templates"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailMarketingController.GetAllEmailTemplates") GetAllEmailTemplates

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```csharp
Task<GetAllEmailTemplatesResponse> GetAllEmailTemplates()
```

#### Example Usage

```csharp

GetAllEmailTemplatesResponse result = await emailMarketing.GetAllEmailTemplates();

```


### <a name="get_specific_email_template"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailMarketingController.GetSpecificEmailTemplate") GetSpecificEmailTemplate

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```csharp
Task<GetSpecificEmailTemplateResponse> GetSpecificEmailTemplate(double templateId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | The email template id. |


#### Example Usage

```csharp
double templateId = 291;

GetSpecificEmailTemplateResponse result = await emailMarketing.GetSpecificEmailTemplate(templateId);

```


### <a name="create_new_email_template_from_master_template"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailMarketingController.CreateNewEmailTemplateFromMasterTemplate") CreateNewEmailTemplateFromMasterTemplate

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```csharp
Task<CreateNewEmailTemplateFromMasterTemplateResponse> CreateNewEmailTemplateFromMasterTemplate(CreateNewEmailTemplateFromMasterTemplateRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "{  \"template_name\": \"Minions\",  \"template_id_master\": 57}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<CreateNewEmailTemplateFromMasterTemplateRequest>(bodyValue);

CreateNewEmailTemplateFromMasterTemplateResponse result = await emailMarketing.CreateNewEmailTemplateFromMasterTemplate(body);

```


### <a name="update_an_email_template"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailMarketingController.UpdateAnEmailTemplate") UpdateAnEmailTemplate

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```csharp
Task<UpdateAnEmailTemplateResponse> UpdateAnEmailTemplate(double templateId, UpdateAnEmailTemplateRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | The id of the template to be updated. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
double templateId = 291;
string bodyValue = "    {        \"template_name\":\"Minions\",        \"body\":\"This is a sample content: Sc0KNWgSMG for this template.\"    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<UpdateAnEmailTemplateRequest>(bodyValue);

UpdateAnEmailTemplateResponse result = await emailMarketing.UpdateAnEmailTemplate(templateId, body);

```


### <a name="delete_email_template"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailMarketingController.DeleteEmailTemplate") DeleteEmailTemplate

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```csharp
Task<DeleteEmailTemplateResponse> DeleteEmailTemplate(double templateId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |


#### Example Usage

```csharp
double templateId = 25;

DeleteEmailTemplateResponse result = await emailMarketing.DeleteEmailTemplate(templateId);

```


### <a name="get_all_master_email_templates"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailMarketingController.GetAllMasterEmailTemplates") GetAllMasterEmailTemplates

> Master templates are templates that you can clone to a User Email Template which lets you edit and save it.


```csharp
Task<GetAllMasterEmailTemplatesResponse> GetAllMasterEmailTemplates()
```

#### Example Usage

```csharp

GetAllMasterEmailTemplatesResponse result = await emailMarketing.GetAllMasterEmailTemplates();

```


### <a name="get_specific_master_template"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailMarketingController.GetSpecificMasterTemplate") GetSpecificMasterTemplate

> Master templates are templates that you can clone to a User Email Template which lets you edit and save it.


```csharp
Task<GetSpecificMasterTemplateResponse> GetSpecificMasterTemplate(string templateId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |


#### Example Usage

```csharp
string templateId = "25";

GetSpecificMasterTemplateResponse result = await emailMarketing.GetSpecificMasterTemplate(templateId);

```


### <a name="get_all_master_template_categories"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailMarketingController.GetAllMasterTemplateCategories") GetAllMasterTemplateCategories

> TODO: Add a method description


```csharp
Task<GetAllMasterTemplateCategoriesResponse> GetAllMasterTemplateCategories()
```

#### Example Usage

```csharp

GetAllMasterTemplateCategoriesResponse result = await emailMarketing.GetAllMasterTemplateCategories();

```


### <a name="get_specific_email_template_category"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailMarketingController.GetSpecificEmailTemplateCategory") GetSpecificEmailTemplateCategory

> TODO: Add a method description


```csharp
Task<GetSpecificEmailTemplateCategoryResponse> GetSpecificEmailTemplateCategory(string categoryId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| categoryId |  ``` Required ```  | Your category id. |


#### Example Usage

```csharp
string categoryId = "25";

GetSpecificEmailTemplateCategoryResponse result = await emailMarketing.GetSpecificEmailTemplateCategory(categoryId);

```


### <a name="get_all_templates_for_category"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailMarketingController.GetAllTemplatesForCategory") GetAllTemplatesForCategory

> TODO: Add a method description


```csharp
Task<GetAllTemplatesForCategoryResponse> GetAllTemplatesForCategory(string categoryId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| categoryId |  ``` Required ```  | Your category id. |


#### Example Usage

```csharp
string categoryId = "1";

GetAllTemplatesForCategoryResponse result = await emailMarketing.GetAllTemplatesForCategory(categoryId);

```


### <a name="upload_image_to_specific_template"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailMarketingController.UploadImageToSpecificTemplate") UploadImageToSpecificTemplate

> TODO: Add a method description


```csharp
Task<UploadImageToSpecificTemplateResponse> UploadImageToSpecificTemplate(string templateId, UploadImageToSpecificTemplateRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string templateId = "1";
string bodyValue = "{    \"image\": \"image.png\",    \"url\" : \"http://www.downloadimg.from/here.png\"}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<UploadImageToSpecificTemplateRequest>(bodyValue);

UploadImageToSpecificTemplateResponse result = await emailMarketing.UploadImageToSpecificTemplate(templateId, body);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="email_to_sms_allowed_address_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.EmailToSMSAllowedAddressController") EmailToSMSAllowedAddressController

### Get singleton instance

The singleton instance of the ``` EmailToSMSAllowedAddressController ``` class can be accessed from the API Client.

```csharp
EmailToSMSAllowedAddressController emailToSMSAllowedAddress = client.EmailToSMSAllowedAddress;
```

### <a name="list_of_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailToSMSAllowedAddressController.ListOfEmailToSMSAllowedAddress") ListOfEmailToSMSAllowedAddress

> Get list of allowed email addresses.


```csharp
Task<ListOfEmailToSMSAllowedAddressResponse> ListOfEmailToSMSAllowedAddress()
```

#### Example Usage

```csharp

ListOfEmailToSMSAllowedAddressResponse result = await emailToSMSAllowedAddress.ListOfEmailToSMSAllowedAddress();

```


### <a name="create_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailToSMSAllowedAddressController.CreateEmailToSMSAllowedAddress") CreateEmailToSMSAllowedAddress

> Create an allowed email address.


```csharp
Task<CreateEmailToSMSAllowedAddressResponse> CreateEmailToSMSAllowedAddress(CreateEmailToSMSAllowedAddressRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "    {        \"email_address\":\"Cv3p0@gmail.com\",        \"from\":\"+17128845887\"    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<CreateEmailToSMSAllowedAddressRequest>(bodyValue);

CreateEmailToSMSAllowedAddressResponse result = await emailToSMSAllowedAddress.CreateEmailToSMSAllowedAddress(body);

```


### <a name="get_specific_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailToSMSAllowedAddressController.GetSpecificEmailToSMSAllowedAddress") GetSpecificEmailToSMSAllowedAddress

> Get a specific allowed email address.


```csharp
Task<GetSpecificEmailToSMSAllowedAddressResponse> GetSpecificEmailToSMSAllowedAddress(double emailAddressId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | Your email address id. |


#### Example Usage

```csharp
double emailAddressId = 113;

GetSpecificEmailToSMSAllowedAddressResponse result = await emailToSMSAllowedAddress.GetSpecificEmailToSMSAllowedAddress(emailAddressId);

```


### <a name="update_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailToSMSAllowedAddressController.UpdateEmailToSMSAllowedAddress") UpdateEmailToSMSAllowedAddress

> Update a specific allowed email address.


```csharp
Task<UpdateEmailToSMSAllowedAddressResponse> UpdateEmailToSMSAllowedAddress(double emailAddressId, UpdateEmailToSMSAllowedAddressRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | Your email address id. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
double emailAddressId = 107;
string bodyValue = "    {        \"email_address\":\"pfvRZ@gmail.com\",        \"from\":\"+17128842283\"    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<UpdateEmailToSMSAllowedAddressRequest>(bodyValue);

UpdateEmailToSMSAllowedAddressResponse result = await emailToSMSAllowedAddress.UpdateEmailToSMSAllowedAddress(emailAddressId, body);

```


### <a name="delete_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailToSMSAllowedAddressController.DeleteEmailToSMSAllowedAddress") DeleteEmailToSMSAllowedAddress

> Delete a specific allowed email address.


```csharp
Task<DeleteEmailToSMSAllowedAddressResponse> DeleteEmailToSMSAllowedAddress(double emailAddressId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | Your email address id. |


#### Example Usage

```csharp
double emailAddressId = 107;

DeleteEmailToSMSAllowedAddressResponse result = await emailToSMSAllowedAddress.DeleteEmailToSMSAllowedAddress(emailAddressId);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="email_to_sms_stripped_strings_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.EmailToSMSStrippedStringsController") EmailToSMSStrippedStringsController

### Get singleton instance

The singleton instance of the ``` EmailToSMSStrippedStringsController ``` class can be accessed from the API Client.

```csharp
EmailToSMSStrippedStringsController emailToSMSStrippedStrings = client.EmailToSMSStrippedStrings;
```

### <a name="list_stripped_strings"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailToSMSStrippedStringsController.ListStrippedStrings") ListStrippedStrings

> TODO: Add a method description


```csharp
Task<ListStrippedStringsResponse> ListStrippedStrings()
```

#### Example Usage

```csharp

ListStrippedStringsResponse result = await emailToSMSStrippedStrings.ListStrippedStrings();

```


### <a name="find_specific_stripped_string"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailToSMSStrippedStringsController.FindSpecificStrippedString") FindSpecificStrippedString

> TODO: Add a method description


```csharp
Task<FindSpecificStrippedStringResponse> FindSpecificStrippedString(double ruleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |


#### Example Usage

```csharp
double ruleId = 18;

FindSpecificStrippedStringResponse result = await emailToSMSStrippedStrings.FindSpecificStrippedString(ruleId);

```


### <a name="create_stripped_string"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailToSMSStrippedStringsController.CreateStrippedString") CreateStrippedString

> TODO: Add a method description


```csharp
Task<CreateStrippedStringResponse> CreateStrippedString(CreateStrippedStringRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "{    \"strip_string\" : \"~~~test~~~\"}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<CreateStrippedStringRequest>(bodyValue);

CreateStrippedStringResponse result = await emailToSMSStrippedStrings.CreateStrippedString(body);

```


### <a name="update_stripped_string"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailToSMSStrippedStringsController.UpdateStrippedString") UpdateStrippedString

> TODO: Add a method description


```csharp
Task<UpdateStrippedStringResponse> UpdateStrippedString(double ruleId, UpdateStrippedStringRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
double ruleId = 20;
string bodyValue = "{    \"strip_string\" : \"~~~test1~~~\"}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<UpdateStrippedStringRequest>(bodyValue);

UpdateStrippedStringResponse result = await emailToSMSStrippedStrings.UpdateStrippedString(ruleId, body);

```


### <a name="delete_stripped_string"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.EmailToSMSStrippedStringsController.DeleteStrippedString") DeleteStrippedString

> TODO: Add a method description


```csharp
Task<DeleteStrippedStringResponse> DeleteStrippedString(double ruleId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |


#### Example Usage

```csharp
double ruleId = 20;

DeleteStrippedStringResponse result = await emailToSMSStrippedStrings.DeleteStrippedString(ruleId);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="fax_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.FaxController") FaxController

### Get singleton instance

The singleton instance of the ``` FaxController ``` class can be accessed from the API Client.

```csharp
FaxController fax = client.Fax;
```

### <a name="create_send_fax"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.FaxController.CreateSendFax") CreateSendFax

> **Letter File Options**
> **Use existing URL**
> With this option, you can use an existing URL to a PDF document. For example, you might generate the pdf on your server.
> **Upload File to Our Server**
> With this option, you can use the `/uploads` endpoint to upload the document. The `/uploads` endpoint returns a URL that can be used in the `/fax/send` endpoint.


```csharp
Task<SendFaxResponse> CreateSendFax(SendFaxRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new SendFaxRequest();

SendFaxResponse result = await fax.CreateSendFax(body);

```


### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.FaxController.CreateCalculatePrice") CreateCalculatePrice

> TODO: Add a method description


```csharp
Task<CalculatePriceResponse> CreateCalculatePrice(CalculatePriceRequest132 body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new CalculatePriceRequest132();

CalculatePriceResponse result = await fax.CreateCalculatePrice(body);

```


### <a name="get_fax_history"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.FaxController.GetFaxHistory") GetFaxHistory

> Get a list of Fax History.


```csharp
Task<GetFaxHistoryResponse> GetFaxHistory(
        double? dateFrom = null,
        double? dateTo = null,
        string q = null,
        string orderBy = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateFrom |  ``` Optional ```  | Customize result by setting from date (timestsamp) |
| dateTo |  ``` Optional ```  | Customize result by setting to date (timestamp) |
| q |  ``` Optional ```  | Custom query |
| orderBy |  ``` Optional ```  | Order result by |


#### Example Usage

```csharp
double? dateFrom = 1457572619;
double? dateTo = 1457573000;
string q = "status:Sent,status_code:201";
string orderBy = "subject:desc";

GetFaxHistoryResponse result = await fax.GetFaxHistory(dateFrom, dateTo, q, orderBy);

```


### <a name="list_of_fax_delivery_receipts"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.FaxController.ListOfFaxDeliveryReceipts") ListOfFaxDeliveryReceipts

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


```csharp
Task<ListOfFaxDeliveryReceiptsResponse> ListOfFaxDeliveryReceipts()
```

#### Example Usage

```csharp

ListOfFaxDeliveryReceiptsResponse result = await fax.ListOfFaxDeliveryReceipts();

```


### <a name="get_a_specific_fax_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.FaxController.GetASpecificFaxDeliveryReceipt") GetASpecificFaxDeliveryReceipt

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


```csharp
Task<GetASpecificFaxDeliveryReceiptResponse> GetASpecificFaxDeliveryReceipt(string messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | D2AF-479B-8955-6395D561DEF4" (required, number) - Message ID. |


#### Example Usage

```csharp
string messageId = "\"3FAC74F1";

GetASpecificFaxDeliveryReceiptResponse result = await fax.GetASpecificFaxDeliveryReceipt(messageId);

```


### <a name="update_mark_fax_delivery_receipts_as_read"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.FaxController.UpdateMarkFaxDeliveryReceiptsAsRead") UpdateMarkFaxDeliveryReceiptsAsRead

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


```csharp
Task<MarkFaxDeliveryReceiptsAsReadResponse> UpdateMarkFaxDeliveryReceiptsAsRead(MarkFaxDeliveryReceiptsAsReadRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "{    \"date_before\": 1441958441}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<MarkFaxDeliveryReceiptsAsReadRequest>(bodyValue);

MarkFaxDeliveryReceiptsAsReadResponse result = await fax.UpdateMarkFaxDeliveryReceiptsAsRead(body);

```


### <a name="add_a_test_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.FaxController.AddATestDeliveryReceipt") AddATestDeliveryReceipt

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


```csharp
Task<AddATestDeliveryReceiptResponse> AddATestDeliveryReceipt(AddATestDeliveryReceiptRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "    {        \"url\":\"http://yourUrl.com\"    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<AddATestDeliveryReceiptRequest>(bodyValue);

AddATestDeliveryReceiptResponse result = await fax.AddATestDeliveryReceipt(body);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="forgot_account_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.ForgotAccountController") ForgotAccountController

### Get singleton instance

The singleton instance of the ``` ForgotAccountController ``` class can be accessed from the API Client.

```csharp
ForgotAccountController forgotAccount = client.ForgotAccount;
```

### <a name="update_forgot_username"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ForgotAccountController.UpdateForgotUsername") UpdateForgotUsername

> TODO: Add a method description


```csharp
Task<ForgotUsernameResponse> UpdateForgotUsername(ForgotUsernameRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new ForgotUsernameRequest();

ForgotUsernameResponse result = await forgotAccount.UpdateForgotUsername(body);

```


### <a name="update_forgot_password"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ForgotAccountController.UpdateForgotPassword") UpdateForgotPassword

> TODO: Add a method description


```csharp
Task<ForgotPasswordResponse> UpdateForgotPassword(ForgotPasswordRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "    {        \"username\": \"0F6pKiiuca\"    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<ForgotPasswordRequest>(bodyValue);

ForgotPasswordResponse result = await forgotAccount.UpdateForgotPassword(body);

```


### <a name="update_verify_forgot_password"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ForgotAccountController.UpdateVerifyForgotPassword") UpdateVerifyForgotPassword

> TODO: Add a method description


```csharp
Task<VerifyForgotPasswordResponse> UpdateVerifyForgotPassword(VerifyForgotPasswordRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "    {        \"subaccount_id\": 54,        \"activation_token\": \"9C648BAD-EB7F-4E7E-96BC-B433140C4F1F\",        \"password\": \"0F6pKiiuca\"    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<VerifyForgotPasswordRequest>(bodyValue);

VerifyForgotPasswordResponse result = await forgotAccount.UpdateVerifyForgotPassword(body);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="mms_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.MMSController") MMSController

### Get singleton instance

The singleton instance of the ``` MMSController ``` class can be accessed from the API Client.

```csharp
MMSController mMS = client.MMS;
```

### <a name="create_send_mms"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.MMSController.CreateSendMMS") CreateSendMMS

> TODO: Add a method description


```csharp
Task<SendMMSResponse> CreateSendMMS(SendMMSRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new SendMMSRequest();

SendMMSResponse result = await mMS.CreateSendMMS(body);

```


### <a name="create_get_price"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.MMSController.CreateGetPrice") CreateGetPrice

> TODO: Add a method description


```csharp
Task<GetPriceResponse> CreateGetPrice(GetPriceRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new GetPriceRequest();

GetPriceResponse result = await mMS.CreateGetPrice(body);

```


### <a name="get_mms_history"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.MMSController.GetMMSHistory") GetMMSHistory

> TODO: Add a method description


```csharp
Task<GetMMSHistoryResponse> GetMMSHistory(
        string q = null,
        string orderBy = null,
        int? dateFrom = null,
        int? dateTo = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| q |  ``` Optional ```  | A custom query. |
| orderBy |  ``` Optional ```  | Sort records by. |
| dateFrom |  ``` Optional ```  | Timestamp (from) used to show records by date. |
| dateTo |  ``` Optional ```  | Timestamp (to) used to show records by date. |


#### Example Usage

```csharp
string q = "list_id:429,direction:out";
string orderBy = "subject:desc";
int? dateFrom = 1443501617;
int? dateTo = 1443501727;

GetMMSHistoryResponse result = await mMS.GetMMSHistory(q, orderBy, dateFrom, dateTo);

```


### <a name="get_export_mms_history"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.MMSController.GetExportMMSHistory") GetExportMMSHistory

> TODO: Add a method description


```csharp
Task<ExportMMSHistoryResponse> GetExportMMSHistory(string filename)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | Your export filename. |


#### Example Usage

```csharp
string filename = "export.csv";

ExportMMSHistoryResponse result = await mMS.GetExportMMSHistory(filename);

```


### <a name="update_cancel_mms"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.MMSController.UpdateCancelMMS") UpdateCancelMMS

> TODO: Add a method description


```csharp
Task<CancelMMSResponse> UpdateCancelMMS(string messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Message ID. |


#### Example Usage

```csharp
string messageId = "message_id";

CancelMMSResponse result = await mMS.UpdateCancelMMS(messageId);

```


### <a name="update_cancel_all_mms"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.MMSController.UpdateCancelAllMMS") UpdateCancelAllMMS

> TODO: Add a method description


```csharp
Task<CancelAllMMSResponse> UpdateCancelAllMMS()
```

#### Example Usage

```csharp

CancelAllMMSResponse result = await mMS.UpdateCancelAllMMS();

```


### <a name="get_all_delivery_receipts"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.MMSController.GetAllDeliveryReceipts") GetAllDeliveryReceipts

> TODO: Add a method description


```csharp
Task<GetAllDeliveryReceiptsResponse> GetAllDeliveryReceipts()
```

#### Example Usage

```csharp

GetAllDeliveryReceiptsResponse result = await mMS.GetAllDeliveryReceipts();

```


### <a name="get_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.MMSController.GetDeliveryReceipt") GetDeliveryReceipt

> TODO: Add a method description


```csharp
Task<GetDeliveryReceiptResponse> GetDeliveryReceipt(string messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Message ID. |


#### Example Usage

```csharp
string messageId = "3E0DC217-7D0F-4C20-A3F2-E3362B938CAF";

GetDeliveryReceiptResponse result = await mMS.GetDeliveryReceipt(messageId);

```


### <a name="update_mark_receipts_as_read"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.MMSController.UpdateMarkReceiptsAsRead") UpdateMarkReceiptsAsRead

> TODO: Add a method description


```csharp
Task<MarkReceiptsAsReadResponse> UpdateMarkReceiptsAsRead()
```

#### Example Usage

```csharp

MarkReceiptsAsReadResponse result = await mMS.UpdateMarkReceiptsAsRead();

```


### <a name="get_all_inbound_sms_pull"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.MMSController.GetAllInboundSMSPull") GetAllInboundSMSPull

> Inbound MMS shares the same rules/settings/endpoints as SMS. Any attachments will be converted to a URL.
> **Push Inbound SMS**
> If you prefer, we can push message replies to your server as they arrive with us.
> Refer to SMS->Inbound SMS in the docs.
> **Pull Inbound SMS**
> Receive SMS by polling your Inbox.
> Refer to SMS->Inbound SMS in the docs.


```csharp
Task<dynamic> GetAllInboundSMSPull()
```

#### Example Usage

```csharp

dynamic result = await mMS.GetAllInboundSMSPull();

```


[Back to List of Controllers](#list_of_controllers)

## <a name="numbers_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.NumbersController") NumbersController

### Get singleton instance

The singleton instance of the ``` NumbersController ``` class can be accessed from the API Client.

```csharp
NumbersController numbers = client.Numbers;
```

### <a name="get_all_dedicated_numbers"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.NumbersController.GetAllDedicatedNumbers") GetAllDedicatedNumbers

> TODO: Add a method description


```csharp
Task<GetAllDedicatedNumbersResponse> GetAllDedicatedNumbers()
```

#### Example Usage

```csharp

GetAllDedicatedNumbersResponse result = await numbers.GetAllDedicatedNumbers();

```


### <a name="create_buy_dedicated_number"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.NumbersController.CreateBuyDedicatedNumber") CreateBuyDedicatedNumber

> TODO: Add a method description


```csharp
Task<BuyDedicatedNumberResponse> CreateBuyDedicatedNumber(string dedicatedNumber)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dedicatedNumber |  ``` Required ```  | Your phone number in E.164 format. |


#### Example Usage

```csharp
string dedicatedNumber = "+12282060576";

BuyDedicatedNumberResponse result = await numbers.CreateBuyDedicatedNumber(dedicatedNumber);

```


### <a name="search_dedicated_numbers_by_country"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.NumbersController.SearchDedicatedNumbersByCountry") SearchDedicatedNumbersByCountry

> TODO: Add a method description


```csharp
Task<SearchDedicatedNumbersByCountryResponse> SearchDedicatedNumbersByCountry(string country, string search = null, double? searchType = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Required ```  | Your preferred country. |
| search |  ``` Optional ```  | Your search pattern or query. |
| searchType |  ``` Optional ```  | Your strategy for searching, 0 = starts with, 1 = anywhere, 2 = ends with. |


#### Example Usage

```csharp
string country = "US";
string search = "88";
double? searchType = 1;

SearchDedicatedNumbersByCountryResponse result = await numbers.SearchDedicatedNumbersByCountry(country, search, searchType);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="pricing_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.PricingController") PricingController

### Get singleton instance

The singleton instance of the ``` PricingController ``` class can be accessed from the API Client.

```csharp
PricingController pricing = client.Pricing;
```

### <a name="get_country_pricing"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.PricingController.GetCountryPricing") GetCountryPricing

> TODO: Add a method description


```csharp
Task<GetCountryPricingResponse> GetCountryPricing(string country, string currency = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Required ```  | Two-letter representation of the country. |
| currency |  ``` Optional ```  | Three-letter representation of the currency. |


#### Example Usage

```csharp
string country = "AU";
string currency = "AUD";

GetCountryPricingResponse result = await pricing.GetCountryPricing(country, currency);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="post_direct_mail_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.PostDirectMailController") PostDirectMailController

### Get singleton instance

The singleton instance of the ``` PostDirectMailController ``` class can be accessed from the API Client.

```csharp
PostDirectMailController postDirectMail = client.PostDirectMail;
```

### <a name="search_locations"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.PostDirectMailController.SearchLocations") SearchLocations

> TODO: Add a method description


```csharp
Task<SearchLocationsResponse> SearchLocations(string country, string query)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Required ```  | Country code. |
| query |  ``` Required ```  | A postal code or place name. |


#### Example Usage

```csharp
string country = "AD";
string query = "AD100";

SearchLocationsResponse result = await postDirectMail.SearchLocations(country, query);

```


### <a name="create_new_campaign"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.PostDirectMailController.CreateNewCampaign") CreateNewCampaign

> Create new direct mail campaign.


```csharp
Task<CreateNewCampaignResponse> CreateNewCampaign(CreateNewCampaignRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new CreateNewCampaignRequest();

CreateNewCampaignResponse result = await postDirectMail.CreateNewCampaign(body);

```


### <a name="create_calculate_direct_mail_campaign_price"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.PostDirectMailController.CreateCalculateDirectMailCampaignPrice") CreateCalculateDirectMailCampaignPrice

> Calculate direct mail campaign price.


```csharp
Task<CalculateDirectMailCampaignPriceResponse> CreateCalculateDirectMailCampaignPrice(CalculateDirectMailCampaignPriceRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new CalculateDirectMailCampaignPriceRequest();

CalculateDirectMailCampaignPriceResponse result = await postDirectMail.CreateCalculateDirectMailCampaignPrice(body);

```


### <a name="list_direct_mail_campaigns"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.PostDirectMailController.ListDirectMailCampaigns") ListDirectMailCampaigns

> Get list of direct mail campaigns.


```csharp
Task<ListDirectMailCampaignsResponse> ListDirectMailCampaigns()
```

#### Example Usage

```csharp

ListDirectMailCampaignsResponse result = await postDirectMail.ListDirectMailCampaigns();

```


[Back to List of Controllers](#list_of_controllers)

## <a name="post_letter_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.PostLetterController") PostLetterController

### Get singleton instance

The singleton instance of the ``` PostLetterController ``` class can be accessed from the API Client.

```csharp
PostLetterController postLetter = client.PostLetter;
```

### <a name="create_send_post_letter"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.PostLetterController.CreateSendPostLetter") CreateSendPostLetter

> **Supported File Types**
> We support `pdf`, `docx` and `doc` files. Contact us to add support for any other file type. If you're using `docx` or `doc` files, you'll need to convert the file first using our uploads endpoint with the querystring parameter `convert=post` e.g. `POST /uploads?convert=post`. This will return a URL to the converted pdf file that can be used in the `/post/letters/send` endpoint.
> **Letter File Options**
> **Use existing URL**
> With this option, you can use an existing URL to a `pdf` document. For example, you might generate the `pdf` on your server.
> **Upload File to Our Server**
> With this option, you can use the `/uploads` endpoint to upload the document. The `/uploads` endpoint returns a URL that can be used in the `/post/letters/send` endpoint.


```csharp
Task<SendPostLetterResponse> CreateSendPostLetter(SendPostLetterRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "{  \"file_url\": \"http://server.com/file.pdf\",  \"template_used\": 1,  \"colour\": 1,  \"duplex\": 0,  \"recipients\": [    {      \"address_name\": \"My Home Address\",      \"address_line_1\": \"Address 1\",      \"address_line_2\": \"Address 2\",      \"address_city\": \"CITY\",      \"address_state\": \"State\",      \"address_postal_code\": 123456,      \"address_country\": \"AU\",      \"return_address_id\": 1,      \"schedule\": 1449573604    }  ]}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<SendPostLetterRequest>(bodyValue);

SendPostLetterResponse result = await postLetter.CreateSendPostLetter(body);

```


### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.PostLetterController.CreateCalculatePrice") CreateCalculatePrice

> TODO: Add a method description


```csharp
Task<CalculatePriceResponse> CreateCalculatePrice(CalculatePriceRequest170 body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "{  \"file_url\": \"http://server.com/file.pdf\",  \"template_used\": 1,  \"colour\": 1,  \"duplex\": 0,  \"recipients\": [    \"[]\"  ],  \"Body\": \"\"}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<CalculatePriceRequest170>(bodyValue);

CalculatePriceResponse result = await postLetter.CreateCalculatePrice(body);

```


### <a name="get_post_letter_history"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.PostLetterController.GetPostLetterHistory") GetPostLetterHistory

> TODO: Add a method description


```csharp
Task<GetPostLetterHistoryResponse> GetPostLetterHistory()
```

#### Example Usage

```csharp

GetPostLetterHistoryResponse result = await postLetter.GetPostLetterHistory();

```


### <a name="get_export_post_letter_history"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.PostLetterController.GetExportPostLetterHistory") GetExportPostLetterHistory

> TODO: Add a method description


```csharp
Task<ExportPostLetterHistoryResponse> GetExportPostLetterHistory(string filename)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | Filename for the export file. |


#### Example Usage

```csharp
string filename = "myexport.csv";

ExportPostLetterHistoryResponse result = await postLetter.GetExportPostLetterHistory(filename);

```


### <a name="create_a_post_return_address"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.PostLetterController.CreateAPostReturnAddress") CreateAPostReturnAddress

> TODO: Add a method description


```csharp
Task<CreateAPostReturnAddressResponse> CreateAPostReturnAddress(CreateAPostReturnAddressRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "{    \"address_name\":\"My Home Address\",    \"address_line_1\":\"Maritime Avenue\",    \"address_line_2\":\"\",    \"address_city\":\"Flynn\",    \"address_state\":\"WA\",    \"address_postal_code\":6302,    \"address_country\":\"Australia\"}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<CreateAPostReturnAddressRequest>(bodyValue);

CreateAPostReturnAddressResponse result = await postLetter.CreateAPostReturnAddress(body);

```


### <a name="get_list_of_post_return_addresses"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.PostLetterController.GetListOfPostReturnAddresses") GetListOfPostReturnAddresses

> TODO: Add a method description


```csharp
Task<GetListOfPostReturnAddressesResponse> GetListOfPostReturnAddresses()
```

#### Example Usage

```csharp

GetListOfPostReturnAddressesResponse result = await postLetter.GetListOfPostReturnAddresses();

```


### <a name="get_post_return_address"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.PostLetterController.GetPostReturnAddress") GetPostReturnAddress

> TODO: Add a method description


```csharp
Task<GetPostReturnAddressResponse> GetPostReturnAddress(double returnAddressId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| returnAddressId |  ``` Required ```  | Your return address id. |


#### Example Usage

```csharp
double returnAddressId = 14;

GetPostReturnAddressResponse result = await postLetter.GetPostReturnAddress(returnAddressId);

```


### <a name="update_post_return_address"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.PostLetterController.UpdatePostReturnAddress") UpdatePostReturnAddress

> TODO: Add a method description


```csharp
Task<UpdatePostReturnAddressResponse> UpdatePostReturnAddress(double returnAddressId, UpdatePostReturnAddressRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| returnAddressId |  ``` Required ```  | Your return address id. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
double returnAddressId = 14;
string bodyValue = "{    \"address_name\":\"My Home Address\",    \"address_line_1\":\"Maritime Avenue\",    \"address_line_2\":\"\",    \"address_city\":\"Flynn\",    \"address_state\":\"WA\",    \"address_postal_code\":6302,    \"address_country\":\"Australia\"}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<UpdatePostReturnAddressRequest>(bodyValue);

UpdatePostReturnAddressResponse result = await postLetter.UpdatePostReturnAddress(returnAddressId, body);

```


### <a name="delete_post_return_address"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.PostLetterController.DeletePostReturnAddress") DeletePostReturnAddress

> TODO: Add a method description


```csharp
Task<DeletePostReturnAddressResponse> DeletePostReturnAddress(double returnAddressId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| returnAddressId |  ``` Required ```  | Your return address id. |


#### Example Usage

```csharp
double returnAddressId = 12;

DeletePostReturnAddressResponse result = await postLetter.DeletePostReturnAddress(returnAddressId);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="postcards_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.PostcardsController") PostcardsController

### Get singleton instance

The singleton instance of the ``` PostcardsController ``` class can be accessed from the API Client.

```csharp
PostcardsController postcards = client.Postcards;
```

### <a name="create_send_postcard"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.PostcardsController.CreateSendPostcard") CreateSendPostcard

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


```csharp
Task<SendPostcardResponse> CreateSendPostcard(SendPostcardRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "{    \"file_urls\":[         \"https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_front.pdf\",         \"https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_back.pdf\"    ],    \"recipients\":[        {            \"address_name\":\"My Home Address\",            \"address_line_1\":\"Address 1\",            \"address_line_2\":\"\",            \"address_city\":\"City\",            \"address_state\":\"State\",            \"address_postal_code\":\"123456\",            \"address_country\":\"AU\",            \"return_address_id\":1        }    ]}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<SendPostcardRequest>(bodyValue);

SendPostcardResponse result = await postcards.CreateSendPostcard(body);

```


### <a name="create_calculate_pricing"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.PostcardsController.CreateCalculatePricing") CreateCalculatePricing

> For `file_urls` field. You can attach at least 1 and max of 2 PDF file urls.
> - Supply a single pdf with 2 pages (front and back)
> - Supply 2 urls to seperate PDFs


```csharp
Task<CalculatePricingResponse> CreateCalculatePricing(CalculatePricingRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "{    \"file_urls\":[        \"https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_front.pdf\",        \"https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_back.pdf\"    ],    \"recipients\":[        {            \"address_name\":\"My Home Address\",            \"address_line_1\":\"Address 1\",            \"address_line_2\":\"\",            \"address_city\":\"City\",            \"address_state\":\"State\",            \"address_postal_code\":\"123456\",            \"address_country\":\"AU\",            \"return_address_id\":1        }    ]}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<CalculatePricingRequest>(bodyValue);

CalculatePricingResponse result = await postcards.CreateCalculatePricing(body);

```


### <a name="get_postcard_history"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.PostcardsController.GetPostcardHistory") GetPostcardHistory

> TODO: Add a method description


```csharp
Task<GetPostcardHistoryResponse> GetPostcardHistory()
```

#### Example Usage

```csharp

GetPostcardHistoryResponse result = await postcards.GetPostcardHistory();

```


### <a name="get_export_postcard_history"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.PostcardsController.GetExportPostcardHistory") GetExportPostcardHistory

> TODO: Add a method description


```csharp
Task<ExportPostcardHistoryResponse> GetExportPostcardHistory(string filename)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | Filename for the export file. |


#### Example Usage

```csharp
string filename = "myexport.csv";

ExportPostcardHistoryResponse result = await postcards.GetExportPostcardHistory(filename);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="referral_accounts_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.ReferralAccountsController") ReferralAccountsController

### Get singleton instance

The singleton instance of the ``` ReferralAccountsController ``` class can be accessed from the API Client.

```csharp
ReferralAccountsController referralAccounts = client.ReferralAccounts;
```

### <a name="get_list_of_referral_accounts"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ReferralAccountsController.GetListOfReferralAccounts") GetListOfReferralAccounts

> TODO: Add a method description


```csharp
Task<GetListOfReferralAccountsResponse> GetListOfReferralAccounts()
```

#### Example Usage

```csharp

GetListOfReferralAccountsResponse result = await referralAccounts.GetListOfReferralAccounts();

```


[Back to List of Controllers](#list_of_controllers)

## <a name="reseller_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.ResellerController") ResellerController

### Get singleton instance

The singleton instance of the ``` ResellerController ``` class can be accessed from the API Client.

```csharp
ResellerController reseller = client.Reseller;
```

### <a name="get_reseller_setting"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ResellerController.GetResellerSetting") GetResellerSetting

> Get reseller setting.


```csharp
Task<GetResellerSettingResponse> GetResellerSetting()
```

#### Example Usage

```csharp

GetResellerSettingResponse result = await reseller.GetResellerSetting();

```


### <a name="update_reseller_setting"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ResellerController.UpdateResellerSetting") UpdateResellerSetting

> Update a specific reseller setting.


```csharp
Task<UpdateResellerSettingResponse> UpdateResellerSetting(UpdateResellerSettingRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "    {        \"allow_public_signups\":1,        \"default_margin\":100,        \"default_margin_numbers\":150,        \"trial_balance\":50,        \"subdomain\":\"subdomain\",        \"colour_navigation\":\"#9999FF\",        \"logo_url_light\":\"http://url.com/light\",        \"logo_url_dark\":\"http://url.com/dark\",        \"company_name\":\"MyCompany\"    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<UpdateResellerSettingRequest>(bodyValue);

UpdateResellerSettingResponse result = await reseller.UpdateResellerSetting(body);

```


### <a name="get_reseller_by_subdomain"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ResellerController.GetResellerBySubdomain") GetResellerBySubdomain

> Get reseller setting by subdomin.


```csharp
Task<ResellerBySubdomainResponse> GetResellerBySubdomain(string subdomain)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subdomain |  ``` Required ```  | Subdomain |


#### Example Usage

```csharp
string subdomain = "mysubdomain";

ResellerBySubdomainResponse result = await reseller.GetResellerBySubdomain(subdomain);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="reseller_accounts_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.ResellerAccountsController") ResellerAccountsController

### Get singleton instance

The singleton instance of the ``` ResellerAccountsController ``` class can be accessed from the API Client.

```csharp
ResellerAccountsController resellerAccounts = client.ResellerAccounts;
```

### <a name="list_of_reseller_accounts"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ResellerAccountsController.ListOfResellerAccounts") ListOfResellerAccounts

> Get list of Reseller Accounts


```csharp
Task<ListOfResellerAccountsResponse> ListOfResellerAccounts()
```

#### Example Usage

```csharp

ListOfResellerAccountsResponse result = await resellerAccounts.ListOfResellerAccounts();

```


### <a name="get_reseller_account"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ResellerAccountsController.GetResellerAccount") GetResellerAccount

> Get a specific reseller account.


```csharp
Task<GetResellerAccountResponse> GetResellerAccount(double clientUserId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| clientUserId |  ``` Required ```  | The client user id. |


#### Example Usage

```csharp
double clientUserId = 24;

GetResellerAccountResponse result = await resellerAccounts.GetResellerAccount(clientUserId);

```


### <a name="create_reseller_account"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ResellerAccountsController.CreateResellerAccount") CreateResellerAccount

> TODO: Add a method description


```csharp
Task<CreateResellerAccountResponse> CreateResellerAccount(CreateResellerAccountRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "    {        \"username\":\"johndoe2\",        \"user_email\":\"johndoe2@awesome.com\",        \"user_phone\":\"518-481-1002\",        \"user_first_name\":\"John\",        \"user_last_name\":\"Doe\",        \"country\":\"US\",        \"password\":\"pass\",        \"account_name\":\"The Awesome Company\"    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<CreateResellerAccountRequest>(bodyValue);

CreateResellerAccountResponse result = await resellerAccounts.CreateResellerAccount(body);

```


### <a name="create_reseller_account_public"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ResellerAccountsController.CreateResellerAccountPublic") CreateResellerAccountPublic

> TODO: Add a method description


```csharp
Task<CreateResellerAccountPublicResponse> CreateResellerAccountPublic(CreateResellerAccountPublicRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "{    \"reseller_user_id\":1,    \"username\":\"john_awesome\",    \"user_email\":\"johnis@awesome.com\",    \"user_phone\":\"+61261063270\",    \"user_first_name\":\"John\",    \"user_last_name\":\"Awesome\",    \"country\":\"AU\",    \"password\":\"pass\",    \"account_name\":\"The Awesome Company\"}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<CreateResellerAccountPublicRequest>(bodyValue);

CreateResellerAccountPublicResponse result = await resellerAccounts.CreateResellerAccountPublic(body);

```


### <a name="update_reseller_account"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ResellerAccountsController.UpdateResellerAccount") UpdateResellerAccount

> TODO: Add a method description


```csharp
Task<UpdateResellerAccountResponse> UpdateResellerAccount(double clientUserId, UpdateResellerAccountRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| clientUserId |  ``` Required ```  | Your client user id. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
double clientUserId = 24;
string bodyValue = "    {        \"username\":\"johndoe2\",        \"user_email\":\"johndoe2@awesome.com\",        \"user_phone\":\"518-481-1002\",        \"user_first_name\":\"John\",        \"user_last_name\":\"Doe\",        \"country\":\"US\",        \"password\":\"pass\",        \"account_name\":\"The Awesome Company\"    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<UpdateResellerAccountRequest>(bodyValue);

UpdateResellerAccountResponse result = await resellerAccounts.UpdateResellerAccount(clientUserId, body);

```


### <a name="update_transfer_credit"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.ResellerAccountsController.UpdateTransferCredit") UpdateTransferCredit

> TODO: Add a method description


```csharp
Task<TransferCreditResponse> UpdateTransferCredit(TransferCreditRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new TransferCreditRequest();

TransferCreditResponse result = await resellerAccounts.UpdateTransferCredit(body);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="sdk_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.SDKController") SDKController

### Get singleton instance

The singleton instance of the ``` SDKController ``` class can be accessed from the API Client.

```csharp
SDKController sDK = client.SDK;
```

### <a name="get_sdk_download"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SDKController.GetSDKDownload") GetSDKDownload

> TODO: Add a method description


```csharp
Task<dynamic> GetSDKDownload(string type)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| type |  ``` Required ```  | Supported types. |


#### Example Usage

```csharp
string type = "type";

dynamic result = await sDK.GetSDKDownload(type);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="search_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.SearchController") SearchController

### Get singleton instance

The singleton instance of the ``` SearchController ``` class can be accessed from the API Client.

```csharp
SearchController search = client.Search;
```

### <a name="search_contacts_lists"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SearchController.SearchContactsLists") SearchContactsLists

> TODO: Add a method description


```csharp
Task<SearchContactsListsResponse> SearchContactsLists(string q)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| q |  ``` Required ```  | Your keyword or query. |


#### Example Usage

```csharp
string q = "Gorne";

SearchContactsListsResponse result = await search.SearchContactsLists(q);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="sms_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.SMSController") SMSController

### Get singleton instance

The singleton instance of the ``` SMSController ``` class can be accessed from the API Client.

```csharp
SMSController sMS = client.SMS;
```

### <a name="create_send_an_sms"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SMSController.CreateSendAnSMS") CreateSendAnSMS

> You can post **up to 1000 messages** with each API call.


```csharp
Task<SendAnSMSResponse> CreateSendAnSMS(SendAnSMSRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new SendAnSMSRequest();

SendAnSMSResponse result = await sMS.CreateSendAnSMS(body);

```


### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SMSController.CreateCalculatePrice") CreateCalculatePrice

> TODO: Add a method description


```csharp
Task<CalculatePriceResponse> CreateCalculatePrice(CalculatePriceRequest205 body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new CalculatePriceRequest205();

CalculatePriceResponse result = await sMS.CreateCalculatePrice(body);

```


### <a name="get_all_history"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SMSController.GetAllHistory") GetAllHistory

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


```csharp
Task<GetAllHistoryResponse> GetAllHistory(int? dateFrom = null, int? dateTo = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateFrom |  ``` Optional ```  | Timestamp (from) used to show records by date. |
| dateTo |  ``` Optional ```  | Timestamp (to) used to show recrods by date. |


#### Example Usage

```csharp
int? dateFrom = 1449459940;
int? dateTo = 1449659940;

GetAllHistoryResponse result = await sMS.GetAllHistory(dateFrom, dateTo);

```


### <a name="get_export_sms_history"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SMSController.GetExportSMSHistory") GetExportSMSHistory

> TODO: Add a method description


```csharp
Task<ExportSMSHistoryResponse> GetExportSMSHistory()
```

#### Example Usage

```csharp

ExportSMSHistoryResponse result = await sMS.GetExportSMSHistory();

```


### <a name="get_all_delivery_receipts"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SMSController.GetAllDeliveryReceipts") GetAllDeliveryReceipts

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


```csharp
Task<GetAllDeliveryReceiptsResponse> GetAllDeliveryReceipts()
```

#### Example Usage

```csharp

GetAllDeliveryReceiptsResponse result = await sMS.GetAllDeliveryReceipts();

```


### <a name="get_a_specific_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SMSController.GetASpecificDeliveryReceipt") GetASpecificDeliveryReceipt

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


```csharp
Task<GetASpecificDeliveryReceiptResponse> GetASpecificDeliveryReceipt(string messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Your message id. |


#### Example Usage

```csharp
string messageId = "88AB118E EB1B 478C 98CE 6C73ABA23F67";

GetASpecificDeliveryReceiptResponse result = await sMS.GetASpecificDeliveryReceipt(messageId);

```


### <a name="add_a_test_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SMSController.AddATestDeliveryReceipt") AddATestDeliveryReceipt

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


```csharp
Task<AddATestDeliveryReceiptResponse> AddATestDeliveryReceipt(AddATestDeliveryReceiptRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "    {        \"url\":\"http://yourUrl.com\"    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<AddATestDeliveryReceiptRequest>(bodyValue);

AddATestDeliveryReceiptResponse result = await sMS.AddATestDeliveryReceipt(body);

```


### <a name="update_mark_delivery_receipts_as_read"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SMSController.UpdateMarkDeliveryReceiptsAsRead") UpdateMarkDeliveryReceiptsAsRead

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


```csharp
Task<MarkDeliveryReceiptsAsReadResponse> UpdateMarkDeliveryReceiptsAsRead(MarkDeliveryReceiptsAsReadRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "{    \"date_before\": 1441958441}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<MarkDeliveryReceiptsAsReadRequest>(bodyValue);

MarkDeliveryReceiptsAsReadResponse result = await sMS.UpdateMarkDeliveryReceiptsAsRead(body);

```


### <a name="get_all_inbound_sms_pull"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SMSController.GetAllInboundSMSPull") GetAllInboundSMSPull

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


```csharp
Task<GetAllInboundSMSPullResponse> GetAllInboundSMSPull()
```

#### Example Usage

```csharp

GetAllInboundSMSPullResponse result = await sMS.GetAllInboundSMSPull();

```


### <a name="get_specific_inbound_pull"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SMSController.GetSpecificInboundPull") GetSpecificInboundPull

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


```csharp
Task<GetSpecificInboundPullResponse> GetSpecificInboundPull(string messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Message ID. Must be a valid GUID. |


#### Example Usage

```csharp
string messageId = "5D420421-8715-4461-A9A2-C8F569E41835";

GetSpecificInboundPullResponse result = await sMS.GetSpecificInboundPull(messageId);

```


### <a name="add_a_test_inbound_sms"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SMSController.AddATestInboundSMS") AddATestInboundSMS

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


```csharp
Task<AddATestInboundSMSResponse> AddATestInboundSMS(AddATestInboundSMSRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "    {        \"url\":\"http://yourUrl.com\"    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<AddATestInboundSMSRequest>(bodyValue);

AddATestInboundSMSResponse result = await sMS.AddATestInboundSMS(body);

```


### <a name="update_mark_a_specific_inbound_sms_as_read"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SMSController.UpdateMarkASpecificInboundSMSAsRead") UpdateMarkASpecificInboundSMSAsRead

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


```csharp
Task<MarkASpecificInboundSMSAsReadResponse> UpdateMarkASpecificInboundSMSAsRead(string messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | B7CE432193CD-0753597B7293 (string, required) - The message ID you want to mark as read. |


#### Example Usage

```csharp
string messageId = "307EF035";

MarkASpecificInboundSMSAsReadResponse result = await sMS.UpdateMarkASpecificInboundSMSAsRead(messageId);

```


### <a name="update_mark_all_inbound_sms_as_read"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SMSController.UpdateMarkAllInboundSMSAsRead") UpdateMarkAllInboundSMSAsRead

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


```csharp
Task<MarkAllInboundSMSAsReadResponse> UpdateMarkAllInboundSMSAsRead(MarkAllInboundSMSAsReadRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "    {        \"date_before\":1442398100    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<MarkAllInboundSMSAsReadRequest>(bodyValue);

MarkAllInboundSMSAsReadResponse result = await sMS.UpdateMarkAllInboundSMSAsRead(body);

```


### <a name="update_cancel_a_scheduled_message"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SMSController.UpdateCancelAScheduledMessage") UpdateCancelAScheduledMessage

> TODO: Add a method description


```csharp
Task<CancelAScheduledMessageResponse> UpdateCancelAScheduledMessage(string messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | B7CE432193CD-0753597B7293 (string, required) - The message ID you want to cancel. |


#### Example Usage

```csharp
string messageId = "307EF035";

CancelAScheduledMessageResponse result = await sMS.UpdateCancelAScheduledMessage(messageId);

```


### <a name="update_cancel_all_scheduled_messages"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SMSController.UpdateCancelAllScheduledMessages") UpdateCancelAllScheduledMessages

> TODO: Add a method description


```csharp
Task<CancelAllScheduledMessagesResponse> UpdateCancelAllScheduledMessages()
```

#### Example Usage

```csharp

CancelAllScheduledMessagesResponse result = await sMS.UpdateCancelAllScheduledMessages();

```


[Back to List of Controllers](#list_of_controllers)

## <a name="sms_campaigns_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.SMSCampaignsController") SMSCampaignsController

### Get singleton instance

The singleton instance of the ``` SMSCampaignsController ``` class can be accessed from the API Client.

```csharp
SMSCampaignsController sMSCampaigns = client.SMSCampaigns;
```

### <a name="create_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SMSCampaignsController.CreateSMSCampaign") CreateSMSCampaign

> You can post to a list with **up to 20000 recipients** with each API call.


```csharp
Task<CreateSMSCampaignResponse> CreateSMSCampaign(CreateSMSCampaignRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "{    \"list_id\":428,    \"name\":\"My Campaign 1\",    \"from\":\"+61353787448\",    \"body\":\"This is my new campaign message.\",    \"schedule\":1444821615}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<CreateSMSCampaignRequest>(bodyValue);

CreateSMSCampaignResponse result = await sMSCampaigns.CreateSMSCampaign(body);

```


### <a name="create_calculate_price_for_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SMSCampaignsController.CreateCalculatePriceForSMSCampaign") CreateCalculatePriceForSMSCampaign

> TODO: Add a method description


```csharp
Task<CalculatePriceForSMSCampaignResponse> CreateCalculatePriceForSMSCampaign(CalculatePriceForSMSCampaignRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "{    \"list_id\":428,    \"name\":\"My Campaign 1\",    \"from\":\"+61353787448\",    \"body\":\"(First Name), this is your new campaign message.\"}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<CalculatePriceForSMSCampaignRequest>(bodyValue);

CalculatePriceForSMSCampaignResponse result = await sMSCampaigns.CreateCalculatePriceForSMSCampaign(body);

```


### <a name="update_an_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SMSCampaignsController.UpdateAnSMSCampaign") UpdateAnSMSCampaign

> TODO: Add a method description


```csharp
Task<UpdateAnSMSCampaignResponse> UpdateAnSMSCampaign(double smsCampaignId, UpdateAnSMSCampaignRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| smsCampaignId |  ``` Required ```  | Your SMS Campaign id. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
double smsCampaignId = 1;
string bodyValue = "{    \"list_id\":428,    \"name\":\"Awesome campaign.\",    \"from\":\"+61353787447\",    \"body\":\"his is an awesome message.\",    \"schedule\":1444821615}";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<UpdateAnSMSCampaignRequest>(bodyValue);

UpdateAnSMSCampaignResponse result = await sMSCampaigns.UpdateAnSMSCampaign(smsCampaignId, body);

```


### <a name="get_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SMSCampaignsController.GetSMSCampaign") GetSMSCampaign

> TODO: Add a method description


```csharp
Task<GetSMSCampaignResponse> GetSMSCampaign(double smsCampaignId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| smsCampaignId |  ``` Required ```  | Your SMS campaign id. |


#### Example Usage

```csharp
double smsCampaignId = 1;

GetSMSCampaignResponse result = await sMSCampaigns.GetSMSCampaign(smsCampaignId);

```


### <a name="update_cancel_an_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SMSCampaignsController.UpdateCancelAnSMSCampaign") UpdateCancelAnSMSCampaign

> TODO: Add a method description


```csharp
Task<CancelAnSMSCampaignResponse> UpdateCancelAnSMSCampaign(double smsCampaignId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| smsCampaignId |  ``` Required ```  | Your SMS Campaign id. |


#### Example Usage

```csharp
double smsCampaignId = 1;

CancelAnSMSCampaignResponse result = await sMSCampaigns.UpdateCancelAnSMSCampaign(smsCampaignId);

```


### <a name="get_list_of_sms_campaigns"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SMSCampaignsController.GetListOfSMSCampaigns") GetListOfSMSCampaigns

> TODO: Add a method description


```csharp
Task<GetListOfSMSCampaignsResponse> GetListOfSMSCampaigns()
```

#### Example Usage

```csharp

GetListOfSMSCampaignsResponse result = await sMSCampaigns.GetListOfSMSCampaigns();

```


[Back to List of Controllers](#list_of_controllers)

## <a name="sms_templates_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.SMSTemplatesController") SMSTemplatesController

### Get singleton instance

The singleton instance of the ``` SMSTemplatesController ``` class can be accessed from the API Client.

```csharp
SMSTemplatesController sMSTemplates = client.SMSTemplates;
```

### <a name="list_of_templates"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SMSTemplatesController.ListOfTemplates") ListOfTemplates

> Get list of templates.


```csharp
Task<ListOfTemplatesResponse> ListOfTemplates()
```

#### Example Usage

```csharp

ListOfTemplatesResponse result = await sMSTemplates.ListOfTemplates();

```


### <a name="create_a_template"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SMSTemplatesController.CreateATemplate") CreateATemplate

> Create new template.


```csharp
Task<CreateATemplateResponse> CreateATemplate(CreateATemplateRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "    {        \"template_name\":\"Template 501916\",        \"body\":\"This is a sample content: H7YI68B3yk for this template.\"    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<CreateATemplateRequest>(bodyValue);

CreateATemplateResponse result = await sMSTemplates.CreateATemplate(body);

```


### <a name="update_a_template"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SMSTemplatesController.UpdateATemplate") UpdateATemplate

> TODO: Add a method description


```csharp
Task<UpdateATemplateResponse> UpdateATemplate(string templateId, UpdateATemplateRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string templateId = "25";
string bodyValue = "    {        \"template_name\":\"I am updated\",        \"body\":\"This is a sample content: Sc0KNWgSMG for this template.\"    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<UpdateATemplateRequest>(bodyValue);

UpdateATemplateResponse result = await sMSTemplates.UpdateATemplate(templateId, body);

```


### <a name="delete_a_template"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SMSTemplatesController.DeleteATemplate") DeleteATemplate

> TODO: Add a method description


```csharp
Task<DeleteATemplateResponse> DeleteATemplate(string templateId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |


#### Example Usage

```csharp
string templateId = "25";

DeleteATemplateResponse result = await sMSTemplates.DeleteATemplate(templateId);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="statistics_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.StatisticsController") StatisticsController

### Get singleton instance

The singleton instance of the ``` StatisticsController ``` class can be accessed from the API Client.

```csharp
StatisticsController statistics = client.Statistics;
```

### <a name="get_sms_statistics"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.StatisticsController.GetSMSStatistics") GetSMSStatistics

> TODO: Add a method description


```csharp
Task<GetSMSStatisticsResponse> GetSMSStatistics()
```

#### Example Usage

```csharp

GetSMSStatisticsResponse result = await statistics.GetSMSStatistics();

```


### <a name="get_voice_statistics"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.StatisticsController.GetVoiceStatistics") GetVoiceStatistics

> TODO: Add a method description


```csharp
Task<GetVoiceStatisticsResponse> GetVoiceStatistics()
```

#### Example Usage

```csharp

GetVoiceStatisticsResponse result = await statistics.GetVoiceStatistics();

```


[Back to List of Controllers](#list_of_controllers)

## <a name="subaccounts_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.SubaccountsController") SubaccountsController

### Get singleton instance

The singleton instance of the ``` SubaccountsController ``` class can be accessed from the API Client.

```csharp
SubaccountsController subaccounts = client.Subaccounts;
```

### <a name="get_all_subaccounts"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SubaccountsController.GetAllSubaccounts") GetAllSubaccounts

> TODO: Add a method description


```csharp
Task<GetAllSubaccountsResponse> GetAllSubaccounts()
```

#### Example Usage

```csharp

GetAllSubaccountsResponse result = await subaccounts.GetAllSubaccounts();

```


### <a name="create_a_new_subaccount"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SubaccountsController.CreateANewSubaccount") CreateANewSubaccount

> TODO: Add a method description


```csharp
Task<CreateANewSubaccountResponse> CreateANewSubaccount(CreateANewSubaccountRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "    {        \"api_username\":\"nameP99\",        \"password\":\"pass\",        \"email\":\"testvrq@gmail.com\",        \"phone_number\":\"941-751-3278\",        \"first_name\":\"FirstnameeGPqV\",        \"last_name\":\"LastnamePvjJp\"    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<CreateANewSubaccountRequest>(bodyValue);

CreateANewSubaccountResponse result = await subaccounts.CreateANewSubaccount(body);

```


### <a name="get_a_specific_subaccount"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SubaccountsController.GetASpecificSubaccount") GetASpecificSubaccount

> TODO: Add a method description


```csharp
Task<GetASpecificSubaccountResponse> GetASpecificSubaccount(double subaccountId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |


#### Example Usage

```csharp
double subaccountId = 59;

GetASpecificSubaccountResponse result = await subaccounts.GetASpecificSubaccount(subaccountId);

```


### <a name="update_a_specific_subaccount"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SubaccountsController.UpdateASpecificSubaccount") UpdateASpecificSubaccount

> TODO: Add a method description


```csharp
Task<UpdateASpecificSubaccountResponse> UpdateASpecificSubaccount(double subaccountId, UpdateASpecificSubaccountRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
double subaccountId = 59;
string bodyValue = "    {        \"password\":\"pass\",        \"email\":\"testfP0.updated@gmail.com\",        \"phone_number\":\"+19417519130\",        \"first_name\":\"FirstnameKvdRZUpdated\",        \"last_name\":\"LastnameHUPYGUpdated\",        \"access_users\": 1,        \"access_billing\": 1,        \"access_reporting\": 1,        \"access_contacts\": 1,        \"access_settings\": 1,        \"access_sms\": 1,        \"access_email\": 1,        \"access_voice\": 1,        \"access_fax\": 1,        \"access_post\": 1,        \"access_reseller\": 1,        \"access_mms\": 1,        \"share_campaigns\": 0,        \"notes\": null    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<UpdateASpecificSubaccountRequest>(bodyValue);

UpdateASpecificSubaccountResponse result = await subaccounts.UpdateASpecificSubaccount(subaccountId, body);

```


### <a name="delete_a_specific_subaccount"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SubaccountsController.DeleteASpecificSubaccount") DeleteASpecificSubaccount

> TODO: Add a method description


```csharp
Task<DeleteASpecificSubaccountResponse> DeleteASpecificSubaccount(double subaccountId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |


#### Example Usage

```csharp
double subaccountId = 59;

DeleteASpecificSubaccountResponse result = await subaccounts.DeleteASpecificSubaccount(subaccountId);

```


### <a name="update_regenerate_api_key"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.SubaccountsController.UpdateRegenerateAPIKey") UpdateRegenerateAPIKey

> TODO: Add a method description


```csharp
Task<RegenerateAPIKeyResponse> UpdateRegenerateAPIKey(double subaccountId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |


#### Example Usage

```csharp
double subaccountId = 59;

RegenerateAPIKeyResponse result = await subaccounts.UpdateRegenerateAPIKey(subaccountId);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="timezones_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.TimezonesController") TimezonesController

### Get singleton instance

The singleton instance of the ``` TimezonesController ``` class can be accessed from the API Client.

```csharp
TimezonesController timezones = client.Timezones;
```

### <a name="get_timezones"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.TimezonesController.GetTimezones") GetTimezones

> Get supported list of timezones.


```csharp
Task<GetTimezonesResponse> GetTimezones()
```

#### Example Usage

```csharp

GetTimezonesResponse result = await timezones.GetTimezones();

```


[Back to List of Controllers](#list_of_controllers)

## <a name="transactional_email_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.TransactionalEmailController") TransactionalEmailController

### Get singleton instance

The singleton instance of the ``` TransactionalEmailController ``` class can be accessed from the API Client.

```csharp
TransactionalEmailController transactionalEmail = client.TransactionalEmail;
```

### <a name="create_email_send"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.TransactionalEmailController.CreateEmailSend") CreateEmailSend

> TODO: Add a method description


```csharp
Task<EmailSendResponse> CreateEmailSend(EmailSendRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new EmailSendRequest();

EmailSendResponse result = await transactionalEmail.CreateEmailSend(body);

```


### <a name="create_email_price"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.TransactionalEmailController.CreateEmailPrice") CreateEmailPrice

> TODO: Add a method description


```csharp
Task<EmailPriceResponse> CreateEmailPrice(EmailPriceRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new EmailPriceRequest();

EmailPriceResponse result = await transactionalEmail.CreateEmailPrice(body);

```


### <a name="get_email_history"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.TransactionalEmailController.GetEmailHistory") GetEmailHistory

> TODO: Add a method description


```csharp
Task<EmailHistoryResponse> GetEmailHistory()
```

#### Example Usage

```csharp

EmailHistoryResponse result = await transactionalEmail.GetEmailHistory();

```


### <a name="get_export_history"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.TransactionalEmailController.GetExportHistory") GetExportHistory

> TODO: Add a method description


```csharp
Task<ExportHistoryResponse> GetExportHistory(string filename)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | File name for the export file. |


#### Example Usage

```csharp
string filename = "myexport.csv";

ExportHistoryResponse result = await transactionalEmail.GetExportHistory(filename);

```


### <a name="add_a_test_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.TransactionalEmailController.AddATestDeliveryReceipt") AddATestDeliveryReceipt

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


```csharp
Task<AddATestDeliveryReceiptResponse> AddATestDeliveryReceipt(AddATestDeliveryReceiptRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "    {        \"url\":\"http://yourUrl.com\"    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<AddATestDeliveryReceiptRequest>(bodyValue);

AddATestDeliveryReceiptResponse result = await transactionalEmail.AddATestDeliveryReceipt(body);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="uploads_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.UploadsController") UploadsController

### Get singleton instance

The singleton instance of the ``` UploadsController ``` class can be accessed from the API Client.

```csharp
UploadsController uploads = client.Uploads;
```

### <a name="upload_a_file"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.UploadsController.UploadAFile") UploadAFile

> The `upload` endpoint provides a method for converting files from an unspported format to a format that one of our endpoints can handle.
> Files can be submitted two ways:
> 1. Using `base64` encoding in an `application/json` request. In this case, submit the `base64`-encoded file contents in the `content` field of the request body, and `convert` can be specified either also in the body or as part of the query string.
> 2. Using `multipart/form-data` encoding, in the same way it would be submitted using a HTML form. You may find cURL useful for this. For an example of how to do this, see one of our [SDKs](https://dashboard.clicksend.com/#/libraries-sdk/main). In this case, specify `convert` in the query string.
> Note that `convert` specifies the conversion to take place - that is, what the result should be compatible with - and can be any of `fax`, `mms`, `csv` or `post`.
> All files have 10 minutes expiry.


```csharp
Task<UploadAFileResponse> UploadAFile(UploadAFileRequest body, string convert = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |
| convert |  ``` Optional ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new UploadAFileRequest();
string convert = "convert";

UploadAFileResponse result = await uploads.UploadAFile(body, convert);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="voice_controller"></a>![Class: ](https://apidocs.io/img/class.png "ClickSendRESTAPIV3.Tests.Controllers.VoiceController") VoiceController

### Get singleton instance

The singleton instance of the ``` VoiceController ``` class can be accessed from the API Client.

```csharp
VoiceController voice = client.Voice;
```

### <a name="create_send_a_voice_call"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.VoiceController.CreateSendAVoiceCall") CreateSendAVoiceCall

> You can post **up to 1000 messages** with each API call.


```csharp
Task<SendAVoiceCallResponse> CreateSendAVoiceCall(SendAVoiceCallRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new SendAVoiceCallRequest();

SendAVoiceCallResponse result = await voice.CreateSendAVoiceCall(body);

```


### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.VoiceController.CreateCalculatePrice") CreateCalculatePrice

> TODO: Add a method description


```csharp
Task<CalculatePriceResponse> CreateCalculatePrice(CalculatePriceRequest263 body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new CalculatePriceRequest263();

CalculatePriceResponse result = await voice.CreateCalculatePrice(body);

```


### <a name="get_voice_languages"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.VoiceController.GetVoiceLanguages") GetVoiceLanguages

> TODO: Add a method description


```csharp
Task<VoiceLanguagesResponse> GetVoiceLanguages()
```

#### Example Usage

```csharp

VoiceLanguagesResponse result = await voice.GetVoiceLanguages();

```


### <a name="get_voice_history"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.VoiceController.GetVoiceHistory") GetVoiceHistory

> TODO: Add a method description


```csharp
Task<GetVoiceHistoryResponse> GetVoiceHistory(int? dateFrom = null, int? dateTo = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateFrom |  ``` Optional ```  | Timestamp (from) used to show records by date. |
| dateTo |  ``` Optional ```  | Timestamp (to) used to show recrods by date. |


#### Example Usage

```csharp
int? dateFrom = 1443501617;
int? dateTo = 1443501727;

GetVoiceHistoryResponse result = await voice.GetVoiceHistory(dateFrom, dateTo);

```


### <a name="get_export_voice_history"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.VoiceController.GetExportVoiceHistory") GetExportVoiceHistory

> TODO: Add a method description


```csharp
Task<ExportVoiceHistoryResponse> GetExportVoiceHistory()
```

#### Example Usage

```csharp

ExportVoiceHistoryResponse result = await voice.GetExportVoiceHistory();

```


### <a name="get_voice_receipts"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.VoiceController.GetVoiceReceipts") GetVoiceReceipts

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


```csharp
Task<GetVoiceReceiptsResponse> GetVoiceReceipts()
```

#### Example Usage

```csharp

GetVoiceReceiptsResponse result = await voice.GetVoiceReceipts();

```


### <a name="add_a_test_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.VoiceController.AddATestDeliveryReceipt") AddATestDeliveryReceipt

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


```csharp
Task<AddATestDeliveryReceiptResponse> AddATestDeliveryReceipt(AddATestDeliveryReceiptRequest body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string bodyValue = "    {        \"url\":\"http://yourUrl.com\"    }";
var body = Newtonsoft.Json.JsonConvert.DeserializeObject<AddATestDeliveryReceiptRequest>(bodyValue);

AddATestDeliveryReceiptResponse result = await voice.AddATestDeliveryReceipt(body);

```


### <a name="get_specific_voice_receipt"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.VoiceController.GetSpecificVoiceReceipt") GetSpecificVoiceReceipt

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


```csharp
Task<GetSpecificVoiceReceiptResponse> GetSpecificVoiceReceipt(string messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | 3055-45F1-9B79-F2C43509FD16 (string, required) - The voice receipt message id. |


#### Example Usage

```csharp
string messageId = "28DD2718";

GetSpecificVoiceReceiptResponse result = await voice.GetSpecificVoiceReceipt(messageId);

```


### <a name="update_marked_voice_receipts_as_read"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.VoiceController.UpdateMarkedVoiceReceiptsAsRead") UpdateMarkedVoiceReceiptsAsRead

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


```csharp
Task<MarkedVoiceReceiptsAsReadResponse> UpdateMarkedVoiceReceiptsAsRead(double dateBefore)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateBefore |  ``` Required ```  | An optional timestamp - mark all as read before this timestamp. If not given, all receipts will be marked as read. |


#### Example Usage

```csharp
double dateBefore = 250.23963728698;

MarkedVoiceReceiptsAsReadResponse result = await voice.UpdateMarkedVoiceReceiptsAsRead(dateBefore);

```


### <a name="update_cancel_a_specific_voice_call"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.VoiceController.UpdateCancelASpecificVoiceCall") UpdateCancelASpecificVoiceCall

> TODO: Add a method description


```csharp
Task<CancelASpecificVoiceCallResponse> UpdateCancelASpecificVoiceCall(string messageId)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Your voice message id. |


#### Example Usage

```csharp
string messageId = "7B5BFC19 06B7 49C1 8DCDFB011600E12B";

CancelASpecificVoiceCallResponse result = await voice.UpdateCancelASpecificVoiceCall(messageId);

```


### <a name="update_cancel_all_voice_calls"></a>![Method: ](https://apidocs.io/img/method.png "ClickSendRESTAPIV3.Tests.Controllers.VoiceController.UpdateCancelAllVoiceCalls") UpdateCancelAllVoiceCalls

> TODO: Add a method description


```csharp
Task<CancelAllVoiceCallsResponse> UpdateCancelAllVoiceCalls()
```

#### Example Usage

```csharp

CancelAllVoiceCallsResponse result = await voice.UpdateCancelAllVoiceCalls();

```


[Back to List of Controllers](#list_of_controllers)



