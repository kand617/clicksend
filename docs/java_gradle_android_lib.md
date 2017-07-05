# Getting started

TODO: Add a description

## How to Build

The generated code uses a few Gradle dependencies e.g., Jackson, Volley,
and Apache HttpClient. The reference to these dependencies is already
added in the build.gradle file will be installed automatically. Therefore,
you will need internet access for a successful build.

* In order to open the client library in Android Studio click on ``` Open an Existing Android Project ```.

![Importing SDK into Android Studio - Step 1](https://apidocs.io/illustration/android?step=import1&workspaceFolder=ClickSend%20REST%20API%20v3&workspaceName=ClickSendRESTAPIV3Lib&projectName=ClickSendRESTAPIV3Lib&rootNamespace=com.clicksend.rest)

* Browse to locate the folder containing the source code. Select the location of the ClickSendRESTAPIV3Lib gradle project and click ``` Ok ```.

![Importing SDK into Android Studio - Step 2](https://apidocs.io/illustration/android?step=import2&workspaceFolder=ClickSend%20REST%20API%20v3&workspaceName=ClickSendRESTAPIV3Lib&projectName=ClickSendRESTAPIV3Lib&rootNamespace=com.clicksend.rest)

* Upon successful import, the project can be built by clicking on ``` Build > Make Project ``` or  pressing ``` Ctrl + F9 ```.

![Importing SDK into Android Studio - Step 3](https://apidocs.io/illustration/android?step=import3&workspaceFolder=ClickSend%20REST%20API%20v3&workspaceName=ClickSendRESTAPIV3Lib&projectName=ClickSendRESTAPIV3Lib&rootNamespace=com.clicksend.rest)

## How to Use

The following section explains how to use the ClickSendRESTAPIV3Lib library in a new project.

### 1. Starting a new project 

For starting a new project, click on ``` Create New Android Studio Project ```.

![Add a new project in Android Studio - Step 1](https://apidocs.io/illustration/android?step=createNewProject0&workspaceFolder=ClickSend%20REST%20API%20v3&workspaceName=ClickSendRESTAPIV3Lib&projectName=ClickSendRESTAPIV3Lib&rootNamespace=com.clicksend.rest)

Here, configure the new project by adding the name, domain and location of the sample application followed by clicking ``` Next ```.

![Create a new Android Studio Project - Step 2](https://apidocs.io/illustration/android?step=createNewProject1&workspaceFolder=ClickSend%20REST%20API%20v3&workspaceName=ClickSendRESTAPIV3Lib&projectName=ClickSendRESTAPIV3Lib&rootNamespace=com.clicksend.rest)

Following this, select the ``` Phone and Tablet ```` option as shown in the illustration below and click ``` Next ```. 

![Create a new Android Studio Project - Step 3](https://apidocs.io/illustration/android?step=createNewProject2&workspaceFolder=ClickSend%20REST%20API%20v3&workspaceName=ClickSendRESTAPIV3Lib&projectName=ClickSendRESTAPIV3Lib&rootNamespace=com.clicksend.rest)

In the following step, choose ``` Empty Activity ``` as the activity type and click ``` Next ```.

![Create a new Android Studio Project - Step 4](https://apidocs.io/illustration/android?step=createNewProject3&workspaceFolder=ClickSend%20REST%20API%20v3&workspaceName=ClickSendRESTAPIV3Lib&projectName=ClickSendRESTAPIV3Lib&rootNamespace=com.clicksend.rest)

In this step, provide an ``` Activity Name ``` and ``` Layout Name ``` and click ``` Finish ```.  This would take you to the newly created project.

![Create a new Android Studio Project - Step 4](https://apidocs.io/illustration/android?step=createNewProject4&workspaceFolder=ClickSend%20REST%20API%20v3&workspaceName=ClickSendRESTAPIV3Lib&projectName=ClickSendRESTAPIV3Lib&rootNamespace=com.clicksend.rest)

### 2. Add reference of the library project

In order to add a dependency to this sample application, click on the android button shown in the project explorer on the left side as shown in the picture. Click on ``` Project ``` in the drop down that emerges.  

![Adding dependency to the client library - Step 1](https://apidocs.io/illustration/android?step=testProject0&workspaceFolder=ClickSend%20REST%20API%20v3&workspaceName=ClickSendRESTAPIV3Lib&projectName=ClickSendRESTAPIV3Lib&rootNamespace=com.clicksend.rest)

Right click the sample application in the project explorer and click on ``` New > Module ```  as shown in the picture.

![Adding dependency to the client library - Step 2](https://apidocs.io/illustration/android?step=testProject1&workspaceFolder=ClickSend%20REST%20API%20v3&workspaceName=ClickSendRESTAPIV3Lib&projectName=ClickSendRESTAPIV3Lib&rootNamespace=com.clicksend.rest)

Choose ``` Import Gradle Project ``` and click ``` Next ```.

![Adding dependency to the client library - Step 3](https://apidocs.io/illustration/android?step=testProject2&workspaceFolder=ClickSend%20REST%20API%20v3&workspaceName=ClickSendRESTAPIV3Lib&projectName=ClickSendRESTAPIV3Lib&rootNamespace=com.clicksend.rest)

Click on ``` Finish ``` which would take you back to the sample application with the refernced SDK. 

![Adding dependency to the client library - Step 4](https://apidocs.io/illustration/android?step=testProject3&workspaceFolder=ClickSend%20REST%20API%20v3&workspaceName=ClickSendRESTAPIV3Lib&projectName=ClickSendRESTAPIV3Lib&rootNamespace=com.clicksend.rest)

In the following step naigate to the ``` SampleApplication >  app > build.gradle ``` file and add the following line ```compile project(path: ':ClickSendRESTAPIV3Lib')``` to the dependencies section as shown in the illustration below.

![Adding dependency to the client library - Step 5](https://apidocs.io/illustration/android?step=testProject4&workspaceFolder=ClickSend%20REST%20API%20v3&workspaceName=ClickSendRESTAPIV3Lib&projectName=ClickSendRESTAPIV3Lib&rootNamespace=com.clicksend.rest)

Finally, press ``` Sync Now ``` in the warning visible as shown in the picture below.

![Adding dependency to the client library - Step 6](https://apidocs.io/illustration/android?step=testProject5&workspaceFolder=ClickSend%20REST%20API%20v3&workspaceName=ClickSendRESTAPIV3Lib&projectName=ClickSendRESTAPIV3Lib&rootNamespace=com.clicksend.rest)

### 3. Write sample code

Once the ``` SampleApplication ``` is created, a file named ``` SampleApplication > app > src > main > java > MainActivity ``` will be visible in the *Project Explorer* with an ``` onCreate ``` method. This is the entry point for the execution of the created project.
Here, you can add code to initialize the client library and instantiate a *Controller* class. Sample code to initialize the client library and using controller methods is given in the subsequent sections.

## How to Test

The generated code and the server can be tested using automatically generated test cases. 
JUnit is used as the testing framework and test runner.

In Android Studio, for running the tests do the following:

1. Right click on *SampleApplication > ClickSendRESTAPIV3Lib > androidTest > java)* from the project explorer.
2. Select "Run All Tests" or use "Ctrl + Shift + F10" to run the Tests.

## Initialization

### Authentication
In order to setup authentication and initialization of the API client, you need the following information.

| Parameter | Description |
|-----------|-------------|
| basicAuthUserName | The username to use with basic authentication |
| basicAuthPassword | The password to use with basic authentication |



API client can be initialized as following. The `appContext` being passed is the Android application [`Context`](https://developer.android.com/reference/android/content/Context.html).

```java
// Configuration parameters and credentials
String basicAuthUserName = "basicAuthUserName"; // The username to use with basic authentication
String basicAuthPassword = "basicAuthPassword"; // The password to use with basic authentication

com.clicksend.rest.Configuration.initialize(appContext);
ClickSendRESTAPIV3LibClient client = new ClickSendRESTAPIV3LibClient(basicAuthUserName, basicAuthPassword);
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

## <a name="account_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.AccountController") AccountController

### Get singleton instance

The singleton instance of the ``` AccountController ``` class can be accessed from the API Client.

```java
AccountController account = client.getAccount();
```

### <a name="create_a_new_account_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AccountController.createANewAccountAsync") createANewAccountAsync

> **Note:** *Authentication isn't required to create a new account.*


```java
void createANewAccountAsync(
        final CreateANewAccountRequest body,
        final APICallBack<CreateANewAccountResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "    {        \"username\":\"johndoe1\",        \"user_email\":\"johndoe1@awesome.com\",        \"user_phone\":\"518-481-1001\",        \"user_first_name\":\"John\",        \"user_last_name\":\"Doe\",        \"country\":\"US\",        \"password\":\"pass\",        \"account_name\":\"The Awesome Company\"    }";
    CreateANewAccountRequest body = mapper.readValue(bodyValue,new TypeReference<CreateANewAccountRequest> (){});
    // Invoking the API call with sample inputs
    account.createANewAccountAsync(body, new APICallBack<CreateANewAccountResponse>() {
        public void onSuccess(HttpContext context, CreateANewAccountResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="update_account_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AccountController.updateAccountAsync") updateAccountAsync

> TODO: Add a method description


```java
void updateAccountAsync(
        final UpdateAccountRequest body,
        final APICallBack<UpdateAccountResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "    {        \"username\":\"johndoe\",        \"user_email\":\"johndoe@awesome.com\",        \"user_phone\":\"518-481-1002\",        \"user_first_name\":\"John\",        \"user_last_name\":\"Doe\",        \"country\":\"AU\",        \"password\":\"pass\",        \"account_name\":\"The Awesome Company\",        \"timezone\": \"Australia/Melbourne\",        \"private_uploads\": 1,        \"setting_sms_hide_your_number\": 0,        \"setting_sms_hide_business_name\": 1    }";
    UpdateAccountRequest body = mapper.readValue(bodyValue,new TypeReference<UpdateAccountRequest> (){});
    // Invoking the API call with sample inputs
    account.updateAccountAsync(body, new APICallBack<UpdateAccountResponse>() {
        public void onSuccess(HttpContext context, UpdateAccountResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="get_account_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AccountController.getAccountAsync") getAccountAsync

> TODO: Add a method description


```java
void getAccountAsync(final APICallBack<GetAccountResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
account.getAccountAsync(new APICallBack<GetAccountResponse>() {
    public void onSuccess(HttpContext context, GetAccountResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_account_usage_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AccountController.getAccountUsageAsync") getAccountUsageAsync

> TODO: Add a method description


```java
void getAccountUsageAsync(
        final double year,
        final double month,
        final String type,
        final APICallBack<AccountUsageResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| year |  ``` Required ```  | Your account usage year. |
| month |  ``` Required ```  | Your account usage month. |
| type |  ``` Required ```  | The account type. Value can only be either email or subaccount. |


#### Example Usage

```java
double year = 2016;
double month = 4;
String type = "subaccount";
// Invoking the API call with sample inputs
account.getAccountUsageAsync(year, month, type, new APICallBack<AccountUsageResponse>() {
    public void onSuccess(HttpContext context, AccountUsageResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="update_send_account_activation_token_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AccountController.updateSendAccountActivationTokenAsync") updateSendAccountActivationTokenAsync

> TODO: Add a method description


```java
void updateSendAccountActivationTokenAsync(
        final SendAccountActivationTokenRequest body,
        final APICallBack<SendAccountActivationTokenResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "    {        \"user_phone\":\"352-394-4199\",        \"type\":\"sms\",        \"country\": \"US\"    }";
    SendAccountActivationTokenRequest body = mapper.readValue(bodyValue,new TypeReference<SendAccountActivationTokenRequest> (){});
    // Invoking the API call with sample inputs
    account.updateSendAccountActivationTokenAsync(body, new APICallBack<SendAccountActivationTokenResponse>() {
        public void onSuccess(HttpContext context, SendAccountActivationTokenResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="update_verify_new_account_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AccountController.updateVerifyNewAccountAsync") updateVerifyNewAccountAsync

> TODO: Add a method description


```java
void updateVerifyNewAccountAsync(
        final String activationToken,
        final APICallBack<VerifyNewAccountResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| activationToken |  ``` Required ```  | The ActivationToken to be used to verify an account. |


#### Example Usage

```java
String activationToken = "1827364";
// Invoking the API call with sample inputs
account.updateVerifyNewAccountAsync(activationToken, new APICallBack<VerifyNewAccountResponse>() {
    public void onSuccess(HttpContext context, VerifyNewAccountResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="account_recharge_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.AccountRechargeController") AccountRechargeController

### Get singleton instance

The singleton instance of the ``` AccountRechargeController ``` class can be accessed from the API Client.

```java
AccountRechargeController accountRecharge = client.getAccountRecharge();
```

### <a name="get_credit_card_info_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AccountRechargeController.getCreditCardInfoAsync") getCreditCardInfoAsync

> TODO: Add a method description


```java
void getCreditCardInfoAsync(final APICallBack<GetCreditCardInfoResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
accountRecharge.getCreditCardInfoAsync(new APICallBack<GetCreditCardInfoResponse>() {
    public void onSuccess(HttpContext context, GetCreditCardInfoResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="update_credit_card_info_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AccountRechargeController.updateCreditCardInfoAsync") updateCreditCardInfoAsync

> TODO: Add a method description


```java
void updateCreditCardInfoAsync(
        final UpdateCreditCardInfoRequest body,
        final APICallBack<UpdateCreditCardInfoResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    UpdateCreditCardInfoRequest body = new UpdateCreditCardInfoRequest();
    // Invoking the API call with sample inputs
    accountRecharge.updateCreditCardInfoAsync(body, new APICallBack<UpdateCreditCardInfoResponse>() {
        public void onSuccess(HttpContext context, UpdateCreditCardInfoResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="list_of_packages_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AccountRechargeController.listOfPackagesAsync") listOfPackagesAsync

> TODO: Add a method description


```java
void listOfPackagesAsync(
        final String country,
        final APICallBack<ListOfPackagesResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Optional ```  | Your country. |


#### Example Usage

```java
String country = "\"AU\"";
// Invoking the API call with sample inputs
accountRecharge.listOfPackagesAsync(country, new APICallBack<ListOfPackagesResponse>() {
    public void onSuccess(HttpContext context, ListOfPackagesResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="update_purchase_a_package_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AccountRechargeController.updatePurchaseAPackageAsync") updatePurchaseAPackageAsync

> TODO: Add a method description


```java
void updatePurchaseAPackageAsync(
        final double packageId,
        final APICallBack<PurchaseAPackageResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| packageId |  ``` Required ```  | Your package id. |


#### Example Usage

```java
double packageId = 1;
// Invoking the API call with sample inputs
accountRecharge.updatePurchaseAPackageAsync(packageId, new APICallBack<PurchaseAPackageResponse>() {
    public void onSuccess(HttpContext context, PurchaseAPackageResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_transactions_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AccountRechargeController.getTransactionsAsync") getTransactionsAsync

> TODO: Add a method description


```java
void getTransactionsAsync(final APICallBack<GetTransactionsResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
accountRecharge.getTransactionsAsync(new APICallBack<GetTransactionsResponse>() {
    public void onSuccess(HttpContext context, GetTransactionsResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_a_specific_transaction_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AccountRechargeController.getASpecificTransactionAsync") getASpecificTransactionAsync

> TODO: Add a method description


```java
void getASpecificTransactionAsync(
        final String transactionId,
        final APICallBack<InputStream> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| transactionId |  ``` Required ```  | 1c65-47fa-aea2-3ded9ed57557 (number, required) - Your transction id. |


#### Example Usage

```java
String transactionId = "transaction_id";
// Invoking the API call with sample inputs
accountRecharge.getASpecificTransactionAsync(transactionId, new APICallBack<InputStream>() {
    public void onSuccess(HttpContext context, InputStream response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="automation_rules_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.AutomationRulesController") AutomationRulesController

### Get singleton instance

The singleton instance of the ``` AutomationRulesController ``` class can be accessed from the API Client.

```java
AutomationRulesController automationRules = client.getAutomationRules();
```

### <a name="list_rules_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.listRulesAsync") listRulesAsync

> TODO: Add a method description


```java
void listRulesAsync(final APICallBack<ListRulesResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
automationRules.listRulesAsync(new APICallBack<ListRulesResponse>() {
    public void onSuccess(HttpContext context, ListRulesResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_a_specific_rule_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.getASpecificRuleAsync") getASpecificRuleAsync

> TODO: Add a method description


```java
void getASpecificRuleAsync(
        final double inboundRuleId,
        final APICallBack<GetASpecificRuleResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Inbound Rule ID. |


#### Example Usage

```java
double inboundRuleId = 1;
// Invoking the API call with sample inputs
automationRules.getASpecificRuleAsync(inboundRuleId, new APICallBack<GetASpecificRuleResponse>() {
    public void onSuccess(HttpContext context, GetASpecificRuleResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_a_new_rule_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.createANewRuleAsync") createANewRuleAsync

> TODO: Add a method description


```java
void createANewRuleAsync(
        final CreateANewRuleRequest body,
        final APICallBack<CreateANewRuleResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    CreateANewRuleRequest body = new CreateANewRuleRequest();
    // Invoking the API call with sample inputs
    automationRules.createANewRuleAsync(body, new APICallBack<CreateANewRuleResponse>() {
        public void onSuccess(HttpContext context, CreateANewRuleResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="update_a_rule_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.updateARuleAsync") updateARuleAsync

> TODO: Add a method description


```java
void updateARuleAsync(
        final double inboundRuleId,
        final UpdateARuleRequest body,
        final APICallBack<UpdateARuleResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Inbound Rule ID. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    double inboundRuleId = 1;
    String bodyValue = "{    \"dedicated_number\":\"+61298441484\",    \"rule_name\":\"My Rule\",    \"message_search_type\":3,    \"message_search_term\":\"My Search Term\",    \"action\":\"EMAIL_FIXED\",    \"action_address\":\"john@doe.com\",    \"enabled\":1}";
    UpdateARuleRequest body = mapper.readValue(bodyValue,new TypeReference<UpdateARuleRequest> (){});
    // Invoking the API call with sample inputs
    automationRules.updateARuleAsync(inboundRuleId, body, new APICallBack<UpdateARuleResponse>() {
        public void onSuccess(HttpContext context, UpdateARuleResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="delete_a_rule_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.deleteARuleAsync") deleteARuleAsync

> TODO: Add a method description


```java
void deleteARuleAsync(
        final double inboundRuleId,
        final APICallBack<DeleteARuleResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Inbound Rule ID. |


#### Example Usage

```java
double inboundRuleId = 1;
// Invoking the API call with sample inputs
automationRules.deleteARuleAsync(inboundRuleId, new APICallBack<DeleteARuleResponse>() {
    public void onSuccess(HttpContext context, DeleteARuleResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="list_rules1_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.listRules1Async") listRules1Async

> TODO: Add a method description


```java
void listRules1Async(final APICallBack<ListRulesResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
automationRules.listRules1Async(new APICallBack<ListRulesResponse>() {
    public void onSuccess(HttpContext context, ListRulesResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_a_specific_rule1_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.getASpecificRule1Async") getASpecificRule1Async

> TODO: Add a method description


```java
void getASpecificRule1Async(
        final double receiptRuleId,
        final APICallBack<GetASpecificRuleResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |


#### Example Usage

```java
double receiptRuleId = 2;
// Invoking the API call with sample inputs
automationRules.getASpecificRule1Async(receiptRuleId, new APICallBack<GetASpecificRuleResponse>() {
    public void onSuccess(HttpContext context, GetASpecificRuleResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_a_new_rule1_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.createANewRule1Async") createANewRule1Async

> TODO: Add a method description


```java
void createANewRule1Async(
        final CreateANewRuleRequest24 body,
        final APICallBack<CreateANewRuleResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "{    \"rule_name\": \"My Rule\",    \"match_type\": 3,    \"action\": \"EMAIL_FIXED\",    \"action_address\": \"john@doe.com\",    \"enabled\": 1}";
    CreateANewRuleRequest24 body = mapper.readValue(bodyValue,new TypeReference<CreateANewRuleRequest24> (){});
    // Invoking the API call with sample inputs
    automationRules.createANewRule1Async(body, new APICallBack<CreateANewRuleResponse>() {
        public void onSuccess(HttpContext context, CreateANewRuleResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="update_a_rule1_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.updateARule1Async") updateARule1Async

> TODO: Add a method description


```java
void updateARule1Async(
        final double receiptRuleId,
        final UpdateARuleRequest26 body,
        final APICallBack<UpdateARuleResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    double receiptRuleId = 7;
    String bodyValue = "{    \"rule_name\": \"My Rule\",    \"match_type\": 3,    \"action\": \"EMAIL_FIXED\",    \"action_address\": \"john@doe.com\",    \"enabled\": 1}";
    UpdateARuleRequest26 body = mapper.readValue(bodyValue,new TypeReference<UpdateARuleRequest26> (){});
    // Invoking the API call with sample inputs
    automationRules.updateARule1Async(receiptRuleId, body, new APICallBack<UpdateARuleResponse>() {
        public void onSuccess(HttpContext context, UpdateARuleResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="delete_a_rule1_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.deleteARule1Async") deleteARule1Async

> TODO: Add a method description


```java
void deleteARule1Async(
        final double receiptRuleId,
        final APICallBack<DeleteARuleResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |


#### Example Usage

```java
double receiptRuleId = 7;
// Invoking the API call with sample inputs
automationRules.deleteARule1Async(receiptRuleId, new APICallBack<DeleteARuleResponse>() {
    public void onSuccess(HttpContext context, DeleteARuleResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="list_rules2_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.listRules2Async") listRules2Async

> TODO: Add a method description


```java
void listRules2Async(final APICallBack<ListRulesResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
automationRules.listRules2Async(new APICallBack<ListRulesResponse>() {
    public void onSuccess(HttpContext context, ListRulesResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_a_specific_rule11_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.getASpecificRule11Async") getASpecificRule11Async

> TODO: Add a method description


```java
void getASpecificRule11Async(
        final double receiptRuleId,
        final APICallBack<GetASpecificRuleResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |


#### Example Usage

```java
double receiptRuleId = 2;
// Invoking the API call with sample inputs
automationRules.getASpecificRule11Async(receiptRuleId, new APICallBack<GetASpecificRuleResponse>() {
    public void onSuccess(HttpContext context, GetASpecificRuleResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_a_new_rule2_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.createANewRule2Async") createANewRule2Async

> TODO: Add a method description


```java
void createANewRule2Async(
        final CreateANewRuleRequest24 body,
        final APICallBack<CreateANewRuleResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "{    \"rule_name\":\"My Rule\",    \"match_type\":3,    \"action\":\"EMAIL_FIXED\",    \"action_address\":\"john@doe.com\",    \"enabled\":1}";
    CreateANewRuleRequest24 body = mapper.readValue(bodyValue,new TypeReference<CreateANewRuleRequest24> (){});
    // Invoking the API call with sample inputs
    automationRules.createANewRule2Async(body, new APICallBack<CreateANewRuleResponse>() {
        public void onSuccess(HttpContext context, CreateANewRuleResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="update_a_rule11_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.updateARule11Async") updateARule11Async

> TODO: Add a method description


```java
void updateARule11Async(
        final double receiptRuleId,
        final UpdateARuleRequest26 body,
        final APICallBack<UpdateARuleResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    double receiptRuleId = 2;
    String bodyValue = "{    \"rule_name\":\"My Rule\",    \"match_type\":3,    \"action\":\"EMAIL_FIXED\",    \"action_address\":\"john@doe.com\",    \"enabled\":1}";
    UpdateARuleRequest26 body = mapper.readValue(bodyValue,new TypeReference<UpdateARuleRequest26> (){});
    // Invoking the API call with sample inputs
    automationRules.updateARule11Async(receiptRuleId, body, new APICallBack<UpdateARuleResponse>() {
        public void onSuccess(HttpContext context, UpdateARuleResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="delete_a_rule11_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.deleteARule11Async") deleteARule11Async

> TODO: Add a method description


```java
void deleteARule11Async(
        final double receiptRuleId,
        final APICallBack<DeleteARuleResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |


#### Example Usage

```java
double receiptRuleId = 2;
// Invoking the API call with sample inputs
automationRules.deleteARule11Async(receiptRuleId, new APICallBack<DeleteARuleResponse>() {
    public void onSuccess(HttpContext context, DeleteARuleResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="list_rules3_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.listRules3Async") listRules3Async

> TODO: Add a method description


```java
void listRules3Async(final APICallBack<ListRulesResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
automationRules.listRules3Async(new APICallBack<ListRulesResponse>() {
    public void onSuccess(HttpContext context, ListRulesResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_a_specific_rule111_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.getASpecificRule111Async") getASpecificRule111Async

> TODO: Add a method description


```java
void getASpecificRule111Async(
        final double inboundRuleId,
        final APICallBack<GetASpecificRuleResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Fax inbound rule id |


#### Example Usage

```java
double inboundRuleId = 14;
// Invoking the API call with sample inputs
automationRules.getASpecificRule111Async(inboundRuleId, new APICallBack<GetASpecificRuleResponse>() {
    public void onSuccess(HttpContext context, GetASpecificRuleResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_a_new_rule3_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.createANewRule3Async") createANewRule3Async

> TODO: Add a method description


```java
void createANewRule3Async(
        final CreateANewRuleRequest38 body,
        final APICallBack<CreateANewRuleResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "    {        \"dedicated_number\":\"+61298441484\",        \"rule_name\":\"Rule Name\",        \"action\":\"EMAIL_FIXED\",        \"action_address\":\"email@domain.com\",        \"enabled\":1    }";
    CreateANewRuleRequest38 body = mapper.readValue(bodyValue,new TypeReference<CreateANewRuleRequest38> (){});
    // Invoking the API call with sample inputs
    automationRules.createANewRule3Async(body, new APICallBack<CreateANewRuleResponse>() {
        public void onSuccess(HttpContext context, CreateANewRuleResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="update_a_rule111_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.updateARule111Async") updateARule111Async

> TODO: Add a method description


```java
void updateARule111Async(
        final double inboundRuleId,
        final UpdateARuleRequest40 body,
        final APICallBack<UpdateARuleResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Fax inbound rule id |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    double inboundRuleId = 14;
    String bodyValue = "    {        \"dedicated_number\":\"+61298441484\",        \"rule_name\":\"Rule Name\",        \"action\":\"EMAIL_FIXED\",        \"action_address\":\"email@domain.com\",        \"enabled\":1    }";
    UpdateARuleRequest40 body = mapper.readValue(bodyValue,new TypeReference<UpdateARuleRequest40> (){});
    // Invoking the API call with sample inputs
    automationRules.updateARule111Async(inboundRuleId, body, new APICallBack<UpdateARuleResponse>() {
        public void onSuccess(HttpContext context, UpdateARuleResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="delete_a_rule111_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.deleteARule111Async") deleteARule111Async

> TODO: Add a method description


```java
void deleteARule111Async(
        final double inboundRuleId,
        final APICallBack<DeleteARuleResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Fax inbound rule id |


#### Example Usage

```java
double inboundRuleId = 14;
// Invoking the API call with sample inputs
automationRules.deleteARule111Async(inboundRuleId, new APICallBack<DeleteARuleResponse>() {
    public void onSuccess(HttpContext context, DeleteARuleResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="list_rules4_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.listRules4Async") listRules4Async

> TODO: Add a method description


```java
void listRules4Async(final APICallBack<ListRulesResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
automationRules.listRules4Async(new APICallBack<ListRulesResponse>() {
    public void onSuccess(HttpContext context, ListRulesResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_a_specific_rule2_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.getASpecificRule2Async") getASpecificRule2Async

> TODO: Add a method description


```java
void getASpecificRule2Async(
        final double ruleId,
        final APICallBack<GetASpecificRuleResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |


#### Example Usage

```java
double ruleId = 4;
// Invoking the API call with sample inputs
automationRules.getASpecificRule2Async(ruleId, new APICallBack<GetASpecificRuleResponse>() {
    public void onSuccess(HttpContext context, GetASpecificRuleResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_a_new_rule4_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.createANewRule4Async") createANewRule4Async

> TODO: Add a method description


```java
void createANewRule4Async(
        final CreateANewRuleRequest24 body,
        final APICallBack<CreateANewRuleResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "    {        \"rule_name\":\"My Rule\",        \"match_type\":2,        \"action\":\"EMAIL_FIXED\",        \"action_address\":\"john@doe.com\",        \"enabled\":1    }";
    CreateANewRuleRequest24 body = mapper.readValue(bodyValue,new TypeReference<CreateANewRuleRequest24> (){});
    // Invoking the API call with sample inputs
    automationRules.createANewRule4Async(body, new APICallBack<CreateANewRuleResponse>() {
        public void onSuccess(HttpContext context, CreateANewRuleResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="update_a_rule2_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.updateARule2Async") updateARule2Async

> TODO: Add a method description


```java
void updateARule2Async(
        final double ruleId,
        final UpdateARuleRequest26 body,
        final APICallBack<UpdateARuleResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    double ruleId = 4;
    String bodyValue = "    {        \"rule_name\":\"My Rule\",        \"match_type\":1,        \"action\":\"EMAIL_FIXED\",        \"action_address\":\"john@doe.com\",        \"enabled\":1    }";
    UpdateARuleRequest26 body = mapper.readValue(bodyValue,new TypeReference<UpdateARuleRequest26> (){});
    // Invoking the API call with sample inputs
    automationRules.updateARule2Async(ruleId, body, new APICallBack<UpdateARuleResponse>() {
        public void onSuccess(HttpContext context, UpdateARuleResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="delete_a_rule2_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.deleteARule2Async") deleteARule2Async

> TODO: Add a method description


```java
void deleteARule2Async(
        final double ruleId,
        final APICallBack<DeleteARuleResponse49> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to delete. |


#### Example Usage

```java
double ruleId = 147.35966813162;
// Invoking the API call with sample inputs
automationRules.deleteARule2Async(ruleId, new APICallBack<DeleteARuleResponse49>() {
    public void onSuccess(HttpContext context, DeleteARuleResponse49 response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="list_rules5_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.listRules5Async") listRules5Async

> TODO: Add a method description


```java
void listRules5Async(final APICallBack<ListRulesResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
automationRules.listRules5Async(new APICallBack<ListRulesResponse>() {
    public void onSuccess(HttpContext context, ListRulesResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_a_specific_rule12_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.getASpecificRule12Async") getASpecificRule12Async

> TODO: Add a method description


```java
void getASpecificRule12Async(
        final double ruleId,
        final APICallBack<GetASpecificRuleResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |


#### Example Usage

```java
double ruleId = 5;
// Invoking the API call with sample inputs
automationRules.getASpecificRule12Async(ruleId, new APICallBack<GetASpecificRuleResponse>() {
    public void onSuccess(HttpContext context, GetASpecificRuleResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_a_new_rule5_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.createANewRule5Async") createANewRule5Async

> TODO: Add a method description


```java
void createANewRule5Async(
        final CreateANewRuleRequest24 body,
        final APICallBack<CreateANewRuleResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "    {        \"rule_name\":\"My Rule\",        \"match_type\": 0,        \"action\":\"URL\",        \"action_address\":\"http://testurl.com\",        \"enabled\":1    }";
    CreateANewRuleRequest24 body = mapper.readValue(bodyValue,new TypeReference<CreateANewRuleRequest24> (){});
    // Invoking the API call with sample inputs
    automationRules.createANewRule5Async(body, new APICallBack<CreateANewRuleResponse>() {
        public void onSuccess(HttpContext context, CreateANewRuleResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="update_a_rule12_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.updateARule12Async") updateARule12Async

> TODO: Add a method description


```java
void updateARule12Async(
        final double ruleId,
        final UpdateARuleRequest26 body,
        final APICallBack<UpdateARuleResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    double ruleId = 8;
    String bodyValue = "    {        \"rule_name\":\"My Rule\",        \"match_type\": 0,        \"action\":\"URL\",        \"action_address\":\"http://testurl.com\",        \"enabled\":1    }";
    UpdateARuleRequest26 body = mapper.readValue(bodyValue,new TypeReference<UpdateARuleRequest26> (){});
    // Invoking the API call with sample inputs
    automationRules.updateARule12Async(ruleId, body, new APICallBack<UpdateARuleResponse>() {
        public void onSuccess(HttpContext context, UpdateARuleResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="delete_a_rule12_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.AutomationRulesController.deleteARule12Async") deleteARule12Async

> TODO: Add a method description


```java
void deleteARule12Async(
        final double ruleId,
        final APICallBack<DeleteARuleResponse56> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to delete. |


#### Example Usage

```java
double ruleId = 8;
// Invoking the API call with sample inputs
automationRules.deleteARule12Async(ruleId, new APICallBack<DeleteARuleResponse56>() {
    public void onSuccess(HttpContext context, DeleteARuleResponse56 response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="contact_lists_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.ContactListsController") ContactListsController

### Get singleton instance

The singleton instance of the ``` ContactListsController ``` class can be accessed from the API Client.

```java
ContactListsController contactLists = client.getContactLists();
```

### <a name="get_all_contact_lists_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ContactListsController.getAllContactListsAsync") getAllContactListsAsync

> TODO: Add a method description


```java
void getAllContactListsAsync(final APICallBack<GetAllContactListsResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
contactLists.getAllContactListsAsync(new APICallBack<GetAllContactListsResponse>() {
    public void onSuccess(HttpContext context, GetAllContactListsResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_a_new_contact_list_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ContactListsController.createANewContactListAsync") createANewContactListAsync

> TODO: Add a method description


```java
void createANewContactListAsync(
        final CreateANewContactListRequest body,
        final APICallBack<CreateANewContactListResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "    {        \"list_name\":\"ListCT3QrVL4od\"    }";
    CreateANewContactListRequest body = mapper.readValue(bodyValue,new TypeReference<CreateANewContactListRequest> (){});
    // Invoking the API call with sample inputs
    contactLists.createANewContactListAsync(body, new APICallBack<CreateANewContactListResponse>() {
        public void onSuccess(HttpContext context, CreateANewContactListResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="get_a_specific_contact_list_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ContactListsController.getASpecificContactListAsync") getASpecificContactListAsync

> TODO: Add a method description


```java
void getASpecificContactListAsync(
        final double listId,
        final APICallBack<GetASpecificContactListResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |


#### Example Usage

```java
double listId = 437;
// Invoking the API call with sample inputs
contactLists.getASpecificContactListAsync(listId, new APICallBack<GetASpecificContactListResponse>() {
    public void onSuccess(HttpContext context, GetASpecificContactListResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="update_a_specific_contact_list_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ContactListsController.updateASpecificContactListAsync") updateASpecificContactListAsync

> TODO: Add a method description


```java
void updateASpecificContactListAsync(
        final double listId,
        final UpdateASpecificContactListRequest body,
        final APICallBack<UpdateASpecificContactListResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    double listId = 439;
    String bodyValue = "    {        \"list_name\":\"ListlPJf33ksjP\"    }";
    UpdateASpecificContactListRequest body = mapper.readValue(bodyValue,new TypeReference<UpdateASpecificContactListRequest> (){});
    // Invoking the API call with sample inputs
    contactLists.updateASpecificContactListAsync(listId, body, new APICallBack<UpdateASpecificContactListResponse>() {
        public void onSuccess(HttpContext context, UpdateASpecificContactListResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="delete_a_specific_contact_list_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ContactListsController.deleteASpecificContactListAsync") deleteASpecificContactListAsync

> TODO: Add a method description


```java
void deleteASpecificContactListAsync(
        final double listId,
        final APICallBack<DeleteASpecificContactListResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |


#### Example Usage

```java
double listId = 442;
// Invoking the API call with sample inputs
contactLists.deleteASpecificContactListAsync(listId, new APICallBack<DeleteASpecificContactListResponse>() {
    public void onSuccess(HttpContext context, DeleteASpecificContactListResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_import_contacts_to_list_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ContactListsController.createImportContactsToListAsync") createImportContactsToListAsync

> TODO: Add a method description


```java
void createImportContactsToListAsync(
        final double listId,
        final ImportContactsToListRequest body,
        final APICallBack<ImportContactsToListResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    double listId = 437;
    String bodyValue = "{    \"file_url\":\"http://yourdomain.com/5485EA6144/79E8/import.csv\",    \"field_order\":[        \"phone\",        \"first_name\",        \"last_name\",        \"custom1\",        \"custom2\",        \"custom3\",        \"custom4\",        \"fax_number\",        \"organization_name\",        \"email\",        \"address_line_1\",        \"address_line_2\",        \"address_city\",        \"address_state\",        \"address_postal_code\",        \"address_country\"    ]}";
    ImportContactsToListRequest body = mapper.readValue(bodyValue,new TypeReference<ImportContactsToListRequest> (){});
    // Invoking the API call with sample inputs
    contactLists.createImportContactsToListAsync(listId, body, new APICallBack<ImportContactsToListResponse>() {
        public void onSuccess(HttpContext context, ImportContactsToListResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="update_remove_duplicate_contacts_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ContactListsController.updateRemoveDuplicateContactsAsync") updateRemoveDuplicateContactsAsync

> TODO: Add a method description


```java
void updateRemoveDuplicateContactsAsync(
        final double listId,
        final RemoveDuplicateContactsRequest body,
        final APICallBack<RemoveDuplicateContactsResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    double listId = 439;
    String bodyValue = "{    \"fields\":[        \"phone_number\",        \"first_name\",        \"last_name\",        \"fax_number\",        \"address_country\"    ]}";
    RemoveDuplicateContactsRequest body = mapper.readValue(bodyValue,new TypeReference<RemoveDuplicateContactsRequest> (){});
    // Invoking the API call with sample inputs
    contactLists.updateRemoveDuplicateContactsAsync(listId, body, new APICallBack<RemoveDuplicateContactsResponse>() {
        public void onSuccess(HttpContext context, RemoveDuplicateContactsResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="get_list_of_acceptable_import_fields_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ContactListsController.getListOfAcceptableImportFieldsAsync") getListOfAcceptableImportFieldsAsync

> TODO: Add a method description


```java
void getListOfAcceptableImportFieldsAsync(
        final String listId,
        final APICallBack<GetListOfAcceptableImportFieldsResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Optional ```  | TODO: Add a parameter description |


#### Example Usage

```java
String listId = "list_id";
// Invoking the API call with sample inputs
contactLists.getListOfAcceptableImportFieldsAsync(listId, new APICallBack<GetListOfAcceptableImportFieldsResponse>() {
    public void onSuccess(HttpContext context, GetListOfAcceptableImportFieldsResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_show_csv_import_file_preview_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ContactListsController.createShowCSVImportFilePreviewAsync") createShowCSVImportFilePreviewAsync

> Show first row of the csv import file.


```java
void createShowCSVImportFilePreviewAsync(
        final double listId,
        final ShowCSVImportFilePreviewRequest body,
        final APICallBack<ShowCSVImportFilePreviewResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    double listId = 439;
    String bodyValue = "{    \"file_url\":\"http://yourdomain.com/5485EA6144/79E8/import.csv\"}";
    ShowCSVImportFilePreviewRequest body = mapper.readValue(bodyValue,new TypeReference<ShowCSVImportFilePreviewRequest> (){});
    // Invoking the API call with sample inputs
    contactLists.createShowCSVImportFilePreviewAsync(listId, body, new APICallBack<ShowCSVImportFilePreviewResponse>() {
        public void onSuccess(HttpContext context, ShowCSVImportFilePreviewResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


[Back to List of Controllers](#list_of_controllers)

## <a name="contact_suggestions_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.ContactSuggestionsController") ContactSuggestionsController

### Get singleton instance

The singleton instance of the ``` ContactSuggestionsController ``` class can be accessed from the API Client.

```java
ContactSuggestionsController contactSuggestions = client.getContactSuggestions();
```

### <a name="list_contact_suggestions_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ContactSuggestionsController.listContactSuggestionsAsync") listContactSuggestionsAsync

> TODO: Add a method description


```java
void listContactSuggestionsAsync(final APICallBack<ListContactSuggestionsResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
contactSuggestions.listContactSuggestionsAsync(new APICallBack<ListContactSuggestionsResponse>() {
    public void onSuccess(HttpContext context, ListContactSuggestionsResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="contacts_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.ContactsController") ContactsController

### Get singleton instance

The singleton instance of the ``` ContactsController ``` class can be accessed from the API Client.

```java
ContactsController contacts = client.getContacts();
```

### <a name="get_all_contacts_in_a_list_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ContactsController.getAllContactsInAListAsync") getAllContactsInAListAsync

> TODO: Add a method description


```java
void getAllContactsInAListAsync(
        final double listId,
        final APICallBack<GetAllContactsInAListResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id where your contacts belong. |


#### Example Usage

```java
double listId = 428;
// Invoking the API call with sample inputs
contacts.getAllContactsInAListAsync(listId, new APICallBack<GetAllContactsInAListResponse>() {
    public void onSuccess(HttpContext context, GetAllContactsInAListResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_a_new_contact_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ContactsController.createANewContactAsync") createANewContactAsync

> TODO: Add a method description


```java
void createANewContactAsync(
        final double listId,
        final CreateANewContactRequest body,
        final APICallBack<CreateANewContactResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id where your contact be associated. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    double listId = 428;
    String bodyValue = "    {        \"phone_number\":\"+16783270696\",        \"first_name\":\"Ellen\",        \"last_name\":\"Diaz\",        \"custom_1\":\"Custom 1\",        \"custom_2\":\"Custom 2\",        \"custom_3\":\"Custom 3\",        \"custom_4\":\"Custom 4\",        \"fax_number\":\"+16783270696\",        \"organization_name\":\"Awesome Organization\",        \"email\":\"ellen@diaz.com\",        \"address_line_1\":\"Block 2\",        \"address_line_2\":\"Cool Bldg.\",        \"address_city\":\"Nevada\",        \"address_state\":\"Las Vegas\",        \"address_postal_code\":\"36063\",        \"address_country\":\"US\"    }";
    CreateANewContactRequest body = mapper.readValue(bodyValue,new TypeReference<CreateANewContactRequest> (){});
    // Invoking the API call with sample inputs
    contacts.createANewContactAsync(listId, body, new APICallBack<CreateANewContactResponse>() {
        public void onSuccess(HttpContext context, CreateANewContactResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="get_a_specific_contact_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ContactsController.getASpecificContactAsync") getASpecificContactAsync

> TODO: Add a method description


```java
void getASpecificContactAsync(
        final double listId,
        final double contactId,
        final APICallBack<GetASpecificContactResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| contactId |  ``` Required ```  | Your contact id you want to access. |


#### Example Usage

```java
double listId = 428;
double contactId = 552802;
// Invoking the API call with sample inputs
contacts.getASpecificContactAsync(listId, contactId, new APICallBack<GetASpecificContactResponse>() {
    public void onSuccess(HttpContext context, GetASpecificContactResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="update_a_specific_contact_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ContactsController.updateASpecificContactAsync") updateASpecificContactAsync

> TODO: Add a method description


```java
void updateASpecificContactAsync(
        final double listId,
        final double contactId,
        final UpdateASpecificContactRequest body,
        final APICallBack<UpdateASpecificContactResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| contactId |  ``` Required ```  | Your contact id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    double listId = 428;
    double contactId = 552802;
    String bodyValue = "{        \"phone_number\":\"+16783275492\",        \"first_name\":\"Ellen\",        \"last_name\":\"Diaz\",        \"custom_1\":\"Custom S72oJ9Teba\",        \"custom_2\":\"Custom NvrRJrKWeq\",        \"custom_3\":\"Custom 2ws94p1Dop\",        \"custom_4\":\"Custom Ku0AaIS5xb\",        \"fax_number\":\"+16783276356\",        \"organization_name\":\"Awesome Organization\",        \"email\":\"ellen@diaz.com\",        \"address_line_1\":\"Block 6\",        \"address_line_2\":\"Cool Bldg.\",        \"address_city\":\"Nevada\",        \"address_state\":\"Las Vegas\",        \"address_postal_code\":\"36063\",        \"address_country\":\"US\"    }";
    UpdateASpecificContactRequest body = mapper.readValue(bodyValue,new TypeReference<UpdateASpecificContactRequest> (){});
    // Invoking the API call with sample inputs
    contacts.updateASpecificContactAsync(listId, contactId, body, new APICallBack<UpdateASpecificContactResponse>() {
        public void onSuccess(HttpContext context, UpdateASpecificContactResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="delete_a_specific_contact_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ContactsController.deleteASpecificContactAsync") deleteASpecificContactAsync

> TODO: Add a method description


```java
void deleteASpecificContactAsync(
        final double listId,
        final double contactId,
        final APICallBack<DeleteASpecificContactResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| contactId |  ``` Required ```  | Your contact id you want to access. |


#### Example Usage

```java
double listId = 428;
double contactId = 552807;
// Invoking the API call with sample inputs
contacts.deleteASpecificContactAsync(listId, contactId, new APICallBack<DeleteASpecificContactResponse>() {
    public void onSuccess(HttpContext context, DeleteASpecificContactResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="update_remove_opted_out_contacts_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ContactsController.updateRemoveOptedOutContactsAsync") updateRemoveOptedOutContactsAsync

> TODO: Add a method description


```java
void updateRemoveOptedOutContactsAsync(
        final double listId,
        final double optOutListId,
        final APICallBack<RemoveOptedOutContactsResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id. |
| optOutListId |  ``` Required ```  | Your opt out list id. |


#### Example Usage

```java
double listId = 439;
double optOutListId = 512;
// Invoking the API call with sample inputs
contacts.updateRemoveOptedOutContactsAsync(listId, optOutListId, new APICallBack<RemoveOptedOutContactsResponse>() {
    public void onSuccess(HttpContext context, RemoveOptedOutContactsResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="update_transfer_a_contact_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ContactsController.updateTransferAContactAsync") updateTransferAContactAsync

> Transfers a specific contact to another list.


```java
void updateTransferAContactAsync(
        final double fromListId,
        final double contactId,
        final double toListId,
        final APICallBack<TransferAContactResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| fromListId |  ``` Required ```  | From list id. |
| contactId |  ``` Required ```  | Contact ID. |
| toListId |  ``` Required ```  | To list id. |


#### Example Usage

```java
double fromListId = 428;
double contactId = 1;
double toListId = 429;
// Invoking the API call with sample inputs
contacts.updateTransferAContactAsync(fromListId, contactId, toListId, new APICallBack<TransferAContactResponse>() {
    public void onSuccess(HttpContext context, TransferAContactResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="countries_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.CountriesController") CountriesController

### Get singleton instance

The singleton instance of the ``` CountriesController ``` class can be accessed from the API Client.

```java
CountriesController countries = client.getCountries();
```

### <a name="get_all_countries_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.CountriesController.getAllCountriesAsync") getAllCountriesAsync

> TODO: Add a method description


```java
void getAllCountriesAsync(final APICallBack<GetAllCountriesResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
countries.getAllCountriesAsync(new APICallBack<GetAllCountriesResponse>() {
    public void onSuccess(HttpContext context, GetAllCountriesResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="delivery_issues_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.DeliveryIssuesController") DeliveryIssuesController

### Get singleton instance

The singleton instance of the ``` DeliveryIssuesController ``` class can be accessed from the API Client.

```java
DeliveryIssuesController deliveryIssues = client.getDeliveryIssues();
```

### <a name="get_delivery_issues_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.DeliveryIssuesController.getDeliveryIssuesAsync") getDeliveryIssuesAsync

> TODO: Add a method description


```java
void getDeliveryIssuesAsync(final APICallBack<GetDeliveryIssuesResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
deliveryIssues.getDeliveryIssuesAsync(new APICallBack<GetDeliveryIssuesResponse>() {
    public void onSuccess(HttpContext context, GetDeliveryIssuesResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_delivery_issue_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.DeliveryIssuesController.createDeliveryIssueAsync") createDeliveryIssueAsync

> TODO: Add a method description


```java
void createDeliveryIssueAsync(
        final CreateDeliveryIssueRequest body,
        final APICallBack<CreateDeliveryIssueResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "{  \"message_id\": \"B388828B\",  \"type\": \"SMS\",  \"description\": \"This is a test\",  \"client_comments\": \"test\",  \"email_address: john_doe@user.com\": \"\",  \"Body\": \"\"}";
    CreateDeliveryIssueRequest body = mapper.readValue(bodyValue,new TypeReference<CreateDeliveryIssueRequest> (){});
    // Invoking the API call with sample inputs
    deliveryIssues.createDeliveryIssueAsync(body, new APICallBack<CreateDeliveryIssueResponse>() {
        public void onSuccess(HttpContext context, CreateDeliveryIssueResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


[Back to List of Controllers](#list_of_controllers)

## <a name="email_marketing_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.EmailMarketingController") EmailMarketingController

### Get singleton instance

The singleton instance of the ``` EmailMarketingController ``` class can be accessed from the API Client.

```java
EmailMarketingController emailMarketing = client.getEmailMarketing();
```

### <a name="get_all_allowed_email_addresses_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailMarketingController.getAllAllowedEmailAddressesAsync") getAllAllowedEmailAddressesAsync

> TODO: Add a method description


```java
void getAllAllowedEmailAddressesAsync(final APICallBack<GetAllAllowedEmailAddressesResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
emailMarketing.getAllAllowedEmailAddressesAsync(new APICallBack<GetAllAllowedEmailAddressesResponse>() {
    public void onSuccess(HttpContext context, GetAllAllowedEmailAddressesResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_allowed_email_address_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailMarketingController.createAllowedEmailAddressAsync") createAllowedEmailAddressAsync

> TODO: Add a method description


```java
void createAllowedEmailAddressAsync(
        final CreateAllowedEmailAddressRequest body,
        final APICallBack<CreateAllowedEmailAddressResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "{  \"email_address\": \"johndoe1@user.com\",  \"Body\": \"\"}";
    CreateAllowedEmailAddressRequest body = mapper.readValue(bodyValue,new TypeReference<CreateAllowedEmailAddressRequest> (){});
    // Invoking the API call with sample inputs
    emailMarketing.createAllowedEmailAddressAsync(body, new APICallBack<CreateAllowedEmailAddressResponse>() {
        public void onSuccess(HttpContext context, CreateAllowedEmailAddressResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="update_send_verification_token_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailMarketingController.updateSendVerificationTokenAsync") updateSendVerificationTokenAsync

> TODO: Add a method description


```java
void updateSendVerificationTokenAsync(
        final double emailAddressId,
        final APICallBack<SendVerificationTokenResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email addess id you want to access. |


#### Example Usage

```java
double emailAddressId = 238.854950023282;
// Invoking the API call with sample inputs
emailMarketing.updateSendVerificationTokenAsync(emailAddressId, new APICallBack<SendVerificationTokenResponse>() {
    public void onSuccess(HttpContext context, SendVerificationTokenResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="update_verify_allowed_email_address_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailMarketingController.updateVerifyAllowedEmailAddressAsync") updateVerifyAllowedEmailAddressAsync

> TODO: Add a method description


```java
void updateVerifyAllowedEmailAddressAsync(
        final double emailAddressId,
        final String activationToken,
        final APICallBack<VerifyAllowedEmailAddressResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email address id you want to access. |
| activationToken |  ``` Required ```  | 6E8B-4FDB-99A7-7ED08DF97BCC (required, string) - Your activation token. |


#### Example Usage

```java
double emailAddressId = 5;
String activationToken = "3BD73304";
// Invoking the API call with sample inputs
emailMarketing.updateVerifyAllowedEmailAddressAsync(emailAddressId, activationToken, new APICallBack<VerifyAllowedEmailAddressResponse>() {
    public void onSuccess(HttpContext context, VerifyAllowedEmailAddressResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="delete_allowed_email_address_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailMarketingController.deleteAllowedEmailAddressAsync") deleteAllowedEmailAddressAsync

> TODO: Add a method description


```java
void deleteAllowedEmailAddressAsync(
        final double emailAddressId,
        final APICallBack<DeleteAllowedEmailAddressResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email address you want to access. |


#### Example Usage

```java
double emailAddressId = 238.854950023282;
// Invoking the API call with sample inputs
emailMarketing.deleteAllowedEmailAddressAsync(emailAddressId, new APICallBack<DeleteAllowedEmailAddressResponse>() {
    public void onSuccess(HttpContext context, DeleteAllowedEmailAddressResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_specific_allowed_email_address_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailMarketingController.getSpecificAllowedEmailAddressAsync") getSpecificAllowedEmailAddressAsync

> TODO: Add a method description


```java
void getSpecificAllowedEmailAddressAsync(
        final double emailAddressId,
        final APICallBack<GetSpecificAllowedEmailAddressResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email address you want to access. |


#### Example Usage

```java
double emailAddressId = 4;
// Invoking the API call with sample inputs
emailMarketing.getSpecificAllowedEmailAddressAsync(emailAddressId, new APICallBack<GetSpecificAllowedEmailAddressResponse>() {
    public void onSuccess(HttpContext context, GetSpecificAllowedEmailAddressResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_all_email_campaigns_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailMarketingController.getAllEmailCampaignsAsync") getAllEmailCampaignsAsync

> TODO: Add a method description


```java
void getAllEmailCampaignsAsync(final APICallBack<GetAllEmailCampaignsResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
emailMarketing.getAllEmailCampaignsAsync(new APICallBack<GetAllEmailCampaignsResponse>() {
    public void onSuccess(HttpContext context, GetAllEmailCampaignsResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_specific_email_campaign_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailMarketingController.getSpecificEmailCampaignAsync") getSpecificEmailCampaignAsync

> TODO: Add a method description


```java
void getSpecificEmailCampaignAsync(
        final double emailCampaignId,
        final APICallBack<GetSpecificEmailCampaignResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailCampaignId |  ``` Required ```  | The email campaign id you want to access. |


#### Example Usage

```java
double emailCampaignId = 1;
// Invoking the API call with sample inputs
emailMarketing.getSpecificEmailCampaignAsync(emailCampaignId, new APICallBack<GetSpecificEmailCampaignResponse>() {
    public void onSuccess(HttpContext context, GetSpecificEmailCampaignResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_email_campaign_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailMarketingController.createEmailCampaignAsync") createEmailCampaignAsync

> TODO: Add a method description


```java
void createEmailCampaignAsync(
        final CreateEmailCampaignRequest body,
        final APICallBack<CreateEmailCampaignResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "{  \"name\" : \"John Doe\",  \"subject\" : \"Lorem Ipsum\",  \"from_email_address_id\" : 2,  \"from_name\" : \"From name\",  \"template_id\" : 31,  \"body\" : \"<p>This is a test</p>\",  \"list_id\" : 456}";
    CreateEmailCampaignRequest body = mapper.readValue(bodyValue,new TypeReference<CreateEmailCampaignRequest> (){});
    // Invoking the API call with sample inputs
    emailMarketing.createEmailCampaignAsync(body, new APICallBack<CreateEmailCampaignResponse>() {
        public void onSuccess(HttpContext context, CreateEmailCampaignResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="update_email_campaign_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailMarketingController.updateEmailCampaignAsync") updateEmailCampaignAsync

> TODO: Add a method description


```java
void updateEmailCampaignAsync(
        final double emailCampaignId,
        final UpdateEmailCampaignRequest body,
        final APICallBack<UpdateEmailCampaignResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailCampaignId |  ``` Required ```  | The email campaign id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    double emailCampaignId = 1;
    String bodyValue = "{  \"name\" : \"John Doe\",  \"subject\" : \"Lorem Ipsum\",  \"from_email_address_id\" : 2,  \"from_name\" : \"From name\",  \"template_id\" : 31,  \"body\" : \"<p>This is a test</p>\",  \"list_id\" : 456}";
    UpdateEmailCampaignRequest body = mapper.readValue(bodyValue,new TypeReference<UpdateEmailCampaignRequest> (){});
    // Invoking the API call with sample inputs
    emailMarketing.updateEmailCampaignAsync(emailCampaignId, body, new APICallBack<UpdateEmailCampaignResponse>() {
        public void onSuccess(HttpContext context, UpdateEmailCampaignResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="update_cancel_email_campaign_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailMarketingController.updateCancelEmailCampaignAsync") updateCancelEmailCampaignAsync

> TODO: Add a method description


```java
void updateCancelEmailCampaignAsync(
        final double emailCampaignId,
        final APICallBack<CancelEmailCampaignResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailCampaignId |  ``` Required ```  | The email campaign id you want to cancel. |


#### Example Usage

```java
double emailCampaignId = 1;
// Invoking the API call with sample inputs
emailMarketing.updateCancelEmailCampaignAsync(emailCampaignId, new APICallBack<CancelEmailCampaignResponse>() {
    public void onSuccess(HttpContext context, CancelEmailCampaignResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_calculate_price_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailMarketingController.createCalculatePriceAsync") createCalculatePriceAsync

> TODO: Add a method description


```java
void createCalculatePriceAsync(
        final CalculatePriceRequest body,
        final APICallBack<CalculatePriceResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "{  \"name\" : \"John Doe\",  \"subject\" : \"Lorem Ipsum\",  \"from_email_address_id\" : 2,  \"from_name\" : \"From name\",  \"template_id\" : 31,  \"body\" : \"<p>This is a test</p>\",  \"list_id\" : 456}";
    CalculatePriceRequest body = mapper.readValue(bodyValue,new TypeReference<CalculatePriceRequest> (){});
    // Invoking the API call with sample inputs
    emailMarketing.createCalculatePriceAsync(body, new APICallBack<CalculatePriceResponse>() {
        public void onSuccess(HttpContext context, CalculatePriceResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="get_specific_email_campaign_history_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailMarketingController.getSpecificEmailCampaignHistoryAsync") getSpecificEmailCampaignHistoryAsync

> TODO: Add a method description


```java
void getSpecificEmailCampaignHistoryAsync(
        final double campaignId,
        final APICallBack<GetSpecificEmailCampaignHistoryResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| campaignId |  ``` Required ```  | The email campaign id you want to access. |


#### Example Usage

```java
double campaignId = 77;
// Invoking the API call with sample inputs
emailMarketing.getSpecificEmailCampaignHistoryAsync(campaignId, new APICallBack<GetSpecificEmailCampaignHistoryResponse>() {
    public void onSuccess(HttpContext context, GetSpecificEmailCampaignHistoryResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_all_email_templates_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailMarketingController.getAllEmailTemplatesAsync") getAllEmailTemplatesAsync

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```java
void getAllEmailTemplatesAsync(final APICallBack<GetAllEmailTemplatesResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
emailMarketing.getAllEmailTemplatesAsync(new APICallBack<GetAllEmailTemplatesResponse>() {
    public void onSuccess(HttpContext context, GetAllEmailTemplatesResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_specific_email_template_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailMarketingController.getSpecificEmailTemplateAsync") getSpecificEmailTemplateAsync

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```java
void getSpecificEmailTemplateAsync(
        final double templateId,
        final APICallBack<GetSpecificEmailTemplateResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | The email template id. |


#### Example Usage

```java
double templateId = 291;
// Invoking the API call with sample inputs
emailMarketing.getSpecificEmailTemplateAsync(templateId, new APICallBack<GetSpecificEmailTemplateResponse>() {
    public void onSuccess(HttpContext context, GetSpecificEmailTemplateResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_new_email_template_from_master_template_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailMarketingController.createNewEmailTemplateFromMasterTemplateAsync") createNewEmailTemplateFromMasterTemplateAsync

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```java
void createNewEmailTemplateFromMasterTemplateAsync(
        final CreateNewEmailTemplateFromMasterTemplateRequest body,
        final APICallBack<CreateNewEmailTemplateFromMasterTemplateResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "{  \"template_name\": \"Minions\",  \"template_id_master\": 57}";
    CreateNewEmailTemplateFromMasterTemplateRequest body = mapper.readValue(bodyValue,new TypeReference<CreateNewEmailTemplateFromMasterTemplateRequest> (){});
    // Invoking the API call with sample inputs
    emailMarketing.createNewEmailTemplateFromMasterTemplateAsync(body, new APICallBack<CreateNewEmailTemplateFromMasterTemplateResponse>() {
        public void onSuccess(HttpContext context, CreateNewEmailTemplateFromMasterTemplateResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="update_an_email_template_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailMarketingController.updateAnEmailTemplateAsync") updateAnEmailTemplateAsync

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```java
void updateAnEmailTemplateAsync(
        final double templateId,
        final UpdateAnEmailTemplateRequest body,
        final APICallBack<UpdateAnEmailTemplateResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | The id of the template to be updated. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    double templateId = 291;
    String bodyValue = "    {        \"template_name\":\"Minions\",        \"body\":\"This is a sample content: Sc0KNWgSMG for this template.\"    }";
    UpdateAnEmailTemplateRequest body = mapper.readValue(bodyValue,new TypeReference<UpdateAnEmailTemplateRequest> (){});
    // Invoking the API call with sample inputs
    emailMarketing.updateAnEmailTemplateAsync(templateId, body, new APICallBack<UpdateAnEmailTemplateResponse>() {
        public void onSuccess(HttpContext context, UpdateAnEmailTemplateResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="delete_email_template_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailMarketingController.deleteEmailTemplateAsync") deleteEmailTemplateAsync

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```java
void deleteEmailTemplateAsync(
        final double templateId,
        final APICallBack<DeleteEmailTemplateResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |


#### Example Usage

```java
double templateId = 25;
// Invoking the API call with sample inputs
emailMarketing.deleteEmailTemplateAsync(templateId, new APICallBack<DeleteEmailTemplateResponse>() {
    public void onSuccess(HttpContext context, DeleteEmailTemplateResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_all_master_email_templates_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailMarketingController.getAllMasterEmailTemplatesAsync") getAllMasterEmailTemplatesAsync

> Master templates are templates that you can clone to a User Email Template which lets you edit and save it.


```java
void getAllMasterEmailTemplatesAsync(final APICallBack<GetAllMasterEmailTemplatesResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
emailMarketing.getAllMasterEmailTemplatesAsync(new APICallBack<GetAllMasterEmailTemplatesResponse>() {
    public void onSuccess(HttpContext context, GetAllMasterEmailTemplatesResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_specific_master_template_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailMarketingController.getSpecificMasterTemplateAsync") getSpecificMasterTemplateAsync

> Master templates are templates that you can clone to a User Email Template which lets you edit and save it.


```java
void getSpecificMasterTemplateAsync(
        final String templateId,
        final APICallBack<GetSpecificMasterTemplateResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |


#### Example Usage

```java
String templateId = "25";
// Invoking the API call with sample inputs
emailMarketing.getSpecificMasterTemplateAsync(templateId, new APICallBack<GetSpecificMasterTemplateResponse>() {
    public void onSuccess(HttpContext context, GetSpecificMasterTemplateResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_all_master_template_categories_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailMarketingController.getAllMasterTemplateCategoriesAsync") getAllMasterTemplateCategoriesAsync

> TODO: Add a method description


```java
void getAllMasterTemplateCategoriesAsync(final APICallBack<GetAllMasterTemplateCategoriesResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
emailMarketing.getAllMasterTemplateCategoriesAsync(new APICallBack<GetAllMasterTemplateCategoriesResponse>() {
    public void onSuccess(HttpContext context, GetAllMasterTemplateCategoriesResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_specific_email_template_category_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailMarketingController.getSpecificEmailTemplateCategoryAsync") getSpecificEmailTemplateCategoryAsync

> TODO: Add a method description


```java
void getSpecificEmailTemplateCategoryAsync(
        final String categoryId,
        final APICallBack<GetSpecificEmailTemplateCategoryResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| categoryId |  ``` Required ```  | Your category id. |


#### Example Usage

```java
String categoryId = "25";
// Invoking the API call with sample inputs
emailMarketing.getSpecificEmailTemplateCategoryAsync(categoryId, new APICallBack<GetSpecificEmailTemplateCategoryResponse>() {
    public void onSuccess(HttpContext context, GetSpecificEmailTemplateCategoryResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_all_templates_for_category_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailMarketingController.getAllTemplatesForCategoryAsync") getAllTemplatesForCategoryAsync

> TODO: Add a method description


```java
void getAllTemplatesForCategoryAsync(
        final String categoryId,
        final APICallBack<GetAllTemplatesForCategoryResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| categoryId |  ``` Required ```  | Your category id. |


#### Example Usage

```java
String categoryId = "1";
// Invoking the API call with sample inputs
emailMarketing.getAllTemplatesForCategoryAsync(categoryId, new APICallBack<GetAllTemplatesForCategoryResponse>() {
    public void onSuccess(HttpContext context, GetAllTemplatesForCategoryResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="upload_image_to_specific_template_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailMarketingController.uploadImageToSpecificTemplateAsync") uploadImageToSpecificTemplateAsync

> TODO: Add a method description


```java
void uploadImageToSpecificTemplateAsync(
        final String templateId,
        final UploadImageToSpecificTemplateRequest body,
        final APICallBack<UploadImageToSpecificTemplateResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String templateId = "1";
    String bodyValue = "{    \"image\": \"image.png\",    \"url\" : \"http://www.downloadimg.from/here.png\"}";
    UploadImageToSpecificTemplateRequest body = mapper.readValue(bodyValue,new TypeReference<UploadImageToSpecificTemplateRequest> (){});
    // Invoking the API call with sample inputs
    emailMarketing.uploadImageToSpecificTemplateAsync(templateId, body, new APICallBack<UploadImageToSpecificTemplateResponse>() {
        public void onSuccess(HttpContext context, UploadImageToSpecificTemplateResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


[Back to List of Controllers](#list_of_controllers)

## <a name="email_to_sms_allowed_address_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.EmailToSMSAllowedAddressController") EmailToSMSAllowedAddressController

### Get singleton instance

The singleton instance of the ``` EmailToSMSAllowedAddressController ``` class can be accessed from the API Client.

```java
EmailToSMSAllowedAddressController emailToSMSAllowedAddress = client.getEmailToSMSAllowedAddress();
```

### <a name="list_of_email_to_sms_allowed_address_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailToSMSAllowedAddressController.listOfEmailToSMSAllowedAddressAsync") listOfEmailToSMSAllowedAddressAsync

> Get list of allowed email addresses.


```java
void listOfEmailToSMSAllowedAddressAsync(final APICallBack<ListOfEmailToSMSAllowedAddressResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
emailToSMSAllowedAddress.listOfEmailToSMSAllowedAddressAsync(new APICallBack<ListOfEmailToSMSAllowedAddressResponse>() {
    public void onSuccess(HttpContext context, ListOfEmailToSMSAllowedAddressResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_email_to_sms_allowed_address_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailToSMSAllowedAddressController.createEmailToSMSAllowedAddressAsync") createEmailToSMSAllowedAddressAsync

> Create an allowed email address.


```java
void createEmailToSMSAllowedAddressAsync(
        final CreateEmailToSMSAllowedAddressRequest body,
        final APICallBack<CreateEmailToSMSAllowedAddressResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "    {        \"email_address\":\"Cv3p0@gmail.com\",        \"from\":\"+17128845887\"    }";
    CreateEmailToSMSAllowedAddressRequest body = mapper.readValue(bodyValue,new TypeReference<CreateEmailToSMSAllowedAddressRequest> (){});
    // Invoking the API call with sample inputs
    emailToSMSAllowedAddress.createEmailToSMSAllowedAddressAsync(body, new APICallBack<CreateEmailToSMSAllowedAddressResponse>() {
        public void onSuccess(HttpContext context, CreateEmailToSMSAllowedAddressResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="get_specific_email_to_sms_allowed_address_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailToSMSAllowedAddressController.getSpecificEmailToSMSAllowedAddressAsync") getSpecificEmailToSMSAllowedAddressAsync

> Get a specific allowed email address.


```java
void getSpecificEmailToSMSAllowedAddressAsync(
        final double emailAddressId,
        final APICallBack<GetSpecificEmailToSMSAllowedAddressResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | Your email address id. |


#### Example Usage

```java
double emailAddressId = 113;
// Invoking the API call with sample inputs
emailToSMSAllowedAddress.getSpecificEmailToSMSAllowedAddressAsync(emailAddressId, new APICallBack<GetSpecificEmailToSMSAllowedAddressResponse>() {
    public void onSuccess(HttpContext context, GetSpecificEmailToSMSAllowedAddressResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="update_email_to_sms_allowed_address_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailToSMSAllowedAddressController.updateEmailToSMSAllowedAddressAsync") updateEmailToSMSAllowedAddressAsync

> Update a specific allowed email address.


```java
void updateEmailToSMSAllowedAddressAsync(
        final double emailAddressId,
        final UpdateEmailToSMSAllowedAddressRequest body,
        final APICallBack<UpdateEmailToSMSAllowedAddressResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | Your email address id. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    double emailAddressId = 107;
    String bodyValue = "    {        \"email_address\":\"pfvRZ@gmail.com\",        \"from\":\"+17128842283\"    }";
    UpdateEmailToSMSAllowedAddressRequest body = mapper.readValue(bodyValue,new TypeReference<UpdateEmailToSMSAllowedAddressRequest> (){});
    // Invoking the API call with sample inputs
    emailToSMSAllowedAddress.updateEmailToSMSAllowedAddressAsync(emailAddressId, body, new APICallBack<UpdateEmailToSMSAllowedAddressResponse>() {
        public void onSuccess(HttpContext context, UpdateEmailToSMSAllowedAddressResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="delete_email_to_sms_allowed_address_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailToSMSAllowedAddressController.deleteEmailToSMSAllowedAddressAsync") deleteEmailToSMSAllowedAddressAsync

> Delete a specific allowed email address.


```java
void deleteEmailToSMSAllowedAddressAsync(
        final double emailAddressId,
        final APICallBack<DeleteEmailToSMSAllowedAddressResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | Your email address id. |


#### Example Usage

```java
double emailAddressId = 107;
// Invoking the API call with sample inputs
emailToSMSAllowedAddress.deleteEmailToSMSAllowedAddressAsync(emailAddressId, new APICallBack<DeleteEmailToSMSAllowedAddressResponse>() {
    public void onSuccess(HttpContext context, DeleteEmailToSMSAllowedAddressResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="email_to_sms_stripped_strings_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.EmailToSMSStrippedStringsController") EmailToSMSStrippedStringsController

### Get singleton instance

The singleton instance of the ``` EmailToSMSStrippedStringsController ``` class can be accessed from the API Client.

```java
EmailToSMSStrippedStringsController emailToSMSStrippedStrings = client.getEmailToSMSStrippedStrings();
```

### <a name="list_stripped_strings_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailToSMSStrippedStringsController.listStrippedStringsAsync") listStrippedStringsAsync

> TODO: Add a method description


```java
void listStrippedStringsAsync(final APICallBack<ListStrippedStringsResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
emailToSMSStrippedStrings.listStrippedStringsAsync(new APICallBack<ListStrippedStringsResponse>() {
    public void onSuccess(HttpContext context, ListStrippedStringsResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="find_specific_stripped_string_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailToSMSStrippedStringsController.findSpecificStrippedStringAsync") findSpecificStrippedStringAsync

> TODO: Add a method description


```java
void findSpecificStrippedStringAsync(
        final double ruleId,
        final APICallBack<FindSpecificStrippedStringResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |


#### Example Usage

```java
double ruleId = 18;
// Invoking the API call with sample inputs
emailToSMSStrippedStrings.findSpecificStrippedStringAsync(ruleId, new APICallBack<FindSpecificStrippedStringResponse>() {
    public void onSuccess(HttpContext context, FindSpecificStrippedStringResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_stripped_string_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailToSMSStrippedStringsController.createStrippedStringAsync") createStrippedStringAsync

> TODO: Add a method description


```java
void createStrippedStringAsync(
        final CreateStrippedStringRequest body,
        final APICallBack<CreateStrippedStringResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "{    \"strip_string\" : \"~~~test~~~\"}";
    CreateStrippedStringRequest body = mapper.readValue(bodyValue,new TypeReference<CreateStrippedStringRequest> (){});
    // Invoking the API call with sample inputs
    emailToSMSStrippedStrings.createStrippedStringAsync(body, new APICallBack<CreateStrippedStringResponse>() {
        public void onSuccess(HttpContext context, CreateStrippedStringResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="update_stripped_string_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailToSMSStrippedStringsController.updateStrippedStringAsync") updateStrippedStringAsync

> TODO: Add a method description


```java
void updateStrippedStringAsync(
        final double ruleId,
        final UpdateStrippedStringRequest body,
        final APICallBack<UpdateStrippedStringResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    double ruleId = 20;
    String bodyValue = "{    \"strip_string\" : \"~~~test1~~~\"}";
    UpdateStrippedStringRequest body = mapper.readValue(bodyValue,new TypeReference<UpdateStrippedStringRequest> (){});
    // Invoking the API call with sample inputs
    emailToSMSStrippedStrings.updateStrippedStringAsync(ruleId, body, new APICallBack<UpdateStrippedStringResponse>() {
        public void onSuccess(HttpContext context, UpdateStrippedStringResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="delete_stripped_string_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.EmailToSMSStrippedStringsController.deleteStrippedStringAsync") deleteStrippedStringAsync

> TODO: Add a method description


```java
void deleteStrippedStringAsync(
        final double ruleId,
        final APICallBack<DeleteStrippedStringResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |


#### Example Usage

```java
double ruleId = 20;
// Invoking the API call with sample inputs
emailToSMSStrippedStrings.deleteStrippedStringAsync(ruleId, new APICallBack<DeleteStrippedStringResponse>() {
    public void onSuccess(HttpContext context, DeleteStrippedStringResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="fax_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.FaxController") FaxController

### Get singleton instance

The singleton instance of the ``` FaxController ``` class can be accessed from the API Client.

```java
FaxController fax = client.getFax();
```

### <a name="create_send_fax_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.FaxController.createSendFaxAsync") createSendFaxAsync

> **Letter File Options**
> **Use existing URL**
> With this option, you can use an existing URL to a PDF document. For example, you might generate the pdf on your server.
> **Upload File to Our Server**
> With this option, you can use the `/uploads` endpoint to upload the document. The `/uploads` endpoint returns a URL that can be used in the `/fax/send` endpoint.


```java
void createSendFaxAsync(
        final SendFaxRequest body,
        final APICallBack<SendFaxResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    SendFaxRequest body = new SendFaxRequest();
    // Invoking the API call with sample inputs
    fax.createSendFaxAsync(body, new APICallBack<SendFaxResponse>() {
        public void onSuccess(HttpContext context, SendFaxResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="create_calculate_price_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.FaxController.createCalculatePriceAsync") createCalculatePriceAsync

> TODO: Add a method description


```java
void createCalculatePriceAsync(
        final CalculatePriceRequest132 body,
        final APICallBack<CalculatePriceResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    CalculatePriceRequest132 body = new CalculatePriceRequest132();
    // Invoking the API call with sample inputs
    fax.createCalculatePriceAsync(body, new APICallBack<CalculatePriceResponse>() {
        public void onSuccess(HttpContext context, CalculatePriceResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="get_fax_history_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.FaxController.getFaxHistoryAsync") getFaxHistoryAsync

> Get a list of Fax History.


```java
void getFaxHistoryAsync(
        final Double dateFrom,
        final Double dateTo,
        final String q,
        final String orderBy,
        final APICallBack<GetFaxHistoryResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateFrom |  ``` Optional ```  | Customize result by setting from date (timestsamp) |
| dateTo |  ``` Optional ```  | Customize result by setting to date (timestamp) |
| q |  ``` Optional ```  | Custom query |
| orderBy |  ``` Optional ```  | Order result by |


#### Example Usage

```java
Double dateFrom = 1457572619;
Double dateTo = 1457573000;
String q = "status:Sent,status_code:201";
String orderBy = "subject:desc";
// Invoking the API call with sample inputs
fax.getFaxHistoryAsync(dateFrom, dateTo, q, orderBy, new APICallBack<GetFaxHistoryResponse>() {
    public void onSuccess(HttpContext context, GetFaxHistoryResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="list_of_fax_delivery_receipts_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.FaxController.listOfFaxDeliveryReceiptsAsync") listOfFaxDeliveryReceiptsAsync

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


```java
void listOfFaxDeliveryReceiptsAsync(final APICallBack<ListOfFaxDeliveryReceiptsResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
fax.listOfFaxDeliveryReceiptsAsync(new APICallBack<ListOfFaxDeliveryReceiptsResponse>() {
    public void onSuccess(HttpContext context, ListOfFaxDeliveryReceiptsResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_a_specific_fax_delivery_receipt_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.FaxController.getASpecificFaxDeliveryReceiptAsync") getASpecificFaxDeliveryReceiptAsync

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


```java
void getASpecificFaxDeliveryReceiptAsync(
        final String messageId,
        final APICallBack<GetASpecificFaxDeliveryReceiptResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | D2AF-479B-8955-6395D561DEF4" (required, number) - Message ID. |


#### Example Usage

```java
String messageId = "\"3FAC74F1";
// Invoking the API call with sample inputs
fax.getASpecificFaxDeliveryReceiptAsync(messageId, new APICallBack<GetASpecificFaxDeliveryReceiptResponse>() {
    public void onSuccess(HttpContext context, GetASpecificFaxDeliveryReceiptResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="update_mark_fax_delivery_receipts_as_read_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.FaxController.updateMarkFaxDeliveryReceiptsAsReadAsync") updateMarkFaxDeliveryReceiptsAsReadAsync

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


```java
void updateMarkFaxDeliveryReceiptsAsReadAsync(
        final MarkFaxDeliveryReceiptsAsReadRequest body,
        final APICallBack<MarkFaxDeliveryReceiptsAsReadResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "{    \"date_before\": 1441958441}";
    MarkFaxDeliveryReceiptsAsReadRequest body = mapper.readValue(bodyValue,new TypeReference<MarkFaxDeliveryReceiptsAsReadRequest> (){});
    // Invoking the API call with sample inputs
    fax.updateMarkFaxDeliveryReceiptsAsReadAsync(body, new APICallBack<MarkFaxDeliveryReceiptsAsReadResponse>() {
        public void onSuccess(HttpContext context, MarkFaxDeliveryReceiptsAsReadResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="add_a_test_delivery_receipt_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.FaxController.addATestDeliveryReceiptAsync") addATestDeliveryReceiptAsync

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


```java
void addATestDeliveryReceiptAsync(
        final AddATestDeliveryReceiptRequest body,
        final APICallBack<AddATestDeliveryReceiptResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "    {        \"url\":\"http://yourUrl.com\"    }";
    AddATestDeliveryReceiptRequest body = mapper.readValue(bodyValue,new TypeReference<AddATestDeliveryReceiptRequest> (){});
    // Invoking the API call with sample inputs
    fax.addATestDeliveryReceiptAsync(body, new APICallBack<AddATestDeliveryReceiptResponse>() {
        public void onSuccess(HttpContext context, AddATestDeliveryReceiptResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


[Back to List of Controllers](#list_of_controllers)

## <a name="forgot_account_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.ForgotAccountController") ForgotAccountController

### Get singleton instance

The singleton instance of the ``` ForgotAccountController ``` class can be accessed from the API Client.

```java
ForgotAccountController forgotAccount = client.getForgotAccount();
```

### <a name="update_forgot_username_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ForgotAccountController.updateForgotUsernameAsync") updateForgotUsernameAsync

> TODO: Add a method description


```java
void updateForgotUsernameAsync(
        final ForgotUsernameRequest body,
        final APICallBack<ForgotUsernameResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    ForgotUsernameRequest body = new ForgotUsernameRequest();
    // Invoking the API call with sample inputs
    forgotAccount.updateForgotUsernameAsync(body, new APICallBack<ForgotUsernameResponse>() {
        public void onSuccess(HttpContext context, ForgotUsernameResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="update_forgot_password_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ForgotAccountController.updateForgotPasswordAsync") updateForgotPasswordAsync

> TODO: Add a method description


```java
void updateForgotPasswordAsync(
        final ForgotPasswordRequest body,
        final APICallBack<ForgotPasswordResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "    {        \"username\": \"0F6pKiiuca\"    }";
    ForgotPasswordRequest body = mapper.readValue(bodyValue,new TypeReference<ForgotPasswordRequest> (){});
    // Invoking the API call with sample inputs
    forgotAccount.updateForgotPasswordAsync(body, new APICallBack<ForgotPasswordResponse>() {
        public void onSuccess(HttpContext context, ForgotPasswordResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="update_verify_forgot_password_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ForgotAccountController.updateVerifyForgotPasswordAsync") updateVerifyForgotPasswordAsync

> TODO: Add a method description


```java
void updateVerifyForgotPasswordAsync(
        final VerifyForgotPasswordRequest body,
        final APICallBack<VerifyForgotPasswordResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "    {        \"subaccount_id\": 54,        \"activation_token\": \"9C648BAD-EB7F-4E7E-96BC-B433140C4F1F\",        \"password\": \"0F6pKiiuca\"    }";
    VerifyForgotPasswordRequest body = mapper.readValue(bodyValue,new TypeReference<VerifyForgotPasswordRequest> (){});
    // Invoking the API call with sample inputs
    forgotAccount.updateVerifyForgotPasswordAsync(body, new APICallBack<VerifyForgotPasswordResponse>() {
        public void onSuccess(HttpContext context, VerifyForgotPasswordResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


[Back to List of Controllers](#list_of_controllers)

## <a name="mms_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.MMSController") MMSController

### Get singleton instance

The singleton instance of the ``` MMSController ``` class can be accessed from the API Client.

```java
MMSController mMS = client.getMMS();
```

### <a name="create_send_mms_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.MMSController.createSendMMSAsync") createSendMMSAsync

> TODO: Add a method description


```java
void createSendMMSAsync(
        final SendMMSRequest body,
        final APICallBack<SendMMSResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    SendMMSRequest body = new SendMMSRequest();
    // Invoking the API call with sample inputs
    mMS.createSendMMSAsync(body, new APICallBack<SendMMSResponse>() {
        public void onSuccess(HttpContext context, SendMMSResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="create_get_price_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.MMSController.createGetPriceAsync") createGetPriceAsync

> TODO: Add a method description


```java
void createGetPriceAsync(
        final GetPriceRequest body,
        final APICallBack<GetPriceResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    GetPriceRequest body = new GetPriceRequest();
    // Invoking the API call with sample inputs
    mMS.createGetPriceAsync(body, new APICallBack<GetPriceResponse>() {
        public void onSuccess(HttpContext context, GetPriceResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="get_mms_history_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.MMSController.getMMSHistoryAsync") getMMSHistoryAsync

> TODO: Add a method description


```java
void getMMSHistoryAsync(
        final String q,
        final String orderBy,
        final Integer dateFrom,
        final Integer dateTo,
        final APICallBack<GetMMSHistoryResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| q |  ``` Optional ```  | A custom query. |
| orderBy |  ``` Optional ```  | Sort records by. |
| dateFrom |  ``` Optional ```  | Timestamp (from) used to show records by date. |
| dateTo |  ``` Optional ```  | Timestamp (to) used to show records by date. |


#### Example Usage

```java
String q = "list_id:429,direction:out";
String orderBy = "subject:desc";
Integer dateFrom = 1443501617;
Integer dateTo = 1443501727;
// Invoking the API call with sample inputs
mMS.getMMSHistoryAsync(q, orderBy, dateFrom, dateTo, new APICallBack<GetMMSHistoryResponse>() {
    public void onSuccess(HttpContext context, GetMMSHistoryResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_export_mms_history_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.MMSController.getExportMMSHistoryAsync") getExportMMSHistoryAsync

> TODO: Add a method description


```java
void getExportMMSHistoryAsync(
        final String filename,
        final APICallBack<ExportMMSHistoryResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | Your export filename. |


#### Example Usage

```java
String filename = "export.csv";
// Invoking the API call with sample inputs
mMS.getExportMMSHistoryAsync(filename, new APICallBack<ExportMMSHistoryResponse>() {
    public void onSuccess(HttpContext context, ExportMMSHistoryResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="update_cancel_mms_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.MMSController.updateCancelMMSAsync") updateCancelMMSAsync

> TODO: Add a method description


```java
void updateCancelMMSAsync(
        final String messageId,
        final APICallBack<CancelMMSResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Message ID. |


#### Example Usage

```java
String messageId = "message_id";
// Invoking the API call with sample inputs
mMS.updateCancelMMSAsync(messageId, new APICallBack<CancelMMSResponse>() {
    public void onSuccess(HttpContext context, CancelMMSResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="update_cancel_all_mms_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.MMSController.updateCancelAllMMSAsync") updateCancelAllMMSAsync

> TODO: Add a method description


```java
void updateCancelAllMMSAsync(final APICallBack<CancelAllMMSResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
mMS.updateCancelAllMMSAsync(new APICallBack<CancelAllMMSResponse>() {
    public void onSuccess(HttpContext context, CancelAllMMSResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_all_delivery_receipts_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.MMSController.getAllDeliveryReceiptsAsync") getAllDeliveryReceiptsAsync

> TODO: Add a method description


```java
void getAllDeliveryReceiptsAsync(final APICallBack<GetAllDeliveryReceiptsResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
mMS.getAllDeliveryReceiptsAsync(new APICallBack<GetAllDeliveryReceiptsResponse>() {
    public void onSuccess(HttpContext context, GetAllDeliveryReceiptsResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_delivery_receipt_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.MMSController.getDeliveryReceiptAsync") getDeliveryReceiptAsync

> TODO: Add a method description


```java
void getDeliveryReceiptAsync(
        final String messageId,
        final APICallBack<GetDeliveryReceiptResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Message ID. |


#### Example Usage

```java
String messageId = "3E0DC217-7D0F-4C20-A3F2-E3362B938CAF";
// Invoking the API call with sample inputs
mMS.getDeliveryReceiptAsync(messageId, new APICallBack<GetDeliveryReceiptResponse>() {
    public void onSuccess(HttpContext context, GetDeliveryReceiptResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="update_mark_receipts_as_read_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.MMSController.updateMarkReceiptsAsReadAsync") updateMarkReceiptsAsReadAsync

> TODO: Add a method description


```java
void updateMarkReceiptsAsReadAsync(final APICallBack<MarkReceiptsAsReadResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
mMS.updateMarkReceiptsAsReadAsync(new APICallBack<MarkReceiptsAsReadResponse>() {
    public void onSuccess(HttpContext context, MarkReceiptsAsReadResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_all_inbound_sms_pull_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.MMSController.getAllInboundSMSPullAsync") getAllInboundSMSPullAsync

> Inbound MMS shares the same rules/settings/endpoints as SMS. Any attachments will be converted to a URL.
> **Push Inbound SMS**
> If you prefer, we can push message replies to your server as they arrive with us.
> Refer to SMS->Inbound SMS in the docs.
> **Pull Inbound SMS**
> Receive SMS by polling your Inbox.
> Refer to SMS->Inbound SMS in the docs.


```java
void getAllInboundSMSPullAsync(final APICallBack<DynamicResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
mMS.getAllInboundSMSPullAsync(new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="numbers_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.NumbersController") NumbersController

### Get singleton instance

The singleton instance of the ``` NumbersController ``` class can be accessed from the API Client.

```java
NumbersController numbers = client.getNumbers();
```

### <a name="get_all_dedicated_numbers_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.NumbersController.getAllDedicatedNumbersAsync") getAllDedicatedNumbersAsync

> TODO: Add a method description


```java
void getAllDedicatedNumbersAsync(final APICallBack<GetAllDedicatedNumbersResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
numbers.getAllDedicatedNumbersAsync(new APICallBack<GetAllDedicatedNumbersResponse>() {
    public void onSuccess(HttpContext context, GetAllDedicatedNumbersResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_buy_dedicated_number_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.NumbersController.createBuyDedicatedNumberAsync") createBuyDedicatedNumberAsync

> TODO: Add a method description


```java
void createBuyDedicatedNumberAsync(
        final String dedicatedNumber,
        final APICallBack<BuyDedicatedNumberResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dedicatedNumber |  ``` Required ```  | Your phone number in E.164 format. |


#### Example Usage

```java
String dedicatedNumber = "+12282060576";
// Invoking the API call with sample inputs
numbers.createBuyDedicatedNumberAsync(dedicatedNumber, new APICallBack<BuyDedicatedNumberResponse>() {
    public void onSuccess(HttpContext context, BuyDedicatedNumberResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="search_dedicated_numbers_by_country_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.NumbersController.searchDedicatedNumbersByCountryAsync") searchDedicatedNumbersByCountryAsync

> TODO: Add a method description


```java
void searchDedicatedNumbersByCountryAsync(
        final String country,
        final String search,
        final Double searchType,
        final APICallBack<SearchDedicatedNumbersByCountryResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Required ```  | Your preferred country. |
| search |  ``` Optional ```  | Your search pattern or query. |
| searchType |  ``` Optional ```  | Your strategy for searching, 0 = starts with, 1 = anywhere, 2 = ends with. |


#### Example Usage

```java
String country = "US";
String search = "88";
Double searchType = 1;
// Invoking the API call with sample inputs
numbers.searchDedicatedNumbersByCountryAsync(country, search, searchType, new APICallBack<SearchDedicatedNumbersByCountryResponse>() {
    public void onSuccess(HttpContext context, SearchDedicatedNumbersByCountryResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="pricing_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.PricingController") PricingController

### Get singleton instance

The singleton instance of the ``` PricingController ``` class can be accessed from the API Client.

```java
PricingController pricing = client.getPricing();
```

### <a name="get_country_pricing_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.PricingController.getCountryPricingAsync") getCountryPricingAsync

> TODO: Add a method description


```java
void getCountryPricingAsync(
        final String country,
        final String currency,
        final APICallBack<GetCountryPricingResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Required ```  | Two-letter representation of the country. |
| currency |  ``` Optional ```  | Three-letter representation of the currency. |


#### Example Usage

```java
String country = "AU";
String currency = "AUD";
// Invoking the API call with sample inputs
pricing.getCountryPricingAsync(country, currency, new APICallBack<GetCountryPricingResponse>() {
    public void onSuccess(HttpContext context, GetCountryPricingResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="post_direct_mail_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.PostDirectMailController") PostDirectMailController

### Get singleton instance

The singleton instance of the ``` PostDirectMailController ``` class can be accessed from the API Client.

```java
PostDirectMailController postDirectMail = client.getPostDirectMail();
```

### <a name="search_locations_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.PostDirectMailController.searchLocationsAsync") searchLocationsAsync

> TODO: Add a method description


```java
void searchLocationsAsync(
        final String country,
        final String query,
        final APICallBack<SearchLocationsResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Required ```  | Country code. |
| query |  ``` Required ```  | A postal code or place name. |


#### Example Usage

```java
String country = "AD";
String query = "AD100";
// Invoking the API call with sample inputs
postDirectMail.searchLocationsAsync(country, query, new APICallBack<SearchLocationsResponse>() {
    public void onSuccess(HttpContext context, SearchLocationsResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_new_campaign_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.PostDirectMailController.createNewCampaignAsync") createNewCampaignAsync

> Create new direct mail campaign.


```java
void createNewCampaignAsync(
        final CreateNewCampaignRequest body,
        final APICallBack<CreateNewCampaignResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    CreateNewCampaignRequest body = new CreateNewCampaignRequest();
    // Invoking the API call with sample inputs
    postDirectMail.createNewCampaignAsync(body, new APICallBack<CreateNewCampaignResponse>() {
        public void onSuccess(HttpContext context, CreateNewCampaignResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="create_calculate_direct_mail_campaign_price_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.PostDirectMailController.createCalculateDirectMailCampaignPriceAsync") createCalculateDirectMailCampaignPriceAsync

> Calculate direct mail campaign price.


```java
void createCalculateDirectMailCampaignPriceAsync(
        final CalculateDirectMailCampaignPriceRequest body,
        final APICallBack<CalculateDirectMailCampaignPriceResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    CalculateDirectMailCampaignPriceRequest body = new CalculateDirectMailCampaignPriceRequest();
    // Invoking the API call with sample inputs
    postDirectMail.createCalculateDirectMailCampaignPriceAsync(body, new APICallBack<CalculateDirectMailCampaignPriceResponse>() {
        public void onSuccess(HttpContext context, CalculateDirectMailCampaignPriceResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="list_direct_mail_campaigns_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.PostDirectMailController.listDirectMailCampaignsAsync") listDirectMailCampaignsAsync

> Get list of direct mail campaigns.


```java
void listDirectMailCampaignsAsync(final APICallBack<ListDirectMailCampaignsResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
postDirectMail.listDirectMailCampaignsAsync(new APICallBack<ListDirectMailCampaignsResponse>() {
    public void onSuccess(HttpContext context, ListDirectMailCampaignsResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="post_letter_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.PostLetterController") PostLetterController

### Get singleton instance

The singleton instance of the ``` PostLetterController ``` class can be accessed from the API Client.

```java
PostLetterController postLetter = client.getPostLetter();
```

### <a name="create_send_post_letter_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.PostLetterController.createSendPostLetterAsync") createSendPostLetterAsync

> **Supported File Types**
> We support `pdf`, `docx` and `doc` files. Contact us to add support for any other file type. If you're using `docx` or `doc` files, you'll need to convert the file first using our uploads endpoint with the querystring parameter `convert=post` e.g. `POST /uploads?convert=post`. This will return a URL to the converted pdf file that can be used in the `/post/letters/send` endpoint.
> **Letter File Options**
> **Use existing URL**
> With this option, you can use an existing URL to a `pdf` document. For example, you might generate the `pdf` on your server.
> **Upload File to Our Server**
> With this option, you can use the `/uploads` endpoint to upload the document. The `/uploads` endpoint returns a URL that can be used in the `/post/letters/send` endpoint.


```java
void createSendPostLetterAsync(
        final SendPostLetterRequest body,
        final APICallBack<SendPostLetterResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "{  \"file_url\": \"http://server.com/file.pdf\",  \"template_used\": 1,  \"colour\": 1,  \"duplex\": 0,  \"recipients\": [    {      \"address_name\": \"My Home Address\",      \"address_line_1\": \"Address 1\",      \"address_line_2\": \"Address 2\",      \"address_city\": \"CITY\",      \"address_state\": \"State\",      \"address_postal_code\": 123456,      \"address_country\": \"AU\",      \"return_address_id\": 1,      \"schedule\": 1449573604    }  ]}";
    SendPostLetterRequest body = mapper.readValue(bodyValue,new TypeReference<SendPostLetterRequest> (){});
    // Invoking the API call with sample inputs
    postLetter.createSendPostLetterAsync(body, new APICallBack<SendPostLetterResponse>() {
        public void onSuccess(HttpContext context, SendPostLetterResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="create_calculate_price_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.PostLetterController.createCalculatePriceAsync") createCalculatePriceAsync

> TODO: Add a method description


```java
void createCalculatePriceAsync(
        final CalculatePriceRequest170 body,
        final APICallBack<CalculatePriceResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "{  \"file_url\": \"http://server.com/file.pdf\",  \"template_used\": 1,  \"colour\": 1,  \"duplex\": 0,  \"recipients\": [    \"[]\"  ],  \"Body\": \"\"}";
    CalculatePriceRequest170 body = mapper.readValue(bodyValue,new TypeReference<CalculatePriceRequest170> (){});
    // Invoking the API call with sample inputs
    postLetter.createCalculatePriceAsync(body, new APICallBack<CalculatePriceResponse>() {
        public void onSuccess(HttpContext context, CalculatePriceResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="get_post_letter_history_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.PostLetterController.getPostLetterHistoryAsync") getPostLetterHistoryAsync

> TODO: Add a method description


```java
void getPostLetterHistoryAsync(final APICallBack<GetPostLetterHistoryResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
postLetter.getPostLetterHistoryAsync(new APICallBack<GetPostLetterHistoryResponse>() {
    public void onSuccess(HttpContext context, GetPostLetterHistoryResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_export_post_letter_history_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.PostLetterController.getExportPostLetterHistoryAsync") getExportPostLetterHistoryAsync

> TODO: Add a method description


```java
void getExportPostLetterHistoryAsync(
        final String filename,
        final APICallBack<ExportPostLetterHistoryResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | Filename for the export file. |


#### Example Usage

```java
String filename = "myexport.csv";
// Invoking the API call with sample inputs
postLetter.getExportPostLetterHistoryAsync(filename, new APICallBack<ExportPostLetterHistoryResponse>() {
    public void onSuccess(HttpContext context, ExportPostLetterHistoryResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_a_post_return_address_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.PostLetterController.createAPostReturnAddressAsync") createAPostReturnAddressAsync

> TODO: Add a method description


```java
void createAPostReturnAddressAsync(
        final CreateAPostReturnAddressRequest body,
        final APICallBack<CreateAPostReturnAddressResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "{    \"address_name\":\"My Home Address\",    \"address_line_1\":\"Maritime Avenue\",    \"address_line_2\":\"\",    \"address_city\":\"Flynn\",    \"address_state\":\"WA\",    \"address_postal_code\":6302,    \"address_country\":\"Australia\"}";
    CreateAPostReturnAddressRequest body = mapper.readValue(bodyValue,new TypeReference<CreateAPostReturnAddressRequest> (){});
    // Invoking the API call with sample inputs
    postLetter.createAPostReturnAddressAsync(body, new APICallBack<CreateAPostReturnAddressResponse>() {
        public void onSuccess(HttpContext context, CreateAPostReturnAddressResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="get_list_of_post_return_addresses_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.PostLetterController.getListOfPostReturnAddressesAsync") getListOfPostReturnAddressesAsync

> TODO: Add a method description


```java
void getListOfPostReturnAddressesAsync(final APICallBack<GetListOfPostReturnAddressesResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
postLetter.getListOfPostReturnAddressesAsync(new APICallBack<GetListOfPostReturnAddressesResponse>() {
    public void onSuccess(HttpContext context, GetListOfPostReturnAddressesResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_post_return_address_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.PostLetterController.getPostReturnAddressAsync") getPostReturnAddressAsync

> TODO: Add a method description


```java
void getPostReturnAddressAsync(
        final double returnAddressId,
        final APICallBack<GetPostReturnAddressResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| returnAddressId |  ``` Required ```  | Your return address id. |


#### Example Usage

```java
double returnAddressId = 14;
// Invoking the API call with sample inputs
postLetter.getPostReturnAddressAsync(returnAddressId, new APICallBack<GetPostReturnAddressResponse>() {
    public void onSuccess(HttpContext context, GetPostReturnAddressResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="update_post_return_address_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.PostLetterController.updatePostReturnAddressAsync") updatePostReturnAddressAsync

> TODO: Add a method description


```java
void updatePostReturnAddressAsync(
        final double returnAddressId,
        final UpdatePostReturnAddressRequest body,
        final APICallBack<UpdatePostReturnAddressResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| returnAddressId |  ``` Required ```  | Your return address id. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    double returnAddressId = 14;
    String bodyValue = "{    \"address_name\":\"My Home Address\",    \"address_line_1\":\"Maritime Avenue\",    \"address_line_2\":\"\",    \"address_city\":\"Flynn\",    \"address_state\":\"WA\",    \"address_postal_code\":6302,    \"address_country\":\"Australia\"}";
    UpdatePostReturnAddressRequest body = mapper.readValue(bodyValue,new TypeReference<UpdatePostReturnAddressRequest> (){});
    // Invoking the API call with sample inputs
    postLetter.updatePostReturnAddressAsync(returnAddressId, body, new APICallBack<UpdatePostReturnAddressResponse>() {
        public void onSuccess(HttpContext context, UpdatePostReturnAddressResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="delete_post_return_address_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.PostLetterController.deletePostReturnAddressAsync") deletePostReturnAddressAsync

> TODO: Add a method description


```java
void deletePostReturnAddressAsync(
        final double returnAddressId,
        final APICallBack<DeletePostReturnAddressResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| returnAddressId |  ``` Required ```  | Your return address id. |


#### Example Usage

```java
double returnAddressId = 12;
// Invoking the API call with sample inputs
postLetter.deletePostReturnAddressAsync(returnAddressId, new APICallBack<DeletePostReturnAddressResponse>() {
    public void onSuccess(HttpContext context, DeletePostReturnAddressResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="postcards_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.PostcardsController") PostcardsController

### Get singleton instance

The singleton instance of the ``` PostcardsController ``` class can be accessed from the API Client.

```java
PostcardsController postcards = client.getPostcards();
```

### <a name="create_send_postcard_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.PostcardsController.createSendPostcardAsync") createSendPostcardAsync

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


```java
void createSendPostcardAsync(
        final SendPostcardRequest body,
        final APICallBack<SendPostcardResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "{    \"file_urls\":[         \"https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_front.pdf\",         \"https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_back.pdf\"    ],    \"recipients\":[        {            \"address_name\":\"My Home Address\",            \"address_line_1\":\"Address 1\",            \"address_line_2\":\"\",            \"address_city\":\"City\",            \"address_state\":\"State\",            \"address_postal_code\":\"123456\",            \"address_country\":\"AU\",            \"return_address_id\":1        }    ]}";
    SendPostcardRequest body = mapper.readValue(bodyValue,new TypeReference<SendPostcardRequest> (){});
    // Invoking the API call with sample inputs
    postcards.createSendPostcardAsync(body, new APICallBack<SendPostcardResponse>() {
        public void onSuccess(HttpContext context, SendPostcardResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="create_calculate_pricing_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.PostcardsController.createCalculatePricingAsync") createCalculatePricingAsync

> For `file_urls` field. You can attach at least 1 and max of 2 PDF file urls.
> - Supply a single pdf with 2 pages (front and back)
> - Supply 2 urls to seperate PDFs


```java
void createCalculatePricingAsync(
        final CalculatePricingRequest body,
        final APICallBack<CalculatePricingResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "{    \"file_urls\":[        \"https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_front.pdf\",        \"https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_back.pdf\"    ],    \"recipients\":[        {            \"address_name\":\"My Home Address\",            \"address_line_1\":\"Address 1\",            \"address_line_2\":\"\",            \"address_city\":\"City\",            \"address_state\":\"State\",            \"address_postal_code\":\"123456\",            \"address_country\":\"AU\",            \"return_address_id\":1        }    ]}";
    CalculatePricingRequest body = mapper.readValue(bodyValue,new TypeReference<CalculatePricingRequest> (){});
    // Invoking the API call with sample inputs
    postcards.createCalculatePricingAsync(body, new APICallBack<CalculatePricingResponse>() {
        public void onSuccess(HttpContext context, CalculatePricingResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="get_postcard_history_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.PostcardsController.getPostcardHistoryAsync") getPostcardHistoryAsync

> TODO: Add a method description


```java
void getPostcardHistoryAsync(final APICallBack<GetPostcardHistoryResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
postcards.getPostcardHistoryAsync(new APICallBack<GetPostcardHistoryResponse>() {
    public void onSuccess(HttpContext context, GetPostcardHistoryResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_export_postcard_history_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.PostcardsController.getExportPostcardHistoryAsync") getExportPostcardHistoryAsync

> TODO: Add a method description


```java
void getExportPostcardHistoryAsync(
        final String filename,
        final APICallBack<ExportPostcardHistoryResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | Filename for the export file. |


#### Example Usage

```java
String filename = "myexport.csv";
// Invoking the API call with sample inputs
postcards.getExportPostcardHistoryAsync(filename, new APICallBack<ExportPostcardHistoryResponse>() {
    public void onSuccess(HttpContext context, ExportPostcardHistoryResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="referral_accounts_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.ReferralAccountsController") ReferralAccountsController

### Get singleton instance

The singleton instance of the ``` ReferralAccountsController ``` class can be accessed from the API Client.

```java
ReferralAccountsController referralAccounts = client.getReferralAccounts();
```

### <a name="get_list_of_referral_accounts_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ReferralAccountsController.getListOfReferralAccountsAsync") getListOfReferralAccountsAsync

> TODO: Add a method description


```java
void getListOfReferralAccountsAsync(final APICallBack<GetListOfReferralAccountsResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
referralAccounts.getListOfReferralAccountsAsync(new APICallBack<GetListOfReferralAccountsResponse>() {
    public void onSuccess(HttpContext context, GetListOfReferralAccountsResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="reseller_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.ResellerController") ResellerController

### Get singleton instance

The singleton instance of the ``` ResellerController ``` class can be accessed from the API Client.

```java
ResellerController reseller = client.getReseller();
```

### <a name="get_reseller_setting_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ResellerController.getResellerSettingAsync") getResellerSettingAsync

> Get reseller setting.


```java
void getResellerSettingAsync(final APICallBack<GetResellerSettingResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
reseller.getResellerSettingAsync(new APICallBack<GetResellerSettingResponse>() {
    public void onSuccess(HttpContext context, GetResellerSettingResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="update_reseller_setting_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ResellerController.updateResellerSettingAsync") updateResellerSettingAsync

> Update a specific reseller setting.


```java
void updateResellerSettingAsync(
        final UpdateResellerSettingRequest body,
        final APICallBack<UpdateResellerSettingResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "    {        \"allow_public_signups\":1,        \"default_margin\":100,        \"default_margin_numbers\":150,        \"trial_balance\":50,        \"subdomain\":\"subdomain\",        \"colour_navigation\":\"#9999FF\",        \"logo_url_light\":\"http://url.com/light\",        \"logo_url_dark\":\"http://url.com/dark\",        \"company_name\":\"MyCompany\"    }";
    UpdateResellerSettingRequest body = mapper.readValue(bodyValue,new TypeReference<UpdateResellerSettingRequest> (){});
    // Invoking the API call with sample inputs
    reseller.updateResellerSettingAsync(body, new APICallBack<UpdateResellerSettingResponse>() {
        public void onSuccess(HttpContext context, UpdateResellerSettingResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="get_reseller_by_subdomain_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ResellerController.getResellerBySubdomainAsync") getResellerBySubdomainAsync

> Get reseller setting by subdomin.


```java
void getResellerBySubdomainAsync(
        final String subdomain,
        final APICallBack<ResellerBySubdomainResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subdomain |  ``` Required ```  | Subdomain |


#### Example Usage

```java
String subdomain = "mysubdomain";
// Invoking the API call with sample inputs
reseller.getResellerBySubdomainAsync(subdomain, new APICallBack<ResellerBySubdomainResponse>() {
    public void onSuccess(HttpContext context, ResellerBySubdomainResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="reseller_accounts_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.ResellerAccountsController") ResellerAccountsController

### Get singleton instance

The singleton instance of the ``` ResellerAccountsController ``` class can be accessed from the API Client.

```java
ResellerAccountsController resellerAccounts = client.getResellerAccounts();
```

### <a name="list_of_reseller_accounts_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ResellerAccountsController.listOfResellerAccountsAsync") listOfResellerAccountsAsync

> Get list of Reseller Accounts


```java
void listOfResellerAccountsAsync(final APICallBack<ListOfResellerAccountsResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
resellerAccounts.listOfResellerAccountsAsync(new APICallBack<ListOfResellerAccountsResponse>() {
    public void onSuccess(HttpContext context, ListOfResellerAccountsResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_reseller_account_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ResellerAccountsController.getResellerAccountAsync") getResellerAccountAsync

> Get a specific reseller account.


```java
void getResellerAccountAsync(
        final double clientUserId,
        final APICallBack<GetResellerAccountResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| clientUserId |  ``` Required ```  | The client user id. |


#### Example Usage

```java
double clientUserId = 24;
// Invoking the API call with sample inputs
resellerAccounts.getResellerAccountAsync(clientUserId, new APICallBack<GetResellerAccountResponse>() {
    public void onSuccess(HttpContext context, GetResellerAccountResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_reseller_account_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ResellerAccountsController.createResellerAccountAsync") createResellerAccountAsync

> TODO: Add a method description


```java
void createResellerAccountAsync(
        final CreateResellerAccountRequest body,
        final APICallBack<CreateResellerAccountResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "    {        \"username\":\"johndoe2\",        \"user_email\":\"johndoe2@awesome.com\",        \"user_phone\":\"518-481-1002\",        \"user_first_name\":\"John\",        \"user_last_name\":\"Doe\",        \"country\":\"US\",        \"password\":\"pass\",        \"account_name\":\"The Awesome Company\"    }";
    CreateResellerAccountRequest body = mapper.readValue(bodyValue,new TypeReference<CreateResellerAccountRequest> (){});
    // Invoking the API call with sample inputs
    resellerAccounts.createResellerAccountAsync(body, new APICallBack<CreateResellerAccountResponse>() {
        public void onSuccess(HttpContext context, CreateResellerAccountResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="create_reseller_account_public_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ResellerAccountsController.createResellerAccountPublicAsync") createResellerAccountPublicAsync

> TODO: Add a method description


```java
void createResellerAccountPublicAsync(
        final CreateResellerAccountPublicRequest body,
        final APICallBack<CreateResellerAccountPublicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "{    \"reseller_user_id\":1,    \"username\":\"john_awesome\",    \"user_email\":\"johnis@awesome.com\",    \"user_phone\":\"+61261063270\",    \"user_first_name\":\"John\",    \"user_last_name\":\"Awesome\",    \"country\":\"AU\",    \"password\":\"pass\",    \"account_name\":\"The Awesome Company\"}";
    CreateResellerAccountPublicRequest body = mapper.readValue(bodyValue,new TypeReference<CreateResellerAccountPublicRequest> (){});
    // Invoking the API call with sample inputs
    resellerAccounts.createResellerAccountPublicAsync(body, new APICallBack<CreateResellerAccountPublicResponse>() {
        public void onSuccess(HttpContext context, CreateResellerAccountPublicResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="update_reseller_account_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ResellerAccountsController.updateResellerAccountAsync") updateResellerAccountAsync

> TODO: Add a method description


```java
void updateResellerAccountAsync(
        final double clientUserId,
        final UpdateResellerAccountRequest body,
        final APICallBack<UpdateResellerAccountResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| clientUserId |  ``` Required ```  | Your client user id. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    double clientUserId = 24;
    String bodyValue = "    {        \"username\":\"johndoe2\",        \"user_email\":\"johndoe2@awesome.com\",        \"user_phone\":\"518-481-1002\",        \"user_first_name\":\"John\",        \"user_last_name\":\"Doe\",        \"country\":\"US\",        \"password\":\"pass\",        \"account_name\":\"The Awesome Company\"    }";
    UpdateResellerAccountRequest body = mapper.readValue(bodyValue,new TypeReference<UpdateResellerAccountRequest> (){});
    // Invoking the API call with sample inputs
    resellerAccounts.updateResellerAccountAsync(clientUserId, body, new APICallBack<UpdateResellerAccountResponse>() {
        public void onSuccess(HttpContext context, UpdateResellerAccountResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="update_transfer_credit_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.ResellerAccountsController.updateTransferCreditAsync") updateTransferCreditAsync

> TODO: Add a method description


```java
void updateTransferCreditAsync(
        final TransferCreditRequest body,
        final APICallBack<TransferCreditResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    TransferCreditRequest body = new TransferCreditRequest();
    // Invoking the API call with sample inputs
    resellerAccounts.updateTransferCreditAsync(body, new APICallBack<TransferCreditResponse>() {
        public void onSuccess(HttpContext context, TransferCreditResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


[Back to List of Controllers](#list_of_controllers)

## <a name="sdk_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.SDKController") SDKController

### Get singleton instance

The singleton instance of the ``` SDKController ``` class can be accessed from the API Client.

```java
SDKController sDK = client.getSDK();
```

### <a name="get_sdk_download_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SDKController.getSDKDownloadAsync") getSDKDownloadAsync

> TODO: Add a method description


```java
void getSDKDownloadAsync(
        final String type,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| type |  ``` Required ```  | Supported types. |


#### Example Usage

```java
String type = "type";
// Invoking the API call with sample inputs
sDK.getSDKDownloadAsync(type, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="search_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.SearchController") SearchController

### Get singleton instance

The singleton instance of the ``` SearchController ``` class can be accessed from the API Client.

```java
SearchController search = client.getSearch();
```

### <a name="search_contacts_lists_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SearchController.searchContactsListsAsync") searchContactsListsAsync

> TODO: Add a method description


```java
void searchContactsListsAsync(
        final String q,
        final APICallBack<SearchContactsListsResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| q |  ``` Required ```  | Your keyword or query. |


#### Example Usage

```java
String q = "Gorne";
// Invoking the API call with sample inputs
search.searchContactsListsAsync(q, new APICallBack<SearchContactsListsResponse>() {
    public void onSuccess(HttpContext context, SearchContactsListsResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="sms_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.SMSController") SMSController

### Get singleton instance

The singleton instance of the ``` SMSController ``` class can be accessed from the API Client.

```java
SMSController sMS = client.getSMS();
```

### <a name="create_send_an_sms_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SMSController.createSendAnSMSAsync") createSendAnSMSAsync

> You can post **up to 1000 messages** with each API call.


```java
void createSendAnSMSAsync(
        final SendAnSMSRequest body,
        final APICallBack<SendAnSMSResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    SendAnSMSRequest body = new SendAnSMSRequest();
    // Invoking the API call with sample inputs
    sMS.createSendAnSMSAsync(body, new APICallBack<SendAnSMSResponse>() {
        public void onSuccess(HttpContext context, SendAnSMSResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="create_calculate_price_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SMSController.createCalculatePriceAsync") createCalculatePriceAsync

> TODO: Add a method description


```java
void createCalculatePriceAsync(
        final CalculatePriceRequest205 body,
        final APICallBack<CalculatePriceResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    CalculatePriceRequest205 body = new CalculatePriceRequest205();
    // Invoking the API call with sample inputs
    sMS.createCalculatePriceAsync(body, new APICallBack<CalculatePriceResponse>() {
        public void onSuccess(HttpContext context, CalculatePriceResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="get_all_history_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SMSController.getAllHistoryAsync") getAllHistoryAsync

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


```java
void getAllHistoryAsync(
        final Integer dateFrom,
        final Integer dateTo,
        final APICallBack<GetAllHistoryResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateFrom |  ``` Optional ```  | Timestamp (from) used to show records by date. |
| dateTo |  ``` Optional ```  | Timestamp (to) used to show recrods by date. |


#### Example Usage

```java
Integer dateFrom = 1449459940;
Integer dateTo = 1449659940;
// Invoking the API call with sample inputs
sMS.getAllHistoryAsync(dateFrom, dateTo, new APICallBack<GetAllHistoryResponse>() {
    public void onSuccess(HttpContext context, GetAllHistoryResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_export_sms_history_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SMSController.getExportSMSHistoryAsync") getExportSMSHistoryAsync

> TODO: Add a method description


```java
void getExportSMSHistoryAsync(final APICallBack<ExportSMSHistoryResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
sMS.getExportSMSHistoryAsync(new APICallBack<ExportSMSHistoryResponse>() {
    public void onSuccess(HttpContext context, ExportSMSHistoryResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_all_delivery_receipts_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SMSController.getAllDeliveryReceiptsAsync") getAllDeliveryReceiptsAsync

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


```java
void getAllDeliveryReceiptsAsync(final APICallBack<GetAllDeliveryReceiptsResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
sMS.getAllDeliveryReceiptsAsync(new APICallBack<GetAllDeliveryReceiptsResponse>() {
    public void onSuccess(HttpContext context, GetAllDeliveryReceiptsResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_a_specific_delivery_receipt_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SMSController.getASpecificDeliveryReceiptAsync") getASpecificDeliveryReceiptAsync

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


```java
void getASpecificDeliveryReceiptAsync(
        final String messageId,
        final APICallBack<GetASpecificDeliveryReceiptResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Your message id. |


#### Example Usage

```java
String messageId = "88AB118E EB1B 478C 98CE 6C73ABA23F67";
// Invoking the API call with sample inputs
sMS.getASpecificDeliveryReceiptAsync(messageId, new APICallBack<GetASpecificDeliveryReceiptResponse>() {
    public void onSuccess(HttpContext context, GetASpecificDeliveryReceiptResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="add_a_test_delivery_receipt_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SMSController.addATestDeliveryReceiptAsync") addATestDeliveryReceiptAsync

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


```java
void addATestDeliveryReceiptAsync(
        final AddATestDeliveryReceiptRequest body,
        final APICallBack<AddATestDeliveryReceiptResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "    {        \"url\":\"http://yourUrl.com\"    }";
    AddATestDeliveryReceiptRequest body = mapper.readValue(bodyValue,new TypeReference<AddATestDeliveryReceiptRequest> (){});
    // Invoking the API call with sample inputs
    sMS.addATestDeliveryReceiptAsync(body, new APICallBack<AddATestDeliveryReceiptResponse>() {
        public void onSuccess(HttpContext context, AddATestDeliveryReceiptResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="update_mark_delivery_receipts_as_read_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SMSController.updateMarkDeliveryReceiptsAsReadAsync") updateMarkDeliveryReceiptsAsReadAsync

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


```java
void updateMarkDeliveryReceiptsAsReadAsync(
        final MarkDeliveryReceiptsAsReadRequest body,
        final APICallBack<MarkDeliveryReceiptsAsReadResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "{    \"date_before\": 1441958441}";
    MarkDeliveryReceiptsAsReadRequest body = mapper.readValue(bodyValue,new TypeReference<MarkDeliveryReceiptsAsReadRequest> (){});
    // Invoking the API call with sample inputs
    sMS.updateMarkDeliveryReceiptsAsReadAsync(body, new APICallBack<MarkDeliveryReceiptsAsReadResponse>() {
        public void onSuccess(HttpContext context, MarkDeliveryReceiptsAsReadResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="get_all_inbound_sms_pull_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SMSController.getAllInboundSMSPullAsync") getAllInboundSMSPullAsync

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


```java
void getAllInboundSMSPullAsync(final APICallBack<GetAllInboundSMSPullResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
sMS.getAllInboundSMSPullAsync(new APICallBack<GetAllInboundSMSPullResponse>() {
    public void onSuccess(HttpContext context, GetAllInboundSMSPullResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_specific_inbound_pull_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SMSController.getSpecificInboundPullAsync") getSpecificInboundPullAsync

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


```java
void getSpecificInboundPullAsync(
        final String messageId,
        final APICallBack<GetSpecificInboundPullResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Message ID. Must be a valid GUID. |


#### Example Usage

```java
String messageId = "5D420421-8715-4461-A9A2-C8F569E41835";
// Invoking the API call with sample inputs
sMS.getSpecificInboundPullAsync(messageId, new APICallBack<GetSpecificInboundPullResponse>() {
    public void onSuccess(HttpContext context, GetSpecificInboundPullResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="add_a_test_inbound_sms_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SMSController.addATestInboundSMSAsync") addATestInboundSMSAsync

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


```java
void addATestInboundSMSAsync(
        final AddATestInboundSMSRequest body,
        final APICallBack<AddATestInboundSMSResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "    {        \"url\":\"http://yourUrl.com\"    }";
    AddATestInboundSMSRequest body = mapper.readValue(bodyValue,new TypeReference<AddATestInboundSMSRequest> (){});
    // Invoking the API call with sample inputs
    sMS.addATestInboundSMSAsync(body, new APICallBack<AddATestInboundSMSResponse>() {
        public void onSuccess(HttpContext context, AddATestInboundSMSResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="update_mark_a_specific_inbound_sms_as_read_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SMSController.updateMarkASpecificInboundSMSAsReadAsync") updateMarkASpecificInboundSMSAsReadAsync

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


```java
void updateMarkASpecificInboundSMSAsReadAsync(
        final String messageId,
        final APICallBack<MarkASpecificInboundSMSAsReadResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | B7CE432193CD-0753597B7293 (string, required) - The message ID you want to mark as read. |


#### Example Usage

```java
String messageId = "307EF035";
// Invoking the API call with sample inputs
sMS.updateMarkASpecificInboundSMSAsReadAsync(messageId, new APICallBack<MarkASpecificInboundSMSAsReadResponse>() {
    public void onSuccess(HttpContext context, MarkASpecificInboundSMSAsReadResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="update_mark_all_inbound_sms_as_read_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SMSController.updateMarkAllInboundSMSAsReadAsync") updateMarkAllInboundSMSAsReadAsync

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


```java
void updateMarkAllInboundSMSAsReadAsync(
        final MarkAllInboundSMSAsReadRequest body,
        final APICallBack<MarkAllInboundSMSAsReadResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "    {        \"date_before\":1442398100    }";
    MarkAllInboundSMSAsReadRequest body = mapper.readValue(bodyValue,new TypeReference<MarkAllInboundSMSAsReadRequest> (){});
    // Invoking the API call with sample inputs
    sMS.updateMarkAllInboundSMSAsReadAsync(body, new APICallBack<MarkAllInboundSMSAsReadResponse>() {
        public void onSuccess(HttpContext context, MarkAllInboundSMSAsReadResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="update_cancel_a_scheduled_message_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SMSController.updateCancelAScheduledMessageAsync") updateCancelAScheduledMessageAsync

> TODO: Add a method description


```java
void updateCancelAScheduledMessageAsync(
        final String messageId,
        final APICallBack<CancelAScheduledMessageResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | B7CE432193CD-0753597B7293 (string, required) - The message ID you want to cancel. |


#### Example Usage

```java
String messageId = "307EF035";
// Invoking the API call with sample inputs
sMS.updateCancelAScheduledMessageAsync(messageId, new APICallBack<CancelAScheduledMessageResponse>() {
    public void onSuccess(HttpContext context, CancelAScheduledMessageResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="update_cancel_all_scheduled_messages_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SMSController.updateCancelAllScheduledMessagesAsync") updateCancelAllScheduledMessagesAsync

> TODO: Add a method description


```java
void updateCancelAllScheduledMessagesAsync(final APICallBack<CancelAllScheduledMessagesResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
sMS.updateCancelAllScheduledMessagesAsync(new APICallBack<CancelAllScheduledMessagesResponse>() {
    public void onSuccess(HttpContext context, CancelAllScheduledMessagesResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="sms_campaigns_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.SMSCampaignsController") SMSCampaignsController

### Get singleton instance

The singleton instance of the ``` SMSCampaignsController ``` class can be accessed from the API Client.

```java
SMSCampaignsController sMSCampaigns = client.getSMSCampaigns();
```

### <a name="create_sms_campaign_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SMSCampaignsController.createSMSCampaignAsync") createSMSCampaignAsync

> You can post to a list with **up to 20000 recipients** with each API call.


```java
void createSMSCampaignAsync(
        final CreateSMSCampaignRequest body,
        final APICallBack<CreateSMSCampaignResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "{    \"list_id\":428,    \"name\":\"My Campaign 1\",    \"from\":\"+61353787448\",    \"body\":\"This is my new campaign message.\",    \"schedule\":1444821615}";
    CreateSMSCampaignRequest body = mapper.readValue(bodyValue,new TypeReference<CreateSMSCampaignRequest> (){});
    // Invoking the API call with sample inputs
    sMSCampaigns.createSMSCampaignAsync(body, new APICallBack<CreateSMSCampaignResponse>() {
        public void onSuccess(HttpContext context, CreateSMSCampaignResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="create_calculate_price_for_sms_campaign_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SMSCampaignsController.createCalculatePriceForSMSCampaignAsync") createCalculatePriceForSMSCampaignAsync

> TODO: Add a method description


```java
void createCalculatePriceForSMSCampaignAsync(
        final CalculatePriceForSMSCampaignRequest body,
        final APICallBack<CalculatePriceForSMSCampaignResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "{    \"list_id\":428,    \"name\":\"My Campaign 1\",    \"from\":\"+61353787448\",    \"body\":\"(First Name), this is your new campaign message.\"}";
    CalculatePriceForSMSCampaignRequest body = mapper.readValue(bodyValue,new TypeReference<CalculatePriceForSMSCampaignRequest> (){});
    // Invoking the API call with sample inputs
    sMSCampaigns.createCalculatePriceForSMSCampaignAsync(body, new APICallBack<CalculatePriceForSMSCampaignResponse>() {
        public void onSuccess(HttpContext context, CalculatePriceForSMSCampaignResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="update_an_sms_campaign_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SMSCampaignsController.updateAnSMSCampaignAsync") updateAnSMSCampaignAsync

> TODO: Add a method description


```java
void updateAnSMSCampaignAsync(
        final double smsCampaignId,
        final UpdateAnSMSCampaignRequest body,
        final APICallBack<UpdateAnSMSCampaignResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| smsCampaignId |  ``` Required ```  | Your SMS Campaign id. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    double smsCampaignId = 1;
    String bodyValue = "{    \"list_id\":428,    \"name\":\"Awesome campaign.\",    \"from\":\"+61353787447\",    \"body\":\"his is an awesome message.\",    \"schedule\":1444821615}";
    UpdateAnSMSCampaignRequest body = mapper.readValue(bodyValue,new TypeReference<UpdateAnSMSCampaignRequest> (){});
    // Invoking the API call with sample inputs
    sMSCampaigns.updateAnSMSCampaignAsync(smsCampaignId, body, new APICallBack<UpdateAnSMSCampaignResponse>() {
        public void onSuccess(HttpContext context, UpdateAnSMSCampaignResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="get_sms_campaign_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SMSCampaignsController.getSMSCampaignAsync") getSMSCampaignAsync

> TODO: Add a method description


```java
void getSMSCampaignAsync(
        final double smsCampaignId,
        final APICallBack<GetSMSCampaignResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| smsCampaignId |  ``` Required ```  | Your SMS campaign id. |


#### Example Usage

```java
double smsCampaignId = 1;
// Invoking the API call with sample inputs
sMSCampaigns.getSMSCampaignAsync(smsCampaignId, new APICallBack<GetSMSCampaignResponse>() {
    public void onSuccess(HttpContext context, GetSMSCampaignResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="update_cancel_an_sms_campaign_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SMSCampaignsController.updateCancelAnSMSCampaignAsync") updateCancelAnSMSCampaignAsync

> TODO: Add a method description


```java
void updateCancelAnSMSCampaignAsync(
        final double smsCampaignId,
        final APICallBack<CancelAnSMSCampaignResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| smsCampaignId |  ``` Required ```  | Your SMS Campaign id. |


#### Example Usage

```java
double smsCampaignId = 1;
// Invoking the API call with sample inputs
sMSCampaigns.updateCancelAnSMSCampaignAsync(smsCampaignId, new APICallBack<CancelAnSMSCampaignResponse>() {
    public void onSuccess(HttpContext context, CancelAnSMSCampaignResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_list_of_sms_campaigns_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SMSCampaignsController.getListOfSMSCampaignsAsync") getListOfSMSCampaignsAsync

> TODO: Add a method description


```java
void getListOfSMSCampaignsAsync(final APICallBack<GetListOfSMSCampaignsResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
sMSCampaigns.getListOfSMSCampaignsAsync(new APICallBack<GetListOfSMSCampaignsResponse>() {
    public void onSuccess(HttpContext context, GetListOfSMSCampaignsResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="sms_templates_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.SMSTemplatesController") SMSTemplatesController

### Get singleton instance

The singleton instance of the ``` SMSTemplatesController ``` class can be accessed from the API Client.

```java
SMSTemplatesController sMSTemplates = client.getSMSTemplates();
```

### <a name="list_of_templates_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SMSTemplatesController.listOfTemplatesAsync") listOfTemplatesAsync

> Get list of templates.


```java
void listOfTemplatesAsync(final APICallBack<ListOfTemplatesResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
sMSTemplates.listOfTemplatesAsync(new APICallBack<ListOfTemplatesResponse>() {
    public void onSuccess(HttpContext context, ListOfTemplatesResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_a_template_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SMSTemplatesController.createATemplateAsync") createATemplateAsync

> Create new template.


```java
void createATemplateAsync(
        final CreateATemplateRequest body,
        final APICallBack<CreateATemplateResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "    {        \"template_name\":\"Template 501916\",        \"body\":\"This is a sample content: H7YI68B3yk for this template.\"    }";
    CreateATemplateRequest body = mapper.readValue(bodyValue,new TypeReference<CreateATemplateRequest> (){});
    // Invoking the API call with sample inputs
    sMSTemplates.createATemplateAsync(body, new APICallBack<CreateATemplateResponse>() {
        public void onSuccess(HttpContext context, CreateATemplateResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="update_a_template_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SMSTemplatesController.updateATemplateAsync") updateATemplateAsync

> TODO: Add a method description


```java
void updateATemplateAsync(
        final String templateId,
        final UpdateATemplateRequest body,
        final APICallBack<UpdateATemplateResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String templateId = "25";
    String bodyValue = "    {        \"template_name\":\"I am updated\",        \"body\":\"This is a sample content: Sc0KNWgSMG for this template.\"    }";
    UpdateATemplateRequest body = mapper.readValue(bodyValue,new TypeReference<UpdateATemplateRequest> (){});
    // Invoking the API call with sample inputs
    sMSTemplates.updateATemplateAsync(templateId, body, new APICallBack<UpdateATemplateResponse>() {
        public void onSuccess(HttpContext context, UpdateATemplateResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="delete_a_template_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SMSTemplatesController.deleteATemplateAsync") deleteATemplateAsync

> TODO: Add a method description


```java
void deleteATemplateAsync(
        final String templateId,
        final APICallBack<DeleteATemplateResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |


#### Example Usage

```java
String templateId = "25";
// Invoking the API call with sample inputs
sMSTemplates.deleteATemplateAsync(templateId, new APICallBack<DeleteATemplateResponse>() {
    public void onSuccess(HttpContext context, DeleteATemplateResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="statistics_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.StatisticsController") StatisticsController

### Get singleton instance

The singleton instance of the ``` StatisticsController ``` class can be accessed from the API Client.

```java
StatisticsController statistics = client.getStatistics();
```

### <a name="get_sms_statistics_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.StatisticsController.getSMSStatisticsAsync") getSMSStatisticsAsync

> TODO: Add a method description


```java
void getSMSStatisticsAsync(final APICallBack<GetSMSStatisticsResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
statistics.getSMSStatisticsAsync(new APICallBack<GetSMSStatisticsResponse>() {
    public void onSuccess(HttpContext context, GetSMSStatisticsResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_voice_statistics_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.StatisticsController.getVoiceStatisticsAsync") getVoiceStatisticsAsync

> TODO: Add a method description


```java
void getVoiceStatisticsAsync(final APICallBack<GetVoiceStatisticsResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
statistics.getVoiceStatisticsAsync(new APICallBack<GetVoiceStatisticsResponse>() {
    public void onSuccess(HttpContext context, GetVoiceStatisticsResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="subaccounts_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.SubaccountsController") SubaccountsController

### Get singleton instance

The singleton instance of the ``` SubaccountsController ``` class can be accessed from the API Client.

```java
SubaccountsController subaccounts = client.getSubaccounts();
```

### <a name="get_all_subaccounts_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SubaccountsController.getAllSubaccountsAsync") getAllSubaccountsAsync

> TODO: Add a method description


```java
void getAllSubaccountsAsync(final APICallBack<GetAllSubaccountsResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
subaccounts.getAllSubaccountsAsync(new APICallBack<GetAllSubaccountsResponse>() {
    public void onSuccess(HttpContext context, GetAllSubaccountsResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="create_a_new_subaccount_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SubaccountsController.createANewSubaccountAsync") createANewSubaccountAsync

> TODO: Add a method description


```java
void createANewSubaccountAsync(
        final CreateANewSubaccountRequest body,
        final APICallBack<CreateANewSubaccountResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "    {        \"api_username\":\"nameP99\",        \"password\":\"pass\",        \"email\":\"testvrq@gmail.com\",        \"phone_number\":\"941-751-3278\",        \"first_name\":\"FirstnameeGPqV\",        \"last_name\":\"LastnamePvjJp\"    }";
    CreateANewSubaccountRequest body = mapper.readValue(bodyValue,new TypeReference<CreateANewSubaccountRequest> (){});
    // Invoking the API call with sample inputs
    subaccounts.createANewSubaccountAsync(body, new APICallBack<CreateANewSubaccountResponse>() {
        public void onSuccess(HttpContext context, CreateANewSubaccountResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="get_a_specific_subaccount_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SubaccountsController.getASpecificSubaccountAsync") getASpecificSubaccountAsync

> TODO: Add a method description


```java
void getASpecificSubaccountAsync(
        final double subaccountId,
        final APICallBack<GetASpecificSubaccountResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |


#### Example Usage

```java
double subaccountId = 59;
// Invoking the API call with sample inputs
subaccounts.getASpecificSubaccountAsync(subaccountId, new APICallBack<GetASpecificSubaccountResponse>() {
    public void onSuccess(HttpContext context, GetASpecificSubaccountResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="update_a_specific_subaccount_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SubaccountsController.updateASpecificSubaccountAsync") updateASpecificSubaccountAsync

> TODO: Add a method description


```java
void updateASpecificSubaccountAsync(
        final double subaccountId,
        final UpdateASpecificSubaccountRequest body,
        final APICallBack<UpdateASpecificSubaccountResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    double subaccountId = 59;
    String bodyValue = "    {        \"password\":\"pass\",        \"email\":\"testfP0.updated@gmail.com\",        \"phone_number\":\"+19417519130\",        \"first_name\":\"FirstnameKvdRZUpdated\",        \"last_name\":\"LastnameHUPYGUpdated\",        \"access_users\": 1,        \"access_billing\": 1,        \"access_reporting\": 1,        \"access_contacts\": 1,        \"access_settings\": 1,        \"access_sms\": 1,        \"access_email\": 1,        \"access_voice\": 1,        \"access_fax\": 1,        \"access_post\": 1,        \"access_reseller\": 1,        \"access_mms\": 1,        \"share_campaigns\": 0,        \"notes\": null    }";
    UpdateASpecificSubaccountRequest body = mapper.readValue(bodyValue,new TypeReference<UpdateASpecificSubaccountRequest> (){});
    // Invoking the API call with sample inputs
    subaccounts.updateASpecificSubaccountAsync(subaccountId, body, new APICallBack<UpdateASpecificSubaccountResponse>() {
        public void onSuccess(HttpContext context, UpdateASpecificSubaccountResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="delete_a_specific_subaccount_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SubaccountsController.deleteASpecificSubaccountAsync") deleteASpecificSubaccountAsync

> TODO: Add a method description


```java
void deleteASpecificSubaccountAsync(
        final double subaccountId,
        final APICallBack<DeleteASpecificSubaccountResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |


#### Example Usage

```java
double subaccountId = 59;
// Invoking the API call with sample inputs
subaccounts.deleteASpecificSubaccountAsync(subaccountId, new APICallBack<DeleteASpecificSubaccountResponse>() {
    public void onSuccess(HttpContext context, DeleteASpecificSubaccountResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="update_regenerate_api_key_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.SubaccountsController.updateRegenerateAPIKeyAsync") updateRegenerateAPIKeyAsync

> TODO: Add a method description


```java
void updateRegenerateAPIKeyAsync(
        final double subaccountId,
        final APICallBack<RegenerateAPIKeyResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |


#### Example Usage

```java
double subaccountId = 59;
// Invoking the API call with sample inputs
subaccounts.updateRegenerateAPIKeyAsync(subaccountId, new APICallBack<RegenerateAPIKeyResponse>() {
    public void onSuccess(HttpContext context, RegenerateAPIKeyResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="timezones_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.TimezonesController") TimezonesController

### Get singleton instance

The singleton instance of the ``` TimezonesController ``` class can be accessed from the API Client.

```java
TimezonesController timezones = client.getTimezones();
```

### <a name="get_timezones_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.TimezonesController.getTimezonesAsync") getTimezonesAsync

> Get supported list of timezones.


```java
void getTimezonesAsync(final APICallBack<GetTimezonesResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
timezones.getTimezonesAsync(new APICallBack<GetTimezonesResponse>() {
    public void onSuccess(HttpContext context, GetTimezonesResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="transactional_email_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.TransactionalEmailController") TransactionalEmailController

### Get singleton instance

The singleton instance of the ``` TransactionalEmailController ``` class can be accessed from the API Client.

```java
TransactionalEmailController transactionalEmail = client.getTransactionalEmail();
```

### <a name="create_email_send_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.TransactionalEmailController.createEmailSendAsync") createEmailSendAsync

> TODO: Add a method description


```java
void createEmailSendAsync(
        final EmailSendRequest body,
        final APICallBack<EmailSendResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    EmailSendRequest body = new EmailSendRequest();
    // Invoking the API call with sample inputs
    transactionalEmail.createEmailSendAsync(body, new APICallBack<EmailSendResponse>() {
        public void onSuccess(HttpContext context, EmailSendResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="create_email_price_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.TransactionalEmailController.createEmailPriceAsync") createEmailPriceAsync

> TODO: Add a method description


```java
void createEmailPriceAsync(
        final EmailPriceRequest body,
        final APICallBack<EmailPriceResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    EmailPriceRequest body = new EmailPriceRequest();
    // Invoking the API call with sample inputs
    transactionalEmail.createEmailPriceAsync(body, new APICallBack<EmailPriceResponse>() {
        public void onSuccess(HttpContext context, EmailPriceResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="get_email_history_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.TransactionalEmailController.getEmailHistoryAsync") getEmailHistoryAsync

> TODO: Add a method description


```java
void getEmailHistoryAsync(final APICallBack<EmailHistoryResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
transactionalEmail.getEmailHistoryAsync(new APICallBack<EmailHistoryResponse>() {
    public void onSuccess(HttpContext context, EmailHistoryResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_export_history_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.TransactionalEmailController.getExportHistoryAsync") getExportHistoryAsync

> TODO: Add a method description


```java
void getExportHistoryAsync(
        final String filename,
        final APICallBack<ExportHistoryResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | File name for the export file. |


#### Example Usage

```java
String filename = "myexport.csv";
// Invoking the API call with sample inputs
transactionalEmail.getExportHistoryAsync(filename, new APICallBack<ExportHistoryResponse>() {
    public void onSuccess(HttpContext context, ExportHistoryResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="add_a_test_delivery_receipt_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.TransactionalEmailController.addATestDeliveryReceiptAsync") addATestDeliveryReceiptAsync

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


```java
void addATestDeliveryReceiptAsync(
        final AddATestDeliveryReceiptRequest body,
        final APICallBack<AddATestDeliveryReceiptResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "    {        \"url\":\"http://yourUrl.com\"    }";
    AddATestDeliveryReceiptRequest body = mapper.readValue(bodyValue,new TypeReference<AddATestDeliveryReceiptRequest> (){});
    // Invoking the API call with sample inputs
    transactionalEmail.addATestDeliveryReceiptAsync(body, new APICallBack<AddATestDeliveryReceiptResponse>() {
        public void onSuccess(HttpContext context, AddATestDeliveryReceiptResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


[Back to List of Controllers](#list_of_controllers)

## <a name="uploads_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.UploadsController") UploadsController

### Get singleton instance

The singleton instance of the ``` UploadsController ``` class can be accessed from the API Client.

```java
UploadsController uploads = client.getUploads();
```

### <a name="upload_a_file_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.UploadsController.uploadAFileAsync") uploadAFileAsync

> The `upload` endpoint provides a method for converting files from an unspported format to a format that one of our endpoints can handle.
> Files can be submitted two ways:
> 1. Using `base64` encoding in an `application/json` request. In this case, submit the `base64`-encoded file contents in the `content` field of the request body, and `convert` can be specified either also in the body or as part of the query string.
> 2. Using `multipart/form-data` encoding, in the same way it would be submitted using a HTML form. You may find cURL useful for this. For an example of how to do this, see one of our [SDKs](https://dashboard.clicksend.com/#/libraries-sdk/main). In this case, specify `convert` in the query string.
> Note that `convert` specifies the conversion to take place - that is, what the result should be compatible with - and can be any of `fax`, `mms`, `csv` or `post`.
> All files have 10 minutes expiry.


```java
void uploadAFileAsync(
        final UploadAFileRequest body,
        final String convert,
        final APICallBack<UploadAFileResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |
| convert |  ``` Optional ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    UploadAFileRequest body = new UploadAFileRequest();
    String convert = "convert";
    // Invoking the API call with sample inputs
    uploads.uploadAFileAsync(body, convert, new APICallBack<UploadAFileResponse>() {
        public void onSuccess(HttpContext context, UploadAFileResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


[Back to List of Controllers](#list_of_controllers)

## <a name="voice_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.clicksend.rest.controllers.VoiceController") VoiceController

### Get singleton instance

The singleton instance of the ``` VoiceController ``` class can be accessed from the API Client.

```java
VoiceController voice = client.getVoice();
```

### <a name="create_send_a_voice_call_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.VoiceController.createSendAVoiceCallAsync") createSendAVoiceCallAsync

> You can post **up to 1000 messages** with each API call.


```java
void createSendAVoiceCallAsync(
        final SendAVoiceCallRequest body,
        final APICallBack<SendAVoiceCallResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    SendAVoiceCallRequest body = new SendAVoiceCallRequest();
    // Invoking the API call with sample inputs
    voice.createSendAVoiceCallAsync(body, new APICallBack<SendAVoiceCallResponse>() {
        public void onSuccess(HttpContext context, SendAVoiceCallResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="create_calculate_price_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.VoiceController.createCalculatePriceAsync") createCalculatePriceAsync

> TODO: Add a method description


```java
void createCalculatePriceAsync(
        final CalculatePriceRequest263 body,
        final APICallBack<CalculatePriceResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    CalculatePriceRequest263 body = new CalculatePriceRequest263();
    // Invoking the API call with sample inputs
    voice.createCalculatePriceAsync(body, new APICallBack<CalculatePriceResponse>() {
        public void onSuccess(HttpContext context, CalculatePriceResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="get_voice_languages_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.VoiceController.getVoiceLanguagesAsync") getVoiceLanguagesAsync

> TODO: Add a method description


```java
void getVoiceLanguagesAsync(final APICallBack<VoiceLanguagesResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
voice.getVoiceLanguagesAsync(new APICallBack<VoiceLanguagesResponse>() {
    public void onSuccess(HttpContext context, VoiceLanguagesResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_voice_history_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.VoiceController.getVoiceHistoryAsync") getVoiceHistoryAsync

> TODO: Add a method description


```java
void getVoiceHistoryAsync(
        final Integer dateFrom,
        final Integer dateTo,
        final APICallBack<GetVoiceHistoryResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateFrom |  ``` Optional ```  | Timestamp (from) used to show records by date. |
| dateTo |  ``` Optional ```  | Timestamp (to) used to show recrods by date. |


#### Example Usage

```java
Integer dateFrom = 1443501617;
Integer dateTo = 1443501727;
// Invoking the API call with sample inputs
voice.getVoiceHistoryAsync(dateFrom, dateTo, new APICallBack<GetVoiceHistoryResponse>() {
    public void onSuccess(HttpContext context, GetVoiceHistoryResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_export_voice_history_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.VoiceController.getExportVoiceHistoryAsync") getExportVoiceHistoryAsync

> TODO: Add a method description


```java
void getExportVoiceHistoryAsync(final APICallBack<ExportVoiceHistoryResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
voice.getExportVoiceHistoryAsync(new APICallBack<ExportVoiceHistoryResponse>() {
    public void onSuccess(HttpContext context, ExportVoiceHistoryResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_voice_receipts_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.VoiceController.getVoiceReceiptsAsync") getVoiceReceiptsAsync

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


```java
void getVoiceReceiptsAsync(final APICallBack<GetVoiceReceiptsResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
voice.getVoiceReceiptsAsync(new APICallBack<GetVoiceReceiptsResponse>() {
    public void onSuccess(HttpContext context, GetVoiceReceiptsResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="add_a_test_delivery_receipt_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.VoiceController.addATestDeliveryReceiptAsync") addATestDeliveryReceiptAsync

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


```java
void addATestDeliveryReceiptAsync(
        final AddATestDeliveryReceiptRequest body,
        final APICallBack<AddATestDeliveryReceiptResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String bodyValue = "    {        \"url\":\"http://yourUrl.com\"    }";
    AddATestDeliveryReceiptRequest body = mapper.readValue(bodyValue,new TypeReference<AddATestDeliveryReceiptRequest> (){});
    // Invoking the API call with sample inputs
    voice.addATestDeliveryReceiptAsync(body, new APICallBack<AddATestDeliveryReceiptResponse>() {
        public void onSuccess(HttpContext context, AddATestDeliveryReceiptResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="get_specific_voice_receipt_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.VoiceController.getSpecificVoiceReceiptAsync") getSpecificVoiceReceiptAsync

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


```java
void getSpecificVoiceReceiptAsync(
        final String messageId,
        final APICallBack<GetSpecificVoiceReceiptResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | 3055-45F1-9B79-F2C43509FD16 (string, required) - The voice receipt message id. |


#### Example Usage

```java
String messageId = "28DD2718";
// Invoking the API call with sample inputs
voice.getSpecificVoiceReceiptAsync(messageId, new APICallBack<GetSpecificVoiceReceiptResponse>() {
    public void onSuccess(HttpContext context, GetSpecificVoiceReceiptResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="update_marked_voice_receipts_as_read_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.VoiceController.updateMarkedVoiceReceiptsAsReadAsync") updateMarkedVoiceReceiptsAsReadAsync

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


```java
void updateMarkedVoiceReceiptsAsReadAsync(
        final double dateBefore,
        final APICallBack<MarkedVoiceReceiptsAsReadResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateBefore |  ``` Required ```  | An optional timestamp - mark all as read before this timestamp. If not given, all receipts will be marked as read. |


#### Example Usage

```java
double dateBefore = 83.3991673534732;
// Invoking the API call with sample inputs
voice.updateMarkedVoiceReceiptsAsReadAsync(dateBefore, new APICallBack<MarkedVoiceReceiptsAsReadResponse>() {
    public void onSuccess(HttpContext context, MarkedVoiceReceiptsAsReadResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="update_cancel_a_specific_voice_call_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.VoiceController.updateCancelASpecificVoiceCallAsync") updateCancelASpecificVoiceCallAsync

> TODO: Add a method description


```java
void updateCancelASpecificVoiceCallAsync(
        final String messageId,
        final APICallBack<CancelASpecificVoiceCallResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Your voice message id. |


#### Example Usage

```java
String messageId = "7B5BFC19 06B7 49C1 8DCDFB011600E12B";
// Invoking the API call with sample inputs
voice.updateCancelASpecificVoiceCallAsync(messageId, new APICallBack<CancelASpecificVoiceCallResponse>() {
    public void onSuccess(HttpContext context, CancelASpecificVoiceCallResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="update_cancel_all_voice_calls_async"></a>![Method: ](https://apidocs.io/img/method.png "com.clicksend.rest.controllers.VoiceController.updateCancelAllVoiceCallsAsync") updateCancelAllVoiceCallsAsync

> TODO: Add a method description


```java
void updateCancelAllVoiceCallsAsync(final APICallBack<CancelAllVoiceCallsResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
voice.updateCancelAllVoiceCallsAsync(new APICallBack<CancelAllVoiceCallsResponse>() {
    public void onSuccess(HttpContext context, CancelAllVoiceCallsResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)



