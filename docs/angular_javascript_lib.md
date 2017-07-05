# Getting started

TODO: Add a description

## How to Build

The generated SDK requires AngularJS framework to work. If you do not already have angular downloaded, please go ahead and do it from [here](https://angularjs.org/).
If any of your models have `Date` or `Datetime` type fields or your endpoints have `Date`/`Datetime` type response, you will need to download and link [angular-moment](https://cdnjs.cloudflare.com/ajax/libs/angular-moment/1.0.1/angular-moment.min.js) and [moment.js](https://cdnjs.cloudflare.com/ajax/libs/moment.js/2.17.1/moment.min.js) with your project.

## How to Use

The following section describes how to use the generated SDK in an existing/new project.

### 1. Configure Angular and Generated SDK
Perform the following steps to configure angular and the SDK:
+ Make a `scripts` folder inside the root folder of the project. If you already have a `scripts` folder, skip to the next step.
+ Move the `angular.min.js` file inside the scripts folder. 
+ Move the `clicksendrestapiv3lib` folder inside the scripts folder.
+ If any of the Custom Types in your API have `Date`/`Datetime` type fields or any endpoint has `Date`/`Datetime` response, you will need to download angular-moment and moment.js. Move these 2 files into the `scripts` folder as well.

![folder-structure-image](https://apidocs.io/illustration/angularjs?step=folderStructure&workspaceFolder=ClickSend%20REST%20API%20v3-Angular&projectName=ClickSendRESTAPIV3Lib)

### 2. Open Project Folder
Open an IDE/Text Editor for JavaScript like Sublime Text. The basic workflow presented here is also applicable if you prefer using a different editor or IDE.  
Click on `File` and select `Open Folder`

Select the folder of your SDK and click on `Select Folder` to open it up in Sublime Text. The folder will become visible in the bar on the left.

![open-folder-image](https://apidocs.io/illustration/angularjs?step=openFolder&workspaceFolder=ClickSend%20REST%20API%20v3-Angular)

### 3. Create an Angular Application
Since Angular JS is used for client-side web development, in order to use the generated library, you will have to develop an application first.
If you already have an angular application, [skip to Step 6](#6-include-sdk-references-in-html-file). Otherwise, follow these steps to create one:

+ In the IDE, click on `File` and choose `New File` to create a new file.
+ Add the following starting code in the file:
```js
    var app = angular.module('myApp', []);
    app.controller('testController', function($scope) 
    {

    });
```
+ Save it with the name `app.js` in the `scripts` folder.


### 4. Create HTML File
Skip to the next step if you are working with an existing project and already have an html file. Otherwise follow the steps to create one:
+ Inside the IDE, right click on the project folder name and select the `New File` option to create a new test file.
+ Save it with an appropriate name such as `index.html` in the root of your project folder.
`index.html` should look like this:
```html
	<!DOCTYPE html>
	<html>
	<head>
		<title>Angular Project</title>
		<script></script>
	</head>

	<body>
	</body>

	</html>
```

![initial-html-code-image](https://apidocs.io/illustration/angularjs?step=initialCode&workspaceFolder=ClickSend%20REST%20API%20v3-Angular)

### 5. Including links to Angular in HTML file
Your HTML file needs to have a link to `angular.min.js` file to use Angular-JS. Add the link using `script` tags inside the `head` section of `index.html` like:
```html
	<script src="scripts/angular.min.js" ></script>
```
If any of the Custom Types that you have defined have `Date`/`Datetime` type fields or any endpoint has `Date`/`Datetime` response, you will also need to link to angular-moment and moment.js like:
```html
	<script src="scripts/angular.min.js" ></script>
	<script src="scripts/moment.min.js" ></script>
	<script src="scripts/angular-moment.min.js" ></script>
```

### 6. Include SDK references in HTML file
Import the reference to the generated SDK files inside your html file like:
```html
	<head>
		...
		<!-- Helper files -->
		<script src="scripts/clicksendrestapiv3lib/Module.js"></script>
		<script src="scripts/clicksendrestapiv3lib/Configuration.js"></script>
		<script src="scripts/clicksendrestapiv3lib/ModelFactory.js"></script>
		<script src="scripts/clicksendrestapiv3lib/ObjectMapper.js"></script>
		<script src="scripts/clicksendrestapiv3lib/APIHelper.js"></script>
		<script src="scripts/clicksendrestapiv3lib/Http/Client/HttpContext.js"></script>
		<script src="scripts/clicksendrestapiv3lib/Http/Client/RequestClient.js"></script>
		<script src="scripts/clicksendrestapiv3lib/Http/Request/HttpRequest.js"></script>
		<script src="scripts/clicksendrestapiv3lib/Http/Response/HttpResponse.js"></script>

		<!-- API Controllers -->
        <script src="scripts/clicksendrestapiv3lib/Controllers/BaseController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/AccountController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/AccountRechargeController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/AutomationRulesController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/ContactListsController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/ContactSuggestionsController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/ContactsController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/CountriesController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/DeliveryIssuesController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/EmailMarketingController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/EmailToSMSAllowedAddressController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/EmailToSMSStrippedStringsController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/FaxController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/ForgotAccountController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/MMSController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/NumbersController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/PricingController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/PostDirectMailController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/PostLetterController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/PostcardsController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/ReferralAccountsController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/ResellerController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/ResellerAccountsController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/SDKController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/SearchController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/SMSController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/SMSCampaignsController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/SMSTemplatesController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/StatisticsController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/SubaccountsController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/TimezonesController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/TransactionalEmailController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/UploadsController.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Controllers/VoiceController.js"></script>


		<!-- Models -->
        <script src="scripts/clicksendrestapiv3lib/Models/BaseModel.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/AddATestInboundSMSRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/ForgotPasswordRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/AddATestDeliveryReceiptRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateStrippedStringRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateStrippedStringRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/ShowCSVImportFilePreviewRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/RemoveDuplicateContactsRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateASpecificContactListRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateANewContactListRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetAccountResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateANewAccountRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateANewAccountResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateAccountRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateAccountResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/AccountUsageResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/SendAccountActivationTokenRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/SendAccountActivationTokenResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/VerifyNewAccountResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetCreditCardInfoResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateCreditCardInfoRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateCreditCardInfoResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/ListOfPackagesResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/PurchaseAPackageResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetTransactionsResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/ListRulesResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetASpecificRuleResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateANewRuleRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateANewRuleResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateARuleRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateARuleResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/DeleteARuleResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateANewRuleRequest24.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateARuleRequest26.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateANewRuleRequest38.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateARuleRequest40.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/DeleteARuleResponse49.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/DeleteARuleResponse56.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetAllContactListsResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateANewContactListResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetASpecificContactListResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateASpecificContactListResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/DeleteASpecificContactListResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/ImportContactsToListRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/ImportContactsToListResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/RemoveDuplicateContactsResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetListOfAcceptableImportFieldsResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/ShowCSVImportFilePreviewResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/ListContactSuggestionsResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetAllContactsInAListResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateANewContactRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateANewContactResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetASpecificContactResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateASpecificContactRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateASpecificContactResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/DeleteASpecificContactResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/RemoveOptedOutContactsResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/TransferAContactResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetAllCountriesResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetDeliveryIssuesResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateDeliveryIssueRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateDeliveryIssueResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetAllAllowedEmailAddressesResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateAllowedEmailAddressRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateAllowedEmailAddressResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/SendVerificationTokenResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/VerifyAllowedEmailAddressResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/DeleteAllowedEmailAddressResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetSpecificAllowedEmailAddressResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetAllEmailCampaignsResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetSpecificEmailCampaignResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateEmailCampaignRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateEmailCampaignResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateEmailCampaignRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateEmailCampaignResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CancelEmailCampaignResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CalculatePriceRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CalculatePriceResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetSpecificEmailCampaignHistoryResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetAllEmailTemplatesResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetSpecificEmailTemplateResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateNewEmailTemplateFromMasterTemplateRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateNewEmailTemplateFromMasterTemplateResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateAnEmailTemplateRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateAnEmailTemplateResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/DeleteEmailTemplateResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetAllMasterEmailTemplatesResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetSpecificMasterTemplateResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetAllMasterTemplateCategoriesResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetSpecificEmailTemplateCategoryResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetAllTemplatesForCategoryResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UploadImageToSpecificTemplateRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UploadImageToSpecificTemplateResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/ListOfEmailToSMSAllowedAddressResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateEmailToSMSAllowedAddressRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateEmailToSMSAllowedAddressResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetSpecificEmailToSMSAllowedAddressResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateEmailToSMSAllowedAddressRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateEmailToSMSAllowedAddressResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/DeleteEmailToSMSAllowedAddressResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/ListStrippedStringsResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/FindSpecificStrippedStringResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateStrippedStringResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateStrippedStringResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/DeleteStrippedStringResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/SendFaxRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/SendFaxResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CalculatePriceRequest132.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetFaxHistoryResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/ListOfFaxDeliveryReceiptsResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetASpecificFaxDeliveryReceiptResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/MarkFaxDeliveryReceiptsAsReadRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/MarkFaxDeliveryReceiptsAsReadResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/AddATestDeliveryReceiptResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/ForgotUsernameRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/ForgotUsernameResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/ForgotPasswordResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/VerifyForgotPasswordRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/VerifyForgotPasswordResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/SendMMSRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/SendMMSResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetPriceRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetPriceResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetMMSHistoryResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/ExportMMSHistoryResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CancelMMSResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CancelAllMMSResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetAllDeliveryReceiptsResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetDeliveryReceiptResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/MarkReceiptsAsReadResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetAllDedicatedNumbersResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/BuyDedicatedNumberResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/SearchDedicatedNumbersByCountryResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetCountryPricingResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/SearchLocationsResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateNewCampaignRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateNewCampaignResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CalculateDirectMailCampaignPriceRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CalculateDirectMailCampaignPriceResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/ListDirectMailCampaignsResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/SendPostLetterRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/SendPostLetterResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CalculatePriceRequest170.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetPostLetterHistoryResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/ExportPostLetterHistoryResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateAPostReturnAddressRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateAPostReturnAddressResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetListOfPostReturnAddressesResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetPostReturnAddressResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdatePostReturnAddressRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdatePostReturnAddressResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/DeletePostReturnAddressResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/SendPostcardRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/SendPostcardResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CalculatePricingRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CalculatePricingResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetPostcardHistoryResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/ExportPostcardHistoryResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetListOfReferralAccountsResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetResellerSettingResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateResellerSettingRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateResellerSettingResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/ResellerBySubdomainResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/ListOfResellerAccountsResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetResellerAccountResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateResellerAccountRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateResellerAccountResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateResellerAccountPublicRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateResellerAccountPublicResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateResellerAccountRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateResellerAccountResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/TransferCreditRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/TransferCreditResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/SearchContactsListsResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/SendAnSMSRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/SendAnSMSResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CalculatePriceRequest205.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetAllHistoryResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/ExportSMSHistoryResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetASpecificDeliveryReceiptResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/MarkDeliveryReceiptsAsReadRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/MarkDeliveryReceiptsAsReadResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetAllInboundSMSPullResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetSpecificInboundPullResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/AddATestInboundSMSResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/MarkASpecificInboundSMSAsReadResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/MarkAllInboundSMSAsReadRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/MarkAllInboundSMSAsReadResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CancelAScheduledMessageResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CancelAllScheduledMessagesResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateSMSCampaignRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateSMSCampaignResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CalculatePriceForSMSCampaignRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CalculatePriceForSMSCampaignResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateAnSMSCampaignRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateAnSMSCampaignResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetSMSCampaignResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CancelAnSMSCampaignResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetListOfSMSCampaignsResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/ListOfTemplatesResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateATemplateRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateATemplateResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateATemplateRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateATemplateResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/DeleteATemplateResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetSMSStatisticsResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetVoiceStatisticsResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetAllSubaccountsResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateANewSubaccountRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CreateANewSubaccountResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetASpecificSubaccountResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateASpecificSubaccountRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UpdateASpecificSubaccountResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/DeleteASpecificSubaccountResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/RegenerateAPIKeyResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetTimezonesResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/EmailSendRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/EmailSendResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/EmailPriceRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/EmailPriceResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/EmailHistoryResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/ExportHistoryResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UploadAFileRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UploadAFileResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/UploadAFileRequest260.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/SendAVoiceCallRequest.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/SendAVoiceCallResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CalculatePriceRequest263.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/VoiceLanguagesResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetVoiceHistoryResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/ExportVoiceHistoryResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetVoiceReceiptsResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/GetSpecificVoiceReceiptResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/MarkedVoiceReceiptsAsReadResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CancelASpecificVoiceCallResponse.js"></script>
        <script src="scripts/clicksendrestapiv3lib/Models/CancelAllVoiceCallsResponse.js"></script>

		...
	</head>
```
> The `Module.js` file should be imported before the other files. After `Module.js`, `Configuration.js` should be imported.
> The `ModelFactory.js` file is needed by `ObjectMapper.js` file. The `ObjectMapper` in turn, is needed by `BaseController.js`.

### 7. Including link to `app.js` in HTML file
Link your `app.js` file to your `index.html` file like:
```html
	<head>
		...
		<script src="scripts/app.js"></script>
	</head>
```
> The link to app.js needs to be included at the very end of the head tag, after the SDK references have been added

### 8. Initializing the Angular App
You need to initialize your app and the controller associated with your view inside your `index.html` file. Do so like:
+ Add ng-app directive to initialize your app inside the `body` tag.
```html
	<body ng-app="myApp">
```
+ Add ng-controller directive to initialize your controller and bind it with your view (`index.html` file).
```html
	...
	<body ng-app="myApp">
		<div ng-controller="testController">
			...
		</div>
		...
	</body>
	...
```

### 9. Consuming the SDK 
In order to use the generated SDK's modules, controllers and factories, the project needs to be added as a dependency in your angular app's module. This will be done inside the `app.js` file.
Add the dependency like this:

```js
    var app = angular.module('myApp', ['ClickSendRESTAPIV3Lib']);
```
At this point, the SDK has been successfully included in your project. Further steps include using a service/factory from the generated SDK. To see working example of this, please head on [over here](#list-of-controllers) and choose any class to see its functions and example usage.  

### 10. Running The App
To run the app, simply open up the `index.html` file in a browser.

![app-running](https://apidocs.io/illustration/angularjs?step=appRunning)

## Initialization

### Authentication
In order to setup authentication and initialization of the Angular App, you need the following information.

| Parameter | Description |
|-----------|-------------|
| basicAuthUserName | The username to use with basic authentication |
| basicAuthPassword | The password to use with basic authentication |



```JavaScript
// Configuration parameters and credentials
basicAuthUserName = "basicAuthUserName"; // The username to use with basic authentication
basicAuthPassword = "basicAuthPassword"; // The password to use with basic authentication

```
The Angular App can be initialized as following:
```html
<body ng-app="myApp">
    <div ng-controller="testController">
        ...
    </div>
    ...
</body>
```
> The initialization code will be added inside the `index.html` file (which is the view of the app you have created). More detail about this can be found in the [`How to Use`](#how-to-use) section

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

The singleton instance of the ``` AccountController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, AccountController, CreateANewAccountResponse, UpdateAccountResponse, GetAccountResponse, AccountUsageResponse, SendAccountActivationTokenResponse, VerifyNewAccountResponse){
	});
```

### <a name="create_a_new_member"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.createANewMember") createANewMember

> **Note:** *Authentication isn't required to create a new account.*


```javascript
function createANewMember(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AccountController, CreateANewAccountResponse){
        var body = new CreateANewAccountRequest({"key":"value"});


		var result = AccountController.createANewMember(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_account"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.updateAccount") updateAccount

> TODO: Add a method description


```javascript
function updateAccount(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AccountController, UpdateAccountResponse){
        var body = new UpdateAccountRequest(    {        "username":"johndoe",        "user_email":"johndoe@awesome.com",        "user_phone":"518-481-1002",        "user_first_name":"John",        "user_last_name":"Doe",        "country":"AU",        "password":"pass",        "account_name":"The Awesome Company",        "timezone": "Australia/Melbourne",        "private_uploads": 1,        "setting_sms_hide_your_number": 0,        "setting_sms_hide_business_name": 1    });


		var result = AccountController.updateAccount(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_account"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.getAccount") getAccount

> TODO: Add a method description


```javascript
function getAccount()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, AccountController, GetAccountResponse){


		var result = AccountController.getAccount();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_account_usage"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.getAccountUsage") getAccountUsage

> TODO: Add a method description


```javascript
function getAccountUsage(year, month, type)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| year |  ``` Required ```  | Your account usage year. |
| month |  ``` Required ```  | Your account usage month. |
| type |  ``` Required ```  | The account type. Value can only be either email or subaccount. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AccountController, AccountUsageResponse){
        var year = 2016;
        var month = 4;
        var type = 'subaccount';


		var result = AccountController.getAccountUsage(year, month, type);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_send_account_activation_token"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.updateSendAccountActivationToken") updateSendAccountActivationToken

> TODO: Add a method description


```javascript
function updateSendAccountActivationToken(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AccountController, SendAccountActivationTokenResponse){
        var body = new SendAccountActivationTokenRequest(    {        "user_phone":"352-394-4199",        "type":"sms",        "country": "US"    });


		var result = AccountController.updateSendAccountActivationToken(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_verify_new_account"></a>![Method: ](https://apidocs.io/img/method.png ".AccountController.updateVerifyNewAccount") updateVerifyNewAccount

> TODO: Add a method description


```javascript
function updateVerifyNewAccount(activationToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| activationToken |  ``` Required ```  | The ActivationToken to be used to verify an account. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AccountController, VerifyNewAccountResponse){
        var activationToken = 1827364;


		var result = AccountController.updateVerifyNewAccount(activationToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="account_recharge_controller"></a>![Class: ](https://apidocs.io/img/class.png ".AccountRechargeController") AccountRechargeController

### Get singleton instance

The singleton instance of the ``` AccountRechargeController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, AccountRechargeController, GetCreditCardInfoResponse, UpdateCreditCardInfoResponse, ListOfPackagesResponse, PurchaseAPackageResponse, GetTransactionsResponse){
	});
```

### <a name="get_credit_card_info"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.getCreditCardInfo") getCreditCardInfo

> TODO: Add a method description


```javascript
function getCreditCardInfo()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, AccountRechargeController, GetCreditCardInfoResponse){


		var result = AccountRechargeController.getCreditCardInfo();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_credit_card_info"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.updateCreditCardInfo") updateCreditCardInfo

> TODO: Add a method description


```javascript
function updateCreditCardInfo(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AccountRechargeController, UpdateCreditCardInfoResponse){
        var body = new UpdateCreditCardInfoRequest({"key":"value"});


		var result = AccountRechargeController.updateCreditCardInfo(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="list_of_packages"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.listOfPackages") listOfPackages

> TODO: Add a method description


```javascript
function listOfPackages(country)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Optional ```  | Your country. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AccountRechargeController, ListOfPackagesResponse){
        var country = '"AU"';


		var result = AccountRechargeController.listOfPackages(country);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_purchase_a_package"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.updatePurchaseAPackage") updatePurchaseAPackage

> TODO: Add a method description


```javascript
function updatePurchaseAPackage(packageId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| packageId |  ``` Required ```  | Your package id. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AccountRechargeController, PurchaseAPackageResponse){
        var packageId = 1;


		var result = AccountRechargeController.updatePurchaseAPackage(packageId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_transactions"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.getTransactions") getTransactions

> TODO: Add a method description


```javascript
function getTransactions()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, AccountRechargeController, GetTransactionsResponse){


		var result = AccountRechargeController.getTransactions();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_a_specific_transaction"></a>![Method: ](https://apidocs.io/img/method.png ".AccountRechargeController.getASpecificTransaction") getASpecificTransaction

> TODO: Add a method description


```javascript
function getASpecificTransaction(transactionId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| transactionId |  ``` Required ```  | 1c65-47fa-aea2-3ded9ed57557 (number, required) - Your transction id. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AccountRechargeController){
        var transactionId = transaction_id;


		var result = AccountRechargeController.getASpecificTransaction(transactionId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="automation_rules_controller"></a>![Class: ](https://apidocs.io/img/class.png ".AutomationRulesController") AutomationRulesController

### Get singleton instance

The singleton instance of the ``` AutomationRulesController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, AutomationRulesController, ListRulesResponse, GetASpecificRuleResponse, CreateANewRuleResponse, UpdateARuleResponse, DeleteARuleResponse, DeleteARuleResponse49, DeleteARuleResponse56){
	});
```

### <a name="list_rules"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.listRules") listRules

> TODO: Add a method description


```javascript
function listRules()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, ListRulesResponse){


		var result = AutomationRulesController.listRules();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_a_specific_rule"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.getASpecificRule") getASpecificRule

> TODO: Add a method description


```javascript
function getASpecificRule(inboundRuleId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Inbound Rule ID. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, GetASpecificRuleResponse){
        var inboundRuleId = 1;


		var result = AutomationRulesController.getASpecificRule(inboundRuleId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_a_new_rule"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.createANewRule") createANewRule

> TODO: Add a method description


```javascript
function createANewRule(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, CreateANewRuleResponse){
        var body = new CreateANewRuleRequest({"key":"value"});


		var result = AutomationRulesController.createANewRule(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_a_rule"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.updateARule") updateARule

> TODO: Add a method description


```javascript
function updateARule(inboundRuleId, body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Inbound Rule ID. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, UpdateARuleResponse){
        var inboundRuleId = 1;
        var body = new UpdateARuleRequest({    "dedicated_number":"+61298441484",    "rule_name":"My Rule",    "message_search_type":3,    "message_search_term":"My Search Term",    "action":"EMAIL_FIXED",    "action_address":"john@doe.com",    "enabled":1});


		var result = AutomationRulesController.updateARule(inboundRuleId, body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="delete_a_rule"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.deleteARule") deleteARule

> TODO: Add a method description


```javascript
function deleteARule(inboundRuleId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Inbound Rule ID. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, DeleteARuleResponse){
        var inboundRuleId = 1;


		var result = AutomationRulesController.deleteARule(inboundRuleId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="list_rules1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.listRules1") listRules1

> TODO: Add a method description


```javascript
function listRules1()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, ListRulesResponse){


		var result = AutomationRulesController.listRules1();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_a_specific_rule"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.getASpecificRule") getASpecificRule

> TODO: Add a method description


```javascript
function getASpecificRule(receiptRuleId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, GetASpecificRuleResponse){
        var receiptRuleId = 2;


		var result = AutomationRulesController.getASpecificRule(receiptRuleId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_a_new_rule1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.createANewRule1") createANewRule1

> TODO: Add a method description


```javascript
function createANewRule1(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, CreateANewRuleResponse){
        var body = new CreateANewRuleRequest24({    "rule_name": "My Rule",    "match_type": 3,    "action": "EMAIL_FIXED",    "action_address": "john@doe.com",    "enabled": 1});


		var result = AutomationRulesController.createANewRule1(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_a_rule"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.updateARule") updateARule

> TODO: Add a method description


```javascript
function updateARule(receiptRuleId, body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, UpdateARuleResponse){
        var receiptRuleId = 7;
        var body = new UpdateARuleRequest26({    "rule_name": "My Rule",    "match_type": 3,    "action": "EMAIL_FIXED",    "action_address": "john@doe.com",    "enabled": 1});


		var result = AutomationRulesController.updateARule(receiptRuleId, body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="delete_a_rule"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.deleteARule") deleteARule

> TODO: Add a method description


```javascript
function deleteARule(receiptRuleId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, DeleteARuleResponse){
        var receiptRuleId = 7;


		var result = AutomationRulesController.deleteARule(receiptRuleId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="list_rules2"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.listRules2") listRules2

> TODO: Add a method description


```javascript
function listRules2()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, ListRulesResponse){


		var result = AutomationRulesController.listRules2();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_a_specific_rule1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.getASpecificRule1") getASpecificRule1

> TODO: Add a method description


```javascript
function getASpecificRule1(receiptRuleId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, GetASpecificRuleResponse){
        var receiptRuleId = 2;


		var result = AutomationRulesController.getASpecificRule1(receiptRuleId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_a_new_rule2"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.createANewRule2") createANewRule2

> TODO: Add a method description


```javascript
function createANewRule2(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, CreateANewRuleResponse){
        var body = new CreateANewRuleRequest24({    "rule_name":"My Rule",    "match_type":3,    "action":"EMAIL_FIXED",    "action_address":"john@doe.com",    "enabled":1});


		var result = AutomationRulesController.createANewRule2(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_a_rule1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.updateARule1") updateARule1

> TODO: Add a method description


```javascript
function updateARule1(receiptRuleId, body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, UpdateARuleResponse){
        var receiptRuleId = 2;
        var body = new UpdateARuleRequest26({    "rule_name":"My Rule",    "match_type":3,    "action":"EMAIL_FIXED",    "action_address":"john@doe.com",    "enabled":1});


		var result = AutomationRulesController.updateARule1(receiptRuleId, body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="delete_a_rule1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.deleteARule1") deleteARule1

> TODO: Add a method description


```javascript
function deleteARule1(receiptRuleId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| receiptRuleId |  ``` Required ```  | Receipt Rule ID. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, DeleteARuleResponse){
        var receiptRuleId = 2;


		var result = AutomationRulesController.deleteARule1(receiptRuleId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="list_rules3"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.listRules3") listRules3

> TODO: Add a method description


```javascript
function listRules3()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, ListRulesResponse){


		var result = AutomationRulesController.listRules3();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_a_specific_rule1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.getASpecificRule1") getASpecificRule1

> TODO: Add a method description


```javascript
function getASpecificRule1(inboundRuleId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Fax inbound rule id |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, GetASpecificRuleResponse){
        var inboundRuleId = 14;


		var result = AutomationRulesController.getASpecificRule1(inboundRuleId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_a_new_rule3"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.createANewRule3") createANewRule3

> TODO: Add a method description


```javascript
function createANewRule3(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, CreateANewRuleResponse){
        var body = new CreateANewRuleRequest38(    {        "dedicated_number":"+61298441484",        "rule_name":"Rule Name",        "action":"EMAIL_FIXED",        "action_address":"email@domain.com",        "enabled":1    });


		var result = AutomationRulesController.createANewRule3(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_a_rule1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.updateARule1") updateARule1

> TODO: Add a method description


```javascript
function updateARule1(inboundRuleId, body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Fax inbound rule id |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, UpdateARuleResponse){
        var inboundRuleId = 14;
        var body = new UpdateARuleRequest40(    {        "dedicated_number":"+61298441484",        "rule_name":"Rule Name",        "action":"EMAIL_FIXED",        "action_address":"email@domain.com",        "enabled":1    });


		var result = AutomationRulesController.updateARule1(inboundRuleId, body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="delete_a_rule1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.deleteARule1") deleteARule1

> TODO: Add a method description


```javascript
function deleteARule1(inboundRuleId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| inboundRuleId |  ``` Required ```  | Fax inbound rule id |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, DeleteARuleResponse){
        var inboundRuleId = 14;


		var result = AutomationRulesController.deleteARule1(inboundRuleId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="list_rules4"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.listRules4") listRules4

> TODO: Add a method description


```javascript
function listRules4()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, ListRulesResponse){


		var result = AutomationRulesController.listRules4();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_a_specific_rule"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.getASpecificRule") getASpecificRule

> TODO: Add a method description


```javascript
function getASpecificRule(ruleId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, GetASpecificRuleResponse){
        var ruleId = 4;


		var result = AutomationRulesController.getASpecificRule(ruleId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_a_new_rule4"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.createANewRule4") createANewRule4

> TODO: Add a method description


```javascript
function createANewRule4(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, CreateANewRuleResponse){
        var body = new CreateANewRuleRequest24(    {        "rule_name":"My Rule",        "match_type":2,        "action":"EMAIL_FIXED",        "action_address":"john@doe.com",        "enabled":1    });


		var result = AutomationRulesController.createANewRule4(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_a_rule"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.updateARule") updateARule

> TODO: Add a method description


```javascript
function updateARule(ruleId, body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, UpdateARuleResponse){
        var ruleId = 4;
        var body = new UpdateARuleRequest26(    {        "rule_name":"My Rule",        "match_type":1,        "action":"EMAIL_FIXED",        "action_address":"john@doe.com",        "enabled":1    });


		var result = AutomationRulesController.updateARule(ruleId, body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="delete_a_rule"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.deleteARule") deleteARule

> TODO: Add a method description


```javascript
function deleteARule(ruleId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to delete. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, DeleteARuleResponse49){
        var ruleId = 18.3189679511445;


		var result = AutomationRulesController.deleteARule(ruleId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="list_rules5"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.listRules5") listRules5

> TODO: Add a method description


```javascript
function listRules5()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, ListRulesResponse){


		var result = AutomationRulesController.listRules5();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_a_specific_rule1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.getASpecificRule1") getASpecificRule1

> TODO: Add a method description


```javascript
function getASpecificRule1(ruleId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, GetASpecificRuleResponse){
        var ruleId = 5;


		var result = AutomationRulesController.getASpecificRule1(ruleId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_a_new_rule5"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.createANewRule5") createANewRule5

> TODO: Add a method description


```javascript
function createANewRule5(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, CreateANewRuleResponse){
        var body = new CreateANewRuleRequest24(    {        "rule_name":"My Rule",        "match_type": 0,        "action":"URL",        "action_address":"http://testurl.com",        "enabled":1    });


		var result = AutomationRulesController.createANewRule5(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_a_rule1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.updateARule1") updateARule1

> TODO: Add a method description


```javascript
function updateARule1(ruleId, body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, UpdateARuleResponse){
        var ruleId = 8;
        var body = new UpdateARuleRequest26(    {        "rule_name":"My Rule",        "match_type": 0,        "action":"URL",        "action_address":"http://testurl.com",        "enabled":1    });


		var result = AutomationRulesController.updateARule1(ruleId, body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="delete_a_rule1"></a>![Method: ](https://apidocs.io/img/method.png ".AutomationRulesController.deleteARule1") deleteARule1

> TODO: Add a method description


```javascript
function deleteARule1(ruleId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The email receipt rule id you want to delete. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AutomationRulesController, DeleteARuleResponse56){
        var ruleId = 8;


		var result = AutomationRulesController.deleteARule1(ruleId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="contact_lists_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ContactListsController") ContactListsController

### Get singleton instance

The singleton instance of the ``` ContactListsController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, ContactListsController, GetAllContactListsResponse, CreateANewContactListResponse, GetASpecificContactListResponse, UpdateASpecificContactListResponse, DeleteASpecificContactListResponse, ImportContactsToListResponse, RemoveDuplicateContactsResponse, GetListOfAcceptableImportFieldsResponse, ShowCSVImportFilePreviewResponse){
	});
```

### <a name="get_all_contact_lists"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.getAllContactLists") getAllContactLists

> TODO: Add a method description


```javascript
function getAllContactLists()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactListsController, GetAllContactListsResponse){


		var result = ContactListsController.getAllContactLists();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_a_new_contact_list"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.createANewContactList") createANewContactList

> TODO: Add a method description


```javascript
function createANewContactList(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactListsController, CreateANewContactListResponse){
        var body = new CreateANewContactListRequest(    {        "list_name":"ListCT3QrVL4od"    });


		var result = ContactListsController.createANewContactList(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_a_specific_contact_list"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.getASpecificContactList") getASpecificContactList

> TODO: Add a method description


```javascript
function getASpecificContactList(listId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactListsController, GetASpecificContactListResponse){
        var listId = 437;


		var result = ContactListsController.getASpecificContactList(listId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_a_specific_contact_list"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.updateASpecificContactList") updateASpecificContactList

> TODO: Add a method description


```javascript
function updateASpecificContactList(listId, body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactListsController, UpdateASpecificContactListResponse){
        var listId = 439;
        var body = new UpdateASpecificContactListRequest(    {        "list_name":"ListlPJf33ksjP"    });


		var result = ContactListsController.updateASpecificContactList(listId, body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="delete_a_specific_contact_list"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.deleteASpecificContactList") deleteASpecificContactList

> TODO: Add a method description


```javascript
function deleteASpecificContactList(listId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactListsController, DeleteASpecificContactListResponse){
        var listId = 442;


		var result = ContactListsController.deleteASpecificContactList(listId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_import_contacts_to_list"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.createImportContactsToList") createImportContactsToList

> TODO: Add a method description


```javascript
function createImportContactsToList(listId, body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactListsController, ImportContactsToListResponse){
        var listId = 437;
        var body = new ImportContactsToListRequest({    "file_url":"http://yourdomain.com/5485EA6144/79E8/import.csv",    "field_order":[        "phone",        "first_name",        "last_name",        "custom1",        "custom2",        "custom3",        "custom4",        "fax_number",        "organization_name",        "email",        "address_line_1",        "address_line_2",        "address_city",        "address_state",        "address_postal_code",        "address_country"    ]});


		var result = ContactListsController.createImportContactsToList(listId, body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_remove_duplicate_contacts"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.updateRemoveDuplicateContacts") updateRemoveDuplicateContacts

> TODO: Add a method description


```javascript
function updateRemoveDuplicateContacts(listId, body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactListsController, RemoveDuplicateContactsResponse){
        var listId = 439;
        var body = new RemoveDuplicateContactsRequest({    "fields":[        "phone_number",        "first_name",        "last_name",        "fax_number",        "address_country"    ]});


		var result = ContactListsController.updateRemoveDuplicateContacts(listId, body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_list_of_acceptable_import_fields"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.getListOfAcceptableImportFields") getListOfAcceptableImportFields

> TODO: Add a method description


```javascript
function getListOfAcceptableImportFields(listId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Optional ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactListsController, GetListOfAcceptableImportFieldsResponse){
        var listId = list_id;


		var result = ContactListsController.getListOfAcceptableImportFields(listId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_show_csv_import_file_preview"></a>![Method: ](https://apidocs.io/img/method.png ".ContactListsController.createShowCSVImportFilePreview") createShowCSVImportFilePreview

> Show first row of the csv import file.


```javascript
function createShowCSVImportFilePreview(listId, body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactListsController, ShowCSVImportFilePreviewResponse){
        var listId = 439;
        var body = new ShowCSVImportFilePreviewRequest({    "file_url":"http://yourdomain.com/5485EA6144/79E8/import.csv"});


		var result = ContactListsController.createShowCSVImportFilePreview(listId, body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="contact_suggestions_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ContactSuggestionsController") ContactSuggestionsController

### Get singleton instance

The singleton instance of the ``` ContactSuggestionsController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, ContactSuggestionsController, ListContactSuggestionsResponse){
	});
```

### <a name="list_contact_suggestions"></a>![Method: ](https://apidocs.io/img/method.png ".ContactSuggestionsController.listContactSuggestions") listContactSuggestions

> TODO: Add a method description


```javascript
function listContactSuggestions()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactSuggestionsController, ListContactSuggestionsResponse){


		var result = ContactSuggestionsController.listContactSuggestions();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="contacts_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ContactsController") ContactsController

### Get singleton instance

The singleton instance of the ``` ContactsController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, ContactsController, GetAllContactsInAListResponse, CreateANewContactResponse, GetASpecificContactResponse, UpdateASpecificContactResponse, DeleteASpecificContactResponse, RemoveOptedOutContactsResponse, TransferAContactResponse){
	});
```

### <a name="get_all_contacts_in_a_list"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.getAllContactsInAList") getAllContactsInAList

> TODO: Add a method description


```javascript
function getAllContactsInAList(listId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id where your contacts belong. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactsController, GetAllContactsInAListResponse){
        var listId = 428;


		var result = ContactsController.getAllContactsInAList(listId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_a_new_contact"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.createANewContact") createANewContact

> TODO: Add a method description


```javascript
function createANewContact(listId, body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id where your contact be associated. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactsController, CreateANewContactResponse){
        var listId = 428;
        var body = new CreateANewContactRequest(    {        "phone_number":"+16783270696",        "first_name":"Ellen",        "last_name":"Diaz",        "custom_1":"Custom 1",        "custom_2":"Custom 2",        "custom_3":"Custom 3",        "custom_4":"Custom 4",        "fax_number":"+16783270696",        "organization_name":"Awesome Organization",        "email":"ellen@diaz.com",        "address_line_1":"Block 2",        "address_line_2":"Cool Bldg.",        "address_city":"Nevada",        "address_state":"Las Vegas",        "address_postal_code":"36063",        "address_country":"US"    });


		var result = ContactsController.createANewContact(listId, body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_a_specific_contact"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.getASpecificContact") getASpecificContact

> TODO: Add a method description


```javascript
function getASpecificContact(listId, contactId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| contactId |  ``` Required ```  | Your contact id you want to access. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactsController, GetASpecificContactResponse){
        var listId = 428;
        var contactId = 552802;


		var result = ContactsController.getASpecificContact(listId, contactId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_a_specific_contact"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.updateASpecificContact") updateASpecificContact

> TODO: Add a method description


```javascript
function updateASpecificContact(listId, contactId, body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| contactId |  ``` Required ```  | Your contact id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactsController, UpdateASpecificContactResponse){
        var listId = 428;
        var contactId = 552802;
        var body = new UpdateASpecificContactRequest({        "phone_number":"+16783275492",        "first_name":"Ellen",        "last_name":"Diaz",        "custom_1":"Custom S72oJ9Teba",        "custom_2":"Custom NvrRJrKWeq",        "custom_3":"Custom 2ws94p1Dop",        "custom_4":"Custom Ku0AaIS5xb",        "fax_number":"+16783276356",        "organization_name":"Awesome Organization",        "email":"ellen@diaz.com",        "address_line_1":"Block 6",        "address_line_2":"Cool Bldg.",        "address_city":"Nevada",        "address_state":"Las Vegas",        "address_postal_code":"36063",        "address_country":"US"    });


		var result = ContactsController.updateASpecificContact(listId, contactId, body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="delete_a_specific_contact"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.deleteASpecificContact") deleteASpecificContact

> TODO: Add a method description


```javascript
function deleteASpecificContact(listId, contactId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id you want to access. |
| contactId |  ``` Required ```  | Your contact id you want to access. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactsController, DeleteASpecificContactResponse){
        var listId = 428;
        var contactId = 552807;


		var result = ContactsController.deleteASpecificContact(listId, contactId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_remove_opted_out_contacts"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.updateRemoveOptedOutContacts") updateRemoveOptedOutContacts

> TODO: Add a method description


```javascript
function updateRemoveOptedOutContacts(listId, optOutListId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| listId |  ``` Required ```  | Your contact list id. |
| optOutListId |  ``` Required ```  | Your opt out list id. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactsController, RemoveOptedOutContactsResponse){
        var listId = 439;
        var optOutListId = 512;


		var result = ContactsController.updateRemoveOptedOutContacts(listId, optOutListId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_transfer_a_contact"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.updateTransferAContact") updateTransferAContact

> Transfers a specific contact to another list.


```javascript
function updateTransferAContact(fromListId, contactId, toListId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| fromListId |  ``` Required ```  | From list id. |
| contactId |  ``` Required ```  | Contact ID. |
| toListId |  ``` Required ```  | To list id. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactsController, TransferAContactResponse){
        var fromListId = 428;
        var contactId = 1;
        var toListId = 429;


		var result = ContactsController.updateTransferAContact(fromListId, contactId, toListId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_hello_contact"></a>![Method: ](https://apidocs.io/img/method.png ".ContactsController.getHelloContact") getHelloContact

> TODO: Add a method description


```javascript
function getHelloContact()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactsController){


		var result = ContactsController.getHelloContact();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="countries_controller"></a>![Class: ](https://apidocs.io/img/class.png ".CountriesController") CountriesController

### Get singleton instance

The singleton instance of the ``` CountriesController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, CountriesController, GetAllCountriesResponse){
	});
```

### <a name="get_all_countries"></a>![Method: ](https://apidocs.io/img/method.png ".CountriesController.getAllCountries") getAllCountries

> TODO: Add a method description


```javascript
function getAllCountries()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, CountriesController, GetAllCountriesResponse){


		var result = CountriesController.getAllCountries();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="delivery_issues_controller"></a>![Class: ](https://apidocs.io/img/class.png ".DeliveryIssuesController") DeliveryIssuesController

### Get singleton instance

The singleton instance of the ``` DeliveryIssuesController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, DeliveryIssuesController, GetDeliveryIssuesResponse, CreateDeliveryIssueResponse){
	});
```

### <a name="get_delivery_issues"></a>![Method: ](https://apidocs.io/img/method.png ".DeliveryIssuesController.getDeliveryIssues") getDeliveryIssues

> TODO: Add a method description


```javascript
function getDeliveryIssues()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, DeliveryIssuesController, GetDeliveryIssuesResponse){


		var result = DeliveryIssuesController.getDeliveryIssues();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_delivery_issue"></a>![Method: ](https://apidocs.io/img/method.png ".DeliveryIssuesController.createDeliveryIssue") createDeliveryIssue

> TODO: Add a method description


```javascript
function createDeliveryIssue(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, DeliveryIssuesController, CreateDeliveryIssueResponse){
        var body = new CreateDeliveryIssueRequest({  "message_id": "B388828B",  "type": "SMS",  "description": "This is a test",  "client_comments": "test",  "email_address: john_doe@user.com": "",  "Body": ""});


		var result = DeliveryIssuesController.createDeliveryIssue(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="email_marketing_controller"></a>![Class: ](https://apidocs.io/img/class.png ".EmailMarketingController") EmailMarketingController

### Get singleton instance

The singleton instance of the ``` EmailMarketingController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, EmailMarketingController, GetAllAllowedEmailAddressesResponse, CreateAllowedEmailAddressResponse, SendVerificationTokenResponse, VerifyAllowedEmailAddressResponse, DeleteAllowedEmailAddressResponse, GetSpecificAllowedEmailAddressResponse, GetAllEmailCampaignsResponse, GetSpecificEmailCampaignResponse, CreateEmailCampaignResponse, UpdateEmailCampaignResponse, CancelEmailCampaignResponse, CalculatePriceResponse, GetSpecificEmailCampaignHistoryResponse, GetAllEmailTemplatesResponse, GetSpecificEmailTemplateResponse, CreateNewEmailTemplateFromMasterTemplateResponse, UpdateAnEmailTemplateResponse, DeleteEmailTemplateResponse, GetAllMasterEmailTemplatesResponse, GetSpecificMasterTemplateResponse, GetAllMasterTemplateCategoriesResponse, GetSpecificEmailTemplateCategoryResponse, GetAllTemplatesForCategoryResponse, UploadImageToSpecificTemplateResponse){
	});
```

### <a name="get_all_allowed_email_addresses"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getAllAllowedEmailAddresses") getAllAllowedEmailAddresses

> TODO: Add a method description


```javascript
function getAllAllowedEmailAddresses()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailMarketingController, GetAllAllowedEmailAddressesResponse){


		var result = EmailMarketingController.getAllAllowedEmailAddresses();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_allowed_email_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.createAllowedEmailAddress") createAllowedEmailAddress

> TODO: Add a method description


```javascript
function createAllowedEmailAddress(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailMarketingController, CreateAllowedEmailAddressResponse){
        var body = new CreateAllowedEmailAddressRequest({  "email_address": "johndoe1@user.com",  "Body": ""});


		var result = EmailMarketingController.createAllowedEmailAddress(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_send_verification_token"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.updateSendVerificationToken") updateSendVerificationToken

> TODO: Add a method description


```javascript
function updateSendVerificationToken(emailAddressId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email addess id you want to access. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailMarketingController, SendVerificationTokenResponse){
        var emailAddressId = 18.3189679511445;


		var result = EmailMarketingController.updateSendVerificationToken(emailAddressId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_verify_allowed_email_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.updateVerifyAllowedEmailAddress") updateVerifyAllowedEmailAddress

> TODO: Add a method description


```javascript
function updateVerifyAllowedEmailAddress(emailAddressId, activationToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email address id you want to access. |
| activationToken |  ``` Required ```  | 6E8B-4FDB-99A7-7ED08DF97BCC (required, string) - Your activation token. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailMarketingController, VerifyAllowedEmailAddressResponse){
        var emailAddressId = 5;
        var activationToken = 3BD73304;


		var result = EmailMarketingController.updateVerifyAllowedEmailAddress(emailAddressId, activationToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="delete_allowed_email_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.deleteAllowedEmailAddress") deleteAllowedEmailAddress

> TODO: Add a method description


```javascript
function deleteAllowedEmailAddress(emailAddressId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email address you want to access. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailMarketingController, DeleteAllowedEmailAddressResponse){
        var emailAddressId = 18.3189679511445;


		var result = EmailMarketingController.deleteAllowedEmailAddress(emailAddressId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_specific_allowed_email_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getSpecificAllowedEmailAddress") getSpecificAllowedEmailAddress

> TODO: Add a method description


```javascript
function getSpecificAllowedEmailAddress(emailAddressId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | The email address you want to access. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailMarketingController, GetSpecificAllowedEmailAddressResponse){
        var emailAddressId = 4;


		var result = EmailMarketingController.getSpecificAllowedEmailAddress(emailAddressId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_all_email_campaigns"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getAllEmailCampaigns") getAllEmailCampaigns

> TODO: Add a method description


```javascript
function getAllEmailCampaigns()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailMarketingController, GetAllEmailCampaignsResponse){


		var result = EmailMarketingController.getAllEmailCampaigns();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_specific_email_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getSpecificEmailCampaign") getSpecificEmailCampaign

> TODO: Add a method description


```javascript
function getSpecificEmailCampaign(emailCampaignId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailCampaignId |  ``` Required ```  | The email campaign id you want to access. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailMarketingController, GetSpecificEmailCampaignResponse){
        var emailCampaignId = 1;


		var result = EmailMarketingController.getSpecificEmailCampaign(emailCampaignId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_email_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.createEmailCampaign") createEmailCampaign

> TODO: Add a method description


```javascript
function createEmailCampaign(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailMarketingController, CreateEmailCampaignResponse){
        var body = new CreateEmailCampaignRequest({  "name" : "John Doe",  "subject" : "Lorem Ipsum",  "from_email_address_id" : 2,  "from_name" : "From name",  "template_id" : 31,  "body" : "<p>This is a test</p>",  "list_id" : 456});


		var result = EmailMarketingController.createEmailCampaign(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_email_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.updateEmailCampaign") updateEmailCampaign

> TODO: Add a method description


```javascript
function updateEmailCampaign(emailCampaignId, body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailCampaignId |  ``` Required ```  | The email campaign id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailMarketingController, UpdateEmailCampaignResponse){
        var emailCampaignId = 1;
        var body = new UpdateEmailCampaignRequest({  "name" : "John Doe",  "subject" : "Lorem Ipsum",  "from_email_address_id" : 2,  "from_name" : "From name",  "template_id" : 31,  "body" : "<p>This is a test</p>",  "list_id" : 456});


		var result = EmailMarketingController.updateEmailCampaign(emailCampaignId, body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_cancel_email_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.updateCancelEmailCampaign") updateCancelEmailCampaign

> TODO: Add a method description


```javascript
function updateCancelEmailCampaign(emailCampaignId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailCampaignId |  ``` Required ```  | The email campaign id you want to cancel. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailMarketingController, CancelEmailCampaignResponse){
        var emailCampaignId = 1;


		var result = EmailMarketingController.updateCancelEmailCampaign(emailCampaignId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.createCalculatePrice") createCalculatePrice

> TODO: Add a method description


```javascript
function createCalculatePrice(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailMarketingController, CalculatePriceResponse){
        var body = new CalculatePriceRequest({  "name" : "John Doe",  "subject" : "Lorem Ipsum",  "from_email_address_id" : 2,  "from_name" : "From name",  "template_id" : 31,  "body" : "<p>This is a test</p>",  "list_id" : 456});


		var result = EmailMarketingController.createCalculatePrice(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_specific_email_campaign_history"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getSpecificEmailCampaignHistory") getSpecificEmailCampaignHistory

> TODO: Add a method description


```javascript
function getSpecificEmailCampaignHistory(campaignId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| campaignId |  ``` Required ```  | The email campaign id you want to access. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailMarketingController, GetSpecificEmailCampaignHistoryResponse){
        var campaignId = 77;


		var result = EmailMarketingController.getSpecificEmailCampaignHistory(campaignId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_all_email_templates"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getAllEmailTemplates") getAllEmailTemplates

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```javascript
function getAllEmailTemplates()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailMarketingController, GetAllEmailTemplatesResponse){


		var result = EmailMarketingController.getAllEmailTemplates();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_specific_email_template"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getSpecificEmailTemplate") getSpecificEmailTemplate

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```javascript
function getSpecificEmailTemplate(templateId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | The email template id. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailMarketingController, GetSpecificEmailTemplateResponse){
        var templateId = 291;


		var result = EmailMarketingController.getSpecificEmailTemplate(templateId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_new_email_template_from_master_template"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.createNewEmailTemplateFromMasterTemplate") createNewEmailTemplateFromMasterTemplate

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```javascript
function createNewEmailTemplateFromMasterTemplate(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailMarketingController, CreateNewEmailTemplateFromMasterTemplateResponse){
        var body = new CreateNewEmailTemplateFromMasterTemplateRequest({  "template_name": "Minions",  "template_id_master": 57});


		var result = EmailMarketingController.createNewEmailTemplateFromMasterTemplate(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_an_email_template"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.updateAnEmailTemplate") updateAnEmailTemplate

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```javascript
function updateAnEmailTemplate(templateId, body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | The id of the template to be updated. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailMarketingController, UpdateAnEmailTemplateResponse){
        var templateId = 291;
        var body = new UpdateAnEmailTemplateRequest(    {        "template_name":"Minions",        "body":"This is a sample content: Sc0KNWgSMG for this template."    });


		var result = EmailMarketingController.updateAnEmailTemplate(templateId, body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="delete_email_template"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.deleteEmailTemplate") deleteEmailTemplate

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.


```javascript
function deleteEmailTemplate(templateId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailMarketingController, DeleteEmailTemplateResponse){
        var templateId = 25;


		var result = EmailMarketingController.deleteEmailTemplate(templateId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_all_master_email_templates"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getAllMasterEmailTemplates") getAllMasterEmailTemplates

> Master templates are templates that you can clone to a User Email Template which lets you edit and save it.


```javascript
function getAllMasterEmailTemplates()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailMarketingController, GetAllMasterEmailTemplatesResponse){


		var result = EmailMarketingController.getAllMasterEmailTemplates();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_specific_master_template"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getSpecificMasterTemplate") getSpecificMasterTemplate

> Master templates are templates that you can clone to a User Email Template which lets you edit and save it.


```javascript
function getSpecificMasterTemplate(templateId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailMarketingController, GetSpecificMasterTemplateResponse){
        var templateId = 25;


		var result = EmailMarketingController.getSpecificMasterTemplate(templateId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_all_master_template_categories"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getAllMasterTemplateCategories") getAllMasterTemplateCategories

> TODO: Add a method description


```javascript
function getAllMasterTemplateCategories()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailMarketingController, GetAllMasterTemplateCategoriesResponse){


		var result = EmailMarketingController.getAllMasterTemplateCategories();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_specific_email_template_category"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getSpecificEmailTemplateCategory") getSpecificEmailTemplateCategory

> TODO: Add a method description


```javascript
function getSpecificEmailTemplateCategory(categoryId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| categoryId |  ``` Required ```  | Your category id. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailMarketingController, GetSpecificEmailTemplateCategoryResponse){
        var categoryId = 25;


		var result = EmailMarketingController.getSpecificEmailTemplateCategory(categoryId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_all_templates_for_category"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.getAllTemplatesForCategory") getAllTemplatesForCategory

> TODO: Add a method description


```javascript
function getAllTemplatesForCategory(categoryId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| categoryId |  ``` Required ```  | Your category id. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailMarketingController, GetAllTemplatesForCategoryResponse){
        var categoryId = 1;


		var result = EmailMarketingController.getAllTemplatesForCategory(categoryId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="upload_image_to_specific_template"></a>![Method: ](https://apidocs.io/img/method.png ".EmailMarketingController.uploadImageToSpecificTemplate") uploadImageToSpecificTemplate

> TODO: Add a method description


```javascript
function uploadImageToSpecificTemplate(templateId, body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailMarketingController, UploadImageToSpecificTemplateResponse){
        var templateId = 1;
        var body = new UploadImageToSpecificTemplateRequest({    "image": "image.png",    "url" : "http://www.downloadimg.from/here.png"});


		var result = EmailMarketingController.uploadImageToSpecificTemplate(templateId, body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="email_to_sms_allowed_address_controller"></a>![Class: ](https://apidocs.io/img/class.png ".EmailToSMSAllowedAddressController") EmailToSMSAllowedAddressController

### Get singleton instance

The singleton instance of the ``` EmailToSMSAllowedAddressController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, EmailToSMSAllowedAddressController, ListOfEmailToSMSAllowedAddressResponse, CreateEmailToSMSAllowedAddressResponse, GetSpecificEmailToSMSAllowedAddressResponse, UpdateEmailToSMSAllowedAddressResponse, DeleteEmailToSMSAllowedAddressResponse){
	});
```

### <a name="list_of_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSAllowedAddressController.listOfEmailToSMSAllowedAddress") listOfEmailToSMSAllowedAddress

> Get list of allowed email addresses.


```javascript
function listOfEmailToSMSAllowedAddress()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailToSMSAllowedAddressController, ListOfEmailToSMSAllowedAddressResponse){


		var result = EmailToSMSAllowedAddressController.listOfEmailToSMSAllowedAddress();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSAllowedAddressController.createEmailToSMSAllowedAddress") createEmailToSMSAllowedAddress

> Create an allowed email address.


```javascript
function createEmailToSMSAllowedAddress(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailToSMSAllowedAddressController, CreateEmailToSMSAllowedAddressResponse){
        var body = new CreateEmailToSMSAllowedAddressRequest(    {        "email_address":"Cv3p0@gmail.com",        "from":"+17128845887"    });


		var result = EmailToSMSAllowedAddressController.createEmailToSMSAllowedAddress(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_specific_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSAllowedAddressController.getSpecificEmailToSMSAllowedAddress") getSpecificEmailToSMSAllowedAddress

> Get a specific allowed email address.


```javascript
function getSpecificEmailToSMSAllowedAddress(emailAddressId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | Your email address id. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailToSMSAllowedAddressController, GetSpecificEmailToSMSAllowedAddressResponse){
        var emailAddressId = 113;


		var result = EmailToSMSAllowedAddressController.getSpecificEmailToSMSAllowedAddress(emailAddressId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSAllowedAddressController.updateEmailToSMSAllowedAddress") updateEmailToSMSAllowedAddress

> Update a specific allowed email address.


```javascript
function updateEmailToSMSAllowedAddress(emailAddressId, body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | Your email address id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailToSMSAllowedAddressController, UpdateEmailToSMSAllowedAddressResponse){
        var emailAddressId = 107;
        var body = new UpdateEmailToSMSAllowedAddressRequest(    {        "email_address":"pfvRZ@gmail.com",        "from":"+17128842283"    });


		var result = EmailToSMSAllowedAddressController.updateEmailToSMSAllowedAddress(emailAddressId, body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="delete_email_to_sms_allowed_address"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSAllowedAddressController.deleteEmailToSMSAllowedAddress") deleteEmailToSMSAllowedAddress

> Delete a specific allowed email address.


```javascript
function deleteEmailToSMSAllowedAddress(emailAddressId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| emailAddressId |  ``` Required ```  | Your email address id. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailToSMSAllowedAddressController, DeleteEmailToSMSAllowedAddressResponse){
        var emailAddressId = 107;


		var result = EmailToSMSAllowedAddressController.deleteEmailToSMSAllowedAddress(emailAddressId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="email_to_sms_stripped_strings_controller"></a>![Class: ](https://apidocs.io/img/class.png ".EmailToSMSStrippedStringsController") EmailToSMSStrippedStringsController

### Get singleton instance

The singleton instance of the ``` EmailToSMSStrippedStringsController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, EmailToSMSStrippedStringsController, ListStrippedStringsResponse, FindSpecificStrippedStringResponse, CreateStrippedStringResponse, UpdateStrippedStringResponse, DeleteStrippedStringResponse){
	});
```

### <a name="list_stripped_strings"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSStrippedStringsController.listStrippedStrings") listStrippedStrings

> TODO: Add a method description


```javascript
function listStrippedStrings()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailToSMSStrippedStringsController, ListStrippedStringsResponse){


		var result = EmailToSMSStrippedStringsController.listStrippedStrings();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="find_specific_stripped_string"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSStrippedStringsController.findSpecificStrippedString") findSpecificStrippedString

> TODO: Add a method description


```javascript
function findSpecificStrippedString(ruleId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailToSMSStrippedStringsController, FindSpecificStrippedStringResponse){
        var ruleId = 18;


		var result = EmailToSMSStrippedStringsController.findSpecificStrippedString(ruleId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_stripped_string"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSStrippedStringsController.createStrippedString") createStrippedString

> TODO: Add a method description


```javascript
function createStrippedString(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailToSMSStrippedStringsController, CreateStrippedStringResponse){
        var body = new CreateStrippedStringRequest({    "strip_string" : "~~~test~~~"});


		var result = EmailToSMSStrippedStringsController.createStrippedString(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_stripped_string"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSStrippedStringsController.updateStrippedString") updateStrippedString

> TODO: Add a method description


```javascript
function updateStrippedString(ruleId, body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailToSMSStrippedStringsController, UpdateStrippedStringResponse){
        var ruleId = 20;
        var body = new UpdateStrippedStringRequest({    "strip_string" : "~~~test1~~~"});


		var result = EmailToSMSStrippedStringsController.updateStrippedString(ruleId, body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="delete_stripped_string"></a>![Method: ](https://apidocs.io/img/method.png ".EmailToSMSStrippedStringsController.deleteStrippedString") deleteStrippedString

> TODO: Add a method description


```javascript
function deleteStrippedString(ruleId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ruleId |  ``` Required ```  | The rule id you want to access. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailToSMSStrippedStringsController, DeleteStrippedStringResponse){
        var ruleId = 20;


		var result = EmailToSMSStrippedStringsController.deleteStrippedString(ruleId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="fax_controller"></a>![Class: ](https://apidocs.io/img/class.png ".FaxController") FaxController

### Get singleton instance

The singleton instance of the ``` FaxController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, FaxController, SendFaxResponse, CalculatePriceResponse, GetFaxHistoryResponse, ListOfFaxDeliveryReceiptsResponse, GetASpecificFaxDeliveryReceiptResponse, MarkFaxDeliveryReceiptsAsReadResponse, AddATestDeliveryReceiptResponse){
	});
```

### <a name="create_send_fax"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.createSendFax") createSendFax

> **Letter File Options**
> **Use existing URL**
> With this option, you can use an existing URL to a PDF document. For example, you might generate the pdf on your server.
> **Upload File to Our Server**
> With this option, you can use the `/uploads` endpoint to upload the document. The `/uploads` endpoint returns a URL that can be used in the `/fax/send` endpoint.


```javascript
function createSendFax(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, FaxController, SendFaxResponse){
        var body = new SendFaxRequest({"key":"value"});


		var result = FaxController.createSendFax(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.createCalculatePrice") createCalculatePrice

> TODO: Add a method description


```javascript
function createCalculatePrice(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, FaxController, CalculatePriceResponse){
        var body = new CalculatePriceRequest132({"key":"value"});


		var result = FaxController.createCalculatePrice(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_fax_history"></a>![Method: ](https://apidocs.io/img/method.png ".FaxController.getFaxHistory") getFaxHistory

> Get a list of Fax History.


```javascript
function getFaxHistory(dateFrom, dateTo, q, orderBy)
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


	app.controller("testController", function($scope, FaxController, GetFaxHistoryResponse){
        var dateFrom = 1457572619;
        var dateTo = 1457573000;
        var q = 'status:Sent,status_code:201';
        var orderBy = subject:desc;


		var result = FaxController.getFaxHistory(dateFrom, dateTo, q, orderBy);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function listOfFaxDeliveryReceipts()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, FaxController, ListOfFaxDeliveryReceiptsResponse){


		var result = FaxController.listOfFaxDeliveryReceipts();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function getASpecificFaxDeliveryReceipt(messageId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | D2AF-479B-8955-6395D561DEF4" (required, number) - Message ID. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, FaxController, GetASpecificFaxDeliveryReceiptResponse){
        var messageId = "3FAC74F1;


		var result = FaxController.getASpecificFaxDeliveryReceipt(messageId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function updateMarkFaxDeliveryReceiptsAsRead(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, FaxController, MarkFaxDeliveryReceiptsAsReadResponse){
        var body = new MarkFaxDeliveryReceiptsAsReadRequest({    "date_before": 1441958441});


		var result = FaxController.updateMarkFaxDeliveryReceiptsAsRead(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function addATestDeliveryReceipt(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, FaxController, AddATestDeliveryReceiptResponse){
        var body = new AddATestDeliveryReceiptRequest(    {        "url":"http://yourUrl.com"    });


		var result = FaxController.addATestDeliveryReceipt(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="forgot_account_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ForgotAccountController") ForgotAccountController

### Get singleton instance

The singleton instance of the ``` ForgotAccountController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, ForgotAccountController, ForgotUsernameResponse, ForgotPasswordResponse, VerifyForgotPasswordResponse){
	});
```

### <a name="update_forgot_username"></a>![Method: ](https://apidocs.io/img/method.png ".ForgotAccountController.updateForgotUsername") updateForgotUsername

> TODO: Add a method description


```javascript
function updateForgotUsername(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ForgotAccountController, ForgotUsernameResponse){
        var body = new ForgotUsernameRequest({"key":"value"});


		var result = ForgotAccountController.updateForgotUsername(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_forgot_password"></a>![Method: ](https://apidocs.io/img/method.png ".ForgotAccountController.updateForgotPassword") updateForgotPassword

> TODO: Add a method description


```javascript
function updateForgotPassword(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ForgotAccountController, ForgotPasswordResponse){
        var body = new ForgotPasswordRequest(    {        "username": "0F6pKiiuca"    });


		var result = ForgotAccountController.updateForgotPassword(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_verify_forgot_password"></a>![Method: ](https://apidocs.io/img/method.png ".ForgotAccountController.updateVerifyForgotPassword") updateVerifyForgotPassword

> TODO: Add a method description


```javascript
function updateVerifyForgotPassword(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ForgotAccountController, VerifyForgotPasswordResponse){
        var body = new VerifyForgotPasswordRequest(    {        "subaccount_id": 54,        "activation_token": "9C648BAD-EB7F-4E7E-96BC-B433140C4F1F",        "password": "0F6pKiiuca"    });


		var result = ForgotAccountController.updateVerifyForgotPassword(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="mms_controller"></a>![Class: ](https://apidocs.io/img/class.png ".MMSController") MMSController

### Get singleton instance

The singleton instance of the ``` MMSController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, MMSController, SendMMSResponse, GetPriceResponse, GetMMSHistoryResponse, ExportMMSHistoryResponse, CancelMMSResponse, CancelAllMMSResponse, GetAllDeliveryReceiptsResponse, GetDeliveryReceiptResponse, MarkReceiptsAsReadResponse){
	});
```

### <a name="create_send_mms"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.createSendMMS") createSendMMS

> TODO: Add a method description


```javascript
function createSendMMS(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, MMSController, SendMMSResponse){
        var body = new SendMMSRequest({"key":"value"});


		var result = MMSController.createSendMMS(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_get_price"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.createGetPrice") createGetPrice

> TODO: Add a method description


```javascript
function createGetPrice(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, MMSController, GetPriceResponse){
        var body = new GetPriceRequest({"key":"value"});


		var result = MMSController.createGetPrice(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_mms_history"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.getMMSHistory") getMMSHistory

> TODO: Add a method description


```javascript
function getMMSHistory(q, orderBy, dateFrom, dateTo)
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


	app.controller("testController", function($scope, MMSController, GetMMSHistoryResponse){
        var q = 'list_id:429,direction:out';
        var orderBy = subject:desc;
        var dateFrom = 1443501617;
        var dateTo = 1443501727;


		var result = MMSController.getMMSHistory(q, orderBy, dateFrom, dateTo);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_export_mms_history"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.getExportMMSHistory") getExportMMSHistory

> TODO: Add a method description


```javascript
function getExportMMSHistory(filename)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | Your export filename. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, MMSController, ExportMMSHistoryResponse){
        var filename = 'export.csv';


		var result = MMSController.getExportMMSHistory(filename);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_cancel_mms"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.updateCancelMMS") updateCancelMMS

> TODO: Add a method description


```javascript
function updateCancelMMS(messageId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Message ID. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, MMSController, CancelMMSResponse){
        var messageId = message_id;


		var result = MMSController.updateCancelMMS(messageId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_cancel_all_mms"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.updateCancelAllMMS") updateCancelAllMMS

> TODO: Add a method description


```javascript
function updateCancelAllMMS()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, MMSController, CancelAllMMSResponse){


		var result = MMSController.updateCancelAllMMS();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_all_delivery_receipts"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.getAllDeliveryReceipts") getAllDeliveryReceipts

> TODO: Add a method description


```javascript
function getAllDeliveryReceipts()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, MMSController, GetAllDeliveryReceiptsResponse){


		var result = MMSController.getAllDeliveryReceipts();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_delivery_receipt"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.getDeliveryReceipt") getDeliveryReceipt

> TODO: Add a method description


```javascript
function getDeliveryReceipt(messageId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Message ID. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, MMSController, GetDeliveryReceiptResponse){
        var messageId = 3E0DC217-7D0F-4C20-A3F2-E3362B938CAF;


		var result = MMSController.getDeliveryReceipt(messageId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_mark_receipts_as_read"></a>![Method: ](https://apidocs.io/img/method.png ".MMSController.updateMarkReceiptsAsRead") updateMarkReceiptsAsRead

> TODO: Add a method description


```javascript
function updateMarkReceiptsAsRead()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, MMSController, MarkReceiptsAsReadResponse){


		var result = MMSController.updateMarkReceiptsAsRead();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function getAllInboundSMSPull()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, MMSController){


		var result = MMSController.getAllInboundSMSPull();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="numbers_controller"></a>![Class: ](https://apidocs.io/img/class.png ".NumbersController") NumbersController

### Get singleton instance

The singleton instance of the ``` NumbersController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, NumbersController, GetAllDedicatedNumbersResponse, BuyDedicatedNumberResponse, SearchDedicatedNumbersByCountryResponse){
	});
```

### <a name="get_all_dedicated_numbers"></a>![Method: ](https://apidocs.io/img/method.png ".NumbersController.getAllDedicatedNumbers") getAllDedicatedNumbers

> TODO: Add a method description


```javascript
function getAllDedicatedNumbers()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, NumbersController, GetAllDedicatedNumbersResponse){


		var result = NumbersController.getAllDedicatedNumbers();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_buy_dedicated_number"></a>![Method: ](https://apidocs.io/img/method.png ".NumbersController.createBuyDedicatedNumber") createBuyDedicatedNumber

> TODO: Add a method description


```javascript
function createBuyDedicatedNumber(dedicatedNumber)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dedicatedNumber |  ``` Required ```  | Your phone number in E.164 format. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, NumbersController, BuyDedicatedNumberResponse){
        var dedicatedNumber = +12282060576;


		var result = NumbersController.createBuyDedicatedNumber(dedicatedNumber);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="search_dedicated_numbers_by_country"></a>![Method: ](https://apidocs.io/img/method.png ".NumbersController.searchDedicatedNumbersByCountry") searchDedicatedNumbersByCountry

> TODO: Add a method description


```javascript
function searchDedicatedNumbersByCountry(country, search, searchType)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Required ```  | Your preferred country. |
| search |  ``` Optional ```  | Your search pattern or query. |
| searchType |  ``` Optional ```  | Your strategy for searching, 0 = starts with, 1 = anywhere, 2 = ends with. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, NumbersController, SearchDedicatedNumbersByCountryResponse){
        var country = 'US';
        var search = '88';
        var searchType = 1;


		var result = NumbersController.searchDedicatedNumbersByCountry(country, search, searchType);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="pricing_controller"></a>![Class: ](https://apidocs.io/img/class.png ".PricingController") PricingController

### Get singleton instance

The singleton instance of the ``` PricingController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, PricingController, GetCountryPricingResponse){
	});
```

### <a name="get_country_pricing"></a>![Method: ](https://apidocs.io/img/method.png ".PricingController.getCountryPricing") getCountryPricing

> TODO: Add a method description


```javascript
function getCountryPricing(country, currency)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Required ```  | Two-letter representation of the country. |
| currency |  ``` Optional ```  | Three-letter representation of the currency. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, PricingController, GetCountryPricingResponse){
        var country = 'AU';
        var currency = 'AUD';


		var result = PricingController.getCountryPricing(country, currency);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="post_direct_mail_controller"></a>![Class: ](https://apidocs.io/img/class.png ".PostDirectMailController") PostDirectMailController

### Get singleton instance

The singleton instance of the ``` PostDirectMailController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, PostDirectMailController, SearchLocationsResponse, CreateNewCampaignResponse, CalculateDirectMailCampaignPriceResponse, ListDirectMailCampaignsResponse){
	});
```

### <a name="search_locations"></a>![Method: ](https://apidocs.io/img/method.png ".PostDirectMailController.searchLocations") searchLocations

> TODO: Add a method description


```javascript
function searchLocations(country, query)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| country |  ``` Required ```  | Country code. |
| query |  ``` Required ```  | A postal code or place name. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, PostDirectMailController, SearchLocationsResponse){
        var country = 'AD';
        var query = 'AD100';


		var result = PostDirectMailController.searchLocations(country, query);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_new_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".PostDirectMailController.createNewCampaign") createNewCampaign

> Create new direct mail campaign.


```javascript
function createNewCampaign(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, PostDirectMailController, CreateNewCampaignResponse){
        var body = new CreateNewCampaignRequest({"key":"value"});


		var result = PostDirectMailController.createNewCampaign(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_calculate_direct_mail_campaign_price"></a>![Method: ](https://apidocs.io/img/method.png ".PostDirectMailController.createCalculateDirectMailCampaignPrice") createCalculateDirectMailCampaignPrice

> Calculate direct mail campaign price.


```javascript
function createCalculateDirectMailCampaignPrice(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, PostDirectMailController, CalculateDirectMailCampaignPriceResponse){
        var body = new CalculateDirectMailCampaignPriceRequest({"key":"value"});


		var result = PostDirectMailController.createCalculateDirectMailCampaignPrice(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="list_direct_mail_campaigns"></a>![Method: ](https://apidocs.io/img/method.png ".PostDirectMailController.listDirectMailCampaigns") listDirectMailCampaigns

> Get list of direct mail campaigns.


```javascript
function listDirectMailCampaigns()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, PostDirectMailController, ListDirectMailCampaignsResponse){


		var result = PostDirectMailController.listDirectMailCampaigns();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="post_letter_controller"></a>![Class: ](https://apidocs.io/img/class.png ".PostLetterController") PostLetterController

### Get singleton instance

The singleton instance of the ``` PostLetterController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, PostLetterController, SendPostLetterResponse, CalculatePriceResponse, GetPostLetterHistoryResponse, ExportPostLetterHistoryResponse, CreateAPostReturnAddressResponse, GetListOfPostReturnAddressesResponse, GetPostReturnAddressResponse, UpdatePostReturnAddressResponse, DeletePostReturnAddressResponse){
	});
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
function createSendPostLetter(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, PostLetterController, SendPostLetterResponse){
        var body = new SendPostLetterRequest({  "file_url": "http://server.com/file.pdf",  "template_used": 1,  "colour": 1,  "duplex": 0,  "recipients": [    {      "address_name": "My Home Address",      "address_line_1": "Address 1",      "address_line_2": "Address 2",      "address_city": "CITY",      "address_state": "State",      "address_postal_code": 123456,      "address_country": "AU",      "return_address_id": 1,      "schedule": 1449573604    }  ]});


		var result = PostLetterController.createSendPostLetter(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.createCalculatePrice") createCalculatePrice

> TODO: Add a method description


```javascript
function createCalculatePrice(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, PostLetterController, CalculatePriceResponse){
        var body = new CalculatePriceRequest170({  "file_url": "http://server.com/file.pdf",  "template_used": 1,  "colour": 1,  "duplex": 0,  "recipients": [    "[]"  ],  "Body": ""});


		var result = PostLetterController.createCalculatePrice(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_post_letter_history"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.getPostLetterHistory") getPostLetterHistory

> TODO: Add a method description


```javascript
function getPostLetterHistory()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, PostLetterController, GetPostLetterHistoryResponse){


		var result = PostLetterController.getPostLetterHistory();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_export_post_letter_history"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.getExportPostLetterHistory") getExportPostLetterHistory

> TODO: Add a method description


```javascript
function getExportPostLetterHistory(filename)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | Filename for the export file. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, PostLetterController, ExportPostLetterHistoryResponse){
        var filename = 'myexport.csv';


		var result = PostLetterController.getExportPostLetterHistory(filename);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_a_post_return_address"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.createAPostReturnAddress") createAPostReturnAddress

> TODO: Add a method description


```javascript
function createAPostReturnAddress(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, PostLetterController, CreateAPostReturnAddressResponse){
        var body = new CreateAPostReturnAddressRequest({    "address_name":"My Home Address",    "address_line_1":"Maritime Avenue",    "address_line_2":"",    "address_city":"Flynn",    "address_state":"WA",    "address_postal_code":6302,    "address_country":"Australia"});


		var result = PostLetterController.createAPostReturnAddress(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_list_of_post_return_addresses"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.getListOfPostReturnAddresses") getListOfPostReturnAddresses

> TODO: Add a method description


```javascript
function getListOfPostReturnAddresses()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, PostLetterController, GetListOfPostReturnAddressesResponse){


		var result = PostLetterController.getListOfPostReturnAddresses();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_post_return_address"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.getPostReturnAddress") getPostReturnAddress

> TODO: Add a method description


```javascript
function getPostReturnAddress(returnAddressId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| returnAddressId |  ``` Required ```  | Your return address id. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, PostLetterController, GetPostReturnAddressResponse){
        var returnAddressId = 14;


		var result = PostLetterController.getPostReturnAddress(returnAddressId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_post_return_address"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.updatePostReturnAddress") updatePostReturnAddress

> TODO: Add a method description


```javascript
function updatePostReturnAddress(returnAddressId, body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| returnAddressId |  ``` Required ```  | Your return address id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, PostLetterController, UpdatePostReturnAddressResponse){
        var returnAddressId = 14;
        var body = new UpdatePostReturnAddressRequest({    "address_name":"My Home Address",    "address_line_1":"Maritime Avenue",    "address_line_2":"",    "address_city":"Flynn",    "address_state":"WA",    "address_postal_code":6302,    "address_country":"Australia"});


		var result = PostLetterController.updatePostReturnAddress(returnAddressId, body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="delete_post_return_address"></a>![Method: ](https://apidocs.io/img/method.png ".PostLetterController.deletePostReturnAddress") deletePostReturnAddress

> TODO: Add a method description


```javascript
function deletePostReturnAddress(returnAddressId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| returnAddressId |  ``` Required ```  | Your return address id. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, PostLetterController, DeletePostReturnAddressResponse){
        var returnAddressId = 12;


		var result = PostLetterController.deletePostReturnAddress(returnAddressId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="postcards_controller"></a>![Class: ](https://apidocs.io/img/class.png ".PostcardsController") PostcardsController

### Get singleton instance

The singleton instance of the ``` PostcardsController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, PostcardsController, SendPostcardResponse, CalculatePricingResponse, GetPostcardHistoryResponse, ExportPostcardHistoryResponse){
	});
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
function createSendPostcard(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, PostcardsController, SendPostcardResponse){
        var body = new SendPostcardRequest({    "file_urls":[         "https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_front.pdf",         "https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_back.pdf"    ],    "recipients":[        {            "address_name":"My Home Address",            "address_line_1":"Address 1",            "address_line_2":"",            "address_city":"City",            "address_state":"State",            "address_postal_code":"123456",            "address_country":"AU",            "return_address_id":1        }    ]});


		var result = PostcardsController.createSendPostcard(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_calculate_pricing"></a>![Method: ](https://apidocs.io/img/method.png ".PostcardsController.createCalculatePricing") createCalculatePricing

> For `file_urls` field. You can attach at least 1 and max of 2 PDF file urls.
> - Supply a single pdf with 2 pages (front and back)
> - Supply 2 urls to seperate PDFs


```javascript
function createCalculatePricing(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, PostcardsController, CalculatePricingResponse){
        var body = new CalculatePricingRequest({    "file_urls":[        "https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_front.pdf",        "https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_back.pdf"    ],    "recipients":[        {            "address_name":"My Home Address",            "address_line_1":"Address 1",            "address_line_2":"",            "address_city":"City",            "address_state":"State",            "address_postal_code":"123456",            "address_country":"AU",            "return_address_id":1        }    ]});


		var result = PostcardsController.createCalculatePricing(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_postcard_history"></a>![Method: ](https://apidocs.io/img/method.png ".PostcardsController.getPostcardHistory") getPostcardHistory

> TODO: Add a method description


```javascript
function getPostcardHistory()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, PostcardsController, GetPostcardHistoryResponse){


		var result = PostcardsController.getPostcardHistory();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_export_postcard_history"></a>![Method: ](https://apidocs.io/img/method.png ".PostcardsController.getExportPostcardHistory") getExportPostcardHistory

> TODO: Add a method description


```javascript
function getExportPostcardHistory(filename)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | Filename for the export file. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, PostcardsController, ExportPostcardHistoryResponse){
        var filename = 'myexport.csv';


		var result = PostcardsController.getExportPostcardHistory(filename);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="referral_accounts_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ReferralAccountsController") ReferralAccountsController

### Get singleton instance

The singleton instance of the ``` ReferralAccountsController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, ReferralAccountsController, GetListOfReferralAccountsResponse){
	});
```

### <a name="get_list_of_referral_accounts"></a>![Method: ](https://apidocs.io/img/method.png ".ReferralAccountsController.getListOfReferralAccounts") getListOfReferralAccounts

> TODO: Add a method description


```javascript
function getListOfReferralAccounts()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, ReferralAccountsController, GetListOfReferralAccountsResponse){


		var result = ReferralAccountsController.getListOfReferralAccounts();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="reseller_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ResellerController") ResellerController

### Get singleton instance

The singleton instance of the ``` ResellerController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, ResellerController, GetResellerSettingResponse, UpdateResellerSettingResponse, ResellerBySubdomainResponse){
	});
```

### <a name="get_reseller_setting"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerController.getResellerSetting") getResellerSetting

> Get reseller setting.


```javascript
function getResellerSetting()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, ResellerController, GetResellerSettingResponse){


		var result = ResellerController.getResellerSetting();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_reseller_setting"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerController.updateResellerSetting") updateResellerSetting

> Update a specific reseller setting.


```javascript
function updateResellerSetting(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ResellerController, UpdateResellerSettingResponse){
        var body = new UpdateResellerSettingRequest(    {        "allow_public_signups":1,        "default_margin":100,        "default_margin_numbers":150,        "trial_balance":50,        "subdomain":"subdomain",        "colour_navigation":"#9999FF",        "logo_url_light":"http://url.com/light",        "logo_url_dark":"http://url.com/dark",        "company_name":"MyCompany"    });


		var result = ResellerController.updateResellerSetting(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_reseller_by_subdomain"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerController.getResellerBySubdomain") getResellerBySubdomain

> Get reseller setting by subdomin.


```javascript
function getResellerBySubdomain(subdomain)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subdomain |  ``` Required ```  | Subdomain |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ResellerController, ResellerBySubdomainResponse){
        var subdomain = 'mysubdomain';


		var result = ResellerController.getResellerBySubdomain(subdomain);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="reseller_accounts_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ResellerAccountsController") ResellerAccountsController

### Get singleton instance

The singleton instance of the ``` ResellerAccountsController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, ResellerAccountsController, ListOfResellerAccountsResponse, GetResellerAccountResponse, CreateResellerAccountResponse, CreateResellerAccountPublicResponse, UpdateResellerAccountResponse, TransferCreditResponse){
	});
```

### <a name="list_of_reseller_accounts"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.listOfResellerAccounts") listOfResellerAccounts

> Get list of Reseller Accounts


```javascript
function listOfResellerAccounts()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, ResellerAccountsController, ListOfResellerAccountsResponse){


		var result = ResellerAccountsController.listOfResellerAccounts();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_reseller_account"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.getResellerAccount") getResellerAccount

> Get a specific reseller account.


```javascript
function getResellerAccount(clientUserId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| clientUserId |  ``` Required ```  | The client user id. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ResellerAccountsController, GetResellerAccountResponse){
        var clientUserId = 24;


		var result = ResellerAccountsController.getResellerAccount(clientUserId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_reseller_account"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.createResellerAccount") createResellerAccount

> TODO: Add a method description


```javascript
function createResellerAccount(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ResellerAccountsController, CreateResellerAccountResponse){
        var body = new CreateResellerAccountRequest(    {        "username":"johndoe2",        "user_email":"johndoe2@awesome.com",        "user_phone":"518-481-1002",        "user_first_name":"John",        "user_last_name":"Doe",        "country":"US",        "password":"pass",        "account_name":"The Awesome Company"    });


		var result = ResellerAccountsController.createResellerAccount(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_reseller_account_public"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.createResellerAccountPublic") createResellerAccountPublic

> TODO: Add a method description


```javascript
function createResellerAccountPublic(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ResellerAccountsController, CreateResellerAccountPublicResponse){
        var body = new CreateResellerAccountPublicRequest({    "reseller_user_id":1,    "username":"john_awesome",    "user_email":"johnis@awesome.com",    "user_phone":"+61261063270",    "user_first_name":"John",    "user_last_name":"Awesome",    "country":"AU",    "password":"pass",    "account_name":"The Awesome Company"});


		var result = ResellerAccountsController.createResellerAccountPublic(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_reseller_account"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.updateResellerAccount") updateResellerAccount

> TODO: Add a method description


```javascript
function updateResellerAccount(clientUserId, body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| clientUserId |  ``` Required ```  | Your client user id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ResellerAccountsController, UpdateResellerAccountResponse){
        var clientUserId = 24;
        var body = new UpdateResellerAccountRequest(    {        "username":"johndoe2",        "user_email":"johndoe2@awesome.com",        "user_phone":"518-481-1002",        "user_first_name":"John",        "user_last_name":"Doe",        "country":"US",        "password":"pass",        "account_name":"The Awesome Company"    });


		var result = ResellerAccountsController.updateResellerAccount(clientUserId, body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_transfer_credit"></a>![Method: ](https://apidocs.io/img/method.png ".ResellerAccountsController.updateTransferCredit") updateTransferCredit

> TODO: Add a method description


```javascript
function updateTransferCredit(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ResellerAccountsController, TransferCreditResponse){
        var body = new TransferCreditRequest({"key":"value"});


		var result = ResellerAccountsController.updateTransferCredit(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="sdk_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SDKController") SDKController

### Get singleton instance

The singleton instance of the ``` SDKController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, SDKController){
	});
```

### <a name="get_sdk_download"></a>![Method: ](https://apidocs.io/img/method.png ".SDKController.getSDKDownload") getSDKDownload

> TODO: Add a method description


```javascript
function getSDKDownload(type)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| type |  ``` Required ```  | Supported types. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SDKController){
        var type = 'type';


		var result = SDKController.getSDKDownload(type);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="search_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SearchController") SearchController

### Get singleton instance

The singleton instance of the ``` SearchController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, SearchController, SearchContactsListsResponse){
	});
```

### <a name="search_contacts_lists"></a>![Method: ](https://apidocs.io/img/method.png ".SearchController.searchContactsLists") searchContactsLists

> TODO: Add a method description


```javascript
function searchContactsLists(q)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| q |  ``` Required ```  | Your keyword or query. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SearchController, SearchContactsListsResponse){
        var q = 'Gorne';


		var result = SearchController.searchContactsLists(q);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="sms_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SMSController") SMSController

### Get singleton instance

The singleton instance of the ``` SMSController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, SMSController, SendAnSMSResponse, CalculatePriceResponse, GetAllHistoryResponse, ExportSMSHistoryResponse, GetAllDeliveryReceiptsResponse, GetASpecificDeliveryReceiptResponse, AddATestDeliveryReceiptResponse, MarkDeliveryReceiptsAsReadResponse, GetAllInboundSMSPullResponse, GetSpecificInboundPullResponse, AddATestInboundSMSResponse, MarkASpecificInboundSMSAsReadResponse, MarkAllInboundSMSAsReadResponse, CancelAScheduledMessageResponse, CancelAllScheduledMessagesResponse){
	});
```

### <a name="create_send_an_sms"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.createSendAnSMS") createSendAnSMS

> You can post **up to 1000 messages** with each API call.


```javascript
function createSendAnSMS(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SMSController, SendAnSMSResponse){
        var body = new SendAnSMSRequest({"key":"value"});


		var result = SMSController.createSendAnSMS(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.createCalculatePrice") createCalculatePrice

> TODO: Add a method description


```javascript
function createCalculatePrice(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SMSController, CalculatePriceResponse){
        var body = new CalculatePriceRequest205({"key":"value"});


		var result = SMSController.createCalculatePrice(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function getAllHistory(dateFrom, dateTo)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateFrom |  ``` Optional ```  | Timestamp (from) used to show records by date. |
| dateTo |  ``` Optional ```  | Timestamp (to) used to show recrods by date. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SMSController, GetAllHistoryResponse){
        var dateFrom = 1449459940;
        var dateTo = 1449659940;


		var result = SMSController.getAllHistory(dateFrom, dateTo);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_export_sms_history"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.getExportSMSHistory") getExportSMSHistory

> TODO: Add a method description


```javascript
function getExportSMSHistory()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, SMSController, ExportSMSHistoryResponse){


		var result = SMSController.getExportSMSHistory();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function getAllDeliveryReceipts()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, SMSController, GetAllDeliveryReceiptsResponse){


		var result = SMSController.getAllDeliveryReceipts();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function getASpecificDeliveryReceipt(messageId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Your message id. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SMSController, GetASpecificDeliveryReceiptResponse){
        var messageId = 88AB118E EB1B 478C 98CE 6C73ABA23F67;


		var result = SMSController.getASpecificDeliveryReceipt(messageId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function addATestDeliveryReceipt(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SMSController, AddATestDeliveryReceiptResponse){
        var body = new AddATestDeliveryReceiptRequest(    {        "url":"http://yourUrl.com"    });


		var result = SMSController.addATestDeliveryReceipt(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function updateMarkDeliveryReceiptsAsRead(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SMSController, MarkDeliveryReceiptsAsReadResponse){
        var body = new MarkDeliveryReceiptsAsReadRequest({    "date_before": 1441958441});


		var result = SMSController.updateMarkDeliveryReceiptsAsRead(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function getAllInboundSMSPull()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, SMSController, GetAllInboundSMSPullResponse){


		var result = SMSController.getAllInboundSMSPull();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function getSpecificInboundPull(messageId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Message ID. Must be a valid GUID. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SMSController, GetSpecificInboundPullResponse){
        var messageId = 5D420421-8715-4461-A9A2-C8F569E41835;


		var result = SMSController.getSpecificInboundPull(messageId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function addATestInboundSMS(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SMSController, AddATestInboundSMSResponse){
        var body = new AddATestInboundSMSRequest(    {        "url":"http://yourUrl.com"    });


		var result = SMSController.addATestInboundSMS(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function updateMarkASpecificInboundSMSAsRead(messageId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | B7CE432193CD-0753597B7293 (string, required) - The message ID you want to mark as read. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SMSController, MarkASpecificInboundSMSAsReadResponse){
        var messageId = 307EF035;


		var result = SMSController.updateMarkASpecificInboundSMSAsRead(messageId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function updateMarkAllInboundSMSAsRead(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SMSController, MarkAllInboundSMSAsReadResponse){
        var body = new MarkAllInboundSMSAsReadRequest(    {        "date_before":1442398100    });


		var result = SMSController.updateMarkAllInboundSMSAsRead(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_cancel_a_scheduled_message"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.updateCancelAScheduledMessage") updateCancelAScheduledMessage

> TODO: Add a method description


```javascript
function updateCancelAScheduledMessage(messageId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | B7CE432193CD-0753597B7293 (string, required) - The message ID you want to cancel. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SMSController, CancelAScheduledMessageResponse){
        var messageId = 307EF035;


		var result = SMSController.updateCancelAScheduledMessage(messageId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_cancel_all_scheduled_messages"></a>![Method: ](https://apidocs.io/img/method.png ".SMSController.updateCancelAllScheduledMessages") updateCancelAllScheduledMessages

> TODO: Add a method description


```javascript
function updateCancelAllScheduledMessages()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, SMSController, CancelAllScheduledMessagesResponse){


		var result = SMSController.updateCancelAllScheduledMessages();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="sms_campaigns_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SMSCampaignsController") SMSCampaignsController

### Get singleton instance

The singleton instance of the ``` SMSCampaignsController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, SMSCampaignsController, CreateSMSCampaignResponse, CalculatePriceForSMSCampaignResponse, UpdateAnSMSCampaignResponse, GetSMSCampaignResponse, CancelAnSMSCampaignResponse, GetListOfSMSCampaignsResponse){
	});
```

### <a name="create_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.createSMSCampaign") createSMSCampaign

> You can post to a list with **up to 20000 recipients** with each API call.


```javascript
function createSMSCampaign(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SMSCampaignsController, CreateSMSCampaignResponse){
        var body = new CreateSMSCampaignRequest({    "list_id":428,    "name":"My Campaign 1",    "from":"+61353787448",    "body":"This is my new campaign message.",    "schedule":1444821615});


		var result = SMSCampaignsController.createSMSCampaign(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_calculate_price_for_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.createCalculatePriceForSMSCampaign") createCalculatePriceForSMSCampaign

> TODO: Add a method description


```javascript
function createCalculatePriceForSMSCampaign(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SMSCampaignsController, CalculatePriceForSMSCampaignResponse){
        var body = new CalculatePriceForSMSCampaignRequest({    "list_id":428,    "name":"My Campaign 1",    "from":"+61353787448",    "body":"(First Name), this is your new campaign message."});


		var result = SMSCampaignsController.createCalculatePriceForSMSCampaign(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_an_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.updateAnSMSCampaign") updateAnSMSCampaign

> TODO: Add a method description


```javascript
function updateAnSMSCampaign(smsCampaignId, body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| smsCampaignId |  ``` Required ```  | Your SMS Campaign id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SMSCampaignsController, UpdateAnSMSCampaignResponse){
        var smsCampaignId = 1;
        var body = new UpdateAnSMSCampaignRequest({    "list_id":428,    "name":"Awesome campaign.",    "from":"+61353787447",    "body":"his is an awesome message.",    "schedule":1444821615});


		var result = SMSCampaignsController.updateAnSMSCampaign(smsCampaignId, body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.getSMSCampaign") getSMSCampaign

> TODO: Add a method description


```javascript
function getSMSCampaign(smsCampaignId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| smsCampaignId |  ``` Required ```  | Your SMS campaign id. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SMSCampaignsController, GetSMSCampaignResponse){
        var smsCampaignId = 1;


		var result = SMSCampaignsController.getSMSCampaign(smsCampaignId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_cancel_an_sms_campaign"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.updateCancelAnSMSCampaign") updateCancelAnSMSCampaign

> TODO: Add a method description


```javascript
function updateCancelAnSMSCampaign(smsCampaignId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| smsCampaignId |  ``` Required ```  | Your SMS Campaign id. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SMSCampaignsController, CancelAnSMSCampaignResponse){
        var smsCampaignId = 1;


		var result = SMSCampaignsController.updateCancelAnSMSCampaign(smsCampaignId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_list_of_sms_campaigns"></a>![Method: ](https://apidocs.io/img/method.png ".SMSCampaignsController.getListOfSMSCampaigns") getListOfSMSCampaigns

> TODO: Add a method description


```javascript
function getListOfSMSCampaigns()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, SMSCampaignsController, GetListOfSMSCampaignsResponse){


		var result = SMSCampaignsController.getListOfSMSCampaigns();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="sms_templates_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SMSTemplatesController") SMSTemplatesController

### Get singleton instance

The singleton instance of the ``` SMSTemplatesController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, SMSTemplatesController, ListOfTemplatesResponse, CreateATemplateResponse, UpdateATemplateResponse, DeleteATemplateResponse){
	});
```

### <a name="list_of_templates"></a>![Method: ](https://apidocs.io/img/method.png ".SMSTemplatesController.listOfTemplates") listOfTemplates

> Get list of templates.


```javascript
function listOfTemplates()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, SMSTemplatesController, ListOfTemplatesResponse){


		var result = SMSTemplatesController.listOfTemplates();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_a_template"></a>![Method: ](https://apidocs.io/img/method.png ".SMSTemplatesController.createATemplate") createATemplate

> Create new template.


```javascript
function createATemplate(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SMSTemplatesController, CreateATemplateResponse){
        var body = new CreateATemplateRequest(    {        "template_name":"Template 501916",        "body":"This is a sample content: H7YI68B3yk for this template."    });


		var result = SMSTemplatesController.createATemplate(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_a_template"></a>![Method: ](https://apidocs.io/img/method.png ".SMSTemplatesController.updateATemplate") updateATemplate

> TODO: Add a method description


```javascript
function updateATemplate(templateId, body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SMSTemplatesController, UpdateATemplateResponse){
        var templateId = 25;
        var body = new UpdateATemplateRequest(    {        "template_name":"I am updated",        "body":"This is a sample content: Sc0KNWgSMG for this template."    });


		var result = SMSTemplatesController.updateATemplate(templateId, body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="delete_a_template"></a>![Method: ](https://apidocs.io/img/method.png ".SMSTemplatesController.deleteATemplate") deleteATemplate

> TODO: Add a method description


```javascript
function deleteATemplate(templateId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| templateId |  ``` Required ```  | Your template id. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SMSTemplatesController, DeleteATemplateResponse){
        var templateId = 25;


		var result = SMSTemplatesController.deleteATemplate(templateId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="statistics_controller"></a>![Class: ](https://apidocs.io/img/class.png ".StatisticsController") StatisticsController

### Get singleton instance

The singleton instance of the ``` StatisticsController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, StatisticsController, GetSMSStatisticsResponse, GetVoiceStatisticsResponse){
	});
```

### <a name="get_sms_statistics"></a>![Method: ](https://apidocs.io/img/method.png ".StatisticsController.getSMSStatistics") getSMSStatistics

> TODO: Add a method description


```javascript
function getSMSStatistics()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, StatisticsController, GetSMSStatisticsResponse){


		var result = StatisticsController.getSMSStatistics();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_voice_statistics"></a>![Method: ](https://apidocs.io/img/method.png ".StatisticsController.getVoiceStatistics") getVoiceStatistics

> TODO: Add a method description


```javascript
function getVoiceStatistics()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, StatisticsController, GetVoiceStatisticsResponse){


		var result = StatisticsController.getVoiceStatistics();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="subaccounts_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SubaccountsController") SubaccountsController

### Get singleton instance

The singleton instance of the ``` SubaccountsController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, SubaccountsController, GetAllSubaccountsResponse, CreateANewSubaccountResponse, GetASpecificSubaccountResponse, UpdateASpecificSubaccountResponse, DeleteASpecificSubaccountResponse, RegenerateAPIKeyResponse){
	});
```

### <a name="get_all_subaccounts"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.getAllSubaccounts") getAllSubaccounts

> TODO: Add a method description


```javascript
function getAllSubaccounts()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, SubaccountsController, GetAllSubaccountsResponse){


		var result = SubaccountsController.getAllSubaccounts();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_a_new_subaccount"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.createANewSubaccount") createANewSubaccount

> TODO: Add a method description


```javascript
function createANewSubaccount(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SubaccountsController, CreateANewSubaccountResponse){
        var body = new CreateANewSubaccountRequest(    {        "api_username":"nameP99",        "password":"pass",        "email":"testvrq@gmail.com",        "phone_number":"941-751-3278",        "first_name":"FirstnameeGPqV",        "last_name":"LastnamePvjJp"    });


		var result = SubaccountsController.createANewSubaccount(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_a_specific_subaccount"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.getASpecificSubaccount") getASpecificSubaccount

> TODO: Add a method description


```javascript
function getASpecificSubaccount(subaccountId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SubaccountsController, GetASpecificSubaccountResponse){
        var subaccountId = 59;


		var result = SubaccountsController.getASpecificSubaccount(subaccountId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_a_specific_subaccount"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.updateASpecificSubaccount") updateASpecificSubaccount

> TODO: Add a method description


```javascript
function updateASpecificSubaccount(subaccountId, body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SubaccountsController, UpdateASpecificSubaccountResponse){
        var subaccountId = 59;
        var body = new UpdateASpecificSubaccountRequest(    {        "password":"pass",        "email":"testfP0.updated@gmail.com",        "phone_number":"+19417519130",        "first_name":"FirstnameKvdRZUpdated",        "last_name":"LastnameHUPYGUpdated",        "access_users": 1,        "access_billing": 1,        "access_reporting": 1,        "access_contacts": 1,        "access_settings": 1,        "access_sms": 1,        "access_email": 1,        "access_voice": 1,        "access_fax": 1,        "access_post": 1,        "access_reseller": 1,        "access_mms": 1,        "share_campaigns": 0,        "notes": null    });


		var result = SubaccountsController.updateASpecificSubaccount(subaccountId, body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="delete_a_specific_subaccount"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.deleteASpecificSubaccount") deleteASpecificSubaccount

> TODO: Add a method description


```javascript
function deleteASpecificSubaccount(subaccountId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SubaccountsController, DeleteASpecificSubaccountResponse){
        var subaccountId = 59;


		var result = SubaccountsController.deleteASpecificSubaccount(subaccountId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_regenerate_api_key"></a>![Method: ](https://apidocs.io/img/method.png ".SubaccountsController.updateRegenerateAPIKey") updateRegenerateAPIKey

> TODO: Add a method description


```javascript
function updateRegenerateAPIKey(subaccountId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| subaccountId |  ``` Required ```  | The subaccount ID you want to access. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SubaccountsController, RegenerateAPIKeyResponse){
        var subaccountId = 59;


		var result = SubaccountsController.updateRegenerateAPIKey(subaccountId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="timezones_controller"></a>![Class: ](https://apidocs.io/img/class.png ".TimezonesController") TimezonesController

### Get singleton instance

The singleton instance of the ``` TimezonesController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, TimezonesController, GetTimezonesResponse){
	});
```

### <a name="get_timezones"></a>![Method: ](https://apidocs.io/img/method.png ".TimezonesController.getTimezones") getTimezones

> Get supported list of timezones.


```javascript
function getTimezones()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, TimezonesController, GetTimezonesResponse){


		var result = TimezonesController.getTimezones();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="transactional_email_controller"></a>![Class: ](https://apidocs.io/img/class.png ".TransactionalEmailController") TransactionalEmailController

### Get singleton instance

The singleton instance of the ``` TransactionalEmailController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, TransactionalEmailController, EmailSendResponse, EmailPriceResponse, EmailHistoryResponse, ExportHistoryResponse, AddATestDeliveryReceiptResponse){
	});
```

### <a name="create_email_send"></a>![Method: ](https://apidocs.io/img/method.png ".TransactionalEmailController.createEmailSend") createEmailSend

> TODO: Add a method description


```javascript
function createEmailSend(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, TransactionalEmailController, EmailSendResponse){
        var body = new EmailSendRequest({"key":"value"});


		var result = TransactionalEmailController.createEmailSend(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_email_price"></a>![Method: ](https://apidocs.io/img/method.png ".TransactionalEmailController.createEmailPrice") createEmailPrice

> TODO: Add a method description


```javascript
function createEmailPrice(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, TransactionalEmailController, EmailPriceResponse){
        var body = new EmailPriceRequest({"key":"value"});


		var result = TransactionalEmailController.createEmailPrice(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_email_history"></a>![Method: ](https://apidocs.io/img/method.png ".TransactionalEmailController.getEmailHistory") getEmailHistory

> TODO: Add a method description


```javascript
function getEmailHistory()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, TransactionalEmailController, EmailHistoryResponse){


		var result = TransactionalEmailController.getEmailHistory();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_export_history"></a>![Method: ](https://apidocs.io/img/method.png ".TransactionalEmailController.getExportHistory") getExportHistory

> TODO: Add a method description


```javascript
function getExportHistory(filename)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| filename |  ``` Required ```  | File name for the export file. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, TransactionalEmailController, ExportHistoryResponse){
        var filename = 'myexport.csv';


		var result = TransactionalEmailController.getExportHistory(filename);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function addATestDeliveryReceipt(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, TransactionalEmailController, AddATestDeliveryReceiptResponse){
        var body = new AddATestDeliveryReceiptRequest(    {        "url":"http://yourUrl.com"    });


		var result = TransactionalEmailController.addATestDeliveryReceipt(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="uploads_controller"></a>![Class: ](https://apidocs.io/img/class.png ".UploadsController") UploadsController

### Get singleton instance

The singleton instance of the ``` UploadsController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, UploadsController, UploadAFileResponse){
	});
```

### <a name="upload_a_file"></a>![Method: ](https://apidocs.io/img/method.png ".UploadsController.uploadAFile") uploadAFile

> The `upload` endpoint provides a method for converting files from an unspported format to a format that one of our endpoints can handle.
> Files can be submitted two ways:
> 1. Using `base64` encoding in an `application/json` request. In this case, submit the `base64`-encoded file contents in the `content` field of the request body, and `convert` can be specified either also in the body or as part of the query string.
> 2. Using `multipart/form-data` encoding, in the same way it would be submitted using a HTML form. You may find cURL useful for this. For an example of how to do this, see one of our [SDKs](https://dashboard.clicksend.com/#/libraries-sdk/main). In this case, specify `convert` in the query string.
> Note that `convert` specifies the conversion to take place - that is, what the result should be compatible with - and can be any of `fax`, `mms`, `csv` or `post`.
> All files have 10 minutes expiry.


```javascript
function uploadAFile(body, convert)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |
| convert |  ``` Optional ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, UploadsController, UploadAFileResponse){
        var body = new UploadAFileRequest({"key":"value"});
        var convert = 'convert';


		var result = UploadsController.uploadAFile(body, convert);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)

## <a name="voice_controller"></a>![Class: ](https://apidocs.io/img/class.png ".VoiceController") VoiceController

### Get singleton instance

The singleton instance of the ``` VoiceController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, VoiceController, SendAVoiceCallResponse, CalculatePriceResponse, VoiceLanguagesResponse, GetVoiceHistoryResponse, ExportVoiceHistoryResponse, GetVoiceReceiptsResponse, AddATestDeliveryReceiptResponse, GetSpecificVoiceReceiptResponse, MarkedVoiceReceiptsAsReadResponse, CancelASpecificVoiceCallResponse, CancelAllVoiceCallsResponse){
	});
```

### <a name="create_send_a_voice_call"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.createSendAVoiceCall") createSendAVoiceCall

> You can post **up to 1000 messages** with each API call.


```javascript
function createSendAVoiceCall(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, VoiceController, SendAVoiceCallResponse){
        var body = new SendAVoiceCallRequest({"key":"value"});


		var result = VoiceController.createSendAVoiceCall(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="create_calculate_price"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.createCalculatePrice") createCalculatePrice

> TODO: Add a method description


```javascript
function createCalculatePrice(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, VoiceController, CalculatePriceResponse){
        var body = new CalculatePriceRequest263({"key":"value"});


		var result = VoiceController.createCalculatePrice(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_voice_languages"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.getVoiceLanguages") getVoiceLanguages

> TODO: Add a method description


```javascript
function getVoiceLanguages()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, VoiceController, VoiceLanguagesResponse){


		var result = VoiceController.getVoiceLanguages();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_voice_history"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.getVoiceHistory") getVoiceHistory

> TODO: Add a method description


```javascript
function getVoiceHistory(dateFrom, dateTo)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateFrom |  ``` Optional ```  | Timestamp (from) used to show records by date. |
| dateTo |  ``` Optional ```  | Timestamp (to) used to show recrods by date. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, VoiceController, GetVoiceHistoryResponse){
        var dateFrom = 1443501617;
        var dateTo = 1443501727;


		var result = VoiceController.getVoiceHistory(dateFrom, dateTo);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="get_export_voice_history"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.getExportVoiceHistory") getExportVoiceHistory

> TODO: Add a method description


```javascript
function getExportVoiceHistory()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, VoiceController, ExportVoiceHistoryResponse){


		var result = VoiceController.getExportVoiceHistory();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function getVoiceReceipts()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, VoiceController, GetVoiceReceiptsResponse){


		var result = VoiceController.getVoiceReceipts();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function addATestDeliveryReceipt(body)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, VoiceController, AddATestDeliveryReceiptResponse){
        var body = new AddATestDeliveryReceiptRequest(    {        "url":"http://yourUrl.com"    });


		var result = VoiceController.addATestDeliveryReceipt(body);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function getSpecificVoiceReceipt(messageId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | 3055-45F1-9B79-F2C43509FD16 (string, required) - The voice receipt message id. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, VoiceController, GetSpecificVoiceReceiptResponse){
        var messageId = 28DD2718;


		var result = VoiceController.getSpecificVoiceReceipt(messageId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function updateMarkedVoiceReceiptsAsRead(dateBefore)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dateBefore |  ``` Required ```  | An optional timestamp - mark all as read before this timestamp. If not given, all receipts will be marked as read. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, VoiceController, MarkedVoiceReceiptsAsReadResponse){
        var dateBefore = 251.081640399565;


		var result = VoiceController.updateMarkedVoiceReceiptsAsRead(dateBefore);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_cancel_a_specific_voice_call"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.updateCancelASpecificVoiceCall") updateCancelASpecificVoiceCall

> TODO: Add a method description


```javascript
function updateCancelASpecificVoiceCall(messageId)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageId |  ``` Required ```  | Your voice message id. |



#### Example Usage

```javascript


	app.controller("testController", function($scope, VoiceController, CancelASpecificVoiceCallResponse){
        var messageId = 7B5BFC19 06B7 49C1 8DCDFB011600E12B;


		var result = VoiceController.updateCancelASpecificVoiceCall(messageId);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



### <a name="update_cancel_all_voice_calls"></a>![Method: ](https://apidocs.io/img/method.png ".VoiceController.updateCancelAllVoiceCalls") updateCancelAllVoiceCalls

> TODO: Add a method description


```javascript
function updateCancelAllVoiceCalls()
```

#### Example Usage

```javascript


	app.controller("testController", function($scope, VoiceController, CancelAllVoiceCallsResponse){


		var result = VoiceController.updateCancelAllVoiceCalls();
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```



[Back to List of Controllers](#list_of_controllers)



