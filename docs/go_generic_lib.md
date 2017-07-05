# Getting started

TODO: Add a description

## How to Build


* In order to successfully build and run your SDK files, you are required to have the following setup in your system:
    * **Go**  (Visit [https://golang.org/doc/install](https://golang.org/doc/install) for more details on how to install Go)
    * **Java VM** Version 8 or later
    * **Eclipse 4.6 (Neon)** or later ([http://www.eclipse.org/neon/](http://www.eclipse.org/neon/))
    * **GoClipse** setup within above installed Eclipse (Follow the instructions at [this link](https://github.com/GoClipse/goclipse/blob/latest/documentation/Installation.md#instructions) to setup GoClipse)
* Ensure that ```GOPATH``` environment variable is set in the system variables. If not, set it to your workspace directory where you will be adding your Go projects.
* The generated code uses unirest-go http library. Therefore, you will need internet access to resolve this dependency. If Go is properly installed and configured, run the following command to pull the dependency:

```Go
go get github.com/apimatic/unirest-go
```

This will install unirest-go in the ```GOPATH``` you specified in the system variables.

Now follow the steps mentioned below to build your SDK:

1. Open eclipse in the Go language perspective and click on the ```Import``` option in ```File``` menu.

![Importing SDK into Eclipse - Step 1](https://apidocs.io/illustration/go?step=import0)

2. Select ```General -> Existing Projects into Workspace``` option from the tree list.

![Importing SDK into Eclipse - Step 2](https://apidocs.io/illustration/go?step=import1)

3. In ```Select root directory```, provide path to the unzipped archive for the generated code. Once the path is set and the Project becomes visible under ```Projects``` click ```Finish```

![Importing SDK into Eclipse - Step 3](https://apidocs.io/illustration/go?step=import2&workspaceFolder=ClickSend%20REST%20API%20v3-GoLang&projectName=clicksendrestapiv3_lib)

4. The Go library will be imported and its files will be visible in the Project Explorer

![Importing SDK into Eclipse - Step 4](https://apidocs.io/illustration/go?step=import3&projectName=clicksendrestapiv3_lib)

## How to Use

The following section explains how to use the Clicksendrestapiv3Lib library in a new project.

### 1. Add a new Test Project

Create a new project in Eclipse by ```File``` -> ```New``` -> ```Go Project```

![Add a new project in Eclipse](https://apidocs.io/illustration/go?step=createNewProject0)

Name the Project as ```Test``` and click ```Finish```

![Create a new Maven Project - Step 1](https://apidocs.io/illustration/go?step=createNewProject1)

Create a new directory in the ```src``` directory of this project

![Create a new Maven Project - Step 2](https://apidocs.io/illustration/go?step=createNewProject2&projectName=clicksendrestapiv3_lib)

Name it ```test.com```

![Create a new Maven Project - Step 3](https://apidocs.io/illustration/go?step=createNewProject3&projectName=clicksendrestapiv3_lib)

Now create a new file inside ```src/test.com```

![Create a new Maven Project - Step 4](https://apidocs.io/illustration/go?step=createNewProject4&projectName=clicksendrestapiv3_lib)

Name it ```testsdk.go```

![Create a new Maven Project - Step 5](https://apidocs.io/illustration/go?step=createNewProject5&projectName=clicksendrestapiv3_lib)

In this Go file, you can start adding code to initialize the client library. Sample code to initialize the client library and using its methods is given in the subsequent sections.

### 2. Configure the Test Project

You need to import your generated library in this project in order to make use of its functions. In order to import the library, you can add its path in the ```GOPATH``` for this project. Follow the below steps:

Right click on the project name and click on ```Properties```

![Adding dependency to the client library - Step 1](https://apidocs.io/illustration/go?step=testProject0&projectName=clicksendrestapiv3_lib)

Choose ```Go Compiler``` from the side menu. Check ```Use project specific settings``` and uncheck ```Use same value as the GOPATH environment variable.```. By default, the GOPATH value from the environment variables will be visible in ```Eclipse GOPATH```. Do not remove this as this points to the unirest dependency.

![Adding dependency to the client library - Step 2](https://apidocs.io/illustration/go?step=testProject1)

Append the library path to this GOPATH

![Adding dependency to the client library - Step 3](https://apidocs.io/illustration/go?step=testProject2&workspaceFolder=ClickSend%20REST%20API%20v3-GoLang)

Once the path is appended, click on ```OK```

### 3. Build the Test Project

Right click on the project name and click on ```Build Project```

![Build Project](https://apidocs.io/illustration/go?step=buildProject&projectName=clicksendrestapiv3_lib)

### 4. Run the Test Project

If the build is successful, right click on your Go file and click on ```Run As``` -> ```Go Application```

![Run Project](https://apidocs.io/illustration/go?step=runProject&projectName=clicksendrestapiv3_lib)

## Initialization

### Authentication
In order to setup authentication of the API client, you need the following information.

| Parameter | Description |
|-----------|-------------|
| basicAuthUserName | The username to use with basic authentication |
| basicAuthPassword | The password to use with basic authentication |


To configure these for your generated code, open the file "Configuration.go" and edit it's contents.


# Class Reference

## <a name="list_of_controllers"></a>List of Controllers

* [account_pkg](#account_pkg)
* [accountrecharge_pkg](#accountrecharge_pkg)
* [automationrules_pkg](#automationrules_pkg)
* [contactlists_pkg](#contactlists_pkg)
* [contactsuggestions_pkg](#contactsuggestions_pkg)
* [contacts_pkg](#contacts_pkg)
* [countries_pkg](#countries_pkg)
* [deliveryissues_pkg](#deliveryissues_pkg)
* [emailmarketing_pkg](#emailmarketing_pkg)
* [email-to-smsallowedaddress_pkg](#email_to_smsallowedaddress_pkg)
* [email-to-smsstrippedstrings_pkg](#email_to_smsstrippedstrings_pkg)
* [fax_pkg](#fax_pkg)
* [forgotaccount_pkg](#forgotaccount_pkg)
* [mms_pkg](#mms_pkg)
* [numbers_pkg](#numbers_pkg)
* [pricing_pkg](#pricing_pkg)
* [postdirectmail_pkg](#postdirectmail_pkg)
* [postletter_pkg](#postletter_pkg)
* [postcards_pkg](#postcards_pkg)
* [referralaccounts_pkg](#referralaccounts_pkg)
* [reseller_pkg](#reseller_pkg)
* [reselleraccounts_pkg](#reselleraccounts_pkg)
* [sdk_pkg](#sdk_pkg)
* [search_pkg](#search_pkg)
* [sms_pkg](#sms_pkg)
* [smscampaigns_pkg](#smscampaigns_pkg)
* [smstemplates_pkg](#smstemplates_pkg)
* [statistics_pkg](#statistics_pkg)
* [subaccounts_pkg](#subaccounts_pkg)
* [timezones_pkg](#timezones_pkg)
* [transactionalemail_pkg](#transactionalemail_pkg)
* [uploads_pkg](#uploads_pkg)
* [voice_pkg](#voice_pkg)

## <a name="account_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".account_pkg") account_pkg

### Get instance

Factory for the ``` ACCOUNT ``` interface can be accessed from the package account_pkg.

```go
account := account_pkg.NewACCOUNT()
```

### <a name="create_a_new_member"></a>![Method: ](https://apidocs.io/img/method.png ".account_pkg.CreateANewMember") CreateANewMember

> **Note:** *Authentication isn't required to create a new account.*


```go
func (me *ACCOUNT_IMPL) CreateANewMember(body *models_pkg.CreateANewAccountRequest)(*models_pkg.CreateANewAccountResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
var body *models_pkg.CreateANewAccountRequest

var result *models_pkg.CreateANewAccountResponse
result,_ = account.CreateANewMember(body)

```


### <a name="update_account"></a>![Method: ](https://apidocs.io/img/method.png ".account_pkg.UpdateAccount") UpdateAccount

> TODO: Add a method description


```go
func (me *ACCOUNT_IMPL) UpdateAccount(body *models_pkg.UpdateAccountRequest)(*models_pkg.UpdateAccountResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("    {        \"username\":\"johndoe\",        \"user_email\":\"johndoe@awesome.com\",        \"user_phone\":\"518-481-1002\",        \"user_first_name\":\"John\",        \"user_last_name\":\"Doe\",        \"country\":\"AU\",        \"password\":\"pass\",        \"account_name\":\"The Awesome Company\",        \"timezone\": \"Australia/Melbourne\",        \"private_uploads\": 1,        \"setting_sms_hide_your_number\": 0,        \"setting_sms_hide_business_name\": 1    }")
var body *models_pkg.UpdateAccountRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.UpdateAccountResponse
result,_ = account.UpdateAccount(body)

```


### <a name="get_account"></a>![Method: ](https://apidocs.io/img/method.png ".account_pkg.GetAccount") GetAccount

> TODO: Add a method description


```go
func (me *ACCOUNT_IMPL) GetAccount()(*models_pkg.GetAccountResponse,error)
```

#### Example Usage

```go

var result *models_pkg.GetAccountResponse
result,_ = account.GetAccount()

```


### <a name="get_account_usage"></a>![Method: ](https://apidocs.io/img/method.png ".account_pkg.GetAccountUsage") GetAccountUsage

> TODO: Add a method description


```go
func (me *ACCOUNT_IMPL) GetAccountUsage(
            year float64,
            month float64,
            mtype string)(*models_pkg.AccountUsageResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| year |  ``` Required ```  | Your account usage year. |
| month |  ``` Required ```  | Your account usage month. |
| mtype |  ``` Required ```  | The account type. Value can only be either email or subaccount. |


#### Example Usage

```go
year := "2016"
month := "4"
mtype := "subaccount"

var result *models_pkg.AccountUsageResponse
result,_ = account.GetAccountUsage(year, month, mtype)

```


### <a name="update_send_account_activation_token"></a>![Method: ](https://apidocs.io/img/method.png ".account_pkg.UpdateSendAccountActivationToken") UpdateSendAccountActivationToken

> TODO: Add a method description


```go
func (me *ACCOUNT_IMPL) UpdateSendAccountActivationToken(body *models_pkg.SendAccountActivationTokenRequest)(*models_pkg.SendAccountActivationTokenResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("    {        \"user_phone\":\"352-394-4199\",        \"type\":\"sms\",        \"country\": \"US\"    }")
var body *models_pkg.SendAccountActivationTokenRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.SendAccountActivationTokenResponse
result,_ = account.UpdateSendAccountActivationToken(body)

```


### <a name="update_verify_new_account"></a>![Method: ](https://apidocs.io/img/method.png ".account_pkg.UpdateVerifyNewAccount") UpdateVerifyNewAccount

> TODO: Add a method description


```go
func (me *ACCOUNT_IMPL) UpdateVerifyNewAccount(activationToken string)(*models_pkg.VerifyNewAccountResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| activationToken |  ``` Required ```  | The ActivationToken to be used to verify an account. |


#### Example Usage

```go
activationToken := "1827364"

var result *models_pkg.VerifyNewAccountResponse
result,_ = account.UpdateVerifyNewAccount(activationToken)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="accountrecharge_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".accountrecharge_pkg") accountrecharge_pkg

### Get instance

Factory for the ``` ACCOUNTRECHARGE ``` interface can be accessed from the package accountrecharge_pkg.

```go
accountRecharge := accountrecharge_pkg.NewACCOUNTRECHARGE()
```

### <a name="get_credit_card_info"></a>![Method: ](https://apidocs.io/img/method.png ".accountrecharge_pkg.GetCreditCardInfo") GetCreditCardInfo

> TODO: Add a method description


```go
func (me *ACCOUNTRECHARGE_IMPL) GetCreditCardInfo()(*models_pkg.GetCreditCardInfoResponse,error)
```

#### Example Usage

```go

var result *models_pkg.GetCreditCardInfoResponse
result,_ = accountRecharge.GetCreditCardInfo()

```


### <a name="update_credit_card_info"></a>![Method: ](https://apidocs.io/img/method.png ".accountrecharge_pkg.UpdateCreditCardInfo") UpdateCreditCardInfo

> TODO: Add a method description


```go
func (me *ACCOUNTRECHARGE_IMPL) UpdateCreditCardInfo(body *models_pkg.UpdateCreditCardInfoRequest)(*models_pkg.UpdateCreditCardInfoResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
var body *models_pkg.UpdateCreditCardInfoRequest

var result *models_pkg.UpdateCreditCardInfoResponse
result,_ = accountRecharge.UpdateCreditCardInfo(body)

```


### <a name="list_of_packages"></a>![Method: ](https://apidocs.io/img/method.png ".accountrecharge_pkg.ListOfPackages") ListOfPackages

> TODO: Add a method description


```go
func (me *ACCOUNTRECHARGE_IMPL) ListOfPackages(country *string)(*models_pkg.ListOfPackagesResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Optional ```  | Your country. |


#### Example Usage

```go
country := "\"AU\""

var result *models_pkg.ListOfPackagesResponse
result,_ = accountRecharge.ListOfPackages(country)

```


### <a name="update_purchase_a_package"></a>![Method: ](https://apidocs.io/img/method.png ".accountrecharge_pkg.UpdatePurchaseAPackage") UpdatePurchaseAPackage

> TODO: Add a method description


```go
func (me *ACCOUNTRECHARGE_IMPL) UpdatePurchaseAPackage(packageId float64)(*models_pkg.PurchaseAPackageResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| packageId |  ``` Required ```  | Your package id. |


#### Example Usage

```go
packageId := "1"

var result *models_pkg.PurchaseAPackageResponse
result,_ = accountRecharge.UpdatePurchaseAPackage(packageId)

```


### <a name="get_transactions"></a>![Method: ](https://apidocs.io/img/method.png ".accountrecharge_pkg.GetTransactions") GetTransactions

> TODO: Add a method description


```go
func (me *ACCOUNTRECHARGE_IMPL) GetTransactions()(*models_pkg.GetTransactionsResponse,error)
```

#### Example Usage

```go

var result *models_pkg.GetTransactionsResponse
result,_ = accountRecharge.GetTransactions()

```


### <a name="get_a_specific_transaction"></a>![Method: ](https://apidocs.io/img/method.png ".accountrecharge_pkg.GetASpecificTransaction") GetASpecificTransaction

> TODO: Add a method description


```go
func (me *ACCOUNTRECHARGE_IMPL) GetASpecificTransaction(transactionId string)([]byte,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| transactionId |  ``` Required ```  | 1c65-47fa-aea2-3ded9ed57557 (number, required) - Your transction id. |


#### Example Usage

```go
transactionId := "transaction_id"

var result []byte
result,_ = accountRecharge.GetASpecificTransaction(transactionId)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="automationrules_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".automationrules_pkg") automationrules_pkg

### Get instance

Factory for the ``` AUTOMATIONRULES ``` interface can be accessed from the package automationrules_pkg.

```go
automationRules := automationrules_pkg.NewAUTOMATIONRULES()
```

### <a name="list_rules"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.ListRules") ListRules

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) ListRules()(*models_pkg.ListRulesResponse,error)
```

#### Example Usage

```go

var result *models_pkg.ListRulesResponse
result,_ = automationRules.ListRules()

```


### <a name="get_a_specific_rule"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.GetASpecificRule") GetASpecificRule

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) GetASpecificRule(inboundRuleId float64)(*models_pkg.GetASpecificRuleResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Inbound Rule ID. |


#### Example Usage

```go
inboundRuleId := "1"

var result *models_pkg.GetASpecificRuleResponse
result,_ = automationRules.GetASpecificRule(inboundRuleId)

```


### <a name="create_a_new_rule"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.CreateANewRule") CreateANewRule

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) CreateANewRule(body *models_pkg.CreateANewRuleRequest)(*models_pkg.CreateANewRuleResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
var body *models_pkg.CreateANewRuleRequest

var result *models_pkg.CreateANewRuleResponse
result,_ = automationRules.CreateANewRule(body)

```


### <a name="update_a_rule"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.UpdateARule") UpdateARule

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) UpdateARule(
            inboundRuleId float64,
            body *models_pkg.UpdateARuleRequest)(*models_pkg.UpdateARuleResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Inbound Rule ID. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
inboundRuleId := "1"
bodyValue := []byte("{    \"dedicated_number\":\"+61298441484\",    \"rule_name\":\"My Rule\",    \"message_search_type\":3,    \"message_search_term\":\"My Search Term\",    \"action\":\"EMAIL_FIXED\",    \"action_address\":\"john@doe.com\",    \"enabled\":1}")
var body *models_pkg.UpdateARuleRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.UpdateARuleResponse
result,_ = automationRules.UpdateARule(inboundRuleId, body)

```


### <a name="delete_a_rule"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.DeleteARule") DeleteARule

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) DeleteARule(inboundRuleId float64)(*models_pkg.DeleteARuleResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Inbound Rule ID. |


#### Example Usage

```go
inboundRuleId := "1"

var result *models_pkg.DeleteARuleResponse
result,_ = automationRules.DeleteARule(inboundRuleId)

```


### <a name="list_rules1"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.ListRules1") ListRules1

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) ListRules1()(*models_pkg.ListRulesResponse,error)
```

#### Example Usage

```go

var result *models_pkg.ListRulesResponse
result,_ = automationRules.ListRules1()

```


### <a name="get_a_specific_rule1"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.GetASpecificRule1") GetASpecificRule1

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) GetASpecificRule1(receiptRuleId float64)(*models_pkg.GetASpecificRuleResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |


#### Example Usage

```go
receiptRuleId := "2"

var result *models_pkg.GetASpecificRuleResponse
result,_ = automationRules.GetASpecificRule1(receiptRuleId)

```


### <a name="create_a_new_rule1"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.CreateANewRule1") CreateANewRule1

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) CreateANewRule1(body *models_pkg.CreateANewRuleRequest24)(*models_pkg.CreateANewRuleResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("{    \"rule_name\": \"My Rule\",    \"match_type\": 3,    \"action\": \"EMAIL_FIXED\",    \"action_address\": \"john@doe.com\",    \"enabled\": 1}")
var body *models_pkg.CreateANewRuleRequest24
json.Unmarshal(bodyValue,&body)

var result *models_pkg.CreateANewRuleResponse
result,_ = automationRules.CreateANewRule1(body)

```


### <a name="update_a_rule1"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.UpdateARule1") UpdateARule1

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) UpdateARule1(
            receiptRuleId float64,
            body *models_pkg.UpdateARuleRequest26)(*models_pkg.UpdateARuleResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
receiptRuleId := "7"
bodyValue := []byte("{    \"rule_name\": \"My Rule\",    \"match_type\": 3,    \"action\": \"EMAIL_FIXED\",    \"action_address\": \"john@doe.com\",    \"enabled\": 1}")
var body *models_pkg.UpdateARuleRequest26
json.Unmarshal(bodyValue,&body)

var result *models_pkg.UpdateARuleResponse
result,_ = automationRules.UpdateARule1(receiptRuleId, body)

```


### <a name="delete_a_rule1"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.DeleteARule1") DeleteARule1

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) DeleteARule1(receiptRuleId float64)(*models_pkg.DeleteARuleResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |


#### Example Usage

```go
receiptRuleId := "7"

var result *models_pkg.DeleteARuleResponse
result,_ = automationRules.DeleteARule1(receiptRuleId)

```


### <a name="list_rules2"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.ListRules2") ListRules2

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) ListRules2()(*models_pkg.ListRulesResponse,error)
```

#### Example Usage

```go

var result *models_pkg.ListRulesResponse
result,_ = automationRules.ListRules2()

```


### <a name="get_a_specific_rule11"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.GetASpecificRule11") GetASpecificRule11

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) GetASpecificRule11(receiptRuleId float64)(*models_pkg.GetASpecificRuleResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |


#### Example Usage

```go
receiptRuleId := "2"

var result *models_pkg.GetASpecificRuleResponse
result,_ = automationRules.GetASpecificRule11(receiptRuleId)

```


### <a name="create_a_new_rule2"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.CreateANewRule2") CreateANewRule2

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) CreateANewRule2(body *models_pkg.CreateANewRuleRequest24)(*models_pkg.CreateANewRuleResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("{    \"rule_name\":\"My Rule\",    \"match_type\":3,    \"action\":\"EMAIL_FIXED\",    \"action_address\":\"john@doe.com\",    \"enabled\":1}")
var body *models_pkg.CreateANewRuleRequest24
json.Unmarshal(bodyValue,&body)

var result *models_pkg.CreateANewRuleResponse
result,_ = automationRules.CreateANewRule2(body)

```


### <a name="update_a_rule11"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.UpdateARule11") UpdateARule11

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) UpdateARule11(
            receiptRuleId float64,
            body *models_pkg.UpdateARuleRequest26)(*models_pkg.UpdateARuleResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
receiptRuleId := "2"
bodyValue := []byte("{    \"rule_name\":\"My Rule\",    \"match_type\":3,    \"action\":\"EMAIL_FIXED\",    \"action_address\":\"john@doe.com\",    \"enabled\":1}")
var body *models_pkg.UpdateARuleRequest26
json.Unmarshal(bodyValue,&body)

var result *models_pkg.UpdateARuleResponse
result,_ = automationRules.UpdateARule11(receiptRuleId, body)

```


### <a name="delete_a_rule11"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.DeleteARule11") DeleteARule11

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) DeleteARule11(receiptRuleId float64)(*models_pkg.DeleteARuleResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |


#### Example Usage

```go
receiptRuleId := "2"

var result *models_pkg.DeleteARuleResponse
result,_ = automationRules.DeleteARule11(receiptRuleId)

```


### <a name="list_rules3"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.ListRules3") ListRules3

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) ListRules3()(*models_pkg.ListRulesResponse,error)
```

#### Example Usage

```go

var result *models_pkg.ListRulesResponse
result,_ = automationRules.ListRules3()

```


### <a name="get_a_specific_rule111"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.GetASpecificRule111") GetASpecificRule111

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) GetASpecificRule111(inboundRuleId float64)(*models_pkg.GetASpecificRuleResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Fax inbound rule id |


#### Example Usage

```go
inboundRuleId := "14"

var result *models_pkg.GetASpecificRuleResponse
result,_ = automationRules.GetASpecificRule111(inboundRuleId)

```


### <a name="create_a_new_rule3"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.CreateANewRule3") CreateANewRule3

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) CreateANewRule3(body *models_pkg.CreateANewRuleRequest38)(*models_pkg.CreateANewRuleResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("    {        \"dedicated_number\":\"+61298441484\",        \"rule_name\":\"Rule Name\",        \"action\":\"EMAIL_FIXED\",        \"action_address\":\"email@domain.com\",        \"enabled\":1    }")
var body *models_pkg.CreateANewRuleRequest38
json.Unmarshal(bodyValue,&body)

var result *models_pkg.CreateANewRuleResponse
result,_ = automationRules.CreateANewRule3(body)

```


### <a name="update_a_rule111"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.UpdateARule111") UpdateARule111

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) UpdateARule111(
            inboundRuleId float64,
            body *models_pkg.UpdateARuleRequest40)(*models_pkg.UpdateARuleResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Fax inbound rule id |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
inboundRuleId := "14"
bodyValue := []byte("    {        \"dedicated_number\":\"+61298441484\",        \"rule_name\":\"Rule Name\",        \"action\":\"EMAIL_FIXED\",        \"action_address\":\"email@domain.com\",        \"enabled\":1    }")
var body *models_pkg.UpdateARuleRequest40
json.Unmarshal(bodyValue,&body)

var result *models_pkg.UpdateARuleResponse
result,_ = automationRules.UpdateARule111(inboundRuleId, body)

```


### <a name="delete_a_rule111"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.DeleteARule111") DeleteARule111

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) DeleteARule111(inboundRuleId float64)(*models_pkg.DeleteARuleResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Fax inbound rule id |


#### Example Usage

```go
inboundRuleId := "14"

var result *models_pkg.DeleteARuleResponse
result,_ = automationRules.DeleteARule111(inboundRuleId)

```


### <a name="list_rules4"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.ListRules4") ListRules4

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) ListRules4()(*models_pkg.ListRulesResponse,error)
```

#### Example Usage

```go

var result *models_pkg.ListRulesResponse
result,_ = automationRules.ListRules4()

```


### <a name="get_a_specific_rule2"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.GetASpecificRule2") GetASpecificRule2

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) GetASpecificRule2(ruleId float64)(*models_pkg.GetASpecificRuleResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |


#### Example Usage

```go
ruleId := "4"

var result *models_pkg.GetASpecificRuleResponse
result,_ = automationRules.GetASpecificRule2(ruleId)

```


### <a name="create_a_new_rule4"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.CreateANewRule4") CreateANewRule4

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) CreateANewRule4(body *models_pkg.CreateANewRuleRequest24)(*models_pkg.CreateANewRuleResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("    {        \"rule_name\":\"My Rule\",        \"match_type\":2,        \"action\":\"EMAIL_FIXED\",        \"action_address\":\"john@doe.com\",        \"enabled\":1    }")
var body *models_pkg.CreateANewRuleRequest24
json.Unmarshal(bodyValue,&body)

var result *models_pkg.CreateANewRuleResponse
result,_ = automationRules.CreateANewRule4(body)

```


### <a name="update_a_rule2"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.UpdateARule2") UpdateARule2

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) UpdateARule2(
            ruleId float64,
            body *models_pkg.UpdateARuleRequest26)(*models_pkg.UpdateARuleResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
ruleId := "4"
bodyValue := []byte("    {        \"rule_name\":\"My Rule\",        \"match_type\":1,        \"action\":\"EMAIL_FIXED\",        \"action_address\":\"john@doe.com\",        \"enabled\":1    }")
var body *models_pkg.UpdateARuleRequest26
json.Unmarshal(bodyValue,&body)

var result *models_pkg.UpdateARuleResponse
result,_ = automationRules.UpdateARule2(ruleId, body)

```


### <a name="delete_a_rule2"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.DeleteARule2") DeleteARule2

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) DeleteARule2(ruleId float64)(*models_pkg.DeleteARuleResponse49,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to delete. |


#### Example Usage

```go
ruleId := 155.150870406139

var result *models_pkg.DeleteARuleResponse49
result,_ = automationRules.DeleteARule2(ruleId)

```


### <a name="list_rules5"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.ListRules5") ListRules5

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) ListRules5()(*models_pkg.ListRulesResponse,error)
```

#### Example Usage

```go

var result *models_pkg.ListRulesResponse
result,_ = automationRules.ListRules5()

```


### <a name="get_a_specific_rule12"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.GetASpecificRule12") GetASpecificRule12

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) GetASpecificRule12(ruleId float64)(*models_pkg.GetASpecificRuleResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |


#### Example Usage

```go
ruleId := "5"

var result *models_pkg.GetASpecificRuleResponse
result,_ = automationRules.GetASpecificRule12(ruleId)

```


### <a name="create_a_new_rule5"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.CreateANewRule5") CreateANewRule5

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) CreateANewRule5(body *models_pkg.CreateANewRuleRequest24)(*models_pkg.CreateANewRuleResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("    {        \"rule_name\":\"My Rule\",        \"match_type\": 0,        \"action\":\"URL\",        \"action_address\":\"http://testurl.com\",        \"enabled\":1    }")
var body *models_pkg.CreateANewRuleRequest24
json.Unmarshal(bodyValue,&body)

var result *models_pkg.CreateANewRuleResponse
result,_ = automationRules.CreateANewRule5(body)

```


### <a name="update_a_rule12"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.UpdateARule12") UpdateARule12

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) UpdateARule12(
            ruleId float64,
            body *models_pkg.UpdateARuleRequest26)(*models_pkg.UpdateARuleResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
ruleId := "8"
bodyValue := []byte("    {        \"rule_name\":\"My Rule\",        \"match_type\": 0,        \"action\":\"URL\",        \"action_address\":\"http://testurl.com\",        \"enabled\":1    }")
var body *models_pkg.UpdateARuleRequest26
json.Unmarshal(bodyValue,&body)

var result *models_pkg.UpdateARuleResponse
result,_ = automationRules.UpdateARule12(ruleId, body)

```


### <a name="delete_a_rule12"></a>![Method: ](https://apidocs.io/img/method.png ".automationrules_pkg.DeleteARule12") DeleteARule12

> TODO: Add a method description


```go
func (me *AUTOMATIONRULES_IMPL) DeleteARule12(ruleId float64)(*models_pkg.DeleteARuleResponse56,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to delete. |


#### Example Usage

```go
ruleId := "8"

var result *models_pkg.DeleteARuleResponse56
result,_ = automationRules.DeleteARule12(ruleId)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="contactlists_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".contactlists_pkg") contactlists_pkg

### Get instance

Factory for the ``` CONTACTLISTS ``` interface can be accessed from the package contactlists_pkg.

```go
contactLists := contactlists_pkg.NewCONTACTLISTS()
```

### <a name="get_all_contact_lists"></a>![Method: ](https://apidocs.io/img/method.png ".contactlists_pkg.GetAllContactLists") GetAllContactLists

> TODO: Add a method description


```go
func (me *CONTACTLISTS_IMPL) GetAllContactLists()(*models_pkg.GetAllContactListsResponse,error)
```

#### Example Usage

```go

var result *models_pkg.GetAllContactListsResponse
result,_ = contactLists.GetAllContactLists()

```


### <a name="create_a_new_contact_list"></a>![Method: ](https://apidocs.io/img/method.png ".contactlists_pkg.CreateANewContactList") CreateANewContactList

> TODO: Add a method description


```go
func (me *CONTACTLISTS_IMPL) CreateANewContactList(body *models_pkg.CreateANewContactListRequest)(*models_pkg.CreateANewContactListResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("    {        \"list_name\":\"ListCT3QrVL4od\"    }")
var body *models_pkg.CreateANewContactListRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.CreateANewContactListResponse
result,_ = contactLists.CreateANewContactList(body)

```


### <a name="get_a_specific_contact_list"></a>![Method: ](https://apidocs.io/img/method.png ".contactlists_pkg.GetASpecificContactList") GetASpecificContactList

> TODO: Add a method description


```go
func (me *CONTACTLISTS_IMPL) GetASpecificContactList(listId float64)(*models_pkg.GetASpecificContactListResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |


#### Example Usage

```go
listId := "437"

var result *models_pkg.GetASpecificContactListResponse
result,_ = contactLists.GetASpecificContactList(listId)

```


### <a name="update_a_specific_contact_list"></a>![Method: ](https://apidocs.io/img/method.png ".contactlists_pkg.UpdateASpecificContactList") UpdateASpecificContactList

> TODO: Add a method description


```go
func (me *CONTACTLISTS_IMPL) UpdateASpecificContactList(
            listId float64,
            body *models_pkg.UpdateASpecificContactListRequest)(*models_pkg.UpdateASpecificContactListResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
listId := "439"
bodyValue := []byte("    {        \"list_name\":\"ListlPJf33ksjP\"    }")
var body *models_pkg.UpdateASpecificContactListRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.UpdateASpecificContactListResponse
result,_ = contactLists.UpdateASpecificContactList(listId, body)

```


### <a name="delete_a_specific_contact_list"></a>![Method: ](https://apidocs.io/img/method.png ".contactlists_pkg.DeleteASpecificContactList") DeleteASpecificContactList

> TODO: Add a method description


```go
func (me *CONTACTLISTS_IMPL) DeleteASpecificContactList(listId float64)(*models_pkg.DeleteASpecificContactListResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |


#### Example Usage

```go
listId := "442"

var result *models_pkg.DeleteASpecificContactListResponse
result,_ = contactLists.DeleteASpecificContactList(listId)

```


### <a name="create_import_contacts_to_list"></a>![Method: ](https://apidocs.io/img/method.png ".contactlists_pkg.CreateImportContactsToList") CreateImportContactsToList

> TODO: Add a method description


```go
func (me *CONTACTLISTS_IMPL) CreateImportContactsToList(
            listId float64,
            body *models_pkg.ImportContactsToListRequest)(*models_pkg.ImportContactsToListResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
listId := "437"
bodyValue := []byte("{    \"file_url\":\"http://yourdomain.com/5485EA6144/79E8/import.csv\",    \"field_order\":[        \"phone\",        \"first_name\",        \"last_name\",        \"custom1\",        \"custom2\",        \"custom3\",        \"custom4\",        \"fax_number\",        \"organization_name\",        \"email\",        \"address_line_1\",        \"address_line_2\",        \"address_city\",        \"address_state\",        \"address_postal_code\",        \"address_country\"    ]}")
var body *models_pkg.ImportContactsToListRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.ImportContactsToListResponse
result,_ = contactLists.CreateImportContactsToList(listId, body)

```


### <a name="update_remove_duplicate_contacts"></a>![Method: ](https://apidocs.io/img/method.png ".contactlists_pkg.UpdateRemoveDuplicateContacts") UpdateRemoveDuplicateContacts

> TODO: Add a method description


```go
func (me *CONTACTLISTS_IMPL) UpdateRemoveDuplicateContacts(
            listId float64,
            body *models_pkg.RemoveDuplicateContactsRequest)(*models_pkg.RemoveDuplicateContactsResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
listId := "439"
bodyValue := []byte("{    \"fields\":[        \"phone_number\",        \"first_name\",        \"last_name\",        \"fax_number\",        \"address_country\"    ]}")
var body *models_pkg.RemoveDuplicateContactsRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.RemoveDuplicateContactsResponse
result,_ = contactLists.UpdateRemoveDuplicateContacts(listId, body)

```


### <a name="get_list_of_acceptable_import_fields"></a>![Method: ](https://apidocs.io/img/method.png ".contactlists_pkg.GetListOfAcceptableImportFields") GetListOfAcceptableImportFields

> TODO: Add a method description


```go
func (me *CONTACTLISTS_IMPL) GetListOfAcceptableImportFields(listId *string)(*models_pkg.GetListOfAcceptableImportFieldsResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Optional ```  | TODO: Add a parameter description |


#### Example Usage

```go
listId := "list_id"

var result *models_pkg.GetListOfAcceptableImportFieldsResponse
result,_ = contactLists.GetListOfAcceptableImportFields(listId)

```


### <a name="create_show_csv_import_file_preview"></a>![Method: ](https://apidocs.io/img/method.png ".contactlists_pkg.CreateShowCSVImportFilePreview") CreateShowCSVImportFilePreview

> Show first row of the csv import file.


```go
func (me *CONTACTLISTS_IMPL) CreateShowCSVImportFilePreview(
            listId float64,
            body *models_pkg.ShowCSVImportFilePreviewRequest)(*models_pkg.ShowCSVImportFilePreviewResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
listId := "439"
bodyValue := []byte("{    \"file_url\":\"http://yourdomain.com/5485EA6144/79E8/import.csv\"}")
var body *models_pkg.ShowCSVImportFilePreviewRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.ShowCSVImportFilePreviewResponse
result,_ = contactLists.CreateShowCSVImportFilePreview(listId, body)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="contactsuggestions_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".contactsuggestions_pkg") contactsuggestions_pkg

### Get instance

Factory for the ``` CONTACTSUGGESTIONS ``` interface can be accessed from the package contactsuggestions_pkg.

```go
contactSuggestions := contactsuggestions_pkg.NewCONTACTSUGGESTIONS()
```

### <a name="list_contact_suggestions"></a>![Method: ](https://apidocs.io/img/method.png ".contactsuggestions_pkg.ListContactSuggestions") ListContactSuggestions

> TODO: Add a method description


```go
func (me *CONTACTSUGGESTIONS_IMPL) ListContactSuggestions()(*models_pkg.ListContactSuggestionsResponse,error)
```

#### Example Usage

```go

var result *models_pkg.ListContactSuggestionsResponse
result,_ = contactSuggestions.ListContactSuggestions()

```


[Back to List of Controllers](#list_of_controllers)

## <a name="contacts_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".contacts_pkg") contacts_pkg

### Get instance

Factory for the ``` CONTACTS ``` interface can be accessed from the package contacts_pkg.

```go
contacts := contacts_pkg.NewCONTACTS()
```

### <a name="get_all_contacts_in_a_list"></a>![Method: ](https://apidocs.io/img/method.png ".contacts_pkg.GetAllContactsInAList") GetAllContactsInAList

> TODO: Add a method description


```go
func (me *CONTACTS_IMPL) GetAllContactsInAList(listId float64)(*models_pkg.GetAllContactsInAListResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id where your contacts belong. |


#### Example Usage

```go
listId := "428"

var result *models_pkg.GetAllContactsInAListResponse
result,_ = contacts.GetAllContactsInAList(listId)

```


### <a name="create_a_new_contact"></a>![Method: ](https://apidocs.io/img/method.png ".contacts_pkg.CreateANewContact") CreateANewContact

> TODO: Add a method description


```go
func (me *CONTACTS_IMPL) CreateANewContact(
            listId float64,
            body *models_pkg.CreateANewContactRequest)(*models_pkg.CreateANewContactResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id where your contact be associated. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
listId := "428"
bodyValue := []byte("    {        \"phone_number\":\"+16783270696\",        \"first_name\":\"Ellen\",        \"last_name\":\"Diaz\",        \"custom_1\":\"Custom 1\",        \"custom_2\":\"Custom 2\",        \"custom_3\":\"Custom 3\",        \"custom_4\":\"Custom 4\",        \"fax_number\":\"+16783270696\",        \"organization_name\":\"Awesome Organization\",        \"email\":\"ellen@diaz.com\",        \"address_line_1\":\"Block 2\",        \"address_line_2\":\"Cool Bldg.\",        \"address_city\":\"Nevada\",        \"address_state\":\"Las Vegas\",        \"address_postal_code\":\"36063\",        \"address_country\":\"US\"    }")
var body *models_pkg.CreateANewContactRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.CreateANewContactResponse
result,_ = contacts.CreateANewContact(listId, body)

```


### <a name="get_a_specific_contact"></a>![Method: ](https://apidocs.io/img/method.png ".contacts_pkg.GetASpecificContact") GetASpecificContact

> TODO: Add a method description


```go
func (me *CONTACTS_IMPL) GetASpecificContact(
            listId float64,
            contactId float64)(*models_pkg.GetASpecificContactResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| contactId |  ``` Required ```  | Your contact id you want to access. |


#### Example Usage

```go
listId := "428"
contactId := "552802"

var result *models_pkg.GetASpecificContactResponse
result,_ = contacts.GetASpecificContact(listId, contactId)

```


### <a name="update_a_specific_contact"></a>![Method: ](https://apidocs.io/img/method.png ".contacts_pkg.UpdateASpecificContact") UpdateASpecificContact

> TODO: Add a method description


```go
func (me *CONTACTS_IMPL) UpdateASpecificContact(
            listId float64,
            contactId float64,
            body *models_pkg.UpdateASpecificContactRequest)(*models_pkg.UpdateASpecificContactResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| contactId |  ``` Required ```  | Your contact id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
listId := "428"
contactId := "552802"
bodyValue := []byte("{        \"phone_number\":\"+16783275492\",        \"first_name\":\"Ellen\",        \"last_name\":\"Diaz\",        \"custom_1\":\"Custom S72oJ9Teba\",        \"custom_2\":\"Custom NvrRJrKWeq\",        \"custom_3\":\"Custom 2ws94p1Dop\",        \"custom_4\":\"Custom Ku0AaIS5xb\",        \"fax_number\":\"+16783276356\",        \"organization_name\":\"Awesome Organization\",        \"email\":\"ellen@diaz.com\",        \"address_line_1\":\"Block 6\",        \"address_line_2\":\"Cool Bldg.\",        \"address_city\":\"Nevada\",        \"address_state\":\"Las Vegas\",        \"address_postal_code\":\"36063\",        \"address_country\":\"US\"    }")
var body *models_pkg.UpdateASpecificContactRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.UpdateASpecificContactResponse
result,_ = contacts.UpdateASpecificContact(listId, contactId, body)

```


### <a name="delete_a_specific_contact"></a>![Method: ](https://apidocs.io/img/method.png ".contacts_pkg.DeleteASpecificContact") DeleteASpecificContact

> TODO: Add a method description


```go
func (me *CONTACTS_IMPL) DeleteASpecificContact(
            listId float64,
            contactId float64)(*models_pkg.DeleteASpecificContactResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| contactId |  ``` Required ```  | Your contact id you want to access. |


#### Example Usage

```go
listId := "428"
contactId := "552807"

var result *models_pkg.DeleteASpecificContactResponse
result,_ = contacts.DeleteASpecificContact(listId, contactId)

```


### <a name="update_remove_opted_out_contacts"></a>![Method: ](https://apidocs.io/img/method.png ".contacts_pkg.UpdateRemoveOptedOutContacts") UpdateRemoveOptedOutContacts

> TODO: Add a method description


```go
func (me *CONTACTS_IMPL) UpdateRemoveOptedOutContacts(
            listId float64,
            optOutListId float64)(*models_pkg.RemoveOptedOutContactsResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id. |
| optOutListId |  ``` Required ```  | Your opt out list id. |


#### Example Usage

```go
listId := "439"
optOutListId := "512"

var result *models_pkg.RemoveOptedOutContactsResponse
result,_ = contacts.UpdateRemoveOptedOutContacts(listId, optOutListId)

```


### <a name="update_transfer_a_contact"></a>![Method: ](https://apidocs.io/img/method.png ".contacts_pkg.UpdateTransferAContact") UpdateTransferAContact

> Transfers a specific contact to another list.


```go
func (me *CONTACTS_IMPL) UpdateTransferAContact(
            fromListId float64,
            contactId float64,
            toListId float64)(*models_pkg.TransferAContactResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| fromListId |  ``` Required ```  | From list id. |
| contactId |  ``` Required ```  | Contact ID. |
| toListId |  ``` Required ```  | To list id. |


#### Example Usage

```go
fromListId := "428"
contactId := "1"
toListId := "429"

var result *models_pkg.TransferAContactResponse
result,_ = contacts.UpdateTransferAContact(fromListId, contactId, toListId)

```


### <a name="get_hello_contact"></a>![Method: ](https://apidocs.io/img/method.png ".contacts_pkg.GetHelloContact") GetHelloContact

> TODO: Add a method description


```go
func (me *CONTACTS_IMPL) GetHelloContact()(,error)
```

#### Example Usage

```go

var result 
result,_ = contacts.GetHelloContact()

```


[Back to List of Controllers](#list_of_controllers)

## <a name="countries_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".countries_pkg") countries_pkg

### Get instance

Factory for the ``` COUNTRIES ``` interface can be accessed from the package countries_pkg.

```go
countries := countries_pkg.NewCOUNTRIES()
```

### <a name="get_all_countries"></a>![Method: ](https://apidocs.io/img/method.png ".countries_pkg.GetAllCountries") GetAllCountries

> TODO: Add a method description


```go
func (me *COUNTRIES_IMPL) GetAllCountries()(*models_pkg.GetAllCountriesResponse,error)
```

#### Example Usage

```go

var result *models_pkg.GetAllCountriesResponse
result,_ = countries.GetAllCountries()

```


[Back to List of Controllers](#list_of_controllers)

## <a name="deliveryissues_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".deliveryissues_pkg") deliveryissues_pkg

### Get instance

Factory for the ``` DELIVERYISSUES ``` interface can be accessed from the package deliveryissues_pkg.

```go
deliveryIssues := deliveryissues_pkg.NewDELIVERYISSUES()
```

### <a name="get_delivery_issues"></a>![Method: ](https://apidocs.io/img/method.png ".deliveryissues_pkg.GetDeliveryIssues") GetDeliveryIssues

> TODO: Add a method description


```go
func (me *DELIVERYISSUES_IMPL) GetDeliveryIssues()(*models_pkg.GetDeliveryIssuesResponse,error)
```

#### Example Usage

```go

var result *models_pkg.GetDeliveryIssuesResponse
result,_ = deliveryIssues.GetDeliveryIssues()

```


### <a name="create_delivery_issue"></a>![Method: ](https://apidocs.io/img/method.png ".deliveryissues_pkg.CreateDeliveryIssue") CreateDeliveryIssue

> TODO: Add a method description


```go
func (me *DELIVERYISSUES_IMPL) CreateDeliveryIssue(body *models_pkg.CreateDeliveryIssueRequest)(*models_pkg.CreateDeliveryIssueResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("{  \"message_id\": \"B388828B\",  \"type\": \"SMS\",  \"description\": \"This is a test\",  \"client_comments\": \"test\",  \"email_address: john_doe@user.com\": \"\",  \"Body\": \"\"}")
var body *models_pkg.CreateDeliveryIssueRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.CreateDeliveryIssueResponse
result,_ = deliveryIssues.CreateDeliveryIssue(body)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="emailmarketing_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".emailmarketing_pkg") emailmarketing_pkg

### Get instance

Factory for the ``` EMAILMARKETING ``` interface can be accessed from the package emailmarketing_pkg.

```go
emailMarketing := emailmarketing_pkg.NewEMAILMARKETING()
```

### <a name="get_all_allowed_email_addresses"></a>![Method: ](https://apidocs.io/img/method.png ".emailmarketing_pkg.GetAllAllowedEmailAddresses") GetAllAllowedEmailAddresses

> TODO: Add a method description


```go
func (me *EMAILMARKETING_IMPL) GetAllAllowedEmailAddresses()(*models_pkg.GetAllAllowedEmailAddressesResponse,error)
```

#### Example Usage

```go

var result *models_pkg.GetAllAllowedEmailAddressesResponse
result,_ = emailMarketing.GetAllAllowedEmailAddresses()

```


### <a name="create_allowed_email_address"></a>![Method: ](https://apidocs.io/img/method.png ".emailmarketing_pkg.CreateAllowedEmailAddress") CreateAllowedEmailAddress

> TODO: Add a method description


```go
func (me *EMAILMARKETING_IMPL) CreateAllowedEmailAddress(body *models_pkg.CreateAllowedEmailAddressRequest)(*models_pkg.CreateAllowedEmailAddressResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("{  \"email_address\": \"johndoe1@user.com\",  \"Body\": \"\"}")
var body *models_pkg.CreateAllowedEmailAddressRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.CreateAllowedEmailAddressResponse
result,_ = emailMarketing.CreateAllowedEmailAddress(body)

```


### <a name="update_send_verification_token"></a>![Method: ](https://apidocs.io/img/method.png ".emailmarketing_pkg.UpdateSendVerificationToken") UpdateSendVerificationToken

> TODO: Add a method description


```go
func (me *EMAILMARKETING_IMPL) UpdateSendVerificationToken(emailAddressId float64)(*models_pkg.SendVerificationTokenResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email addess id you want to access. |


#### Example Usage

```go
emailAddressId := 113.427697179573

var result *models_pkg.SendVerificationTokenResponse
result,_ = emailMarketing.UpdateSendVerificationToken(emailAddressId)

```


### <a name="update_verify_allowed_email_address"></a>![Method: ](https://apidocs.io/img/method.png ".emailmarketing_pkg.UpdateVerifyAllowedEmailAddress") UpdateVerifyAllowedEmailAddress

> TODO: Add a method description


```go
func (me *EMAILMARKETING_IMPL) UpdateVerifyAllowedEmailAddress(
            emailAddressId float64,
            activationToken string)(*models_pkg.VerifyAllowedEmailAddressResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email address id you want to access. |
| activationToken |  ``` Required ```  | 6E8B-4FDB-99A7-7ED08DF97BCC (required, string) - Your activation token. |


#### Example Usage

```go
emailAddressId := "5"
activationToken := "3BD73304"

var result *models_pkg.VerifyAllowedEmailAddressResponse
result,_ = emailMarketing.UpdateVerifyAllowedEmailAddress(emailAddressId, activationToken)

```


### <a name="delete_allowed_email_address"></a>![Method: ](https://apidocs.io/img/method.png ".emailmarketing_pkg.DeleteAllowedEmailAddress") DeleteAllowedEmailAddress

> TODO: Add a method description


```go
func (me *EMAILMARKETING_IMPL) DeleteAllowedEmailAddress(emailAddressId float64)(*models_pkg.DeleteAllowedEmailAddressResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email address you want to access. |


#### Example Usage

```go
emailAddressId := 113.427697179573

var result *models_pkg.DeleteAllowedEmailAddressResponse
result,_ = emailMarketing.DeleteAllowedEmailAddress(emailAddressId)

```


### <a name="get_specific_allowed_email_address"></a>![Method: ](https://apidocs.io/img/method.png ".emailmarketing_pkg.GetSpecificAllowedEmailAddress") GetSpecificAllowedEmailAddress

> TODO: Add a method description


```go
func (me *EMAILMARKETING_IMPL) GetSpecificAllowedEmailAddress(emailAddressId float64)(*models_pkg.GetSpecificAllowedEmailAddressResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email address you want to access. |


#### Example Usage

```go
emailAddressId := "4"

var result *models_pkg.GetSpecificAllowedEmailAddressResponse
result,_ = emailMarketing.GetSpecificAllowedEmailAddress(emailAddressId)

```


### <a name="get_all_email_campaigns"></a>![Method: ](https://apidocs.io/img/method.png ".emailmarketing_pkg.GetAllEmailCampaigns") GetAllEmailCampaigns

> TODO: Add a method description


```go
func (me *EMAILMARKETING_IMPL) GetAllEmailCampaigns()(*models_pkg.GetAllEmailCampaignsResponse,error)
```

#### Example Usage

```go

var result *models_pkg.GetAllEmailCampaignsResponse
result,_ = emailMarketing.GetAllEmailCampaigns()

```


### <a name="get_specific_email_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".emailmarketing_pkg.GetSpecificEmailCampaign") GetSpecificEmailCampaign

> TODO: Add a method description


```go
func (me *EMAILMARKETING_IMPL) GetSpecificEmailCampaign(emailCampaignId float64)(*models_pkg.GetSpecificEmailCampaignResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailCampaignId |  ``` Required ```  | The email campaign id you want to access. |


#### Example Usage

```go
emailCampaignId := "1"

var result *models_pkg.GetSpecificEmailCampaignResponse
result,_ = emailMarketing.GetSpecificEmailCampaign(emailCampaignId)

```


### <a name="create_email_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".emailmarketing_pkg.CreateEmailCampaign") CreateEmailCampaign

> TODO: Add a method description


```go
func (me *EMAILMARKETING_IMPL) CreateEmailCampaign(body *models_pkg.CreateEmailCampaignRequest)(*models_pkg.CreateEmailCampaignResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("{  \"name\" : \"John Doe\",  \"subject\" : \"Lorem Ipsum\",  \"from_email_address_id\" : 2,  \"from_name\" : \"From name\",  \"template_id\" : 31,  \"body\" : \"<p>This is a test</p>\",  \"list_id\" : 456}")
var body *models_pkg.CreateEmailCampaignRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.CreateEmailCampaignResponse
result,_ = emailMarketing.CreateEmailCampaign(body)

```


### <a name="update_email_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".emailmarketing_pkg.UpdateEmailCampaign") UpdateEmailCampaign

> TODO: Add a method description


```go
func (me *EMAILMARKETING_IMPL) UpdateEmailCampaign(
            emailCampaignId float64,
            body *models_pkg.UpdateEmailCampaignRequest)(*models_pkg.UpdateEmailCampaignResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailCampaignId |  ``` Required ```  | The email campaign id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
emailCampaignId := "1"
bodyValue := []byte("{  \"name\" : \"John Doe\",  \"subject\" : \"Lorem Ipsum\",  \"from_email_address_id\" : 2,  \"from_name\" : \"From name\",  \"template_id\" : 31,  \"body\" : \"<p>This is a test</p>\",  \"list_id\" : 456}")
var body *models_pkg.UpdateEmailCampaignRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.UpdateEmailCampaignResponse
result,_ = emailMarketing.UpdateEmailCampaign(emailCampaignId, body)

```


### <a name="update_cancel_email_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".emailmarketing_pkg.UpdateCancelEmailCampaign") UpdateCancelEmailCampaign

> TODO: Add a method description


```go
func (me *EMAILMARKETING_IMPL) UpdateCancelEmailCampaign(emailCampaignId float64)(*models_pkg.CancelEmailCampaignResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailCampaignId |  ``` Required ```  | The email campaign id you want to cancel. |


#### Example Usage

```go
emailCampaignId := "1"

var result *models_pkg.CancelEmailCampaignResponse
result,_ = emailMarketing.UpdateCancelEmailCampaign(emailCampaignId)

```


### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png ".emailmarketing_pkg.CreateCalculatePrice") CreateCalculatePrice

> TODO: Add a method description


```go
func (me *EMAILMARKETING_IMPL) CreateCalculatePrice(body *models_pkg.CalculatePriceRequest)(*models_pkg.CalculatePriceResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("{  \"name\" : \"John Doe\",  \"subject\" : \"Lorem Ipsum\",  \"from_email_address_id\" : 2,  \"from_name\" : \"From name\",  \"template_id\" : 31,  \"body\" : \"<p>This is a test</p>\",  \"list_id\" : 456}")
var body *models_pkg.CalculatePriceRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.CalculatePriceResponse
result,_ = emailMarketing.CreateCalculatePrice(body)

```


### <a name="get_specific_email_campaign_history"></a>![Method: ](https://apidocs.io/img/method.png ".emailmarketing_pkg.GetSpecificEmailCampaignHistory") GetSpecificEmailCampaignHistory

> TODO: Add a method description


```go
func (me *EMAILMARKETING_IMPL) GetSpecificEmailCampaignHistory(campaignId float64)(*models_pkg.GetSpecificEmailCampaignHistoryResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| campaignId |  ``` Required ```  | The email campaign id you want to access. |


#### Example Usage

```go
campaignId := "77"

var result *models_pkg.GetSpecificEmailCampaignHistoryResponse
result,_ = emailMarketing.GetSpecificEmailCampaignHistory(campaignId)

```


### <a name="get_all_email_templates"></a>![Method: ](https://apidocs.io/img/method.png ".emailmarketing_pkg.GetAllEmailTemplates") GetAllEmailTemplates

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```go
func (me *EMAILMARKETING_IMPL) GetAllEmailTemplates()(*models_pkg.GetAllEmailTemplatesResponse,error)
```

#### Example Usage

```go

var result *models_pkg.GetAllEmailTemplatesResponse
result,_ = emailMarketing.GetAllEmailTemplates()

```


### <a name="get_specific_email_template"></a>![Method: ](https://apidocs.io/img/method.png ".emailmarketing_pkg.GetSpecificEmailTemplate") GetSpecificEmailTemplate

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```go
func (me *EMAILMARKETING_IMPL) GetSpecificEmailTemplate(templateId float64)(*models_pkg.GetSpecificEmailTemplateResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | The email template id. |


#### Example Usage

```go
templateId := "291"

var result *models_pkg.GetSpecificEmailTemplateResponse
result,_ = emailMarketing.GetSpecificEmailTemplate(templateId)

```


### <a name="create_new_email_template_from_master_template"></a>![Method: ](https://apidocs.io/img/method.png ".emailmarketing_pkg.CreateNewEmailTemplateFromMasterTemplate") CreateNewEmailTemplateFromMasterTemplate

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```go
func (me *EMAILMARKETING_IMPL) CreateNewEmailTemplateFromMasterTemplate(body *models_pkg.CreateNewEmailTemplateFromMasterTemplateRequest)(*models_pkg.CreateNewEmailTemplateFromMasterTemplateResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("{  \"template_name\": \"Minions\",  \"template_id_master\": 57}")
var body *models_pkg.CreateNewEmailTemplateFromMasterTemplateRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.CreateNewEmailTemplateFromMasterTemplateResponse
result,_ = emailMarketing.CreateNewEmailTemplateFromMasterTemplate(body)

```


### <a name="update_an_email_template"></a>![Method: ](https://apidocs.io/img/method.png ".emailmarketing_pkg.UpdateAnEmailTemplate") UpdateAnEmailTemplate

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```go
func (me *EMAILMARKETING_IMPL) UpdateAnEmailTemplate(
            templateId float64,
            body *models_pkg.UpdateAnEmailTemplateRequest)(*models_pkg.UpdateAnEmailTemplateResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | The id of the template to be updated. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
templateId := "291"
bodyValue := []byte("    {        \"template_name\":\"Minions\",        \"body\":\"This is a sample content: Sc0KNWgSMG for this template.\"    }")
var body *models_pkg.UpdateAnEmailTemplateRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.UpdateAnEmailTemplateResponse
result,_ = emailMarketing.UpdateAnEmailTemplate(templateId, body)

```


### <a name="delete_email_template"></a>![Method: ](https://apidocs.io/img/method.png ".emailmarketing_pkg.DeleteEmailTemplate") DeleteEmailTemplate

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```go
func (me *EMAILMARKETING_IMPL) DeleteEmailTemplate(templateId float64)(*models_pkg.DeleteEmailTemplateResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |


#### Example Usage

```go
templateId := "25"

var result *models_pkg.DeleteEmailTemplateResponse
result,_ = emailMarketing.DeleteEmailTemplate(templateId)

```


### <a name="get_all_master_email_templates"></a>![Method: ](https://apidocs.io/img/method.png ".emailmarketing_pkg.GetAllMasterEmailTemplates") GetAllMasterEmailTemplates

> Master templates are templates that you can clone to a User Email Template which lets you edit and save it.


```go
func (me *EMAILMARKETING_IMPL) GetAllMasterEmailTemplates()(*models_pkg.GetAllMasterEmailTemplatesResponse,error)
```

#### Example Usage

```go

var result *models_pkg.GetAllMasterEmailTemplatesResponse
result,_ = emailMarketing.GetAllMasterEmailTemplates()

```


### <a name="get_specific_master_template"></a>![Method: ](https://apidocs.io/img/method.png ".emailmarketing_pkg.GetSpecificMasterTemplate") GetSpecificMasterTemplate

> Master templates are templates that you can clone to a User Email Template which lets you edit and save it.


```go
func (me *EMAILMARKETING_IMPL) GetSpecificMasterTemplate(templateId string)(*models_pkg.GetSpecificMasterTemplateResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |


#### Example Usage

```go
templateId := "25"

var result *models_pkg.GetSpecificMasterTemplateResponse
result,_ = emailMarketing.GetSpecificMasterTemplate(templateId)

```


### <a name="get_all_master_template_categories"></a>![Method: ](https://apidocs.io/img/method.png ".emailmarketing_pkg.GetAllMasterTemplateCategories") GetAllMasterTemplateCategories

> TODO: Add a method description


```go
func (me *EMAILMARKETING_IMPL) GetAllMasterTemplateCategories()(*models_pkg.GetAllMasterTemplateCategoriesResponse,error)
```

#### Example Usage

```go

var result *models_pkg.GetAllMasterTemplateCategoriesResponse
result,_ = emailMarketing.GetAllMasterTemplateCategories()

```


### <a name="get_specific_email_template_category"></a>![Method: ](https://apidocs.io/img/method.png ".emailmarketing_pkg.GetSpecificEmailTemplateCategory") GetSpecificEmailTemplateCategory

> TODO: Add a method description


```go
func (me *EMAILMARKETING_IMPL) GetSpecificEmailTemplateCategory(categoryId string)(*models_pkg.GetSpecificEmailTemplateCategoryResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| categoryId |  ``` Required ```  | Your category id. |


#### Example Usage

```go
categoryId := "25"

var result *models_pkg.GetSpecificEmailTemplateCategoryResponse
result,_ = emailMarketing.GetSpecificEmailTemplateCategory(categoryId)

```


### <a name="get_all_templates_for_category"></a>![Method: ](https://apidocs.io/img/method.png ".emailmarketing_pkg.GetAllTemplatesForCategory") GetAllTemplatesForCategory

> TODO: Add a method description


```go
func (me *EMAILMARKETING_IMPL) GetAllTemplatesForCategory(categoryId string)(*models_pkg.GetAllTemplatesForCategoryResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| categoryId |  ``` Required ```  | Your category id. |


#### Example Usage

```go
categoryId := "1"

var result *models_pkg.GetAllTemplatesForCategoryResponse
result,_ = emailMarketing.GetAllTemplatesForCategory(categoryId)

```


### <a name="upload_image_to_specific_template"></a>![Method: ](https://apidocs.io/img/method.png ".emailmarketing_pkg.UploadImageToSpecificTemplate") UploadImageToSpecificTemplate

> TODO: Add a method description


```go
func (me *EMAILMARKETING_IMPL) UploadImageToSpecificTemplate(
            templateId string,
            body *models_pkg.UploadImageToSpecificTemplateRequest)(*models_pkg.UploadImageToSpecificTemplateResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
templateId := "1"
bodyValue := []byte("{    \"image\": \"image.png\",    \"url\" : \"http://www.downloadimg.from/here.png\"}")
var body *models_pkg.UploadImageToSpecificTemplateRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.UploadImageToSpecificTemplateResponse
result,_ = emailMarketing.UploadImageToSpecificTemplate(templateId, body)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="email_to_smsallowedaddress_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".email-to-smsallowedaddress_pkg") email-to-smsallowedaddress_pkg

### Get instance

Factory for the ``` EMAIL-TO-SMSALLOWEDADDRESS ``` interface can be accessed from the package email-to-smsallowedaddress_pkg.

```go
emailToSMSAllowedAddress := email-to-smsallowedaddress_pkg.NewEMAIL-TO-SMSALLOWEDADDRESS()
```

### <a name="list_of_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png ".email-to-smsallowedaddress_pkg.ListOfEmailToSMSAllowedAddress") ListOfEmailToSMSAllowedAddress

> Get list of allowed email addresses.


```go
func (me *EMAILTOSMSALLOWEDADDRESS_IMPL) ListOfEmailToSMSAllowedAddress()(*models_pkg.ListOfEmailToSMSAllowedAddressResponse,error)
```

#### Example Usage

```go

var result *models_pkg.ListOfEmailToSMSAllowedAddressResponse
result,_ = emailToSMSAllowedAddress.ListOfEmailToSMSAllowedAddress()

```


### <a name="create_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png ".email-to-smsallowedaddress_pkg.CreateEmailToSMSAllowedAddress") CreateEmailToSMSAllowedAddress

> Create an allowed email address.


```go
func (me *EMAILTOSMSALLOWEDADDRESS_IMPL) CreateEmailToSMSAllowedAddress(body *models_pkg.CreateEmailToSMSAllowedAddressRequest)(*models_pkg.CreateEmailToSMSAllowedAddressResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("    {        \"email_address\":\"Cv3p0@gmail.com\",        \"from\":\"+17128845887\"    }")
var body *models_pkg.CreateEmailToSMSAllowedAddressRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.CreateEmailToSMSAllowedAddressResponse
result,_ = emailToSMSAllowedAddress.CreateEmailToSMSAllowedAddress(body)

```


### <a name="get_specific_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png ".email-to-smsallowedaddress_pkg.GetSpecificEmailToSMSAllowedAddress") GetSpecificEmailToSMSAllowedAddress

> Get a specific allowed email address.


```go
func (me *EMAILTOSMSALLOWEDADDRESS_IMPL) GetSpecificEmailToSMSAllowedAddress(emailAddressId float64)(*models_pkg.GetSpecificEmailToSMSAllowedAddressResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | Your email address id. |


#### Example Usage

```go
emailAddressId := "113"

var result *models_pkg.GetSpecificEmailToSMSAllowedAddressResponse
result,_ = emailToSMSAllowedAddress.GetSpecificEmailToSMSAllowedAddress(emailAddressId)

```


### <a name="update_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png ".email-to-smsallowedaddress_pkg.UpdateEmailToSMSAllowedAddress") UpdateEmailToSMSAllowedAddress

> Update a specific allowed email address.


```go
func (me *EMAILTOSMSALLOWEDADDRESS_IMPL) UpdateEmailToSMSAllowedAddress(
            emailAddressId float64,
            body *models_pkg.UpdateEmailToSMSAllowedAddressRequest)(*models_pkg.UpdateEmailToSMSAllowedAddressResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | Your email address id. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
emailAddressId := "107"
bodyValue := []byte("    {        \"email_address\":\"pfvRZ@gmail.com\",        \"from\":\"+17128842283\"    }")
var body *models_pkg.UpdateEmailToSMSAllowedAddressRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.UpdateEmailToSMSAllowedAddressResponse
result,_ = emailToSMSAllowedAddress.UpdateEmailToSMSAllowedAddress(emailAddressId, body)

```


### <a name="delete_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png ".email-to-smsallowedaddress_pkg.DeleteEmailToSMSAllowedAddress") DeleteEmailToSMSAllowedAddress

> Delete a specific allowed email address.


```go
func (me *EMAILTOSMSALLOWEDADDRESS_IMPL) DeleteEmailToSMSAllowedAddress(emailAddressId float64)(*models_pkg.DeleteEmailToSMSAllowedAddressResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | Your email address id. |


#### Example Usage

```go
emailAddressId := "107"

var result *models_pkg.DeleteEmailToSMSAllowedAddressResponse
result,_ = emailToSMSAllowedAddress.DeleteEmailToSMSAllowedAddress(emailAddressId)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="email_to_smsstrippedstrings_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".email-to-smsstrippedstrings_pkg") email-to-smsstrippedstrings_pkg

### Get instance

Factory for the ``` EMAIL-TO-SMSSTRIPPEDSTRINGS ``` interface can be accessed from the package email-to-smsstrippedstrings_pkg.

```go
emailToSMSStrippedStrings := email-to-smsstrippedstrings_pkg.NewEMAIL-TO-SMSSTRIPPEDSTRINGS()
```

### <a name="list_stripped_strings"></a>![Method: ](https://apidocs.io/img/method.png ".email-to-smsstrippedstrings_pkg.ListStrippedStrings") ListStrippedStrings

> TODO: Add a method description


```go
func (me *EMAILTOSMSSTRIPPEDSTRINGS_IMPL) ListStrippedStrings()(*models_pkg.ListStrippedStringsResponse,error)
```

#### Example Usage

```go

var result *models_pkg.ListStrippedStringsResponse
result,_ = emailToSMSStrippedStrings.ListStrippedStrings()

```


### <a name="find_specific_stripped_string"></a>![Method: ](https://apidocs.io/img/method.png ".email-to-smsstrippedstrings_pkg.FindSpecificStrippedString") FindSpecificStrippedString

> TODO: Add a method description


```go
func (me *EMAILTOSMSSTRIPPEDSTRINGS_IMPL) FindSpecificStrippedString(ruleId float64)(*models_pkg.FindSpecificStrippedStringResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |


#### Example Usage

```go
ruleId := "18"

var result *models_pkg.FindSpecificStrippedStringResponse
result,_ = emailToSMSStrippedStrings.FindSpecificStrippedString(ruleId)

```


### <a name="create_stripped_string"></a>![Method: ](https://apidocs.io/img/method.png ".email-to-smsstrippedstrings_pkg.CreateStrippedString") CreateStrippedString

> TODO: Add a method description


```go
func (me *EMAILTOSMSSTRIPPEDSTRINGS_IMPL) CreateStrippedString(body *models_pkg.CreateStrippedStringRequest)(*models_pkg.CreateStrippedStringResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("{    \"strip_string\" : \"~~~test~~~\"}")
var body *models_pkg.CreateStrippedStringRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.CreateStrippedStringResponse
result,_ = emailToSMSStrippedStrings.CreateStrippedString(body)

```


### <a name="update_stripped_string"></a>![Method: ](https://apidocs.io/img/method.png ".email-to-smsstrippedstrings_pkg.UpdateStrippedString") UpdateStrippedString

> TODO: Add a method description


```go
func (me *EMAILTOSMSSTRIPPEDSTRINGS_IMPL) UpdateStrippedString(
            ruleId float64,
            body *models_pkg.UpdateStrippedStringRequest)(*models_pkg.UpdateStrippedStringResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
ruleId := "20"
bodyValue := []byte("{    \"strip_string\" : \"~~~test1~~~\"}")
var body *models_pkg.UpdateStrippedStringRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.UpdateStrippedStringResponse
result,_ = emailToSMSStrippedStrings.UpdateStrippedString(ruleId, body)

```


### <a name="delete_stripped_string"></a>![Method: ](https://apidocs.io/img/method.png ".email-to-smsstrippedstrings_pkg.DeleteStrippedString") DeleteStrippedString

> TODO: Add a method description


```go
func (me *EMAILTOSMSSTRIPPEDSTRINGS_IMPL) DeleteStrippedString(ruleId float64)(*models_pkg.DeleteStrippedStringResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |


#### Example Usage

```go
ruleId := "20"

var result *models_pkg.DeleteStrippedStringResponse
result,_ = emailToSMSStrippedStrings.DeleteStrippedString(ruleId)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="fax_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".fax_pkg") fax_pkg

### Get instance

Factory for the ``` FAX ``` interface can be accessed from the package fax_pkg.

```go
fax := fax_pkg.NewFAX()
```

### <a name="create_send_fax"></a>![Method: ](https://apidocs.io/img/method.png ".fax_pkg.CreateSendFax") CreateSendFax

> **Letter File Options**
> **Use existing URL**
> With this option, you can use an existing URL to a PDF document. For example, you might generate the pdf on your server.
> **Upload File to Our Server**
> With this option, you can use the `/uploads` endpoint to upload the document. The `/uploads` endpoint returns a URL that can be used in the `/fax/send` endpoint.


```go
func (me *FAX_IMPL) CreateSendFax(body *models_pkg.SendFaxRequest)(*models_pkg.SendFaxResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
var body *models_pkg.SendFaxRequest

var result *models_pkg.SendFaxResponse
result,_ = fax.CreateSendFax(body)

```


### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png ".fax_pkg.CreateCalculatePrice") CreateCalculatePrice

> TODO: Add a method description


```go
func (me *FAX_IMPL) CreateCalculatePrice(body *models_pkg.CalculatePriceRequest132)(*models_pkg.CalculatePriceResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
var body *models_pkg.CalculatePriceRequest132

var result *models_pkg.CalculatePriceResponse
result,_ = fax.CreateCalculatePrice(body)

```


### <a name="get_fax_history"></a>![Method: ](https://apidocs.io/img/method.png ".fax_pkg.GetFaxHistory") GetFaxHistory

> Get a list of Fax History.


```go
func (me *FAX_IMPL) GetFaxHistory(
            dateFrom *float64,
            dateTo *float64,
            q *string,
            orderBy *string)(*models_pkg.GetFaxHistoryResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateFrom |  ``` Optional ```  | Customize result by setting from date (timestsamp) |
| dateTo |  ``` Optional ```  | Customize result by setting to date (timestamp) |
| q |  ``` Optional ```  | Custom query |
| orderBy |  ``` Optional ```  | Order result by |


#### Example Usage

```go
dateFrom := "1457572619"
dateTo := "1457573000"
q := "status:Sent,status_code:201"
orderBy := "subject:desc"

var result *models_pkg.GetFaxHistoryResponse
result,_ = fax.GetFaxHistory(dateFrom, dateTo, q, orderBy)

```


### <a name="list_of_fax_delivery_receipts"></a>![Method: ](https://apidocs.io/img/method.png ".fax_pkg.ListOfFaxDeliveryReceipts") ListOfFaxDeliveryReceipts

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


```go
func (me *FAX_IMPL) ListOfFaxDeliveryReceipts()(*models_pkg.ListOfFaxDeliveryReceiptsResponse,error)
```

#### Example Usage

```go

var result *models_pkg.ListOfFaxDeliveryReceiptsResponse
result,_ = fax.ListOfFaxDeliveryReceipts()

```


### <a name="get_a_specific_fax_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png ".fax_pkg.GetASpecificFaxDeliveryReceipt") GetASpecificFaxDeliveryReceipt

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


```go
func (me *FAX_IMPL) GetASpecificFaxDeliveryReceipt(messageId string)(*models_pkg.GetASpecificFaxDeliveryReceiptResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | D2AF-479B-8955-6395D561DEF4" (required, number) - Message ID. |


#### Example Usage

```go
messageId := "\"3FAC74F1"

var result *models_pkg.GetASpecificFaxDeliveryReceiptResponse
result,_ = fax.GetASpecificFaxDeliveryReceipt(messageId)

```


### <a name="update_mark_fax_delivery_receipts_as_read"></a>![Method: ](https://apidocs.io/img/method.png ".fax_pkg.UpdateMarkFaxDeliveryReceiptsAsRead") UpdateMarkFaxDeliveryReceiptsAsRead

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


```go
func (me *FAX_IMPL) UpdateMarkFaxDeliveryReceiptsAsRead(body *models_pkg.MarkFaxDeliveryReceiptsAsReadRequest)(*models_pkg.MarkFaxDeliveryReceiptsAsReadResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("{    \"date_before\": 1441958441}")
var body *models_pkg.MarkFaxDeliveryReceiptsAsReadRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.MarkFaxDeliveryReceiptsAsReadResponse
result,_ = fax.UpdateMarkFaxDeliveryReceiptsAsRead(body)

```


### <a name="add_a_test_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png ".fax_pkg.AddATestDeliveryReceipt") AddATestDeliveryReceipt

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


```go
func (me *FAX_IMPL) AddATestDeliveryReceipt(body *models_pkg.AddATestDeliveryReceiptRequest)(*models_pkg.AddATestDeliveryReceiptResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("    {        \"url\":\"http://yourUrl.com\"    }")
var body *models_pkg.AddATestDeliveryReceiptRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.AddATestDeliveryReceiptResponse
result,_ = fax.AddATestDeliveryReceipt(body)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="forgotaccount_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".forgotaccount_pkg") forgotaccount_pkg

### Get instance

Factory for the ``` FORGOTACCOUNT ``` interface can be accessed from the package forgotaccount_pkg.

```go
forgotAccount := forgotaccount_pkg.NewFORGOTACCOUNT()
```

### <a name="update_forgot_username"></a>![Method: ](https://apidocs.io/img/method.png ".forgotaccount_pkg.UpdateForgotUsername") UpdateForgotUsername

> TODO: Add a method description


```go
func (me *FORGOTACCOUNT_IMPL) UpdateForgotUsername(body *models_pkg.ForgotUsernameRequest)(*models_pkg.ForgotUsernameResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
var body *models_pkg.ForgotUsernameRequest

var result *models_pkg.ForgotUsernameResponse
result,_ = forgotAccount.UpdateForgotUsername(body)

```


### <a name="update_forgot_password"></a>![Method: ](https://apidocs.io/img/method.png ".forgotaccount_pkg.UpdateForgotPassword") UpdateForgotPassword

> TODO: Add a method description


```go
func (me *FORGOTACCOUNT_IMPL) UpdateForgotPassword(body *models_pkg.ForgotPasswordRequest)(*models_pkg.ForgotPasswordResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("    {        \"username\": \"0F6pKiiuca\"    }")
var body *models_pkg.ForgotPasswordRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.ForgotPasswordResponse
result,_ = forgotAccount.UpdateForgotPassword(body)

```


### <a name="update_verify_forgot_password"></a>![Method: ](https://apidocs.io/img/method.png ".forgotaccount_pkg.UpdateVerifyForgotPassword") UpdateVerifyForgotPassword

> TODO: Add a method description


```go
func (me *FORGOTACCOUNT_IMPL) UpdateVerifyForgotPassword(body *models_pkg.VerifyForgotPasswordRequest)(*models_pkg.VerifyForgotPasswordResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("    {        \"subaccount_id\": 54,        \"activation_token\": \"9C648BAD-EB7F-4E7E-96BC-B433140C4F1F\",        \"password\": \"0F6pKiiuca\"    }")
var body *models_pkg.VerifyForgotPasswordRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.VerifyForgotPasswordResponse
result,_ = forgotAccount.UpdateVerifyForgotPassword(body)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="mms_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".mms_pkg") mms_pkg

### Get instance

Factory for the ``` MMS ``` interface can be accessed from the package mms_pkg.

```go
mMS := mms_pkg.NewMMS()
```

### <a name="create_send_mms"></a>![Method: ](https://apidocs.io/img/method.png ".mms_pkg.CreateSendMMS") CreateSendMMS

> TODO: Add a method description


```go
func (me *MMS_IMPL) CreateSendMMS(body *models_pkg.SendMMSRequest)(*models_pkg.SendMMSResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
var body *models_pkg.SendMMSRequest

var result *models_pkg.SendMMSResponse
result,_ = mMS.CreateSendMMS(body)

```


### <a name="create_get_price"></a>![Method: ](https://apidocs.io/img/method.png ".mms_pkg.CreateGetPrice") CreateGetPrice

> TODO: Add a method description


```go
func (me *MMS_IMPL) CreateGetPrice(body *models_pkg.GetPriceRequest)(*models_pkg.GetPriceResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
var body *models_pkg.GetPriceRequest

var result *models_pkg.GetPriceResponse
result,_ = mMS.CreateGetPrice(body)

```


### <a name="get_mms_history"></a>![Method: ](https://apidocs.io/img/method.png ".mms_pkg.GetMMSHistory") GetMMSHistory

> TODO: Add a method description


```go
func (me *MMS_IMPL) GetMMSHistory(
            q *string,
            orderBy *string,
            dateFrom *int64,
            dateTo *int64)(*models_pkg.GetMMSHistoryResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| q |  ``` Optional ```  | A custom query. |
| orderBy |  ``` Optional ```  | Sort records by. |
| dateFrom |  ``` Optional ```  | Timestamp (from) used to show records by date. |
| dateTo |  ``` Optional ```  | Timestamp (to) used to show records by date. |


#### Example Usage

```go
q := "list_id:429,direction:out"
orderBy := "subject:desc"
dateFrom,_ := strconv.ParseInt("1443501617", 10, 8)
dateTo,_ := strconv.ParseInt("1443501727", 10, 8)

var result *models_pkg.GetMMSHistoryResponse
result,_ = mMS.GetMMSHistory(q, orderBy, dateFrom, dateTo)

```


### <a name="get_export_mms_history"></a>![Method: ](https://apidocs.io/img/method.png ".mms_pkg.GetExportMMSHistory") GetExportMMSHistory

> TODO: Add a method description


```go
func (me *MMS_IMPL) GetExportMMSHistory(filename string)(*models_pkg.ExportMMSHistoryResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | Your export filename. |


#### Example Usage

```go
filename := "export.csv"

var result *models_pkg.ExportMMSHistoryResponse
result,_ = mMS.GetExportMMSHistory(filename)

```


### <a name="update_cancel_mms"></a>![Method: ](https://apidocs.io/img/method.png ".mms_pkg.UpdateCancelMMS") UpdateCancelMMS

> TODO: Add a method description


```go
func (me *MMS_IMPL) UpdateCancelMMS(messageId string)(*models_pkg.CancelMMSResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Message ID. |


#### Example Usage

```go
messageId := "message_id"

var result *models_pkg.CancelMMSResponse
result,_ = mMS.UpdateCancelMMS(messageId)

```


### <a name="update_cancel_all_mms"></a>![Method: ](https://apidocs.io/img/method.png ".mms_pkg.UpdateCancelAllMMS") UpdateCancelAllMMS

> TODO: Add a method description


```go
func (me *MMS_IMPL) UpdateCancelAllMMS()(*models_pkg.CancelAllMMSResponse,error)
```

#### Example Usage

```go

var result *models_pkg.CancelAllMMSResponse
result,_ = mMS.UpdateCancelAllMMS()

```


### <a name="get_all_delivery_receipts"></a>![Method: ](https://apidocs.io/img/method.png ".mms_pkg.GetAllDeliveryReceipts") GetAllDeliveryReceipts

> TODO: Add a method description


```go
func (me *MMS_IMPL) GetAllDeliveryReceipts()(*models_pkg.GetAllDeliveryReceiptsResponse,error)
```

#### Example Usage

```go

var result *models_pkg.GetAllDeliveryReceiptsResponse
result,_ = mMS.GetAllDeliveryReceipts()

```


### <a name="get_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png ".mms_pkg.GetDeliveryReceipt") GetDeliveryReceipt

> TODO: Add a method description


```go
func (me *MMS_IMPL) GetDeliveryReceipt(messageId string)(*models_pkg.GetDeliveryReceiptResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Message ID. |


#### Example Usage

```go
messageId := "3E0DC217-7D0F-4C20-A3F2-E3362B938CAF"

var result *models_pkg.GetDeliveryReceiptResponse
result,_ = mMS.GetDeliveryReceipt(messageId)

```


### <a name="update_mark_receipts_as_read"></a>![Method: ](https://apidocs.io/img/method.png ".mms_pkg.UpdateMarkReceiptsAsRead") UpdateMarkReceiptsAsRead

> TODO: Add a method description


```go
func (me *MMS_IMPL) UpdateMarkReceiptsAsRead()(*models_pkg.MarkReceiptsAsReadResponse,error)
```

#### Example Usage

```go

var result *models_pkg.MarkReceiptsAsReadResponse
result,_ = mMS.UpdateMarkReceiptsAsRead()

```


### <a name="get_all_inbound_sms_pull"></a>![Method: ](https://apidocs.io/img/method.png ".mms_pkg.GetAllInboundSMSPull") GetAllInboundSMSPull

> Inbound MMS shares the same rules/settings/endpoints as SMS. Any attachments will be converted to a URL.
> **Push Inbound SMS**
> If you prefer, we can push message replies to your server as they arrive with us.
> Refer to SMS->Inbound SMS in the docs.
> **Pull Inbound SMS**
> Receive SMS by polling your Inbox.
> Refer to SMS->Inbound SMS in the docs.


```go
func (me *MMS_IMPL) GetAllInboundSMSPull()(interface{},error)
```

#### Example Usage

```go

var result interface{}
result,_ = mMS.GetAllInboundSMSPull()

```


[Back to List of Controllers](#list_of_controllers)

## <a name="numbers_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".numbers_pkg") numbers_pkg

### Get instance

Factory for the ``` NUMBERS ``` interface can be accessed from the package numbers_pkg.

```go
numbers := numbers_pkg.NewNUMBERS()
```

### <a name="get_all_dedicated_numbers"></a>![Method: ](https://apidocs.io/img/method.png ".numbers_pkg.GetAllDedicatedNumbers") GetAllDedicatedNumbers

> TODO: Add a method description


```go
func (me *NUMBERS_IMPL) GetAllDedicatedNumbers()(*models_pkg.GetAllDedicatedNumbersResponse,error)
```

#### Example Usage

```go

var result *models_pkg.GetAllDedicatedNumbersResponse
result,_ = numbers.GetAllDedicatedNumbers()

```


### <a name="create_buy_dedicated_number"></a>![Method: ](https://apidocs.io/img/method.png ".numbers_pkg.CreateBuyDedicatedNumber") CreateBuyDedicatedNumber

> TODO: Add a method description


```go
func (me *NUMBERS_IMPL) CreateBuyDedicatedNumber(dedicatedNumber string)(*models_pkg.BuyDedicatedNumberResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dedicatedNumber |  ``` Required ```  | Your phone number in E.164 format. |


#### Example Usage

```go
dedicatedNumber := "+12282060576"

var result *models_pkg.BuyDedicatedNumberResponse
result,_ = numbers.CreateBuyDedicatedNumber(dedicatedNumber)

```


### <a name="search_dedicated_numbers_by_country"></a>![Method: ](https://apidocs.io/img/method.png ".numbers_pkg.SearchDedicatedNumbersByCountry") SearchDedicatedNumbersByCountry

> TODO: Add a method description


```go
func (me *NUMBERS_IMPL) SearchDedicatedNumbersByCountry(
            country string,
            search *string,
            searchType *float64)(*models_pkg.SearchDedicatedNumbersByCountryResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Required ```  | Your preferred country. |
| search |  ``` Optional ```  | Your search pattern or query. |
| searchType |  ``` Optional ```  | Your strategy for searching, 0 = starts with, 1 = anywhere, 2 = ends with. |


#### Example Usage

```go
country := "US"
search := "88"
searchType := "1"

var result *models_pkg.SearchDedicatedNumbersByCountryResponse
result,_ = numbers.SearchDedicatedNumbersByCountry(country, search, searchType)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="pricing_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".pricing_pkg") pricing_pkg

### Get instance

Factory for the ``` PRICING ``` interface can be accessed from the package pricing_pkg.

```go
pricing := pricing_pkg.NewPRICING()
```

### <a name="get_country_pricing"></a>![Method: ](https://apidocs.io/img/method.png ".pricing_pkg.GetCountryPricing") GetCountryPricing

> TODO: Add a method description


```go
func (me *PRICING_IMPL) GetCountryPricing(
            country string,
            currency *string)(*models_pkg.GetCountryPricingResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Required ```  | Two-letter representation of the country. |
| currency |  ``` Optional ```  | Three-letter representation of the currency. |


#### Example Usage

```go
country := "AU"
currency := "AUD"

var result *models_pkg.GetCountryPricingResponse
result,_ = pricing.GetCountryPricing(country, currency)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="postdirectmail_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".postdirectmail_pkg") postdirectmail_pkg

### Get instance

Factory for the ``` POSTDIRECTMAIL ``` interface can be accessed from the package postdirectmail_pkg.

```go
postDirectMail := postdirectmail_pkg.NewPOSTDIRECTMAIL()
```

### <a name="search_locations"></a>![Method: ](https://apidocs.io/img/method.png ".postdirectmail_pkg.SearchLocations") SearchLocations

> TODO: Add a method description


```go
func (me *POSTDIRECTMAIL_IMPL) SearchLocations(
            country string,
            query string)(*models_pkg.SearchLocationsResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Required ```  | Country code. |
| query |  ``` Required ```  | A postal code or place name. |


#### Example Usage

```go
country := "AD"
query := "AD100"

var result *models_pkg.SearchLocationsResponse
result,_ = postDirectMail.SearchLocations(country, query)

```


### <a name="create_new_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".postdirectmail_pkg.CreateNewCampaign") CreateNewCampaign

> Create new direct mail campaign.


```go
func (me *POSTDIRECTMAIL_IMPL) CreateNewCampaign(body *models_pkg.CreateNewCampaignRequest)(*models_pkg.CreateNewCampaignResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
var body *models_pkg.CreateNewCampaignRequest

var result *models_pkg.CreateNewCampaignResponse
result,_ = postDirectMail.CreateNewCampaign(body)

```


### <a name="create_calculate_direct_mail_campaign_price"></a>![Method: ](https://apidocs.io/img/method.png ".postdirectmail_pkg.CreateCalculateDirectMailCampaignPrice") CreateCalculateDirectMailCampaignPrice

> Calculate direct mail campaign price.


```go
func (me *POSTDIRECTMAIL_IMPL) CreateCalculateDirectMailCampaignPrice(body *models_pkg.CalculateDirectMailCampaignPriceRequest)(*models_pkg.CalculateDirectMailCampaignPriceResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
var body *models_pkg.CalculateDirectMailCampaignPriceRequest

var result *models_pkg.CalculateDirectMailCampaignPriceResponse
result,_ = postDirectMail.CreateCalculateDirectMailCampaignPrice(body)

```


### <a name="list_direct_mail_campaigns"></a>![Method: ](https://apidocs.io/img/method.png ".postdirectmail_pkg.ListDirectMailCampaigns") ListDirectMailCampaigns

> Get list of direct mail campaigns.


```go
func (me *POSTDIRECTMAIL_IMPL) ListDirectMailCampaigns()(*models_pkg.ListDirectMailCampaignsResponse,error)
```

#### Example Usage

```go

var result *models_pkg.ListDirectMailCampaignsResponse
result,_ = postDirectMail.ListDirectMailCampaigns()

```


[Back to List of Controllers](#list_of_controllers)

## <a name="postletter_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".postletter_pkg") postletter_pkg

### Get instance

Factory for the ``` POSTLETTER ``` interface can be accessed from the package postletter_pkg.

```go
postLetter := postletter_pkg.NewPOSTLETTER()
```

### <a name="create_send_post_letter"></a>![Method: ](https://apidocs.io/img/method.png ".postletter_pkg.CreateSendPostLetter") CreateSendPostLetter

> **Supported File Types**
> We support `pdf`, `docx` and `doc` files. Contact us to add support for any other file type. If you're using `docx` or `doc` files, you'll need to convert the file first using our uploads endpoint with the querystring parameter `convert=post` e.g. `POST /uploads?convert=post`. This will return a URL to the converted pdf file that can be used in the `/post/letters/send` endpoint.
> **Letter File Options**
> **Use existing URL**
> With this option, you can use an existing URL to a `pdf` document. For example, you might generate the `pdf` on your server.
> **Upload File to Our Server**
> With this option, you can use the `/uploads` endpoint to upload the document. The `/uploads` endpoint returns a URL that can be used in the `/post/letters/send` endpoint.


```go
func (me *POSTLETTER_IMPL) CreateSendPostLetter(body *models_pkg.SendPostLetterRequest)(*models_pkg.SendPostLetterResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("{  \"file_url\": \"http://server.com/file.pdf\",  \"template_used\": 1,  \"colour\": 1,  \"duplex\": 0,  \"recipients\": [    {      \"address_name\": \"My Home Address\",      \"address_line_1\": \"Address 1\",      \"address_line_2\": \"Address 2\",      \"address_city\": \"CITY\",      \"address_state\": \"State\",      \"address_postal_code\": 123456,      \"address_country\": \"AU\",      \"return_address_id\": 1,      \"schedule\": 1449573604    }  ]}")
var body *models_pkg.SendPostLetterRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.SendPostLetterResponse
result,_ = postLetter.CreateSendPostLetter(body)

```


### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png ".postletter_pkg.CreateCalculatePrice") CreateCalculatePrice

> TODO: Add a method description


```go
func (me *POSTLETTER_IMPL) CreateCalculatePrice(body *models_pkg.CalculatePriceRequest170)(*models_pkg.CalculatePriceResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("{  \"file_url\": \"http://server.com/file.pdf\",  \"template_used\": 1,  \"colour\": 1,  \"duplex\": 0,  \"recipients\": [    \"[]\"  ],  \"Body\": \"\"}")
var body *models_pkg.CalculatePriceRequest170
json.Unmarshal(bodyValue,&body)

var result *models_pkg.CalculatePriceResponse
result,_ = postLetter.CreateCalculatePrice(body)

```


### <a name="get_post_letter_history"></a>![Method: ](https://apidocs.io/img/method.png ".postletter_pkg.GetPostLetterHistory") GetPostLetterHistory

> TODO: Add a method description


```go
func (me *POSTLETTER_IMPL) GetPostLetterHistory()(*models_pkg.GetPostLetterHistoryResponse,error)
```

#### Example Usage

```go

var result *models_pkg.GetPostLetterHistoryResponse
result,_ = postLetter.GetPostLetterHistory()

```


### <a name="get_export_post_letter_history"></a>![Method: ](https://apidocs.io/img/method.png ".postletter_pkg.GetExportPostLetterHistory") GetExportPostLetterHistory

> TODO: Add a method description


```go
func (me *POSTLETTER_IMPL) GetExportPostLetterHistory(filename string)(*models_pkg.ExportPostLetterHistoryResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | Filename for the export file. |


#### Example Usage

```go
filename := "myexport.csv"

var result *models_pkg.ExportPostLetterHistoryResponse
result,_ = postLetter.GetExportPostLetterHistory(filename)

```


### <a name="create_a_post_return_address"></a>![Method: ](https://apidocs.io/img/method.png ".postletter_pkg.CreateAPostReturnAddress") CreateAPostReturnAddress

> TODO: Add a method description


```go
func (me *POSTLETTER_IMPL) CreateAPostReturnAddress(body *models_pkg.CreateAPostReturnAddressRequest)(*models_pkg.CreateAPostReturnAddressResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("{    \"address_name\":\"My Home Address\",    \"address_line_1\":\"Maritime Avenue\",    \"address_line_2\":\"\",    \"address_city\":\"Flynn\",    \"address_state\":\"WA\",    \"address_postal_code\":6302,    \"address_country\":\"Australia\"}")
var body *models_pkg.CreateAPostReturnAddressRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.CreateAPostReturnAddressResponse
result,_ = postLetter.CreateAPostReturnAddress(body)

```


### <a name="get_list_of_post_return_addresses"></a>![Method: ](https://apidocs.io/img/method.png ".postletter_pkg.GetListOfPostReturnAddresses") GetListOfPostReturnAddresses

> TODO: Add a method description


```go
func (me *POSTLETTER_IMPL) GetListOfPostReturnAddresses()(*models_pkg.GetListOfPostReturnAddressesResponse,error)
```

#### Example Usage

```go

var result *models_pkg.GetListOfPostReturnAddressesResponse
result,_ = postLetter.GetListOfPostReturnAddresses()

```


### <a name="get_post_return_address"></a>![Method: ](https://apidocs.io/img/method.png ".postletter_pkg.GetPostReturnAddress") GetPostReturnAddress

> TODO: Add a method description


```go
func (me *POSTLETTER_IMPL) GetPostReturnAddress(returnAddressId float64)(*models_pkg.GetPostReturnAddressResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| returnAddressId |  ``` Required ```  | Your return address id. |


#### Example Usage

```go
returnAddressId := "14"

var result *models_pkg.GetPostReturnAddressResponse
result,_ = postLetter.GetPostReturnAddress(returnAddressId)

```


### <a name="update_post_return_address"></a>![Method: ](https://apidocs.io/img/method.png ".postletter_pkg.UpdatePostReturnAddress") UpdatePostReturnAddress

> TODO: Add a method description


```go
func (me *POSTLETTER_IMPL) UpdatePostReturnAddress(
            returnAddressId float64,
            body *models_pkg.UpdatePostReturnAddressRequest)(*models_pkg.UpdatePostReturnAddressResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| returnAddressId |  ``` Required ```  | Your return address id. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
returnAddressId := "14"
bodyValue := []byte("{    \"address_name\":\"My Home Address\",    \"address_line_1\":\"Maritime Avenue\",    \"address_line_2\":\"\",    \"address_city\":\"Flynn\",    \"address_state\":\"WA\",    \"address_postal_code\":6302,    \"address_country\":\"Australia\"}")
var body *models_pkg.UpdatePostReturnAddressRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.UpdatePostReturnAddressResponse
result,_ = postLetter.UpdatePostReturnAddress(returnAddressId, body)

```


### <a name="delete_post_return_address"></a>![Method: ](https://apidocs.io/img/method.png ".postletter_pkg.DeletePostReturnAddress") DeletePostReturnAddress

> TODO: Add a method description


```go
func (me *POSTLETTER_IMPL) DeletePostReturnAddress(returnAddressId float64)(*models_pkg.DeletePostReturnAddressResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| returnAddressId |  ``` Required ```  | Your return address id. |


#### Example Usage

```go
returnAddressId := "12"

var result *models_pkg.DeletePostReturnAddressResponse
result,_ = postLetter.DeletePostReturnAddress(returnAddressId)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="postcards_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".postcards_pkg") postcards_pkg

### Get instance

Factory for the ``` POSTCARDS ``` interface can be accessed from the package postcards_pkg.

```go
postcards := postcards_pkg.NewPOSTCARDS()
```

### <a name="create_send_postcard"></a>![Method: ](https://apidocs.io/img/method.png ".postcards_pkg.CreateSendPostcard") CreateSendPostcard

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


```go
func (me *POSTCARDS_IMPL) CreateSendPostcard(body *models_pkg.SendPostcardRequest)(*models_pkg.SendPostcardResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("{    \"file_urls\":[         \"https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_front.pdf\",         \"https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_back.pdf\"    ],    \"recipients\":[        {            \"address_name\":\"My Home Address\",            \"address_line_1\":\"Address 1\",            \"address_line_2\":\"\",            \"address_city\":\"City\",            \"address_state\":\"State\",            \"address_postal_code\":\"123456\",            \"address_country\":\"AU\",            \"return_address_id\":1        }    ]}")
var body *models_pkg.SendPostcardRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.SendPostcardResponse
result,_ = postcards.CreateSendPostcard(body)

```


### <a name="create_calculate_pricing"></a>![Method: ](https://apidocs.io/img/method.png ".postcards_pkg.CreateCalculatePricing") CreateCalculatePricing

> For `file_urls` field. You can attach at least 1 and max of 2 PDF file urls.
> - Supply a single pdf with 2 pages (front and back)
> - Supply 2 urls to seperate PDFs


```go
func (me *POSTCARDS_IMPL) CreateCalculatePricing(body *models_pkg.CalculatePricingRequest)(*models_pkg.CalculatePricingResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("{    \"file_urls\":[        \"https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_front.pdf\",        \"https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_back.pdf\"    ],    \"recipients\":[        {            \"address_name\":\"My Home Address\",            \"address_line_1\":\"Address 1\",            \"address_line_2\":\"\",            \"address_city\":\"City\",            \"address_state\":\"State\",            \"address_postal_code\":\"123456\",            \"address_country\":\"AU\",            \"return_address_id\":1        }    ]}")
var body *models_pkg.CalculatePricingRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.CalculatePricingResponse
result,_ = postcards.CreateCalculatePricing(body)

```


### <a name="get_postcard_history"></a>![Method: ](https://apidocs.io/img/method.png ".postcards_pkg.GetPostcardHistory") GetPostcardHistory

> TODO: Add a method description


```go
func (me *POSTCARDS_IMPL) GetPostcardHistory()(*models_pkg.GetPostcardHistoryResponse,error)
```

#### Example Usage

```go

var result *models_pkg.GetPostcardHistoryResponse
result,_ = postcards.GetPostcardHistory()

```


### <a name="get_export_postcard_history"></a>![Method: ](https://apidocs.io/img/method.png ".postcards_pkg.GetExportPostcardHistory") GetExportPostcardHistory

> TODO: Add a method description


```go
func (me *POSTCARDS_IMPL) GetExportPostcardHistory(filename string)(*models_pkg.ExportPostcardHistoryResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | Filename for the export file. |


#### Example Usage

```go
filename := "myexport.csv"

var result *models_pkg.ExportPostcardHistoryResponse
result,_ = postcards.GetExportPostcardHistory(filename)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="referralaccounts_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".referralaccounts_pkg") referralaccounts_pkg

### Get instance

Factory for the ``` REFERRALACCOUNTS ``` interface can be accessed from the package referralaccounts_pkg.

```go
referralAccounts := referralaccounts_pkg.NewREFERRALACCOUNTS()
```

### <a name="get_list_of_referral_accounts"></a>![Method: ](https://apidocs.io/img/method.png ".referralaccounts_pkg.GetListOfReferralAccounts") GetListOfReferralAccounts

> TODO: Add a method description


```go
func (me *REFERRALACCOUNTS_IMPL) GetListOfReferralAccounts()(*models_pkg.GetListOfReferralAccountsResponse,error)
```

#### Example Usage

```go

var result *models_pkg.GetListOfReferralAccountsResponse
result,_ = referralAccounts.GetListOfReferralAccounts()

```


[Back to List of Controllers](#list_of_controllers)

## <a name="reseller_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".reseller_pkg") reseller_pkg

### Get instance

Factory for the ``` RESELLER ``` interface can be accessed from the package reseller_pkg.

```go
reseller := reseller_pkg.NewRESELLER()
```

### <a name="get_reseller_setting"></a>![Method: ](https://apidocs.io/img/method.png ".reseller_pkg.GetResellerSetting") GetResellerSetting

> Get reseller setting.


```go
func (me *RESELLER_IMPL) GetResellerSetting()(*models_pkg.GetResellerSettingResponse,error)
```

#### Example Usage

```go

var result *models_pkg.GetResellerSettingResponse
result,_ = reseller.GetResellerSetting()

```


### <a name="update_reseller_setting"></a>![Method: ](https://apidocs.io/img/method.png ".reseller_pkg.UpdateResellerSetting") UpdateResellerSetting

> Update a specific reseller setting.


```go
func (me *RESELLER_IMPL) UpdateResellerSetting(body *models_pkg.UpdateResellerSettingRequest)(*models_pkg.UpdateResellerSettingResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("    {        \"allow_public_signups\":1,        \"default_margin\":100,        \"default_margin_numbers\":150,        \"trial_balance\":50,        \"subdomain\":\"subdomain\",        \"colour_navigation\":\"#9999FF\",        \"logo_url_light\":\"http://url.com/light\",        \"logo_url_dark\":\"http://url.com/dark\",        \"company_name\":\"MyCompany\"    }")
var body *models_pkg.UpdateResellerSettingRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.UpdateResellerSettingResponse
result,_ = reseller.UpdateResellerSetting(body)

```


### <a name="get_reseller_by_subdomain"></a>![Method: ](https://apidocs.io/img/method.png ".reseller_pkg.GetResellerBySubdomain") GetResellerBySubdomain

> Get reseller setting by subdomin.


```go
func (me *RESELLER_IMPL) GetResellerBySubdomain(subdomain string)(*models_pkg.ResellerBySubdomainResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subdomain |  ``` Required ```  | Subdomain |


#### Example Usage

```go
subdomain := "mysubdomain"

var result *models_pkg.ResellerBySubdomainResponse
result,_ = reseller.GetResellerBySubdomain(subdomain)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="reselleraccounts_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".reselleraccounts_pkg") reselleraccounts_pkg

### Get instance

Factory for the ``` RESELLERACCOUNTS ``` interface can be accessed from the package reselleraccounts_pkg.

```go
resellerAccounts := reselleraccounts_pkg.NewRESELLERACCOUNTS()
```

### <a name="list_of_reseller_accounts"></a>![Method: ](https://apidocs.io/img/method.png ".reselleraccounts_pkg.ListOfResellerAccounts") ListOfResellerAccounts

> Get list of Reseller Accounts


```go
func (me *RESELLERACCOUNTS_IMPL) ListOfResellerAccounts()(*models_pkg.ListOfResellerAccountsResponse,error)
```

#### Example Usage

```go

var result *models_pkg.ListOfResellerAccountsResponse
result,_ = resellerAccounts.ListOfResellerAccounts()

```


### <a name="get_reseller_account"></a>![Method: ](https://apidocs.io/img/method.png ".reselleraccounts_pkg.GetResellerAccount") GetResellerAccount

> Get a specific reseller account.


```go
func (me *RESELLERACCOUNTS_IMPL) GetResellerAccount(clientUserId float64)(*models_pkg.GetResellerAccountResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| clientUserId |  ``` Required ```  | The client user id. |


#### Example Usage

```go
clientUserId := "24"

var result *models_pkg.GetResellerAccountResponse
result,_ = resellerAccounts.GetResellerAccount(clientUserId)

```


### <a name="create_reseller_account"></a>![Method: ](https://apidocs.io/img/method.png ".reselleraccounts_pkg.CreateResellerAccount") CreateResellerAccount

> TODO: Add a method description


```go
func (me *RESELLERACCOUNTS_IMPL) CreateResellerAccount(body *models_pkg.CreateResellerAccountRequest)(*models_pkg.CreateResellerAccountResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("    {        \"username\":\"johndoe2\",        \"user_email\":\"johndoe2@awesome.com\",        \"user_phone\":\"518-481-1002\",        \"user_first_name\":\"John\",        \"user_last_name\":\"Doe\",        \"country\":\"US\",        \"password\":\"pass\",        \"account_name\":\"The Awesome Company\"    }")
var body *models_pkg.CreateResellerAccountRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.CreateResellerAccountResponse
result,_ = resellerAccounts.CreateResellerAccount(body)

```


### <a name="create_reseller_account_public"></a>![Method: ](https://apidocs.io/img/method.png ".reselleraccounts_pkg.CreateResellerAccountPublic") CreateResellerAccountPublic

> TODO: Add a method description


```go
func (me *RESELLERACCOUNTS_IMPL) CreateResellerAccountPublic(body *models_pkg.CreateResellerAccountPublicRequest)(*models_pkg.CreateResellerAccountPublicResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("{    \"reseller_user_id\":1,    \"username\":\"john_awesome\",    \"user_email\":\"johnis@awesome.com\",    \"user_phone\":\"+61261063270\",    \"user_first_name\":\"John\",    \"user_last_name\":\"Awesome\",    \"country\":\"AU\",    \"password\":\"pass\",    \"account_name\":\"The Awesome Company\"}")
var body *models_pkg.CreateResellerAccountPublicRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.CreateResellerAccountPublicResponse
result,_ = resellerAccounts.CreateResellerAccountPublic(body)

```


### <a name="update_reseller_account"></a>![Method: ](https://apidocs.io/img/method.png ".reselleraccounts_pkg.UpdateResellerAccount") UpdateResellerAccount

> TODO: Add a method description


```go
func (me *RESELLERACCOUNTS_IMPL) UpdateResellerAccount(
            clientUserId float64,
            body *models_pkg.UpdateResellerAccountRequest)(*models_pkg.UpdateResellerAccountResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| clientUserId |  ``` Required ```  | Your client user id. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
clientUserId := "24"
bodyValue := []byte("    {        \"username\":\"johndoe2\",        \"user_email\":\"johndoe2@awesome.com\",        \"user_phone\":\"518-481-1002\",        \"user_first_name\":\"John\",        \"user_last_name\":\"Doe\",        \"country\":\"US\",        \"password\":\"pass\",        \"account_name\":\"The Awesome Company\"    }")
var body *models_pkg.UpdateResellerAccountRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.UpdateResellerAccountResponse
result,_ = resellerAccounts.UpdateResellerAccount(clientUserId, body)

```


### <a name="update_transfer_credit"></a>![Method: ](https://apidocs.io/img/method.png ".reselleraccounts_pkg.UpdateTransferCredit") UpdateTransferCredit

> TODO: Add a method description


```go
func (me *RESELLERACCOUNTS_IMPL) UpdateTransferCredit(body *models_pkg.TransferCreditRequest)(*models_pkg.TransferCreditResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
var body *models_pkg.TransferCreditRequest

var result *models_pkg.TransferCreditResponse
result,_ = resellerAccounts.UpdateTransferCredit(body)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="sdk_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".sdk_pkg") sdk_pkg

### Get instance

Factory for the ``` SDK ``` interface can be accessed from the package sdk_pkg.

```go
sDK := sdk_pkg.NewSDK()
```

### <a name="get_sdk_download"></a>![Method: ](https://apidocs.io/img/method.png ".sdk_pkg.GetSDKDownload") GetSDKDownload

> TODO: Add a method description


```go
func (me *SDK_IMPL) GetSDKDownload(mtype string)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mtype |  ``` Required ```  | Supported types. |


#### Example Usage

```go
mtype := "type"

var result interface{}
result,_ = sDK.GetSDKDownload(mtype)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="search_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".search_pkg") search_pkg

### Get instance

Factory for the ``` SEARCH ``` interface can be accessed from the package search_pkg.

```go
search := search_pkg.NewSEARCH()
```

### <a name="search_contacts_lists"></a>![Method: ](https://apidocs.io/img/method.png ".search_pkg.SearchContactsLists") SearchContactsLists

> TODO: Add a method description


```go
func (me *SEARCH_IMPL) SearchContactsLists(q string)(*models_pkg.SearchContactsListsResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| q |  ``` Required ```  | Your keyword or query. |


#### Example Usage

```go
q := "Gorne"

var result *models_pkg.SearchContactsListsResponse
result,_ = search.SearchContactsLists(q)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="sms_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".sms_pkg") sms_pkg

### Get instance

Factory for the ``` SMS ``` interface can be accessed from the package sms_pkg.

```go
sMS := sms_pkg.NewSMS()
```

### <a name="create_send_an_sms"></a>![Method: ](https://apidocs.io/img/method.png ".sms_pkg.CreateSendAnSMS") CreateSendAnSMS

> You can post **up to 1000 messages** with each API call.


```go
func (me *SMS_IMPL) CreateSendAnSMS(body *models_pkg.SendAnSMSRequest)(*models_pkg.SendAnSMSResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
var body *models_pkg.SendAnSMSRequest

var result *models_pkg.SendAnSMSResponse
result,_ = sMS.CreateSendAnSMS(body)

```


### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png ".sms_pkg.CreateCalculatePrice") CreateCalculatePrice

> TODO: Add a method description


```go
func (me *SMS_IMPL) CreateCalculatePrice(body *models_pkg.CalculatePriceRequest205)(*models_pkg.CalculatePriceResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
var body *models_pkg.CalculatePriceRequest205

var result *models_pkg.CalculatePriceResponse
result,_ = sMS.CreateCalculatePrice(body)

```


### <a name="get_all_history"></a>![Method: ](https://apidocs.io/img/method.png ".sms_pkg.GetAllHistory") GetAllHistory

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


```go
func (me *SMS_IMPL) GetAllHistory(
            dateFrom *int64,
            dateTo *int64)(*models_pkg.GetAllHistoryResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateFrom |  ``` Optional ```  | Timestamp (from) used to show records by date. |
| dateTo |  ``` Optional ```  | Timestamp (to) used to show recrods by date. |


#### Example Usage

```go
dateFrom,_ := strconv.ParseInt("1449459940", 10, 8)
dateTo,_ := strconv.ParseInt("1449659940", 10, 8)

var result *models_pkg.GetAllHistoryResponse
result,_ = sMS.GetAllHistory(dateFrom, dateTo)

```


### <a name="get_export_sms_history"></a>![Method: ](https://apidocs.io/img/method.png ".sms_pkg.GetExportSMSHistory") GetExportSMSHistory

> TODO: Add a method description


```go
func (me *SMS_IMPL) GetExportSMSHistory()(*models_pkg.ExportSMSHistoryResponse,error)
```

#### Example Usage

```go

var result *models_pkg.ExportSMSHistoryResponse
result,_ = sMS.GetExportSMSHistory()

```


### <a name="get_all_delivery_receipts"></a>![Method: ](https://apidocs.io/img/method.png ".sms_pkg.GetAllDeliveryReceipts") GetAllDeliveryReceipts

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


```go
func (me *SMS_IMPL) GetAllDeliveryReceipts()(*models_pkg.GetAllDeliveryReceiptsResponse,error)
```

#### Example Usage

```go

var result *models_pkg.GetAllDeliveryReceiptsResponse
result,_ = sMS.GetAllDeliveryReceipts()

```


### <a name="get_a_specific_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png ".sms_pkg.GetASpecificDeliveryReceipt") GetASpecificDeliveryReceipt

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


```go
func (me *SMS_IMPL) GetASpecificDeliveryReceipt(messageId string)(*models_pkg.GetASpecificDeliveryReceiptResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Your message id. |


#### Example Usage

```go
messageId := "88AB118E EB1B 478C 98CE 6C73ABA23F67"

var result *models_pkg.GetASpecificDeliveryReceiptResponse
result,_ = sMS.GetASpecificDeliveryReceipt(messageId)

```


### <a name="add_a_test_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png ".sms_pkg.AddATestDeliveryReceipt") AddATestDeliveryReceipt

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


```go
func (me *SMS_IMPL) AddATestDeliveryReceipt(body *models_pkg.AddATestDeliveryReceiptRequest)(*models_pkg.AddATestDeliveryReceiptResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("    {        \"url\":\"http://yourUrl.com\"    }")
var body *models_pkg.AddATestDeliveryReceiptRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.AddATestDeliveryReceiptResponse
result,_ = sMS.AddATestDeliveryReceipt(body)

```


### <a name="update_mark_delivery_receipts_as_read"></a>![Method: ](https://apidocs.io/img/method.png ".sms_pkg.UpdateMarkDeliveryReceiptsAsRead") UpdateMarkDeliveryReceiptsAsRead

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


```go
func (me *SMS_IMPL) UpdateMarkDeliveryReceiptsAsRead(body *models_pkg.MarkDeliveryReceiptsAsReadRequest)(*models_pkg.MarkDeliveryReceiptsAsReadResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("{    \"date_before\": 1441958441}")
var body *models_pkg.MarkDeliveryReceiptsAsReadRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.MarkDeliveryReceiptsAsReadResponse
result,_ = sMS.UpdateMarkDeliveryReceiptsAsRead(body)

```


### <a name="get_all_inbound_sms_pull"></a>![Method: ](https://apidocs.io/img/method.png ".sms_pkg.GetAllInboundSMSPull") GetAllInboundSMSPull

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


```go
func (me *SMS_IMPL) GetAllInboundSMSPull()(*models_pkg.GetAllInboundSMSPullResponse,error)
```

#### Example Usage

```go

var result *models_pkg.GetAllInboundSMSPullResponse
result,_ = sMS.GetAllInboundSMSPull()

```


### <a name="get_specific_inbound_pull"></a>![Method: ](https://apidocs.io/img/method.png ".sms_pkg.GetSpecificInboundPull") GetSpecificInboundPull

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


```go
func (me *SMS_IMPL) GetSpecificInboundPull(messageId string)(*models_pkg.GetSpecificInboundPullResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Message ID. Must be a valid GUID. |


#### Example Usage

```go
messageId := "5D420421-8715-4461-A9A2-C8F569E41835"

var result *models_pkg.GetSpecificInboundPullResponse
result,_ = sMS.GetSpecificInboundPull(messageId)

```


### <a name="add_a_test_inbound_sms"></a>![Method: ](https://apidocs.io/img/method.png ".sms_pkg.AddATestInboundSMS") AddATestInboundSMS

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


```go
func (me *SMS_IMPL) AddATestInboundSMS(body *models_pkg.AddATestInboundSMSRequest)(*models_pkg.AddATestInboundSMSResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("    {        \"url\":\"http://yourUrl.com\"    }")
var body *models_pkg.AddATestInboundSMSRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.AddATestInboundSMSResponse
result,_ = sMS.AddATestInboundSMS(body)

```


### <a name="update_mark_a_specific_inbound_sms_as_read"></a>![Method: ](https://apidocs.io/img/method.png ".sms_pkg.UpdateMarkASpecificInboundSMSAsRead") UpdateMarkASpecificInboundSMSAsRead

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


```go
func (me *SMS_IMPL) UpdateMarkASpecificInboundSMSAsRead(messageId string)(*models_pkg.MarkASpecificInboundSMSAsReadResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | B7CE432193CD-0753597B7293 (string, required) - The message ID you want to mark as read. |


#### Example Usage

```go
messageId := "307EF035"

var result *models_pkg.MarkASpecificInboundSMSAsReadResponse
result,_ = sMS.UpdateMarkASpecificInboundSMSAsRead(messageId)

```


### <a name="update_mark_all_inbound_sms_as_read"></a>![Method: ](https://apidocs.io/img/method.png ".sms_pkg.UpdateMarkAllInboundSMSAsRead") UpdateMarkAllInboundSMSAsRead

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


```go
func (me *SMS_IMPL) UpdateMarkAllInboundSMSAsRead(body *models_pkg.MarkAllInboundSMSAsReadRequest)(*models_pkg.MarkAllInboundSMSAsReadResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("    {        \"date_before\":1442398100    }")
var body *models_pkg.MarkAllInboundSMSAsReadRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.MarkAllInboundSMSAsReadResponse
result,_ = sMS.UpdateMarkAllInboundSMSAsRead(body)

```


### <a name="update_cancel_a_scheduled_message"></a>![Method: ](https://apidocs.io/img/method.png ".sms_pkg.UpdateCancelAScheduledMessage") UpdateCancelAScheduledMessage

> TODO: Add a method description


```go
func (me *SMS_IMPL) UpdateCancelAScheduledMessage(messageId string)(*models_pkg.CancelAScheduledMessageResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | B7CE432193CD-0753597B7293 (string, required) - The message ID you want to cancel. |


#### Example Usage

```go
messageId := "307EF035"

var result *models_pkg.CancelAScheduledMessageResponse
result,_ = sMS.UpdateCancelAScheduledMessage(messageId)

```


### <a name="update_cancel_all_scheduled_messages"></a>![Method: ](https://apidocs.io/img/method.png ".sms_pkg.UpdateCancelAllScheduledMessages") UpdateCancelAllScheduledMessages

> TODO: Add a method description


```go
func (me *SMS_IMPL) UpdateCancelAllScheduledMessages()(*models_pkg.CancelAllScheduledMessagesResponse,error)
```

#### Example Usage

```go

var result *models_pkg.CancelAllScheduledMessagesResponse
result,_ = sMS.UpdateCancelAllScheduledMessages()

```


[Back to List of Controllers](#list_of_controllers)

## <a name="smscampaigns_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".smscampaigns_pkg") smscampaigns_pkg

### Get instance

Factory for the ``` SMSCAMPAIGNS ``` interface can be accessed from the package smscampaigns_pkg.

```go
sMSCampaigns := smscampaigns_pkg.NewSMSCAMPAIGNS()
```

### <a name="create_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".smscampaigns_pkg.CreateSMSCampaign") CreateSMSCampaign

> You can post to a list with **up to 20000 recipients** with each API call.


```go
func (me *SMSCAMPAIGNS_IMPL) CreateSMSCampaign(body *models_pkg.CreateSMSCampaignRequest)(*models_pkg.CreateSMSCampaignResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("{    \"list_id\":428,    \"name\":\"My Campaign 1\",    \"from\":\"+61353787448\",    \"body\":\"This is my new campaign message.\",    \"schedule\":1444821615}")
var body *models_pkg.CreateSMSCampaignRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.CreateSMSCampaignResponse
result,_ = sMSCampaigns.CreateSMSCampaign(body)

```


### <a name="create_calculate_price_for_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".smscampaigns_pkg.CreateCalculatePriceForSMSCampaign") CreateCalculatePriceForSMSCampaign

> TODO: Add a method description


```go
func (me *SMSCAMPAIGNS_IMPL) CreateCalculatePriceForSMSCampaign(body *models_pkg.CalculatePriceForSMSCampaignRequest)(*models_pkg.CalculatePriceForSMSCampaignResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("{    \"list_id\":428,    \"name\":\"My Campaign 1\",    \"from\":\"+61353787448\",    \"body\":\"(First Name), this is your new campaign message.\"}")
var body *models_pkg.CalculatePriceForSMSCampaignRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.CalculatePriceForSMSCampaignResponse
result,_ = sMSCampaigns.CreateCalculatePriceForSMSCampaign(body)

```


### <a name="update_an_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".smscampaigns_pkg.UpdateAnSMSCampaign") UpdateAnSMSCampaign

> TODO: Add a method description


```go
func (me *SMSCAMPAIGNS_IMPL) UpdateAnSMSCampaign(
            smsCampaignId float64,
            body *models_pkg.UpdateAnSMSCampaignRequest)(*models_pkg.UpdateAnSMSCampaignResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| smsCampaignId |  ``` Required ```  | Your SMS Campaign id. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
smsCampaignId := "1"
bodyValue := []byte("{    \"list_id\":428,    \"name\":\"Awesome campaign.\",    \"from\":\"+61353787447\",    \"body\":\"his is an awesome message.\",    \"schedule\":1444821615}")
var body *models_pkg.UpdateAnSMSCampaignRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.UpdateAnSMSCampaignResponse
result,_ = sMSCampaigns.UpdateAnSMSCampaign(smsCampaignId, body)

```


### <a name="get_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".smscampaigns_pkg.GetSMSCampaign") GetSMSCampaign

> TODO: Add a method description


```go
func (me *SMSCAMPAIGNS_IMPL) GetSMSCampaign(smsCampaignId float64)(*models_pkg.GetSMSCampaignResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| smsCampaignId |  ``` Required ```  | Your SMS campaign id. |


#### Example Usage

```go
smsCampaignId := "1"

var result *models_pkg.GetSMSCampaignResponse
result,_ = sMSCampaigns.GetSMSCampaign(smsCampaignId)

```


### <a name="update_cancel_an_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".smscampaigns_pkg.UpdateCancelAnSMSCampaign") UpdateCancelAnSMSCampaign

> TODO: Add a method description


```go
func (me *SMSCAMPAIGNS_IMPL) UpdateCancelAnSMSCampaign(smsCampaignId float64)(*models_pkg.CancelAnSMSCampaignResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| smsCampaignId |  ``` Required ```  | Your SMS Campaign id. |


#### Example Usage

```go
smsCampaignId := "1"

var result *models_pkg.CancelAnSMSCampaignResponse
result,_ = sMSCampaigns.UpdateCancelAnSMSCampaign(smsCampaignId)

```


### <a name="get_list_of_sms_campaigns"></a>![Method: ](https://apidocs.io/img/method.png ".smscampaigns_pkg.GetListOfSMSCampaigns") GetListOfSMSCampaigns

> TODO: Add a method description


```go
func (me *SMSCAMPAIGNS_IMPL) GetListOfSMSCampaigns()(*models_pkg.GetListOfSMSCampaignsResponse,error)
```

#### Example Usage

```go

var result *models_pkg.GetListOfSMSCampaignsResponse
result,_ = sMSCampaigns.GetListOfSMSCampaigns()

```


[Back to List of Controllers](#list_of_controllers)

## <a name="smstemplates_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".smstemplates_pkg") smstemplates_pkg

### Get instance

Factory for the ``` SMSTEMPLATES ``` interface can be accessed from the package smstemplates_pkg.

```go
sMSTemplates := smstemplates_pkg.NewSMSTEMPLATES()
```

### <a name="list_of_templates"></a>![Method: ](https://apidocs.io/img/method.png ".smstemplates_pkg.ListOfTemplates") ListOfTemplates

> Get list of templates.


```go
func (me *SMSTEMPLATES_IMPL) ListOfTemplates()(*models_pkg.ListOfTemplatesResponse,error)
```

#### Example Usage

```go

var result *models_pkg.ListOfTemplatesResponse
result,_ = sMSTemplates.ListOfTemplates()

```


### <a name="create_a_template"></a>![Method: ](https://apidocs.io/img/method.png ".smstemplates_pkg.CreateATemplate") CreateATemplate

> Create new template.


```go
func (me *SMSTEMPLATES_IMPL) CreateATemplate(body *models_pkg.CreateATemplateRequest)(*models_pkg.CreateATemplateResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("    {        \"template_name\":\"Template 501916\",        \"body\":\"This is a sample content: H7YI68B3yk for this template.\"    }")
var body *models_pkg.CreateATemplateRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.CreateATemplateResponse
result,_ = sMSTemplates.CreateATemplate(body)

```


### <a name="update_a_template"></a>![Method: ](https://apidocs.io/img/method.png ".smstemplates_pkg.UpdateATemplate") UpdateATemplate

> TODO: Add a method description


```go
func (me *SMSTEMPLATES_IMPL) UpdateATemplate(
            templateId string,
            body *models_pkg.UpdateATemplateRequest)(*models_pkg.UpdateATemplateResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
templateId := "25"
bodyValue := []byte("    {        \"template_name\":\"I am updated\",        \"body\":\"This is a sample content: Sc0KNWgSMG for this template.\"    }")
var body *models_pkg.UpdateATemplateRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.UpdateATemplateResponse
result,_ = sMSTemplates.UpdateATemplate(templateId, body)

```


### <a name="delete_a_template"></a>![Method: ](https://apidocs.io/img/method.png ".smstemplates_pkg.DeleteATemplate") DeleteATemplate

> TODO: Add a method description


```go
func (me *SMSTEMPLATES_IMPL) DeleteATemplate(templateId string)(*models_pkg.DeleteATemplateResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |


#### Example Usage

```go
templateId := "25"

var result *models_pkg.DeleteATemplateResponse
result,_ = sMSTemplates.DeleteATemplate(templateId)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="statistics_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".statistics_pkg") statistics_pkg

### Get instance

Factory for the ``` STATISTICS ``` interface can be accessed from the package statistics_pkg.

```go
statistics := statistics_pkg.NewSTATISTICS()
```

### <a name="get_sms_statistics"></a>![Method: ](https://apidocs.io/img/method.png ".statistics_pkg.GetSMSStatistics") GetSMSStatistics

> TODO: Add a method description


```go
func (me *STATISTICS_IMPL) GetSMSStatistics()(*models_pkg.GetSMSStatisticsResponse,error)
```

#### Example Usage

```go

var result *models_pkg.GetSMSStatisticsResponse
result,_ = statistics.GetSMSStatistics()

```


### <a name="get_voice_statistics"></a>![Method: ](https://apidocs.io/img/method.png ".statistics_pkg.GetVoiceStatistics") GetVoiceStatistics

> TODO: Add a method description


```go
func (me *STATISTICS_IMPL) GetVoiceStatistics()(*models_pkg.GetVoiceStatisticsResponse,error)
```

#### Example Usage

```go

var result *models_pkg.GetVoiceStatisticsResponse
result,_ = statistics.GetVoiceStatistics()

```


[Back to List of Controllers](#list_of_controllers)

## <a name="subaccounts_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".subaccounts_pkg") subaccounts_pkg

### Get instance

Factory for the ``` SUBACCOUNTS ``` interface can be accessed from the package subaccounts_pkg.

```go
subaccounts := subaccounts_pkg.NewSUBACCOUNTS()
```

### <a name="get_all_subaccounts"></a>![Method: ](https://apidocs.io/img/method.png ".subaccounts_pkg.GetAllSubaccounts") GetAllSubaccounts

> TODO: Add a method description


```go
func (me *SUBACCOUNTS_IMPL) GetAllSubaccounts()(*models_pkg.GetAllSubaccountsResponse,error)
```

#### Example Usage

```go

var result *models_pkg.GetAllSubaccountsResponse
result,_ = subaccounts.GetAllSubaccounts()

```


### <a name="create_a_new_subaccount"></a>![Method: ](https://apidocs.io/img/method.png ".subaccounts_pkg.CreateANewSubaccount") CreateANewSubaccount

> TODO: Add a method description


```go
func (me *SUBACCOUNTS_IMPL) CreateANewSubaccount(body *models_pkg.CreateANewSubaccountRequest)(*models_pkg.CreateANewSubaccountResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("    {        \"api_username\":\"nameP99\",        \"password\":\"pass\",        \"email\":\"testvrq@gmail.com\",        \"phone_number\":\"941-751-3278\",        \"first_name\":\"FirstnameeGPqV\",        \"last_name\":\"LastnamePvjJp\"    }")
var body *models_pkg.CreateANewSubaccountRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.CreateANewSubaccountResponse
result,_ = subaccounts.CreateANewSubaccount(body)

```


### <a name="get_a_specific_subaccount"></a>![Method: ](https://apidocs.io/img/method.png ".subaccounts_pkg.GetASpecificSubaccount") GetASpecificSubaccount

> TODO: Add a method description


```go
func (me *SUBACCOUNTS_IMPL) GetASpecificSubaccount(subaccountId float64)(*models_pkg.GetASpecificSubaccountResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |


#### Example Usage

```go
subaccountId := "59"

var result *models_pkg.GetASpecificSubaccountResponse
result,_ = subaccounts.GetASpecificSubaccount(subaccountId)

```


### <a name="update_a_specific_subaccount"></a>![Method: ](https://apidocs.io/img/method.png ".subaccounts_pkg.UpdateASpecificSubaccount") UpdateASpecificSubaccount

> TODO: Add a method description


```go
func (me *SUBACCOUNTS_IMPL) UpdateASpecificSubaccount(
            subaccountId float64,
            body *models_pkg.UpdateASpecificSubaccountRequest)(*models_pkg.UpdateASpecificSubaccountResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
subaccountId := "59"
bodyValue := []byte("    {        \"password\":\"pass\",        \"email\":\"testfP0.updated@gmail.com\",        \"phone_number\":\"+19417519130\",        \"first_name\":\"FirstnameKvdRZUpdated\",        \"last_name\":\"LastnameHUPYGUpdated\",        \"access_users\": 1,        \"access_billing\": 1,        \"access_reporting\": 1,        \"access_contacts\": 1,        \"access_settings\": 1,        \"access_sms\": 1,        \"access_email\": 1,        \"access_voice\": 1,        \"access_fax\": 1,        \"access_post\": 1,        \"access_reseller\": 1,        \"access_mms\": 1,        \"share_campaigns\": 0,        \"notes\": null    }")
var body *models_pkg.UpdateASpecificSubaccountRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.UpdateASpecificSubaccountResponse
result,_ = subaccounts.UpdateASpecificSubaccount(subaccountId, body)

```


### <a name="delete_a_specific_subaccount"></a>![Method: ](https://apidocs.io/img/method.png ".subaccounts_pkg.DeleteASpecificSubaccount") DeleteASpecificSubaccount

> TODO: Add a method description


```go
func (me *SUBACCOUNTS_IMPL) DeleteASpecificSubaccount(subaccountId float64)(*models_pkg.DeleteASpecificSubaccountResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |


#### Example Usage

```go
subaccountId := "59"

var result *models_pkg.DeleteASpecificSubaccountResponse
result,_ = subaccounts.DeleteASpecificSubaccount(subaccountId)

```


### <a name="update_regenerate_api_key"></a>![Method: ](https://apidocs.io/img/method.png ".subaccounts_pkg.UpdateRegenerateAPIKey") UpdateRegenerateAPIKey

> TODO: Add a method description


```go
func (me *SUBACCOUNTS_IMPL) UpdateRegenerateAPIKey(subaccountId float64)(*models_pkg.RegenerateAPIKeyResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |


#### Example Usage

```go
subaccountId := "59"

var result *models_pkg.RegenerateAPIKeyResponse
result,_ = subaccounts.UpdateRegenerateAPIKey(subaccountId)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="timezones_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".timezones_pkg") timezones_pkg

### Get instance

Factory for the ``` TIMEZONES ``` interface can be accessed from the package timezones_pkg.

```go
timezones := timezones_pkg.NewTIMEZONES()
```

### <a name="get_timezones"></a>![Method: ](https://apidocs.io/img/method.png ".timezones_pkg.GetTimezones") GetTimezones

> Get supported list of timezones.


```go
func (me *TIMEZONES_IMPL) GetTimezones()(*models_pkg.GetTimezonesResponse,error)
```

#### Example Usage

```go

var result *models_pkg.GetTimezonesResponse
result,_ = timezones.GetTimezones()

```


[Back to List of Controllers](#list_of_controllers)

## <a name="transactionalemail_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".transactionalemail_pkg") transactionalemail_pkg

### Get instance

Factory for the ``` TRANSACTIONALEMAIL ``` interface can be accessed from the package transactionalemail_pkg.

```go
transactionalEmail := transactionalemail_pkg.NewTRANSACTIONALEMAIL()
```

### <a name="create_email_send"></a>![Method: ](https://apidocs.io/img/method.png ".transactionalemail_pkg.CreateEmailSend") CreateEmailSend

> TODO: Add a method description


```go
func (me *TRANSACTIONALEMAIL_IMPL) CreateEmailSend(body *models_pkg.EmailSendRequest)(*models_pkg.EmailSendResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
var body *models_pkg.EmailSendRequest

var result *models_pkg.EmailSendResponse
result,_ = transactionalEmail.CreateEmailSend(body)

```


### <a name="create_email_price"></a>![Method: ](https://apidocs.io/img/method.png ".transactionalemail_pkg.CreateEmailPrice") CreateEmailPrice

> TODO: Add a method description


```go
func (me *TRANSACTIONALEMAIL_IMPL) CreateEmailPrice(body *models_pkg.EmailPriceRequest)(*models_pkg.EmailPriceResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
var body *models_pkg.EmailPriceRequest

var result *models_pkg.EmailPriceResponse
result,_ = transactionalEmail.CreateEmailPrice(body)

```


### <a name="get_email_history"></a>![Method: ](https://apidocs.io/img/method.png ".transactionalemail_pkg.GetEmailHistory") GetEmailHistory

> TODO: Add a method description


```go
func (me *TRANSACTIONALEMAIL_IMPL) GetEmailHistory()(*models_pkg.EmailHistoryResponse,error)
```

#### Example Usage

```go

var result *models_pkg.EmailHistoryResponse
result,_ = transactionalEmail.GetEmailHistory()

```


### <a name="get_export_history"></a>![Method: ](https://apidocs.io/img/method.png ".transactionalemail_pkg.GetExportHistory") GetExportHistory

> TODO: Add a method description


```go
func (me *TRANSACTIONALEMAIL_IMPL) GetExportHistory(filename string)(*models_pkg.ExportHistoryResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | File name for the export file. |


#### Example Usage

```go
filename := "myexport.csv"

var result *models_pkg.ExportHistoryResponse
result,_ = transactionalEmail.GetExportHistory(filename)

```


### <a name="add_a_test_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png ".transactionalemail_pkg.AddATestDeliveryReceipt") AddATestDeliveryReceipt

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


```go
func (me *TRANSACTIONALEMAIL_IMPL) AddATestDeliveryReceipt(body *models_pkg.AddATestDeliveryReceiptRequest)(*models_pkg.AddATestDeliveryReceiptResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("    {        \"url\":\"http://yourUrl.com\"    }")
var body *models_pkg.AddATestDeliveryReceiptRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.AddATestDeliveryReceiptResponse
result,_ = transactionalEmail.AddATestDeliveryReceipt(body)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="uploads_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".uploads_pkg") uploads_pkg

### Get instance

Factory for the ``` UPLOADS ``` interface can be accessed from the package uploads_pkg.

```go
uploads := uploads_pkg.NewUPLOADS()
```

### <a name="upload_a_file"></a>![Method: ](https://apidocs.io/img/method.png ".uploads_pkg.UploadAFile") UploadAFile

> The `upload` endpoint provides a method for converting files from an unspported format to a format that one of our endpoints can handle.
> Files can be submitted two ways:
> 1. Using `base64` encoding in an `application/json` request. In this case, submit the `base64`-encoded file contents in the `content` field of the request body, and `convert` can be specified either also in the body or as part of the query string.
> 2. Using `multipart/form-data` encoding, in the same way it would be submitted using a HTML form. You may find cURL useful for this. For an example of how to do this, see one of our [SDKs](https://dashboard.clicksend.com/#/libraries-sdk/main). In this case, specify `convert` in the query string.
> Note that `convert` specifies the conversion to take place - that is, what the result should be compatible with - and can be any of `fax`, `mms`, `csv` or `post`.
> All files have 10 minutes expiry.


```go
func (me *UPLOADS_IMPL) UploadAFile(
            body *models_pkg.UploadAFileRequest,
            convert *string)(*models_pkg.UploadAFileResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |
| convert |  ``` Optional ```  | TODO: Add a parameter description |


#### Example Usage

```go
var body *models_pkg.UploadAFileRequest
convert := "convert"

var result *models_pkg.UploadAFileResponse
result,_ = uploads.UploadAFile(body, convert)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="voice_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".voice_pkg") voice_pkg

### Get instance

Factory for the ``` VOICE ``` interface can be accessed from the package voice_pkg.

```go
voice := voice_pkg.NewVOICE()
```

### <a name="create_send_a_voice_call"></a>![Method: ](https://apidocs.io/img/method.png ".voice_pkg.CreateSendAVoiceCall") CreateSendAVoiceCall

> You can post **up to 1000 messages** with each API call.


```go
func (me *VOICE_IMPL) CreateSendAVoiceCall(body *models_pkg.SendAVoiceCallRequest)(*models_pkg.SendAVoiceCallResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
var body *models_pkg.SendAVoiceCallRequest

var result *models_pkg.SendAVoiceCallResponse
result,_ = voice.CreateSendAVoiceCall(body)

```


### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png ".voice_pkg.CreateCalculatePrice") CreateCalculatePrice

> TODO: Add a method description


```go
func (me *VOICE_IMPL) CreateCalculatePrice(body *models_pkg.CalculatePriceRequest263)(*models_pkg.CalculatePriceResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
var body *models_pkg.CalculatePriceRequest263

var result *models_pkg.CalculatePriceResponse
result,_ = voice.CreateCalculatePrice(body)

```


### <a name="get_voice_languages"></a>![Method: ](https://apidocs.io/img/method.png ".voice_pkg.GetVoiceLanguages") GetVoiceLanguages

> TODO: Add a method description


```go
func (me *VOICE_IMPL) GetVoiceLanguages()(*models_pkg.VoiceLanguagesResponse,error)
```

#### Example Usage

```go

var result *models_pkg.VoiceLanguagesResponse
result,_ = voice.GetVoiceLanguages()

```


### <a name="get_voice_history"></a>![Method: ](https://apidocs.io/img/method.png ".voice_pkg.GetVoiceHistory") GetVoiceHistory

> TODO: Add a method description


```go
func (me *VOICE_IMPL) GetVoiceHistory(
            dateFrom *int64,
            dateTo *int64)(*models_pkg.GetVoiceHistoryResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateFrom |  ``` Optional ```  | Timestamp (from) used to show records by date. |
| dateTo |  ``` Optional ```  | Timestamp (to) used to show recrods by date. |


#### Example Usage

```go
dateFrom,_ := strconv.ParseInt("1443501617", 10, 8)
dateTo,_ := strconv.ParseInt("1443501727", 10, 8)

var result *models_pkg.GetVoiceHistoryResponse
result,_ = voice.GetVoiceHistory(dateFrom, dateTo)

```


### <a name="get_export_voice_history"></a>![Method: ](https://apidocs.io/img/method.png ".voice_pkg.GetExportVoiceHistory") GetExportVoiceHistory

> TODO: Add a method description


```go
func (me *VOICE_IMPL) GetExportVoiceHistory()(*models_pkg.ExportVoiceHistoryResponse,error)
```

#### Example Usage

```go

var result *models_pkg.ExportVoiceHistoryResponse
result,_ = voice.GetExportVoiceHistory()

```


### <a name="get_voice_receipts"></a>![Method: ](https://apidocs.io/img/method.png ".voice_pkg.GetVoiceReceipts") GetVoiceReceipts

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


```go
func (me *VOICE_IMPL) GetVoiceReceipts()(*models_pkg.GetVoiceReceiptsResponse,error)
```

#### Example Usage

```go

var result *models_pkg.GetVoiceReceiptsResponse
result,_ = voice.GetVoiceReceipts()

```


### <a name="add_a_test_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png ".voice_pkg.AddATestDeliveryReceipt") AddATestDeliveryReceipt

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


```go
func (me *VOICE_IMPL) AddATestDeliveryReceipt(body *models_pkg.AddATestDeliveryReceiptRequest)(*models_pkg.AddATestDeliveryReceiptResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
bodyValue := []byte("    {        \"url\":\"http://yourUrl.com\"    }")
var body *models_pkg.AddATestDeliveryReceiptRequest
json.Unmarshal(bodyValue,&body)

var result *models_pkg.AddATestDeliveryReceiptResponse
result,_ = voice.AddATestDeliveryReceipt(body)

```


### <a name="get_specific_voice_receipt"></a>![Method: ](https://apidocs.io/img/method.png ".voice_pkg.GetSpecificVoiceReceipt") GetSpecificVoiceReceipt

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


```go
func (me *VOICE_IMPL) GetSpecificVoiceReceipt(messageId string)(*models_pkg.GetSpecificVoiceReceiptResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | 3055-45F1-9B79-F2C43509FD16 (string, required) - The voice receipt message id. |


#### Example Usage

```go
messageId := "28DD2718"

var result *models_pkg.GetSpecificVoiceReceiptResponse
result,_ = voice.GetSpecificVoiceReceipt(messageId)

```


### <a name="update_marked_voice_receipts_as_read"></a>![Method: ](https://apidocs.io/img/method.png ".voice_pkg.UpdateMarkedVoiceReceiptsAsRead") UpdateMarkedVoiceReceiptsAsRead

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


```go
func (me *VOICE_IMPL) UpdateMarkedVoiceReceiptsAsRead(dateBefore float64)(*models_pkg.MarkedVoiceReceiptsAsReadResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateBefore |  ``` Required ```  | An optional timestamp - mark all as read before this timestamp. If not given, all receipts will be marked as read. |


#### Example Usage

```go
dateBefore := 49.4671964014262

var result *models_pkg.MarkedVoiceReceiptsAsReadResponse
result,_ = voice.UpdateMarkedVoiceReceiptsAsRead(dateBefore)

```


### <a name="update_cancel_a_specific_voice_call"></a>![Method: ](https://apidocs.io/img/method.png ".voice_pkg.UpdateCancelASpecificVoiceCall") UpdateCancelASpecificVoiceCall

> TODO: Add a method description


```go
func (me *VOICE_IMPL) UpdateCancelASpecificVoiceCall(messageId string)(*models_pkg.CancelASpecificVoiceCallResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Your voice message id. |


#### Example Usage

```go
messageId := "7B5BFC19 06B7 49C1 8DCDFB011600E12B"

var result *models_pkg.CancelASpecificVoiceCallResponse
result,_ = voice.UpdateCancelASpecificVoiceCall(messageId)

```


### <a name="update_cancel_all_voice_calls"></a>![Method: ](https://apidocs.io/img/method.png ".voice_pkg.UpdateCancelAllVoiceCalls") UpdateCancelAllVoiceCalls

> TODO: Add a method description


```go
func (me *VOICE_IMPL) UpdateCancelAllVoiceCalls()(*models_pkg.CancelAllVoiceCallsResponse,error)
```

#### Example Usage

```go

var result *models_pkg.CancelAllVoiceCallsResponse
result,_ = voice.UpdateCancelAllVoiceCalls()

```


[Back to List of Controllers](#list_of_controllers)



