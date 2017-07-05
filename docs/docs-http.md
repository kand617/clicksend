# 

TODO: Add a description



## Base URL

The Base URL for this API is `https://rest.clicksend.com/v3/`



## Authentication
The type of authentication used by this API is: `Basic Authentication`



# <a name="api_reference"></a>API Reference

* [Account](#account)
* [Account Recharge](#account_recharge)
* [Automation Rules](#automation_rules)
* [Contact Lists](#contact_lists)
* [Contact Suggestions](#contact_suggestions)
* [Contacts](#contacts)
* [Countries](#countries)
* [Delivery Issues](#delivery_issues)
* [Email Marketing](#email_marketing)
* [Email-to-SMS Allowed Address](#email_to_sms_allowed_address)
* [Email-to-SMS Stripped Strings](#email_to_sms_stripped_strings)
* [Fax](#fax)
* [Forgot Account](#forgot_account)
* [MMS](#mms)
* [Numbers](#numbers)
* [Pricing](#pricing)
* [Post Direct Mail](#post_direct_mail)
* [Post Letter](#post_letter)
* [Postcards](#postcards)
* [Referral Accounts](#referral_accounts)
* [Reseller](#reseller)
* [Reseller Accounts](#reseller_accounts)
* [SDK](#sdk)
* [Search](#search)
* [SMS](#sms)
* [SMS Campaigns](#sms_campaigns)
* [SMS Templates](#sms_templates)
* [Statistics](#statistics)
* [Subaccounts](#subaccounts)
* [Timezones](#timezones)
* [Transactional Email](#transactional_email)
* [Uploads](#uploads)
* [Voice](#voice)

## <a name="account"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Account") Account


### <a name="create_a_new_member"></a>![Endpoint: ](https://apidocs.io/img/method.png "Create a new Member") `POST` /account

> **Note:** *Authentication isn't required to create a new account.*



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `create a new account request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "username": "username",
  "password": "password",
  "user_email": "user_email",
  "user_phone": "user_phone",
  "user_first_name": "user_first_name",
  "user_last_name": "user_last_name",
  "account_name": "account_name",
  "country": "country"
}
``` 

#### Responses
**200** 

Body (_Create a new account response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Successfully created an account.",
  "data": {
    "user_id": 116,
    "username": "johndoe1",
    "user_email": "johndoe1@awesome.com",
    "active": 0,
    "banned": 0,
    "balance": "4.998000",
    "user_phone": "+15184811001",
    "reply_to": "originalemail",
    "delivery_to": null,
    "user_first_name": "John",
    "user_last_name": "Doe",
    "account": 0,
    "account_name": "The Awesome Company",
    "account_billing_email": "johndoe1@awesome.com",
    "account_billing_mobile": "+15184811001",
    "country": "US",
    "default_country_sms": "US",
    "auto_recharge": 0,
    "auto_recharge_amount": "20.00",
    "low_credit_amount": "0.00",
    "setting_unicode_sms": 0,
    "setting_email_sms_subject": 0,
    "setting_fix_sender_id": 0,
    "setting_sms_message_char_limit": 6,
    "old_dashboard": 0,
    "balance_commission": "0.299954",
    "timezone": "Australia/Melbourne",
    "_currency": {
      "currency_name_short": "USD",
      "currency_prefix_d": "$",
      "currency_prefix_c": "¢",
      "currency_name_long": "US Dollars"
    },
    "_subaccount": {
      "subaccount_id": 126,
      "api_username": "johndoe1",
      "email": "johndoe1@awesome.com",
      "phone_number": "+15184811001",
      "first_name": "John",
      "last_name": "Doe",
      "api_key": "F3702045-EB2C-0091-C211-7728048DCAE2",
      "access_users": 1,
      "access_billing": 1,
      "access_reporting": 1,
      "access_contacts": 1,
      "access_settings": 1,
      "access_sms": 1,
      "access_email": 1,
      "access_voice": 1,
      "access_fax": 1,
      "access_post": 1,
      "access_reseller": 1,
      "access_mms": 1,
      "share_campaigns": 0,
      "notes": null
    }
  }
}
```


### <a name="update_account"></a>![Endpoint: ](https://apidocs.io/img/method.png "Update Account") `PUT` /account

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `update account request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "username": "johndoe",
  "user_email": "johndoe@awesome.com",
  "user_phone": "518-481-1002",
  "user_first_name": "John",
  "user_last_name": "Doe",
  "country": "AU",
  "password": "pass",
  "account_name": "The Awesome Company",
  "timezone": "Australia/Melbourne",
  "private_uploads": 1,
  "setting_sms_hide_your_number": 0,
  "setting_sms_hide_business_name": 1
}
``` 

#### Responses
**200** 

Body (_Update Account response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your account has been updated.",
  "data": {
    "user_id": 1,
    "username": "johndoe",
    "user_email": "johndoe@awesome.com",
    "active": 1,
    "banned": 0,
    "balance": "0.592200",
    "user_phone": "518-481-1003",
    "reply_to": "11@test.com",
    "delivery_to": "1@test.com",
    "user_first_name": "John",
    "user_last_name": "Doe",
    "account": 0,
    "account_name": "The Awesome Company",
    "account_billing_email": "1@test.com",
    "account_billing_mobile": "+19171234591",
    "country": "AU",
    "default_country_sms": "AU",
    "auto_recharge": 1,
    "auto_recharge_amount": "20.00",
    "low_credit_amount": "200.00",
    "setting_unicode_sms": 0,
    "setting_email_sms_subject": 0,
    "setting_fix_sender_id": 1,
    "setting_sms_message_char_limit": 8,
    "old_dashboard": 1,
    "balance_commission": "0.299954",
    "timezone": "Australia/Melbourne",
    "private_uploads": 0,
    "fax_quality": 0,
    "setting_sms_hide_your_number": 0,
    "setting_sms_hide_business_name": 1,
    "_currency": {
      "currency_name_short": "AUD",
      "currency_prefix_d": "$",
      "currency_prefix_c": "c",
      "currency_name_long": "Australian Dollars"
    },
    "_subaccount": null
  }
}
```


### <a name="get_account"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get account") `GET` /account

> TODO: Add a method description



#### Responses
**200** 

Body (_Get account response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here's your account",
  "data": {
    "user_id": 3819,
    "username": "ULXHP",
    "user_email": "PNUMB@VAPXX.com",
    "active": 1,
    "banned": 0,
    "balance": "1117.461060",
    "user_phone": "+61433333888",
    "user_first_name": "fffff",
    "user_last_name": "llll",
    "account": 0,
    "account_name": "FTHCQ~!@#$ %^&*()XQMPO",
    "account_billing_email": "XDVXC@SJRJU.com",
    "account_billing_mobile": "+61433333888",
    "country": "AU",
    "default_country_sms": "AU",
    "auto_recharge": 0,
    "auto_recharge_amount": "20.00",
    "low_credit_amount": "0.00",
    "setting_unicode_sms": 0,
    "setting_email_sms_subject": 0,
    "setting_fix_sender_id": 0,
    "setting_sms_message_char_limit": 8,
    "old_dashboard": 0,
    "balance_commission": "2.330130",
    "timezone": "Australia/Melbourne",
    "private_uploads": 0,
    "fax_quality": 0,
    "setting_sms_hide_your_number": 0,
    "setting_sms_hide_business_name": 1,
    "_currency": {
      "currency_name_short": "AUD",
      "currency_prefix_d": "$",
      "currency_prefix_c": "c",
      "currency_name_long": "Australian Dollars"
    },
    "_subaccount": {
      "subaccount_id": 1716,
      "api_username": "KCIHOYEYGM",
      "email": "ICMGR@VBSPT.com",
      "phone_number": "+61433333333",
      "first_name": "Firstname40710",
      "last_name": "Lastname3672",
      "api_key": "IJVEGTCF-VOHU-GSVF-KNKK-XHTARJXMQTXK",
      "access_users": 1,
      "access_billing": 1,
      "access_reporting": 1,
      "access_contacts": 0,
      "access_settings": 1,
      "access_sms": 0,
      "access_email": 0,
      "access_voice": 0,
      "access_fax": 0,
      "access_post": 0,
      "access_reseller": 0,
      "access_mms": 1,
      "share_campaigns": 1,
      "notes": null
    }
  }
}
```


### <a name="account_usage"></a>![Endpoint: ](https://apidocs.io/img/method.png "Account Usage") `GET` /account/usage/{year}/{month}/{type}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| year | `precision` |  ``` Required ```  | Your account usage year. | `2016` | 
| month | `precision` |  ``` Required ```  | Your account usage month. | `4` | 
| type | `string` |  ``` Required ```  | The account type. Value can only be either email or subaccount. | `subaccount` | 

#### Responses
**200** 

Body (_Account Usage response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here is your usage for this month.",
  "data": {
    "sms": [
      {
        "subaccount_id": 1039,
        "username": "gerald",
        "total_count": "29.00",
        "total_price": "2.1337"
      },
      {
        "subaccount_id": 1047,
        "username": "user5",
        "total_count": "4.00",
        "total_price": "0.3080"
      }
    ],
    "voice": [
      {
        "subaccount_id": 1039,
        "username": "user1",
        "total_count": "6.00",
        "total_price": "0.1980"
      },
      {
        "subaccount_id": 1047,
        "username": "user5",
        "total_count": "1.00",
        "total_price": "0.0330"
      }
    ],
    "fax": [
      {
        "subaccount_id": 1039,
        "username": "user1",
        "total_count": "3.00",
        "total_price": "0.6943"
      },
      {
        "subaccount_id": 1047,
        "username": "user5",
        "total_count": "1.00",
        "total_price": "0.2314"
      }
    ],
    "post": [
      {
        "subaccount_id": 1039,
        "username": "user1",
        "total_count": "10",
        "total_price": "8.5624"
      },
      {
        "subaccount_id": 1047,
        "username": "user5",
        "total_count": "3",
        "total_price": "2.5586"
      }
    ],
    "email": [
      {
        "subaccount_id": 1039,
        "username": "user1",
        "total_count": 3992,
        "total_price": "9.0020"
      },
      {
        "subaccount_id": 1047,
        "username": "user5",
        "total_count": 998,
        "total_price": "0.0000"
      }
    ],
    "sms_total": {
      "count": 33,
      "price": "2.4417"
    },
    "voice_total": {
      "count": 7,
      "price": "0.2310"
    },
    "fax_total": {
      "count": 4,
      "price": "0.9257"
    },
    "post_total": {
      "count": 13,
      "price": "11.1210"
    },
    "email_total": {
      "count": 4990,
      "price": "9.0020"
    }
  }
}
```


### <a name="send_account_activation_token"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send account activation token") `PUT` /account-verify/send

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `send account activation token request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "user_phone": "352-394-4199",
  "type": "sms",
  "country": "US"
}
``` 

#### Responses
**200** 

Body (_Send account activation token response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Verification sent.",
  "data": {
    "user_phone": "+13523944199",
    "type": "sms",
    "country": "US",
    "activation_token": "547850"
  }
}
```


### <a name="verify_new_account"></a>![Endpoint: ](https://apidocs.io/img/method.png "Verify new account") `PUT` /account-verify/verify/{activation_token}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| activation_token | `string` |  ``` Required ```  | The ActivationToken to be used to verify an account. | `1827364` | 

#### Responses
**200** 

Body (_Verify new account response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "You're account has been verified.",
  "data": {
    "user_id": 1,
    "username": "1",
    "user_email": "1@test.com",
    "active": 1,
    "banned": 0,
    "balance": "4.041500",
    "user_phone": "+13523944199",
    "reply_to": "1@test.com",
    "delivery_to": null,
    "user_first_name": "John",
    "user_last_name": "Doe",
    "account": 1,
    "account_name": null,
    "account_billing_email": "1@test.com",
    "account_billing_mobile": null,
    "country": "US",
    "default_country_sms": "US",
    "unsubscribe_mail": 0,
    "auto_recharge": 0,
    "auto_recharge_amount": "20.00",
    "low_credit_amount": "1.50",
    "setting_unicode_sms": 0,
    "setting_beta": 0,
    "setting_email_sms_subject": 0,
    "setting_fix_sender_id": 1,
    "_currency": {
      "currency_name_short": "USD",
      "currency_prefix_d": "$",
      "currency_prefix_c": "¢",
      "currency_name_long": "US Dollars"
    },
    "_subaccount": {
      "subaccount_id": 1,
      "api_username": "1",
      "email": "1@test.com",
      "mobile": "+639171234501",
      "first_name": "John",
      "last_name": "Doe",
      "api_key": "FD3259F9D0A35548682ACEA84A6FF26A",
      "user_id": 1,
      "sms_deidentify_message": 0,
      "access_smpp": 0,
      "access_users": 1,
      "access_billing": 1,
      "access_reporting": 1,
      "access_contacts": 0,
      "access_settings": 1
    }
  }
}
```


[Back to API Reference](#api_reference)

## <a name="account_recharge"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Account Recharge") Account Recharge


### <a name="get_credit_card_info"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Credit Card info") `GET` /recharge/credit-card

> TODO: Add a method description



#### Responses
**200** 

Body (_Get Credit Card info response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Customer payment info.",
  "data": {
    "display_number": "XXXX-XXXX-XXXX-0000",
    "expiry_month": 5,
    "expiry_year": 2016,
    "name": "Roland Robot"
  }
}
```


### <a name="update_credit_card_info"></a>![Endpoint: ](https://apidocs.io/img/method.png "Update Credit Card info") `PUT` /recharge/credit-card

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `update credit card info request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "expiry_month": 103.694755515873,
  "cvc": 103.694755515873,
  "name": "name",
  "number": 103.694755515873,
  "expiry_year": 103.694755515873
}
``` 

#### Responses
**200** 

Body (_Update Credit Card info response_) 
```
{
  "http_code": 103,
  "response_code": "response_code",
  "response_msg": "response_msg",
  "data": {}
}
```


### <a name="list_of_packages"></a>![Endpoint: ](https://apidocs.io/img/method.png "List of Packages") `GET` /recharge/packages?country={country}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| country | `string` |  ``` Optional ```  | Your country. | `"AU"` | 

#### Responses
**200** 

Body (_List of Packages response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "List of Packages.",
  "data": {
    "packages": [
      {
        "package_id": 1,
        "package_price": "20.00",
        "sms_price": 0.099,
        "sms_quantity": 202,
        "voice_mobile_price": 0.099,
        "voice_mobile_quantity": 202,
        "voice_landline_price": 0.0583,
        "voice_landline_quantity": 343,
        "fax_price": 0.198,
        "fax_quantity": 101,
        "email_price": 0.033,
        "email_quantity": 606,
        "post_letter_black_price": 1.397,
        "post_letter_colour_price": 1.617,
        "post_page_black_price": 0.11,
        "post_page_colour_price": 0.264,
        "post_letter_black_quantity": 13,
        "post_letter_colour_quantity": 10,
        "post_direct_mail_dl_price": 0.44,
        "post_direct_mail_a5_price": 0.66,
        "post_direct_mail_min_quantity": 5000,
        "postcard_price": 11,
        "postcard_quantity": 1
      },
      {
        "package_id": 2,
        "package_price": "50.00",
        "sms_price": 0.099,
        "sms_quantity": 505,
        "voice_mobile_price": 0.099,
        "voice_mobile_quantity": 505,
        "voice_landline_price": 0.0583,
        "voice_landline_quantity": 857,
        "fax_price": 0.198,
        "fax_quantity": 252,
        "email_price": 0.033,
        "email_quantity": 1515,
        "post_letter_black_price": 1.397,
        "post_letter_colour_price": 1.617,
        "post_page_black_price": 0.11,
        "post_page_colour_price": 0.264,
        "post_letter_black_quantity": 33,
        "post_letter_colour_quantity": 26,
        "post_direct_mail_dl_price": 0.44,
        "post_direct_mail_a5_price": 0.66,
        "post_direct_mail_min_quantity": 5000,
        "postcard_price": 11,
        "postcard_quantity": 4
      },
      {
        "package_id": 3,
        "package_price": "100.00",
        "sms_price": 0.099,
        "sms_quantity": 1010,
        "voice_mobile_price": 0.099,
        "voice_mobile_quantity": 1010,
        "voice_landline_price": 0.0583,
        "voice_landline_quantity": 1715,
        "fax_price": 0.198,
        "fax_quantity": 505,
        "email_price": 0.033,
        "email_quantity": 3030,
        "post_letter_black_price": 1.397,
        "post_letter_colour_price": 1.617,
        "post_page_black_price": 0.11,
        "post_page_colour_price": 0.264,
        "post_letter_black_quantity": 66,
        "post_letter_colour_quantity": 53,
        "post_direct_mail_dl_price": 0.44,
        "post_direct_mail_a5_price": 0.66,
        "post_direct_mail_min_quantity": 5000,
        "postcard_price": 11,
        "postcard_quantity": 9
      },
      {
        "package_id": 4,
        "package_price": "200.00",
        "sms_price": 0.088,
        "sms_quantity": 2272,
        "voice_mobile_price": 0.099,
        "voice_mobile_quantity": 2020,
        "voice_landline_price": 0.0583,
        "voice_landline_quantity": 3430,
        "fax_price": 0.198,
        "fax_quantity": 1010,
        "email_price": 0.011,
        "email_quantity": 18181,
        "post_letter_black_price": 1.397,
        "post_letter_colour_price": 1.617,
        "post_page_black_price": 0.11,
        "post_page_colour_price": 0.264,
        "post_letter_black_quantity": 132,
        "post_letter_colour_quantity": 106,
        "post_direct_mail_dl_price": 0.44,
        "post_direct_mail_a5_price": 0.66,
        "post_direct_mail_min_quantity": 5000,
        "postcard_price": 11,
        "postcard_quantity": 18
      },
      {
        "package_id": 5,
        "package_price": "500.00",
        "sms_price": 0.088,
        "sms_quantity": 5681,
        "voice_mobile_price": 0.099,
        "voice_mobile_quantity": 5050,
        "voice_landline_price": 0.0583,
        "voice_landline_quantity": 8576,
        "fax_price": 0.198,
        "fax_quantity": 2525,
        "email_price": 0.011,
        "email_quantity": 45454,
        "post_letter_black_price": 1.397,
        "post_letter_colour_price": 1.617,
        "post_page_black_price": 0.11,
        "post_page_colour_price": 0.264,
        "post_letter_black_quantity": 331,
        "post_letter_colour_quantity": 265,
        "post_direct_mail_dl_price": 0.44,
        "post_direct_mail_a5_price": 0.66,
        "post_direct_mail_min_quantity": 5000,
        "postcard_price": 11,
        "postcard_quantity": 45
      },
      {
        "package_id": 6,
        "package_price": "1000.00",
        "sms_price": 0.077,
        "sms_quantity": 12987,
        "voice_mobile_price": 0.099,
        "voice_mobile_quantity": 10101,
        "voice_landline_price": 0.0583,
        "voice_landline_quantity": 17152,
        "fax_price": 0.198,
        "fax_quantity": 5050,
        "email_price": 0.0055,
        "email_quantity": 181818,
        "post_letter_black_price": 1.397,
        "post_letter_colour_price": 1.617,
        "post_page_black_price": 0.11,
        "post_page_colour_price": 0.264,
        "post_letter_black_quantity": 663,
        "post_letter_colour_quantity": 531,
        "post_direct_mail_dl_price": 0.44,
        "post_direct_mail_a5_price": 0.66,
        "post_direct_mail_min_quantity": 5000,
        "postcard_price": 11,
        "postcard_quantity": 90
      },
      {
        "package_id": 7,
        "package_price": "1500.00",
        "sms_price": 0.077,
        "sms_quantity": 19480,
        "voice_mobile_price": 0.099,
        "voice_mobile_quantity": 15151,
        "voice_landline_price": 0.0583,
        "voice_landline_quantity": 25728,
        "fax_price": 0.198,
        "fax_quantity": 7575,
        "email_price": 0.0055,
        "email_quantity": 272727,
        "post_letter_black_price": 1.397,
        "post_letter_colour_price": 1.617,
        "post_page_black_price": 0.11,
        "post_page_colour_price": 0.264,
        "post_letter_black_quantity": 995,
        "post_letter_colour_quantity": 797,
        "post_direct_mail_dl_price": 0.44,
        "post_direct_mail_a5_price": 0.66,
        "post_direct_mail_min_quantity": 5000,
        "postcard_price": 11,
        "postcard_quantity": 136
      },
      {
        "package_id": 8,
        "package_price": "2000.00",
        "sms_price": 0.077,
        "sms_quantity": 25974,
        "voice_mobile_price": 0.099,
        "voice_mobile_quantity": 20202,
        "voice_landline_price": 0.0583,
        "voice_landline_quantity": 34305,
        "fax_price": 0.198,
        "fax_quantity": 10101,
        "email_price": 0.0055,
        "email_quantity": 363636,
        "post_letter_black_price": 1.397,
        "post_letter_colour_price": 1.617,
        "post_page_black_price": 0.11,
        "post_page_colour_price": 0.264,
        "post_letter_black_quantity": 1327,
        "post_letter_colour_quantity": 1063,
        "post_direct_mail_dl_price": 0.44,
        "post_direct_mail_a5_price": 0.66,
        "post_direct_mail_min_quantity": 5000,
        "postcard_price": 11,
        "postcard_quantity": 181
      },
      {
        "package_id": 9,
        "package_price": "3000.00",
        "sms_price": 0.077,
        "sms_quantity": 38961,
        "voice_mobile_price": 0.099,
        "voice_mobile_quantity": 30303,
        "voice_landline_price": 0.0583,
        "voice_landline_quantity": 51457,
        "fax_price": 0.198,
        "fax_quantity": 15151,
        "email_price": 0.0055,
        "email_quantity": 545454,
        "post_letter_black_price": 1.397,
        "post_letter_colour_price": 1.617,
        "post_page_black_price": 0.11,
        "post_page_colour_price": 0.264,
        "post_letter_black_quantity": 1990,
        "post_letter_colour_quantity": 1594,
        "post_direct_mail_dl_price": 0.44,
        "post_direct_mail_a5_price": 0.66,
        "post_direct_mail_min_quantity": 5000,
        "postcard_price": 11,
        "postcard_quantity": 272
      },
      {
        "package_id": 10,
        "package_price": "5500.00",
        "sms_price": 0.066,
        "sms_quantity": 83333,
        "voice_mobile_price": 0.099,
        "voice_mobile_quantity": 55555,
        "voice_landline_price": 0.0583,
        "voice_landline_quantity": 94339,
        "fax_price": 0.198,
        "fax_quantity": 27777,
        "email_price": 0.0044,
        "email_quantity": 1250000,
        "post_letter_black_price": 1.397,
        "post_letter_colour_price": 1.617,
        "post_page_black_price": 0.11,
        "post_page_colour_price": 0.264,
        "post_letter_black_quantity": 3649,
        "post_letter_colour_quantity": 2923,
        "post_direct_mail_dl_price": 0.44,
        "post_direct_mail_a5_price": 0.66,
        "post_direct_mail_min_quantity": 5000,
        "postcard_price": 11,
        "postcard_quantity": 500
      }
    ],
    "currency": {
      "currency_name_short": "AUD",
      "currency_prefix_d": "$",
      "currency_prefix_c": "c",
      "currency_name_long": "Australian Dollars"
    }
  }
}
```


### <a name="purchase_a_package"></a>![Endpoint: ](https://apidocs.io/img/method.png "Purchase a Package") `PUT` /recharge/purchase/{package_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| package_id | `precision` |  ``` Required ```  | Your package id. | `1` | 

#### Responses
**200** 

Body (_Purchase a Package response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Successfully purchased a package #1",
  "data": {
    "user_id": 1,
    "amount": "50.00",
    "currency": "USD",
    "amount_aud": "61.86",
    "date": 1442216451
  }
}
```


### <a name="get_transactions"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Transactions") `GET` /recharge/transactions

> TODO: Add a method description



#### Responses
**200** 

Body (_Get Transactions response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are your transactions.",
  "data": {
    "total": 16,
    "per_page": 15,
    "current_page": 1,
    "last_page": 2,
    "next_page_url": "https://rest.clicksend.com/v3/recharge/transactions/?page=2",
    "prev_page_url": null,
    "from": 1,
    "to": 15,
    "data": [
      {
        "invoice_number": "cb726c65-1c65-47fa-aea2-3ded9ed57557",
        "amount": "20.00",
        "currency": "AUD",
        "date": 1443420196
      },
      {
        "invoice_number": "13d35606-5f10-4d31-9de4-065b025aa5b8",
        "amount": "20.00",
        "currency": "AUD",
        "date": 1443420094
      },
      {
        "invoice_number": "4e9fc8af-f514-45b1-86c2-fc85630bb14d",
        "amount": "20.00",
        "currency": "AUD",
        "date": 1443418982
      },
      {
        "invoice_number": "65c0bfe0-168c-4b46-9dbd-6120a18b5efa",
        "amount": "20.00",
        "currency": "AUD",
        "date": 1443403590
      },
      {
        "invoice_number": "902e78dc-9a70-417b-8426-6967f0efc6eb",
        "amount": "20.00",
        "currency": "AUD",
        "date": 1443149774
      },
      {
        "invoice_number": "21571831-ae8f-4605-ac3e-3efe424a2a39",
        "amount": "20.00",
        "currency": "AUD",
        "date": 1443148806
      },
      {
        "invoice_number": "b978f05b-3de0-4d17-9796-a852eb82d820",
        "amount": "20.00",
        "currency": "AUD",
        "date": 1443147864
      },
      {
        "invoice_number": "180999f7-1928-4137-a7c3-754420fc1235",
        "amount": "20.00",
        "currency": "AUD",
        "date": 1443146363
      },
      {
        "invoice_number": "3d527e8f-03e1-460b-9f7d-5fce9fc2997e",
        "amount": "20.00",
        "currency": "AUD",
        "date": 1442907133
      },
      {
        "invoice_number": "cdee6647-7b82-49b5-b26e-033eadb2a485",
        "amount": "20.00",
        "currency": "AUD",
        "date": 1442902821
      },
      {
        "invoice_number": "0b6c4073-e214-439d-9821-8f0b69ea61f8",
        "amount": "20.00",
        "currency": "AUD",
        "date": 1442902477
      },
      {
        "invoice_number": "e9d48b44-fad1-4d47-94bb-5d11d88f01f4",
        "amount": "20.00",
        "currency": "AUD",
        "date": 1442902394
      },
      {
        "invoice_number": "1ea56734-a540-4ab6-8b10-fc364065c046",
        "amount": "20.00",
        "currency": "AUD",
        "date": 1442902192
      },
      {
        "invoice_number": "b5031e92-0ca3-47a1-9f66-b14a7eaac9b1",
        "amount": "20.00",
        "currency": "AUD",
        "date": 1442896724
      },
      {
        "invoice_number": "aeb4bff3-ea08-40ba-9f84-3ff000aa9283",
        "amount": "50.00",
        "currency": "USD",
        "date": 1442216451
      }
    ]
  }
}
```


### <a name="get_a_specific_transaction"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get a specific transaction") `GET` /recharge/transactions/{transaction_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| transaction_id | `string` |  ``` Required ```  | 1c65-47fa-aea2-3ded9ed57557 (number, required) - Your transction id. | `cb726c65` | 

#### Responses
**200** 

Body (_binary_)


[Back to API Reference](#api_reference)

## <a name="automation_rules"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Automation Rules") Automation Rules


### <a name="list_rules"></a>![Endpoint: ](https://apidocs.io/img/method.png "List rules") `GET` /automations/sms/inbound

> TODO: Add a method description



#### Responses
**200** 

Body (_List rules response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your list of inbound rules.",
  "data": {
    "total": 10,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 10,
    "data": [
      {
        "inbound_rule_id": 10,
        "dedicated_number": "+61298441484",
        "rule_name": "My Rule 10",
        "message_search_type": 3,
        "message_search_term": "My Search Term",
        "action": "CREATE_CONTACT_PLUS_EMAIL",
        "action_address": "430",
        "body": "test@test.com",
        "enabled": 1
      },
      {
        "inbound_rule_id": 9,
        "dedicated_number": "+61298441484",
        "rule_name": "My Rule 9",
        "message_search_type": 3,
        "message_search_term": "My Search Term",
        "action": "CREATE_CONTACT",
        "action_address": "john@doe.com",
        "body": null,
        "enabled": 1
      },
      {
        "inbound_rule_id": 8,
        "dedicated_number": "+61298441484",
        "rule_name": "My Rule 8",
        "message_search_type": 3,
        "message_search_term": "My Search Term",
        "action": "MOVE_CONTACT",
        "action_address": "john@doe.com",
        "body": null,
        "enabled": 1
      },
      {
        "inbound_rule_id": 7,
        "dedicated_number": "+61298441484",
        "rule_name": "My Rule 7",
        "message_search_type": 3,
        "message_search_term": "My Search Term",
        "action": "GROUP_SMS",
        "action_address": "john@doe.com",
        "body": null,
        "enabled": 1
      },
      {
        "inbound_rule_id": 6,
        "dedicated_number": "+61298441484",
        "rule_name": "My Rule 6",
        "message_search_type": 3,
        "message_search_term": "My Search Term",
        "action": "POLL",
        "action_address": "john@doe.com",
        "body": null,
        "enabled": 1
      },
      {
        "inbound_rule_id": 5,
        "dedicated_number": "+61298441484",
        "rule_name": "My Rule 5",
        "message_search_type": 3,
        "message_search_term": "My Search Term",
        "action": "SMS",
        "action_address": "john@doe.com",
        "body": null,
        "enabled": 1
      },
      {
        "inbound_rule_id": 4,
        "dedicated_number": "+61298441484",
        "rule_name": "My Rule 4",
        "message_search_type": 3,
        "message_search_term": "My Search Term",
        "action": "URL",
        "action_address": "john@doe.com",
        "body": null,
        "enabled": 1
      },
      {
        "inbound_rule_id": 3,
        "dedicated_number": "+61298441484",
        "rule_name": "My Rule 3",
        "message_search_type": 3,
        "message_search_term": "My Search Term",
        "action": "EMAIL_FIXED",
        "action_address": "john@doe.com",
        "body": null,
        "enabled": 1
      },
      {
        "inbound_rule_id": 2,
        "dedicated_number": "+61298441484",
        "rule_name": "My Rule 2",
        "message_search_type": 3,
        "message_search_term": "My Search Term",
        "action": "EMAIL_USER",
        "action_address": "john@doe.com",
        "body": null,
        "enabled": 1
      },
      {
        "inbound_rule_id": 1,
        "dedicated_number": "+61298441484",
        "rule_name": "My Rule 1",
        "message_search_type": 3,
        "message_search_term": null,
        "action": "AUTO_REPLY",
        "action_address": "john@doe.com",
        "body": null,
        "enabled": 1
      },
      {
        "inbound_rule_id": 1,
        "dedicated_number": "+61298441484",
        "rule_name": "My Rule 1",
        "message_search_type": 3,
        "message_search_term": null,
        "action": "CREATE_CONTACT_PLUS_NAME",
        "action_address": 534,
        "body": null,
        "enabled": 1
      }
    ]
  }
}
```


### <a name="get_a_specific_rule"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get a specific rule") `GET` /automations/sms/inbound/{inbound_rule_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| inbound_rule_id | `precision` |  ``` Required ```  | Inbound Rule ID. | `1` | 

#### Responses
**200** 

Body (_Get a specific rule response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your inbound rule.",
  "data": {
    "inbound_rule_id": 1,
    "dedicated_number": "+61298441484",
    "rule_name": "My Rule",
    "message_search_type": 3,
    "message_search_term": null,
    "action": "EMAIL_FIXED",
    "action_address": "john@doe.com",
    "body": null,
    "enabled": 1
  }
}
```


### <a name="create_a_new_rule"></a>![Endpoint: ](https://apidocs.io/img/method.png "Create a new rule") `POST` /automations/sms/inbound/

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `create a new rule request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "dedicated_number": 103.694755515873,
  "rule_name": "rule_name",
  "message_search_type": 103.694755515873,
  "message_search_term": "message_search_term",
  "action": "action",
  "action_address": "action_address",
  "enabled": 103.694755515873
}
``` 

#### Responses
**200** 

Body (_Create a new rule response_) 
```
{
  "http_code": 103,
  "response_code": "response_code",
  "response_msg": "response_msg",
  "data": {}
}
```


### <a name="update_a_rule"></a>![Endpoint: ](https://apidocs.io/img/method.png "Update a rule") `PUT` /automations/sms/inbound/{inbound_rule_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| inbound_rule_id | `precision` |  ``` Required ```  | Inbound Rule ID. | `1` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `update a rule request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "dedicated_number": "+61298441484",
  "rule_name": "My Rule",
  "message_search_type": 3,
  "message_search_term": "My Search Term",
  "action": "EMAIL_FIXED",
  "action_address": "john@doe.com",
  "enabled": 1
}
``` 

#### Responses
**200** 

Body (_Update a rule response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your record has been updated.",
  "data": {
    "inbound_rule_id": 1,
    "dedicated_number": "+61298441484",
    "rule_name": "My Rule",
    "message_search_type": 3,
    "message_search_term": null,
    "action": "EMAIL_FIXED",
    "action_address": "john@doe.com",
    "body": null,
    "enabled": 1
  }
}
```


### <a name="delete_a_rule"></a>![Endpoint: ](https://apidocs.io/img/method.png "Delete a rule") `DELETE` /automations/sms/inbound/{inbound_rule_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| inbound_rule_id | `precision` |  ``` Required ```  | Inbound Rule ID. | `1` | 

#### Responses
**200** 

Body (_Delete a rule response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your record has been deleted.",
  "data": []
}
```


### <a name="list_rules1"></a>![Endpoint: ](https://apidocs.io/img/method.png "List rules1") `GET` /automations/sms/receipts

> TODO: Add a method description



#### Responses
**200** 

Body (_List rules response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your list of rule incoming sms receipt.",
  "data": {
    "total": 5,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 5,
    "data": [
      {
        "receipt_rule_id": 5,
        "rule_name": "My Rule",
        "match_type": 0,
        "action": "EMAIL_FIXED",
        "action_address": "john@doe.com",
        "enabled": 0
      },
      {
        "receipt_rule_id": 6,
        "rule_name": "My Rule",
        "match_type": 0,
        "action": "EMAIL_FIXED",
        "action_address": "john@doe.com",
        "enabled": 1
      },
      {
        "receipt_rule_id": 7,
        "rule_name": "My Rule",
        "match_type": 0,
        "action": "EMAIL_FIXED",
        "action_address": "john@doe.com",
        "enabled": 1
      },
      {
        "receipt_rule_id": 8,
        "rule_name": "My Rule",
        "match_type": 0,
        "action": "SMS",
        "action_address": "+61298441484",
        "enabled": 1
      },
      {
        "receipt_rule_id": 9,
        "rule_name": "My Rule",
        "match_type": 0,
        "action": "URL",
        "action_address": "+61298441485",
        "enabled": 1
      }
    ]
  }
}
```


### <a name="get_a_specific_rule1"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get a specific rule1") `GET` /automations/sms/receipts/{receipt_rule_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| receipt_rule_id | `precision` |  ``` Required ```  | Receipt Rule ID. | `2` | 

#### Responses
**200** 

Body (_Get a specific rule response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your rule incoming voice receipt.",
  "data": {
    "receipt_rule_id": 6,
    "rule_name": "My Rule",
    "match_type": 0,
    "action": "EMAIL_FIXED",
    "action_address": "john@doe.com",
    "enabled": 1
  }
}
```


### <a name="create_a_new_rule1"></a>![Endpoint: ](https://apidocs.io/img/method.png "Create a new rule1") `POST` /automations/sms/receipts

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `create a new rule request24` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "rule_name": "My Rule",
  "match_type": 3,
  "action": "EMAIL_FIXED",
  "action_address": "john@doe.com",
  "enabled": 1
}
``` 

#### Responses
**200** 

Body (_Create a new rule response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your new SMS receipt has been added.",
  "data": {
    "receipt_rule_id": 10,
    "rule_name": "My Rule",
    "match_type": 3,
    "action": "EMAIL_FIXED",
    "action_address": "john@doe.com",
    "enabled": 1
  }
}
```


### <a name="update_a_rule1"></a>![Endpoint: ](https://apidocs.io/img/method.png "Update a rule1") `PUT` /automations/sms/receipts/{receipt_rule_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| receipt_rule_id | `precision` |  ``` Required ```  | Receipt Rule ID. | `7` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `update a rule request26` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "rule_name": "My Rule",
  "match_type": 3,
  "action": "EMAIL_FIXED",
  "action_address": "john@doe.com",
  "enabled": 1
}
``` 

#### Responses
**200** 

Body (_Update a rule response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your rule incoming sms receipt has been updated.",
  "data": {
    "receipt_rule_id": 7,
    "rule_name": "My Rule",
    "match_type": 0,
    "action": "EMAIL_FIXED",
    "action_address": "john@doe.com",
    "enabled": 1
  }
}
```


### <a name="delete_a_rule1"></a>![Endpoint: ](https://apidocs.io/img/method.png "Delete a rule1") `DELETE` /automations/sms/receipts/{receipt_rule_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| receipt_rule_id | `precision` |  ``` Required ```  | Receipt Rule ID. | `7` | 

#### Responses
**200** 

Body (_Delete a rule response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your rule incoming sms receipt has been deleted.",
  "data": []
}
```


### <a name="list_rules2"></a>![Endpoint: ](https://apidocs.io/img/method.png "List rules2") `GET` /automations/voice/receipts

> TODO: Add a method description



#### Responses
**200** 

Body (_List rules response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your voice receipts.",
  "data": {
    "total": 1,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 1,
    "data": [
      {
        "receipt_rule_id": 2,
        "rule_name": "My Rule 2",
        "match_type": 3,
        "action": "URL",
        "action_address": "http://johndoe.com",
        "enabled": 1
      }
    ]
  }
}
```


### <a name="get_a_specific_rule11"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get a specific rule11") `GET` /automations/voice/receipts/{receipt_rule_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| receipt_rule_id | `precision` |  ``` Required ```  | Receipt Rule ID. | `2` | 

#### Responses
**200** 

Body (_Get a specific rule response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your rule incoming voice receipt.",
  "data": {
    "receipt_rule_id": 2,
    "rule_name": "My Rule 2",
    "match_type": 3,
    "action": "URL",
    "action_address": "http://johndoe.com",
    "enabled": 1
  }
}
```


### <a name="create_a_new_rule2"></a>![Endpoint: ](https://apidocs.io/img/method.png "Create a new rule2") `POST` /automations/voice/receipts

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `create a new rule request24` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "rule_name": "My Rule",
  "match_type": 3,
  "action": "EMAIL_FIXED",
  "action_address": "john@doe.com",
  "enabled": 1
}
``` 

#### Responses
**200** 

Body (_Create a new rule response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your new voice receipt has been added.",
  "data": {
    "receipt_rule_id": 3,
    "rule_name": "My Rule",
    "match_type": 3,
    "action": "EMAIL_FIXED",
    "action_address": "john@doe.com",
    "enabled": 1
  }
}
```


### <a name="update_a_rule11"></a>![Endpoint: ](https://apidocs.io/img/method.png "Update a rule11") `PUT` /automations/voice/receipts/{receipt_rule_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| receipt_rule_id | `precision` |  ``` Required ```  | Receipt Rule ID. | `2` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `update a rule request26` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "rule_name": "My Rule",
  "match_type": 3,
  "action": "EMAIL_FIXED",
  "action_address": "john@doe.com",
  "enabled": 1
}
``` 

#### Responses
**200** 

Body (_Update a rule response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your rule incoming voice receipt.",
  "data": {
    "receipt_rule_id": 2,
    "rule_name": "My Rule 2",
    "match_type": 3,
    "action": "URL",
    "action_address": "http://johndoe.com",
    "enabled": 1
  }
}
```


### <a name="delete_a_rule11"></a>![Endpoint: ](https://apidocs.io/img/method.png "Delete a rule11") `DELETE` /automations/voice/receipts/{receipt_rule_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| receipt_rule_id | `precision` |  ``` Required ```  | Receipt Rule ID. | `2` | 

#### Responses
**200** 

Body (_Delete a rule response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your rule voice receipt has been deleted.",
  "data": []
}
```


### <a name="list_rules3"></a>![Endpoint: ](https://apidocs.io/img/method.png "List rules3") `GET` /automations/fax/inbound

> TODO: Add a method description



#### Responses
**200** 

Body (_List rules response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your inbound fax.",
  "data": {
    "total": 20,
    "per_page": 15,
    "current_page": 1,
    "last_page": 2,
    "next_page_url": "https://rest.clicksend.com/v3/automations/fax/inbound?page=2",
    "prev_page_url": null,
    "from": 1,
    "to": 15,
    "data": [
      {
        "inbound_rule_id": 1,
        "dedicated_number": "19",
        "rule_name": "Email",
        "user_id": 1,
        "action": "EMAIL_FIXED",
        "action_address": "test@test.com",
        "enabled": 1
      },
      {
        "inbound_rule_id": 2,
        "dedicated_number": "19",
        "rule_name": "URL",
        "user_id": 1,
        "action": "URL",
        "action_address": "https://url.com",
        "enabled": 0
      },
      {
        "inbound_rule_id": 3,
        "dedicated_number": "19",
        "rule_name": "POLL",
        "user_id": 1,
        "action": "POLL",
        "action_address": "https://ima.poll",
        "enabled": 0
      },
      {
        "inbound_rule_id": 4,
        "dedicated_number": "19",
        "rule_name": "POLL",
        "user_id": 1,
        "action": "EMAIL_FIXED",
        "action_address": "https://ima.poll",
        "enabled": 0
      },
      {
        "inbound_rule_id": 6,
        "dedicated_number": "19",
        "rule_name": "POLL",
        "user_id": 1,
        "action": "NOTHING",
        "action_address": "https://ima.poll",
        "enabled": 0
      },
      {
        "inbound_rule_id": 7,
        "dedicated_number": "19",
        "rule_name": "POLL",
        "user_id": 1,
        "action": "NOTHING",
        "action_address": "https://ima.poll",
        "enabled": 0
      },
      {
        "inbound_rule_id": 8,
        "dedicated_number": "19",
        "rule_name": "POLL",
        "user_id": 1,
        "action": "NOTHING",
        "action_address": "https://ima.poll",
        "enabled": 0
      },
      {
        "inbound_rule_id": 9,
        "dedicated_number": "19",
        "rule_name": "POLL",
        "user_id": 1,
        "action": "NOTHING",
        "action_address": "https://ima.poll",
        "enabled": 0
      },
      {
        "inbound_rule_id": 10,
        "dedicated_number": "19",
        "rule_name": "POLL",
        "user_id": 1,
        "action": "POLL",
        "action_address": "https://ima.poll",
        "enabled": 0
      },
      {
        "inbound_rule_id": 12,
        "dedicated_number": "+61298441484",
        "rule_name": "Rule Name",
        "user_id": 1,
        "action": "EMAIL_FIXED",
        "action_address": "",
        "enabled": 1
      },
      {
        "inbound_rule_id": 13,
        "dedicated_number": "+61298441484",
        "rule_name": "Rule Name",
        "user_id": 1,
        "action": "EMAIL_FIXED",
        "action_address": "",
        "enabled": 1
      },
      {
        "inbound_rule_id": 14,
        "dedicated_number": "+61298441484",
        "rule_name": "Rule Name",
        "user_id": 1,
        "action": "EMAIL_FIXED",
        "action_address": "email@domain.com",
        "enabled": 1
      },
      {
        "inbound_rule_id": 15,
        "dedicated_number": "+61298441484",
        "rule_name": "Rule Name",
        "user_id": 1,
        "action": "EMAIL_FIXED",
        "action_address": "email@domain.com",
        "enabled": 1
      },
      {
        "inbound_rule_id": 16,
        "dedicated_number": "+61298441484",
        "rule_name": "Rule Name",
        "user_id": 1,
        "action": "EMAIL_FIXED",
        "action_address": "email@domain.com",
        "enabled": 1
      },
      {
        "inbound_rule_id": 17,
        "dedicated_number": "+61298441484",
        "rule_name": "Rule Name",
        "user_id": 1,
        "action": "EMAIL_FIXED",
        "action_address": "email@domain.com",
        "enabled": 1
      }
    ]
  }
}
```


### <a name="get_a_specific_rule111"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get a specific rule111") `GET` /automations/fax/inbound/{inbound_rule_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| inbound_rule_id | `precision` |  ``` Required ```  | Fax inbound rule id | `14` | 

#### Responses
**200** 

Body (_Get a specific rule response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your inbound fax.",
  "data": {
    "inbound_rule_id": 14,
    "dedicated_number": "+61298441484",
    "rule_name": "Rule Name",
    "user_id": 1,
    "action": "EMAIL_FIXED",
    "action_address": "email@domain.com",
    "enabled": 1
  }
}
```


### <a name="create_a_new_rule3"></a>![Endpoint: ](https://apidocs.io/img/method.png "Create a new rule3") `POST` /automations/fax/inbound

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `create a new rule request38` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "dedicated_number": "+61298441484",
  "rule_name": "Rule Name",
  "action": "EMAIL_FIXED",
  "action_address": "email@domain.com",
  "enabled": 1
}
``` 

#### Responses
**200** 

Body (_Create a new rule response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "New rule has been added.",
  "data": {
    "inbound_rule_id": 24,
    "dedicated_number": "+61298441484",
    "rule_name": "My Rule",
    "user_id": 1,
    "action": "EMAIL_FIXED",
    "action_address": "email@domain.com",
    "enabled": 1
  }
}
```


### <a name="update_a_rule111"></a>![Endpoint: ](https://apidocs.io/img/method.png "Update a rule111") `PUT` /automations/fax/inbound/{inbound_rule_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| inbound_rule_id | `precision` |  ``` Required ```  | Fax inbound rule id | `14` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `update a rule request40` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "dedicated_number": "+61298441484",
  "rule_name": "Rule Name",
  "action": "EMAIL_FIXED",
  "action_address": "email@domain.com",
  "enabled": 1
}
``` 

#### Responses
**200** 

Body (_Update a rule response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your inbound fax.",
  "data": {
    "inbound_rule_id": 14,
    "dedicated_number": "+61298441484",
    "rule_name": "Rule Name",
    "user_id": 1,
    "action": "EMAIL_FIXED",
    "action_address": "email@domain.com",
    "enabled": 1
  }
}
```


### <a name="delete_a_rule111"></a>![Endpoint: ](https://apidocs.io/img/method.png "Delete a rule111") `DELETE` /automations/fax/inbound/{inbound_rule_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| inbound_rule_id | `precision` |  ``` Required ```  | Fax inbound rule id | `14` | 

#### Responses
**200** 

Body (_Delete a rule response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your fax inbound rule has been deleted.",
  "data": []
}
```


### <a name="list_rules4"></a>![Endpoint: ](https://apidocs.io/img/method.png "List Rules4") `GET` /automations/fax/receipts

> TODO: Add a method description



#### Responses
**200** 

Body (_List rules response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here is your result.",
  "data": {
    "total": 4,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 4,
    "data": [
      {
        "receipt_rule_id": 1,
        "rule_name": "Email Test Rule",
        "match_type": 0,
        "action": "URL",
        "action_address": "http://requestb.in/1821qos1",
        "enabled": 1
      },
      {
        "receipt_rule_id": 2,
        "rule_name": "test",
        "match_type": 0,
        "action": "URL",
        "action_address": "http://testurl.com",
        "enabled": 1
      },
      {
        "receipt_rule_id": 6,
        "rule_name": "test",
        "match_type": 0,
        "action": "URL",
        "action_address": "http://testurl.com",
        "enabled": 1
      },
      {
        "receipt_rule_id": 7,
        "rule_name": "test",
        "match_type": 0,
        "action": "URL",
        "action_address": "http://testurl.com",
        "enabled": 1
      }
    ]
  }
}
```


### <a name="get_a_specific_rule2"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get a Specific Rule2") `GET` /automations/fax/receipts/{rule_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| rule_id | `precision` |  ``` Required ```  | The rule id you want to access. | `4` | 

#### Responses
**200** 

Body (_Get a specific rule response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your rule incoming fax receipt.",
  "data": {
    "receipt_rule_id": 4,
    "rule_name": "My Rule",
    "match_type": 2,
    "action": "EMAIL_FIXED",
    "action_address": "john@doe.com",
    "enabled": 1
  }
}
```


### <a name="create_a_new_rule4"></a>![Endpoint: ](https://apidocs.io/img/method.png "Create a New Rule4") `POST` /automations/fax/receipts

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `create a new rule request24` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "rule_name": "My Rule",
  "match_type": 2,
  "action": "EMAIL_FIXED",
  "action_address": "john@doe.com",
  "enabled": 1
}
``` 

#### Responses
**200** 

Body (_Create a new rule response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your new Fax receipt has been added.",
  "data": {
    "receipt_rule_id": 4,
    "rule_name": "My Rule",
    "match_type": 2,
    "action": "EMAIL_FIXED",
    "action_address": "john@doe.com",
    "enabled": 1
  }
}
```


### <a name="update_a_rule2"></a>![Endpoint: ](https://apidocs.io/img/method.png "Update a Rule2") `PUT` /automations/fax/receipts/{rule_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| rule_id | `precision` |  ``` Required ```  | The email receipt rule id you want to access. | `4` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `update a rule request26` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "rule_name": "My Rule",
  "match_type": 1,
  "action": "EMAIL_FIXED",
  "action_address": "john@doe.com",
  "enabled": 1
}
``` 

#### Responses
**200** 

Body (_Update a rule response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your rule incoming fax receipt has been updated.",
  "data": {
    "receipt_rule_id": 4,
    "rule_name": "My Rule",
    "match_type": 1,
    "action": "EMAIL_FIXED",
    "action_address": "john@doe.com",
    "enabled": 1
  }
}
```


### <a name="delete_a_rule2"></a>![Endpoint: ](https://apidocs.io/img/method.png "Delete a Rule2") `DELETE` /automations/fax/receipts/{rule_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| rule_id | `precision` |  ``` Required ```  | The email receipt rule id you want to delete. | `4` | 

#### Responses
**200** 

Body (_Delete a Rule response49_) 
```
{
  "http_code": 103,
  "response_code": "response_code",
  "response_msg": "response_msg",
  "data": "data"
}
```


### <a name="list_rules5"></a>![Endpoint: ](https://apidocs.io/img/method.png "List Rules5") `GET` /automations/email/receipt

> TODO: Add a method description



#### Responses
**200** 

Body (_List rules response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here is your result.",
  "data": {
    "total": 4,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 4,
    "data": [
      {
        "receipt_rule_id": 1,
        "rule_name": "Email Test Rule",
        "match_type": 0,
        "action": "URL",
        "action_address": "http://requestb.in/1821qos1",
        "enabled": 1
      },
      {
        "receipt_rule_id": 2,
        "rule_name": "test",
        "match_type": 0,
        "action": "URL",
        "action_address": "http://testurl.com",
        "enabled": 1
      },
      {
        "receipt_rule_id": 6,
        "rule_name": "test",
        "match_type": 0,
        "action": "URL",
        "action_address": "http://testurl.com",
        "enabled": 1
      },
      {
        "receipt_rule_id": 7,
        "rule_name": "test",
        "match_type": 0,
        "action": "URL",
        "action_address": "http://testurl.com",
        "enabled": 1
      }
    ]
  }
}
```


### <a name="get_a_specific_rule12"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get a Specific Rule12") `GET` /automations/email/receipt/{rule_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| rule_id | `precision` |  ``` Required ```  | The rule id you want to access. | `5` | 

#### Responses
**200** 

Body (_Get a specific rule response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here is your result.",
  "data": {
    "receipt_rule_id": 1,
    "rule_name": "Email Test Rule",
    "match_type": 0,
    "action": "URL",
    "action_address": "http://testurl.com/1821qos1",
    "enabled": 1
  }
}
```


### <a name="create_a_new_rule5"></a>![Endpoint: ](https://apidocs.io/img/method.png "Create a New Rule5") `POST` /automations/email/receipt

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `create a new rule request24` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "rule_name": "My Rule",
  "match_type": 0,
  "action": "URL",
  "action_address": "http://testurl.com",
  "enabled": 1
}
``` 

#### Responses
**200** 

Body (_Create a new rule response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Automation email receipt rule has been created.",
  "data": {
    "receipt_rule_id": 8,
    "rule_name": "My Rule",
    "match_type": 0,
    "action": "URL",
    "action_address": "http://testurl.com",
    "enabled": 1
  }
}
```


### <a name="update_a_rule12"></a>![Endpoint: ](https://apidocs.io/img/method.png "Update a Rule12") `PUT` /automations/email/receipt/{rule_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| rule_id | `precision` |  ``` Required ```  | The email receipt rule id you want to access. | `8` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `update a rule request26` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "rule_name": "My Rule",
  "match_type": 0,
  "action": "URL",
  "action_address": "http://testurl.com",
  "enabled": 1
}
``` 

#### Responses
**200** 

Body (_Update a rule response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Automation email receipt rule has been updated.",
  "data": {
    "receipt_rule_id": 8,
    "rule_name": "My Rule",
    "match_type": 0,
    "action": "URL",
    "action_address": "http://testurl.com",
    "enabled": 1
  }
}
```


### <a name="delete_a_rule12"></a>![Endpoint: ](https://apidocs.io/img/method.png "Delete a Rule12") `DELETE` /automations/email/receipt/{rule_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| rule_id | `precision` |  ``` Required ```  | The email receipt rule id you want to delete. | `8` | 

#### Responses
**200** 

Body (_Delete a Rule response56_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Automation email receipt rule has been deleted.",
  "data": true
}
```


[Back to API Reference](#api_reference)

## <a name="contact_lists"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Contact Lists") Contact Lists


### <a name="get_all_contact_lists"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get all Contact Lists") `GET` /lists

> TODO: Add a method description



#### Responses
**200** 

Body (_Get all Contact Lists response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are your data.",
  "data": {
    "total": 9,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 9,
    "data": [
      {
        "list_id": 428,
        "list_name": "List-reFSsJkvRC",
        "list_email_id": "GHPAJCCVGMTD9BLA",
        "_contacts_count": 0
      },
      {
        "list_id": 429,
        "list_name": "List6eaG4lGIc9",
        "list_email_id": "IIEXAR72O9UAZ7WW",
        "_contacts_count": 0
      },
      {
        "list_id": 430,
        "list_name": "ListwM4kJrQ7Db",
        "list_email_id": "HSA3VWFEFCZIF2WT",
        "_contacts_count": 0
      },
      {
        "list_id": 431,
        "list_name": "ListzH6Qs6Uqh5",
        "list_email_id": "HSA3VWFEFCZIF2WT",
        "_contacts_count": 0
      },
      {
        "list_id": 432,
        "list_name": "ListJaDZPg7SOy",
        "list_email_id": "3TCFYRPSW8OXRBK7",
        "_contacts_count": 0
      },
      {
        "list_id": 433,
        "list_name": "ListxseEIVS4d5",
        "list_email_id": "BCT20YT185AHVVNI",
        "_contacts_count": 0
      },
      {
        "list_id": 434,
        "list_name": "ListqX62zF5kan",
        "list_email_id": "NODYGVDCEVV9Q0CG",
        "_contacts_count": 0
      },
      {
        "list_id": 435,
        "list_name": "ListklPbrd232Z",
        "list_email_id": "VCYXAZSXNZCVJIPB",
        "_contacts_count": 0
      },
      {
        "list_id": 436,
        "list_name": "ListFfD3OIiTwJ",
        "list_email_id": "KCDKIEBYPBIYQXJQ",
        "_contacts_count": 0
      }
    ]
  }
}
```


### <a name="create_a_new_contact_list"></a>![Endpoint: ](https://apidocs.io/img/method.png "Create a new contact list") `POST` /lists

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `create a new contact list request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "list_name": "ListCT3QrVL4od"
}
``` 

#### Responses
**200** 

Body (_Create a new contact list response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "New list has been created.",
  "data": {
    "list_id": 437,
    "list_name": "ListCT3QrVL4od",
    "list_email_id": "KB0LHD6WXFVHZWTR",
    "_contacts_count": 0
  }
}
```


### <a name="get_a_specific_contact_list"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get a specific contact list") `GET` /lists/{list_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| list_id | `precision` |  ``` Required ```  | Your contact list id you want to access. | `437` | 

#### Responses
**200** 

Body (_Get a specific contact list response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are your data.",
  "data": {
    "list_id": 437,
    "list_name": "ListCT3QrVL4od",
    "list_email_id": "KB0LHD6WXFVHZWTR",
    "_contacts_count": 0
  }
}
```


### <a name="update_a_specific_contact_list"></a>![Endpoint: ](https://apidocs.io/img/method.png "Update a specific contact list") `PUT` /lists/{list_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| list_id | `precision` |  ``` Required ```  | Your contact list id you want to access. | `439` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `update a specific contact list request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "list_name": "ListlPJf33ksjP"
}
``` 

#### Responses
**200** 

Body (_Update a specific contact list response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "List #439 has been updated.",
  "data": {
    "list_id": 439,
    "list_name": "ListlPJf33ksjP",
    "list_email_id": "LINDW2NHNPKHEJB6",
    "_contacts_count": 0
  }
}
```


### <a name="delete_a_specific_contact_list"></a>![Endpoint: ](https://apidocs.io/img/method.png "Delete a specific contact list") `DELETE` /lists/{list_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| list_id | `precision` |  ``` Required ```  | Your contact list id you want to access. | `442` | 

#### Responses
**200** 

Body (_Delete a specific contact list response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "List #442 has been deleted.",
  "data": []
}
```


### <a name="import_contacts_to_list"></a>![Endpoint: ](https://apidocs.io/img/method.png "Import Contacts to List") `POST` /lists/{list_id}/import

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| list_id | `precision` |  ``` Required ```  | Your contact list id you want to access. | `437` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `import contacts to list request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "file_url": "http://yourdomain.com/5485EA6144/79E8/import.csv",
  "field_order": [
    "phone",
    "first_name",
    "last_name",
    "custom1",
    "custom2",
    "custom3",
    "custom4",
    "fax_number",
    "organization_name",
    "email",
    "address_line_1",
    "address_line_2",
    "address_city",
    "address_state",
    "address_postal_code",
    "address_country"
  ]
}
``` 

#### Responses
**200** 

Body (_Import Contacts to List response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your file is now queued.",
  "data": {
    "msg": "Messages put on queue.",
    "ids": [
      "6254358460638066203"
    ],
    "id": "6254358460638066203"
  }
}
```


### <a name="remove_duplicate_contacts"></a>![Endpoint: ](https://apidocs.io/img/method.png "Remove Duplicate Contacts") `PUT` /lists/{list_id}/remove-duplicates

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| list_id | `precision` |  ``` Required ```  | Your contact list id. | `439` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `remove duplicate contacts request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "fields": [
    "phone_number",
    "first_name",
    "last_name",
    "fax_number",
    "address_country"
  ]
}
``` 

#### Responses
**200** 

Body (_Remove Duplicate Contacts response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your list duplicate contacts has been deleted.",
  "data": {
    "deleted": 6
  }
}
```


### <a name="get_list_of_acceptable_import_fields"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get List of Acceptable Import Fields") `GET` /lists/{list_id}/import-fields

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| list_id | `string` |  ``` Optional ```  | TODO: Add a parameter description | `"list_id"` | 

#### Responses
**200** 

Body (_Get List of Acceptable Import Fields response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "List of acceptable import fields.",
  "data": [
    {
      "field": "phone",
      "label": "Phone"
    },
    {
      "field": "first_name",
      "label": "First Name"
    },
    {
      "field": "last_name",
      "label": "Last Name"
    },
    {
      "field": "custom1",
      "label": "Custom String 1"
    },
    {
      "field": "custom2",
      "label": "Custom String 2"
    },
    {
      "field": "custom3",
      "label": "Custom String 3"
    },
    {
      "field": "custom4",
      "label": "Custom String 4"
    },
    {
      "field": "fax_number",
      "label": "Fax Number"
    },
    {
      "field": "organization_name",
      "label": "Organization Name"
    },
    {
      "field": "email",
      "label": "Email"
    },
    {
      "field": "address_line_1",
      "label": "Address Line 1"
    },
    {
      "field": "address_line_2",
      "label": "Address Line 2"
    },
    {
      "field": "address_city",
      "label": "City"
    },
    {
      "field": "address_state",
      "label": "State"
    },
    {
      "field": "address_postal_code",
      "label": "Postal Code"
    },
    {
      "field": "address_country",
      "label": "Country"
    }
  ]
}
```


### <a name="show_csv_import_file_preview"></a>![Endpoint: ](https://apidocs.io/img/method.png "Show CSV Import File Preview") `POST` /lists/{list_id}/import-csv-preview

> Show first row of the csv import file.



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| list_id | `precision` |  ``` Required ```  | Your contact list id. | `439` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `show csv import file preview request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "file_url": "http://yourdomain.com/5485EA6144/79E8/import.csv"
}
``` 

#### Responses
**200** 

Body (_Show CSV Import File Preview response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your file preview.",
  "data": {
    "row": [
      "61298444214",
      "John",
      "Doe 1",
      "Custom A 1",
      "Custom B 1",
      "Custom C 1",
      "Custom D 1",
      "61298444214",
      "Organization 1",
      "johndoe1@gmail.com",
      "3842",
      "Worley Avenue",
      "Altavista",
      "VA",
      "24517",
      "PH"
    ]
  }
}
```


[Back to API Reference](#api_reference)

## <a name="contact_suggestions"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Contact Suggestions") Contact Suggestions


### <a name="list_contact_suggestions"></a>![Endpoint: ](https://apidocs.io/img/method.png "List Contact Suggestions") `GET` /contact-suggestions

> TODO: Add a method description



#### Responses
**200** 

Body (_List Contact Suggestions response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are your results.",
  "data": [
    {
      "contact_id": 4,
      "list_id": 429,
      "phone_number": "+61298444214",
      "first_name": "John",
      "last_name": "Doe",
      "custom_1": "Custom A 1",
      "custom_2": "Custom B 1",
      "custom_3": "Custom C 1",
      "custom_4": "Custom D 1",
      "date_added": "1462856443",
      "fax_number": "+61298444214",
      "organization_name": "Organization 1",
      "email": "johndoe1@gmail.com",
      "address_line_1": "3842",
      "address_line_2": "Worley Avenue",
      "address_city": "Altavista",
      "address_state": "VA",
      "address_postal_code": "24517",
      "address_country": "AU",
      "_list_name": "List6eaG4lGIc9"
    },
    {
      "contact_id": 5,
      "list_id": 429,
      "phone_number": "+61298444214",
      "first_name": "John",
      "last_name": "Doe",
      "custom_1": "Custom A 2",
      "custom_2": "Custom B 1",
      "custom_3": "Custom C 1",
      "custom_4": "Custom D 1",
      "date_added": "1462856443",
      "fax_number": "+61298444214",
      "organization_name": "Organization 1",
      "email": "johndoe1@gmail.com",
      "address_line_1": "3842",
      "address_line_2": "Worley Avenue",
      "address_city": "Altavista",
      "address_state": "VA",
      "address_postal_code": "24517",
      "address_country": "AU",
      "_list_name": "List6eaG4lGIc9"
    },
    {
      "contact_id": 6,
      "list_id": 429,
      "phone_number": "+61298444214",
      "first_name": "John",
      "last_name": "Doe",
      "custom_1": "Custom A 3",
      "custom_2": "Custom B 1",
      "custom_3": "Custom C 1",
      "custom_4": "Custom D 1",
      "date_added": "1462856443",
      "fax_number": "+61298444214",
      "organization_name": "Organization 1",
      "email": "johndoe1@gmail.com",
      "address_line_1": "3842",
      "address_line_2": "Worley Avenue",
      "address_city": "Altavista",
      "address_state": "VA",
      "address_postal_code": "24517",
      "address_country": "AU",
      "_list_name": "List6eaG4lGIc9"
    },
    {
      "contact_id": 7,
      "list_id": 429,
      "phone_number": "+61298444214",
      "first_name": "John",
      "last_name": "Doe",
      "custom_1": "Custom A 4",
      "custom_2": "Custom B 1",
      "custom_3": "Custom C 1",
      "custom_4": "Custom D 1",
      "date_added": "1462856443",
      "fax_number": "+61298444214",
      "organization_name": "Organization 1",
      "email": "johndoe1@gmail.com",
      "address_line_1": "3842",
      "address_line_2": "Worley Avenue",
      "address_city": "Altavista",
      "address_state": "VA",
      "address_postal_code": "24517",
      "address_country": "AU",
      "_list_name": "List6eaG4lGIc9"
    },
    {
      "contact_id": 8,
      "list_id": 429,
      "phone_number": "+61298444214",
      "first_name": "John",
      "last_name": "Doe",
      "custom_1": "Custom A 5",
      "custom_2": "Custom B 1",
      "custom_3": "Custom C 1",
      "custom_4": "Custom D 1",
      "date_added": "1462856443",
      "fax_number": "+61298444214",
      "organization_name": "Organization 1",
      "email": "johndoe1@gmail.com",
      "address_line_1": "3842",
      "address_line_2": "Worley Avenue",
      "address_city": "Altavista",
      "address_state": "VA",
      "address_postal_code": "24517",
      "address_country": "AU",
      "_list_name": "List6eaG4lGIc9"
    },
    {
      "contact_id": 9,
      "list_id": 429,
      "phone_number": "+61298444214",
      "first_name": "John",
      "last_name": "Doe",
      "custom_1": "Custom A 6",
      "custom_2": "Custom B 1",
      "custom_3": "Custom C 1",
      "custom_4": "Custom D 1",
      "date_added": "1462856443",
      "fax_number": "+61298444214",
      "organization_name": "Organization 1",
      "email": "johndoe1@gmail.com",
      "address_line_1": "3842",
      "address_line_2": "Worley Avenue",
      "address_city": "Altavista",
      "address_state": "VA",
      "address_postal_code": "24517",
      "address_country": "AU",
      "_list_name": "List6eaG4lGIc9"
    },
    {
      "contact_id": 10,
      "list_id": 429,
      "phone_number": "+61298444214",
      "first_name": "John",
      "last_name": "Doe",
      "custom_1": "Custom A 7",
      "custom_2": "Custom B 1",
      "custom_3": "Custom C 1",
      "custom_4": "Custom D 1",
      "date_added": "1462856443",
      "fax_number": "+61298444214",
      "organization_name": "Organization 1",
      "email": "johndoe1@gmail.com",
      "address_line_1": "3842",
      "address_line_2": "Worley Avenue",
      "address_city": "Altavista",
      "address_state": "VA",
      "address_postal_code": "24517",
      "address_country": "AU",
      "_list_name": "List6eaG4lGIc9"
    },
    {
      "contact_id": 11,
      "list_id": 429,
      "phone_number": "+61298444214",
      "first_name": "John",
      "last_name": "Doe",
      "custom_1": "Custom A 8",
      "custom_2": "Custom B 1",
      "custom_3": "Custom C 1",
      "custom_4": "Custom D 1",
      "date_added": "1462856443",
      "fax_number": "+61298444214",
      "organization_name": "Organization 1",
      "email": "johndoe1@gmail.com",
      "address_line_1": "3842",
      "address_line_2": "Worley Avenue",
      "address_city": "Altavista",
      "address_state": "VA",
      "address_postal_code": "24517",
      "address_country": "AU",
      "_list_name": "List6eaG4lGIc9"
    }
  ]
}
```


[Back to API Reference](#api_reference)

## <a name="contacts"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Contacts") Contacts


### <a name="get_all_contacts_in_a_list"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get all Contacts in a List") `GET` /lists/{list_id}/contacts

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| list_id | `precision` |  ``` Required ```  | Your contact list id where your contacts belong. | `428` | 

#### Responses
**200** 

Body (_Get all Contacts in a List response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are your data.",
  "data": {
    "total": 6,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 6,
    "data": [
      {
        "contact_id": 552786,
        "list_id": 428,
        "phone_number": "+16783270696",
        "first_name": "Ellen",
        "last_name": "Diaz",
        "custom_1": "",
        "custom_2": "",
        "custom_3": "",
        "custom_4": "",
        "date_added": "1436157486",
        "fax_number": null,
        "organization_name": null,
        "email": null,
        "address_line_1": null,
        "address_line_2": null,
        "address_city": null,
        "address_state": null,
        "address_postal_code": null,
        "address_country": null,
        "_list_name": "List6eaG4lGIc9"
      },
      {
        "contact_id": 552787,
        "list_id": 428,
        "phone_number": "+16783270697",
        "first_name": "Ellen",
        "last_name": "Diaz",
        "custom_1": "",
        "custom_2": "",
        "custom_3": "",
        "custom_4": "",
        "date_added": "1436157925",
        "fax_number": null,
        "organization_name": null,
        "email": null,
        "address_line_1": null,
        "address_line_2": null,
        "address_city": null,
        "address_state": null,
        "address_postal_code": null,
        "address_country": null,
        "_list_name": "List6eaG4lGIc9"
      },
      {
        "contact_id": 552790,
        "list_id": 428,
        "phone_number": "+16783271811",
        "first_name": "Ellen",
        "last_name": "Diaz",
        "custom_1": "",
        "custom_2": "",
        "custom_3": "",
        "custom_4": "",
        "date_added": "1436158227",
        "fax_number": null,
        "organization_name": null,
        "email": null,
        "address_line_1": null,
        "address_line_2": null,
        "address_city": null,
        "address_state": null,
        "address_postal_code": null,
        "address_country": null,
        "_list_name": "List6eaG4lGIc9"
      },
      {
        "contact_id": 552791,
        "list_id": 428,
        "phone_number": "+16783271975",
        "first_name": "Ellen",
        "last_name": "Diaz",
        "custom_1": "",
        "custom_2": "",
        "custom_3": "",
        "custom_4": "",
        "date_added": "1436158297",
        "fax_number": null,
        "organization_name": null,
        "email": null,
        "address_line_1": null,
        "address_line_2": null,
        "address_city": null,
        "address_state": null,
        "address_postal_code": null,
        "address_country": null,
        "_list_name": "List6eaG4lGIc9"
      },
      {
        "contact_id": 552789,
        "list_id": 428,
        "phone_number": "+16783272925",
        "first_name": "Ellen",
        "last_name": "Diaz",
        "custom_1": "",
        "custom_2": "",
        "custom_3": "",
        "custom_4": "",
        "date_added": "1436158143",
        "fax_number": null,
        "organization_name": null,
        "email": null,
        "address_line_1": null,
        "address_line_2": null,
        "address_city": null,
        "address_state": null,
        "address_postal_code": null,
        "address_country": null,
        "_list_name": "List6eaG4lGIc9"
      },
      {
        "contact_id": 552788,
        "list_id": 428,
        "phone_number": "+16783273589",
        "first_name": "Ellen",
        "last_name": "Diaz",
        "custom_1": "",
        "custom_2": "",
        "custom_3": "",
        "custom_4": "",
        "date_added": "1436158047",
        "fax_number": null,
        "organization_name": null,
        "email": null,
        "address_line_1": null,
        "address_line_2": null,
        "address_city": null,
        "address_state": null,
        "address_postal_code": null,
        "address_country": null,
        "_list_name": "List6eaG4lGIc9"
      }
    ]
  }
}
```


### <a name="create_a_new_contact"></a>![Endpoint: ](https://apidocs.io/img/method.png "Create a new contact") `POST` /lists/{list_id}/contacts

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| list_id | `precision` |  ``` Required ```  | Your contact list id where your contact be associated. | `428` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `create a new contact request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "phone_number": "+16783270696",
  "first_name": "Ellen",
  "last_name": "Diaz",
  "custom_1": "Custom 1",
  "custom_2": "Custom 2",
  "custom_3": "Custom 3",
  "custom_4": "Custom 4",
  "fax_number": "+16783270696",
  "organization_name": "Awesome Organization",
  "email": "ellen@diaz.com",
  "address_line_1": "Block 2",
  "address_line_2": "Cool Bldg.",
  "address_city": "Nevada",
  "address_state": "Las Vegas",
  "address_postal_code": "36063",
  "address_country": "US"
}
``` 

#### Responses
**200** 

Body (_Create a new contact response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "New contact has been created.",
  "data": {
    "contact_id": 552802,
    "list_id": 428,
    "phone_number": "+16783270696",
    "first_name": "Ellen",
    "last_name": "Diaz",
    "custom_1": "Custom 1",
    "custom_2": "Custom 2",
    "custom_3": "Custom 3",
    "custom_4": "Custom 4",
    "date_added": "1436160803",
    "fax_number": "+16783270696",
    "organization_name": "Awesome Organization",
    "email": "ellen@diaz.com",
    "address_line_1": "Block 2",
    "address_line_2": "Cool Bldg.",
    "address_city": "Nevada",
    "address_state": "Las Vegas",
    "address_postal_code": "36063",
    "address_country": "US",
    "_list_name": "List6eaG4lGIc9"
  }
}
```


### <a name="get_a_specific_contact"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get a specific contact") `GET` /lists/{list_id}/contacts/{contact_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| list_id | `precision` |  ``` Required ```  | Your contact list id you want to access. | `428` | 
| contact_id | `precision` |  ``` Required ```  | Your contact id you want to access. | `552802` | 

#### Responses
**200** 

Body (_Get a specific contact response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are your data.",
  "data": {
    "contact_id": 552802,
    "list_id": 428,
    "phone_number": "+16783270696",
    "first_name": "Ellen",
    "last_name": "Diaz",
    "custom_1": "Custom 1",
    "custom_2": "Custom 2",
    "custom_3": "Custom 3",
    "custom_4": "Custom 4",
    "date_added": "1436160803",
    "fax_number": "+16783270696",
    "organization_name": "Awesome Organization",
    "email": "ellen@diaz.com",
    "address_line_1": "Block 2",
    "address_line_2": "Cool Bldg.",
    "address_city": "Nevada",
    "address_state": "Las Vegas",
    "address_postal_code": "36063",
    "address_country": "US",
    "_list_name": "List6eaG4lGIc9"
  }
}
```


### <a name="update_a_specific_contact"></a>![Endpoint: ](https://apidocs.io/img/method.png "Update a specific contact") `PUT` /lists/{list_id}/contacts/{contact_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| list_id | `precision` |  ``` Required ```  | Your contact list id you want to access. | `428` | 
| contact_id | `precision` |  ``` Required ```  | Your contact id you want to access. | `552802` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `update a specific contact request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "phone_number": "+16783275492",
  "first_name": "Ellen",
  "last_name": "Diaz",
  "custom_1": "Custom S72oJ9Teba",
  "custom_2": "Custom NvrRJrKWeq",
  "custom_3": "Custom 2ws94p1Dop",
  "custom_4": "Custom Ku0AaIS5xb",
  "fax_number": "+16783276356",
  "organization_name": "Awesome Organization",
  "email": "ellen@diaz.com",
  "address_line_1": "Block 6",
  "address_line_2": "Cool Bldg.",
  "address_city": "Nevada",
  "address_state": "Las Vegas",
  "address_postal_code": "36063",
  "address_country": "US"
}
``` 

#### Responses
**200** 

Body (_Update a specific contact response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Contact #552807 has been updated.",
  "data": {
    "contact_id": 552807,
    "list_id": 428,
    "phone_number": "+16783275492",
    "first_name": "Ellen",
    "last_name": "Diaz",
    "custom_1": "Custom S72oJ9Teba",
    "custom_2": "Custom NvrRJrKWeq",
    "custom_3": "Custom 2ws94p1Dop",
    "custom_4": "Custom Ku0AaIS5xb",
    "date_added": "1436161955",
    "fax_number": "+16783276356",
    "organization_name": "Awesome Organization",
    "email": "ellen@diaz.com",
    "address_line_1": "Block 6",
    "address_line_2": "Cool Bldg.",
    "address_city": "Nevada",
    "address_state": "Las Vegas",
    "address_postal_code": "36063",
    "address_country": "US",
    "_list_name": "List6eaG4lGIc9"
  }
}
```


### <a name="delete_a_specific_contact"></a>![Endpoint: ](https://apidocs.io/img/method.png "Delete a specific contact") `DELETE` /lists/{list_id}/contacts/{contact_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| list_id | `precision` |  ``` Required ```  | Your contact list id you want to access. | `428` | 
| contact_id | `precision` |  ``` Required ```  | Your contact id you want to access. | `552807` | 

#### Responses
**200** 

Body (_Delete a specific contact response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Contact #552807 has been deleted.",
  "data": []
}
```


### <a name="remove_opted_out_contacts"></a>![Endpoint: ](https://apidocs.io/img/method.png "Remove Opted Out Contacts") `PUT` /lists/{list_id}/remove-opted-out-contacts/{opt_out_list_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| list_id | `precision` |  ``` Required ```  | Your contact list id. | `439` | 
| opt_out_list_id | `precision` |  ``` Required ```  | Your opt out list id. | `512` | 

#### Responses
**200** 

Body (_Remove Opted Out Contacts response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Optout contacts has been deleted.",
  "data": {
    "deleted": 6
  }
}
```


### <a name="transfer_a_contact"></a>![Endpoint: ](https://apidocs.io/img/method.png "Transfer a Contact") `PUT` /lists/{from_list_id}/contacts/{contact_id}/{to_list_id}

> Transfers a specific contact to another list.



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| from_list_id | `precision` |  ``` Required ```  | From list id. | `428` | 
| contact_id | `precision` |  ``` Required ```  | Contact ID. | `1` | 
| to_list_id | `precision` |  ``` Required ```  | To list id. | `429` | 

#### Responses
**200** 

Body (_Transfer a Contact response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Contact #1 has been transferred to List #429",
  "data": {
    "contact_id": 1,
    "list_id": 429,
    "phone_number": "+61477141888",
    "first_name": "John",
    "last_name": "Doe",
    "custom_1": "Custom 1",
    "custom_2": "Custom 2",
    "custom_3": "Custom 3",
    "custom_4": "Custom 4",
    "date_added": "1456721694",
    "fax_number": "+61477141888",
    "organization_name": "Awesome Company",
    "email": "john@doe.com",
    "address_line_1": "1554 Buffalo Creek Road",
    "address_line_2": null,
    "address_city": "Nashville",
    "address_state": "TN",
    "address_postal_code": "37214",
    "address_country": "US",
    "_list_name": "List6eaG4lGIc9"
  }
}
```


### <a name="hello_contact"></a>![Endpoint: ](https://apidocs.io/img/method.png "Hello Contact") `GET` /getcontact

> TODO: Add a method description



#### Responses
**200**


[Back to API Reference](#api_reference)

## <a name="countries"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Countries") Countries


### <a name="get_all_countries"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get all Countries") `GET` /countries

> TODO: Add a method description



#### Responses
**200** 

Body (_Get all Countries response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "List of Countries.",
  "data": [
    {
      "code": "AF",
      "value": "Afghanistan"
    },
    {
      "code": "AU",
      "value": "Australia"
    },
    {
      "code": "FI",
      "value": "Finland"
    },
    {
      "code": "FR",
      "value": "France"
    },
    {
      "code": "AE",
      "value": "United Arab Emirates"
    },
    {
      "code": "GB",
      "value": "United Kingdom"
    },
    {
      "code": "US",
      "value": "United States of America"
    },
    {
      "code": "ZW",
      "value": "Zimbabwe"
    }
  ]
}
```


[Back to API Reference](#api_reference)

## <a name="delivery_issues"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Delivery Issues") Delivery Issues


### <a name="get_delivery_issues"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Delivery Issues") `GET` /delivery-issues

> TODO: Add a method description



#### Responses
**200** 

Body (_Get Delivery Issues response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here is your result.",
  "data": {
    "total": 5,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 7,
    "data": [
      {
        "issue_id": 1,
        "user_id": 3820,
        "message_id": "B388828B-AD46-4366-8AD3-0305FF5E3FE5",
        "type": "sms",
        "description": "this is a test.",
        "client_comments": null,
        "support_comments": null,
        "status": null,
        "date_added": 1481610495,
        "resolved": 0,
        "email_address": "test@user.com"
      },
      {
        "issue_id": 2,
        "user_id": 3820,
        "message_id": "90396A38-146B-46C4-A455-675F620C2E05",
        "type": "sms",
        "description": "this is a test.",
        "client_comments": null,
        "support_comments": null,
        "status": null,
        "date_added": 1481610523,
        "resolved": 0,
        "email_address": "test@user.com"
      },
      {
        "issue_id": 3,
        "user_id": 3820,
        "message_id": "4ECFB6CB-0300-45EC-96E1-5AB189432AF5",
        "type": "sms",
        "description": "this is a test.",
        "client_comments": null,
        "support_comments": null,
        "status": null,
        "date_added": 1481611389,
        "resolved": 0,
        "email_address": "test@user.com"
      },
      {
        "issue_id": 4,
        "user_id": 3820,
        "message_id": "test",
        "type": "sms",
        "description": "this is a test.",
        "client_comments": null,
        "support_comments": null,
        "status": null,
        "date_added": 1481611467,
        "resolved": 0,
        "email_address": "test@user.com"
      },
      {
        "issue_id": 5,
        "user_id": 3820,
        "message_id": "test",
        "type": "SMS",
        "description": "this is a test.",
        "client_comments": null,
        "support_comments": null,
        "status": null,
        "date_added": 1481614516,
        "resolved": 0,
        "email_address": "test@user.com"
      }
    ]
  }
}
```


### <a name="create_delivery_issue"></a>![Endpoint: ](https://apidocs.io/img/method.png "Create Delivery Issue") `POST` /delivery-issues

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `create delivery issue request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "message_id": "B388828B",
  "type": "SMS",
  "description": "This is a test",
  "client_comments": "test",
  "email_address: john_doe@user.com": "",
  "Body": ""
}
``` 

#### Responses
**200** 

Body (_Create Delivery Issue response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Delivery issue has been created.",
  "data": {
    "issue_id": 9,
    "user_id": 3820,
    "message_id": "B388828B-AD46-4366-8AD3-0305FF5E3FE5",
    "type": "SMS",
    "description": "this is a test.",
    "date_added": 1481617579,
    "email_address": "john_doe@user.com"
  }
}
```


[Back to API Reference](#api_reference)

## <a name="email_marketing"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Email Marketing") Email Marketing


### <a name="get_all_allowed_email_addresses"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get All Allowed Email Addresses") `GET` /email/addresses

> TODO: Add a method description



#### Responses
**200** 

Body (_Get All Allowed Email Addresses response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are your email addresses",
  "data": {
    "total": 2,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 2,
    "data": [
      {
        "email_address_id": 2,
        "email_address": "test@user.com",
        "verified": 1,
        "date_added": "1447736880"
      },
      {
        "email_address_id": 3,
        "email_address": "test2@user.com",
        "verified": 0,
        "date_added": "1449042967"
      }
    ]
  }
}
```


### <a name="create_allowed_email_address"></a>![Endpoint: ](https://apidocs.io/img/method.png "Create Allowed Email Address") `POST` /email/addresses

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `create allowed email address request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "email_address": "johndoe1@user.com",
  "Body": ""
}
``` 

#### Responses
**200** 

Body (_Create Allowed Email Address response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Email address has been created.",
  "data": {
    "email_address_id": 5,
    "email_address": "test222@user.com",
    "verified": 0,
    "date_added": "1458009394"
  }
}
```


### <a name="send_verification_token"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send Verification Token") `PUT` /email/address-verify/{email_address_id}/send

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| email_address_id | `precision` |  ``` Required ```  | The email addess id you want to access. | `1` | 

#### Responses
**200** 

Body (_Send Verification Token response_) 
```
{
  "http_code": 195,
  "response_code": "response_code",
  "response_msg": "response_msg",
  "data": "data"
}
```


### <a name="verify_allowed_email_address"></a>![Endpoint: ](https://apidocs.io/img/method.png "Verify Allowed Email Address") `PUT` /email/address-verify/{email_address_id}/verify/{activation_token}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| email_address_id | `precision` |  ``` Required ```  | The email address id you want to access. | `5` | 
| activation_token | `string` |  ``` Required ```  | 6E8B-4FDB-99A7-7ED08DF97BCC (required, string) - Your activation token. | `3BD73304` | 

#### Responses
**200** 

Body (_Verify Allowed Email Address response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Email address verified.",
  "data": {
    "email_address_id": 5,
    "email_address": "test222@user.com",
    "verified": 1,
    "date_added": "1458009394"
  }
}
```


### <a name="delete_allowed_email_address"></a>![Endpoint: ](https://apidocs.io/img/method.png "Delete Allowed Email Address") `DELETE` /email/addresses/{email_address_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| email_address_id | `precision` |  ``` Required ```  | The email address you want to access. | `5` | 

#### Responses
**200** 

Body (_Delete Allowed Email Address response_) 
```
{
  "http_code": 195,
  "response_code": "response_code",
  "response_msg": "response_msg",
  "data": "data"
}
```


### <a name="get_specific_allowed_email_address"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Specific Allowed Email Address") `GET` /email/addresses/{email_address_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| email_address_id | `precision` |  ``` Required ```  | The email address you want to access. | `4` | 

#### Responses
**200** 

Body (_Get Specific Allowed Email Address response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here is your email address.",
  "data": {
    "email_address_id": 4,
    "email_address": "test3@user.com",
    "verified": 0,
    "date_added": "1449043066"
  }
}
```


### <a name="get_all_email_campaigns"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get All Email Campaigns") `GET` /email-campaigns

> TODO: Add a method description



#### Responses
**200** 

Body (_Get All Email Campaigns response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are your email campaigns",
  "data": {
    "total": 5,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 5,
    "data": [
      {
        "email_campaign_id": 64,
        "name": "test email",
        "user_id": 1201,
        "subaccount_id": 1038,
        "subject": "My test subject",
        "list_id": 443,
        "from_email_address_id": 2,
        "from_name": "Test name",
        "template_id": 24,
        "schedule": "",
        "status": "Sent",
        "date_added": "1455586793",
        "custom_string": "",
        "send_count": 0,
        "open_count": 5,
        "click_count": 0,
        "hard_bounce_count": 0,
        "soft_bounce_count": 0,
        "abuse_count": 0,
        "unsubscribe_count": 0
      },
      {
        "email_campaign_id": 65,
        "name": "test email",
        "user_id": 1201,
        "subaccount_id": 1038,
        "subject": "My test subject",
        "list_id": 443,
        "from_email_address_id": 2,
        "from_name": "Test name",
        "template_id": 24,
        "schedule": "",
        "status": "Queued",
        "date_added": "1455586848",
        "custom_string": "",
        "send_count": 0,
        "open_count": 0,
        "click_count": 0,
        "hard_bounce_count": 0,
        "soft_bounce_count": 0,
        "abuse_count": 0,
        "unsubscribe_count": 0
      }
    ]
  }
}
```


### <a name="get_specific_email_campaign"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Specific Email Campaign") `GET` /email-campaigns/{email_campaign_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| email_campaign_id | `precision` |  ``` Required ```  | The email campaign id you want to access. | `1` | 

#### Responses
**200** 

Body (_Get Specific Email Campaign response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here is your email campaign.",
  "data": {
    "email_campaign_id": 64,
    "name": "test email",
    "user_id": 1201,
    "subaccount_id": 1038,
    "subject": "My test subject",
    "list_id": 443,
    "from_email_address_id": 2,
    "from_name": "Test name",
    "template_id": 24,
    "schedule": "",
    "status": "Sent",
    "date_added": "1455586793",
    "custom_string": "",
    "send_count": 0,
    "open_count": 5,
    "click_count": 0,
    "hard_bounce_count": 0,
    "soft_bounce_count": 0,
    "abuse_count": 0,
    "unsubscribe_count": 0,
    "body": "<!DOCTYPE html PUBLIC \"-//W3C//DTD HTML 4.0 Transitional//EN\" \"http://www.w3.org/TR/REC-html40/loose.dtd\">\n<html><body><p>This is a test</p></body></html>\n",
    "body_plain_text": "This is a test"
  }
}
```


### <a name="create_email_campaign"></a>![Endpoint: ](https://apidocs.io/img/method.png "Create Email Campaign") `POST` /email-campaigns/send

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `create email campaign request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "name": "John Doe",
  "subject": "Lorem Ipsum",
  "from_email_address_id": 2,
  "from_name": "From name",
  "template_id": 31,
  "body": "<p>This is a test</p>",
  "list_id": 456
}
``` 

#### Responses
**200** 

Body (_Create Email Campaign response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Email campaign has been created.",
  "data": {
    "total_count": 6,
    "total_price": "0.0066",
    "queued_count": 2,
    "data": {
      "email_campaign_id": 69,
      "name": "John Doe",
      "user_id": 1201,
      "subaccount_id": 1038,
      "subject": "Lorem Ipsum",
      "list_id": 456,
      "from_email_address_id": 2,
      "from_name": "From name",
      "template_id": 31,
      "schedule": "",
      "status": "Queued",
      "date_added": "1458011424",
      "custom_string": "",
      "send_count": 0,
      "open_count": 0,
      "click_count": 0,
      "hard_bounce_count": 0,
      "soft_bounce_count": 0,
      "abuse_count": 0,
      "unsubscribe_count": 0,
      "body": "<p>This is a test</p>",
      "body_plain_text": "This is a test"
    },
    "currency": {
      "currency_name_short": "AUD",
      "currency_prefix_d": "$",
      "currency_prefix_c": "c",
      "currency_name_long": "Australian Dollars"
    }
  }
}
```


### <a name="update_email_campaign"></a>![Endpoint: ](https://apidocs.io/img/method.png "Update Email Campaign") `PUT` /email-campaigns/{email_campaign_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| email_campaign_id | `precision` |  ``` Required ```  | The email campaign id you want to access. | `1` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `update email campaign request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "name": "John Doe",
  "subject": "Lorem Ipsum",
  "from_email_address_id": 2,
  "from_name": "From name",
  "template_id": 31,
  "body": "<p>This is a test</p>",
  "list_id": 456
}
``` 

#### Responses
**200** 

Body (_Update Email Campaign response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Email campaign has been updated.",
  "data": {
    "email_campaign_id": 69,
    "name": "John Doe",
    "user_id": 1201,
    "subaccount_id": 1038,
    "subject": "Lorem Ipsum",
    "list_id": 456,
    "from_email_address_id": 2,
    "from_name": "From name",
    "template_id": 31,
    "schedule": "13213213212",
    "status": "Scheduled",
    "date_added": "1458011424",
    "custom_string": "",
    "send_count": 0,
    "open_count": 0,
    "click_count": 0,
    "hard_bounce_count": 0,
    "soft_bounce_count": 0,
    "abuse_count": 0,
    "unsubscribe_count": 0,
    "body": "<p>This is a test</p>",
    "body_plain_text": "This is a test"
  }
}
```


### <a name="cancel_email_campaign"></a>![Endpoint: ](https://apidocs.io/img/method.png "Cancel Email Campaign") `PUT` /email-campaigns/{email_campaign_id}/cancel

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| email_campaign_id | `precision` |  ``` Required ```  | The email campaign id you want to cancel. | `1` | 

#### Responses
**200** 

Body (_Cancel Email Campaign response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Email campaign has been cancelled.",
  "data": {
    "email_campaign_id": 69,
    "name": "John Doe",
    "user_id": 1201,
    "subaccount_id": 1038,
    "subject": "Lorem Ipsum",
    "list_id": 456,
    "from_email_address_id": 2,
    "from_name": "From name",
    "template_id": 31,
    "schedule": "13213213212",
    "status": "Cancelled",
    "date_added": "1458011424",
    "custom_string": "",
    "send_count": 0,
    "open_count": 0,
    "click_count": 0,
    "hard_bounce_count": 0,
    "soft_bounce_count": 0,
    "abuse_count": 0,
    "unsubscribe_count": 0,
    "body": "<p>This is a test</p>",
    "body_plain_text": "This is a test"
  }
}
```


### <a name="calculate_price"></a>![Endpoint: ](https://apidocs.io/img/method.png "Calculate Price") `POST` /email-campaigns/price

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `calculate price request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "name": "John Doe",
  "subject": "Lorem Ipsum",
  "from_email_address_id": 2,
  "from_name": "From name",
  "template_id": 31,
  "body": "<p>This is a test</p>",
  "list_id": 456
}
``` 

#### Responses
**200** 

Body (_Calculate Price response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Total price for email campaign.",
  "data": {
    "total_count": 6,
    "total_price": "0.0066",
    "queued_count": 2,
    "data": {
      "name": "John Doe",
      "subject": "Lorem Ipsum",
      "from_email_address_id": 2,
      "from_name": "From name",
      "template_id": 31,
      "body": "<p>This is a test</p>",
      "list_id": 456
    },
    "currency": {
      "currency_name_short": "AUD",
      "currency_prefix_d": "$",
      "currency_prefix_c": "c",
      "currency_name_long": "Australian Dollars"
    }
  }
}
```


### <a name="get_specific_email_campaign_history"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Specific Email Campaign History") `GET` /email-campaigns/{campaign_id}/history

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| campaign_id | `precision` |  ``` Required ```  | The email campaign id you want to access. | `77` | 

#### Responses
**200** 

Body (_Get Specific Email Campaign History response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here is your result.",
  "data": {
    "total": 3,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 3,
    "data": [
      {
        "email_campaign_id": 77,
        "from_name": "test name",
        "from_address": "4",
        "to_name": "test2@test.com",
        "to_address": "test2@test.com",
        "contact_id": 669105,
        "subject": "tet subject",
        "message_id": "7CB3227C-7F8C-4A72-A0CB-36283236D99F",
        "processed_at": null,
        "status": "SpamReport",
        "open_count": 0,
        "click_count": 0,
        "hard_bounce_count": 13,
        "soft_bounce_count": 1
      },
      {
        "email_campaign_id": 77,
        "from_name": "test name",
        "from_address": "4",
        "to_name": "test@test.com",
        "to_address": "test@test.com",
        "contact_id": 669104,
        "subject": "tet subject",
        "message_id": "603C5349-5A24-40B4-89ED-F7619F7CC8A3",
        "processed_at": null,
        "status": null,
        "open_count": 0,
        "click_count": 0,
        "hard_bounce_count": 0,
        "soft_bounce_count": 0
      },
      {
        "email_campaign_id": 77,
        "from_name": "test name",
        "from_address": "4",
        "to_name": "test2@test.com",
        "to_address": "test2@test.com",
        "contact_id": 669105,
        "subject": "tet subject",
        "message_id": "5C5C0918-B263-42AA-8B5D-9E8ACECC0C64",
        "processed_at": null,
        "status": null,
        "open_count": 0,
        "click_count": 0,
        "hard_bounce_count": 0,
        "soft_bounce_count": 0
      }
    ]
  }
}
```


### <a name="get_all_email_templates"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get All Email Templates") `GET` /email/templates

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.



#### Responses
**200** 

Body (_Get All Email Templates response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are your email templates.",
  "data": {
    "total": 2,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 2,
    "data": [
      {
        "template_id": 281,
        "template_name": "Test"
      },
      {
        "template_id": 290,
        "template_name": "Minions"
      }
    ]
  }
}
```


### <a name="get_specific_email_template"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Specific Email Template") `GET` /email/templates/{template_id}

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| template_id | `precision` |  ``` Required ```  | The email template id. | `291` | 

#### Responses
**200** 

Body (_Get Specific Email Template response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here is your email template.",
  "data": {
    "template_id": 281,
    "template_id_master": 11,
    "template_name": "Test",
    "body": "<div id=\"nb_wrapper\"><!DOCTYPE html PUBLIC \"-//W3C//DTD XHTML 1.0 Transitional//EN\" \"http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd\"> \n<html xmlns:v=\"urn:schemas-microsoft-com:vml\">\n<head>\n\n   <!-- Define Charset -->\n   ..."
  }
}
```


### <a name="create_new_email_template_from_master_template"></a>![Endpoint: ](https://apidocs.io/img/method.png "Create New Email Template from Master Template") `POST` /email/templates

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `create new email template from master template request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "template_name": "Minions",
  "template_id_master": 57
}
``` 

#### Responses
**200** 

Body (_Create New Email Template from Master Template response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "New email template has been saved.",
  "data": {
    "template_id": 292,
    "template_id_master": 57,
    "template_name": "new minion template!",
    "body": "<div id=\"nb_wrapper\"><!DOCTYPE html PUBLIC \"-//W3C//DTD XHTML 1.0 Transitional//EN\"..."
  }
}
```


### <a name="update_an_email_template"></a>![Endpoint: ](https://apidocs.io/img/method.png "Update an Email Template") `PUT` /email/templates/{template_id}

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| template_id | `precision` |  ``` Required ```  | The id of the template to be updated. | `291` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `update an email template request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "template_name": "Minions",
  "body": "This is a sample content: Sc0KNWgSMG for this template."
}
``` 

#### Responses
**200** 

Body (_Update an Email Template response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your email template has been updated.",
  "data": {
    "template_id": 281,
    "template_id_master": 11,
    "template_name": "NewTemplate",
    "body": "This is the new body of your template"
  }
}
```


### <a name="delete_email_template"></a>![Endpoint: ](https://apidocs.io/img/method.png "Delete Email Template") `DELETE` /email/templates/{template_id}

> These are your templates which can be edited and saved. You can create an email template by cloning from a Master Template.



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| template_id | `precision` |  ``` Required ```  | Your template id. | `25` | 

#### Responses
**200** 

Body (_Delete Email Template response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your email template has been deleted.",
  "data": []
}
```


### <a name="get_all_master_email_templates"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get All Master Email Templates") `GET` /email/master-templates

> Master templates are templates that you can clone to a User Email Template which lets you edit and save it.



#### Responses
**200** 

Body (_Get All Master Email Templates response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "List of Email Master Templates",
  "data": [
    {
      "template_id_master": 57,
      "template_name": "Basic 2",
      "date_added": "1458182912",
      "thumbnail": {
        "small": "https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_email-marketing/_templates-master/basic2/thumb-small.jpg",
        "large": "https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_email-marketing/_templates-master/basic2/thumb-large.jpg"
      }
    },
    {
      "template_id_master": 1,
      "template_name": "Minty",
      "date_added": "1445848821",
      "thumbnail": {
        "small": "https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_email-marketing/_templates-master/minty/thumb-small.jpg",
        "large": "https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_email-marketing/_templates-master/minty/thumb-large.jpg"
      }
    }
  ]
}
```


### <a name="get_specific_master_template"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Specific Master Template") `GET` /email/master-templates/{template_id}

> Master templates are templates that you can clone to a User Email Template which lets you edit and save it.



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| template_id | `string` |  ``` Required ```  | Your template id. | `25` | 

#### Responses
**200** 

Body (_Get Specific Master Template response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here is your email template",
  "data": {
    "template_id_master": 57,
    "template_name": "Basic 2",
    "date_added": "1458182912",
    "thumbnail": {
      "small": "https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_email-marketing/_templates-master/basic2/thumb-small.jpg",
      "large": "https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_email-marketing/_templates-master/basic2/thumb-large.jpg"
    }
  }
}
```


### <a name="get_all_master_template_categories"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get All Master Template Categories") `GET` /email/master-templates-categories

> TODO: Add a method description



#### Responses
**200** 

Body (_Get All Master Template Categories response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "List of Email Categories",
  "data": [
    {
      "category_id": 2,
      "name": "Alerts/Notificartions"
    },
    {
      "category_id": 3,
      "name": "Art"
    },
    {
      "category_id": 4,
      "name": "Birthday"
    },
    {
      "category_id": 23,
      "name": "Blank Template"
    },
    {
      "category_id": 5,
      "name": "Coupons"
    },
    {
      "category_id": 6,
      "name": "eCommerce"
    },
    {
      "category_id": 7,
      "name": "Education"
    },
    {
      "category_id": 8,
      "name": "Events/Reminders"
    },
    {
      "category_id": 1,
      "name": "Featured"
    },
    {
      "category_id": 9,
      "name": "Fitness"
    },
    {
      "category_id": 11,
      "name": "Holiday/Travel"
    },
    {
      "category_id": 12,
      "name": "Inspirational"
    },
    {
      "category_id": 13,
      "name": "Kids"
    },
    {
      "category_id": 14,
      "name": "Music"
    },
    {
      "category_id": 15,
      "name": "Newsletters"
    },
    {
      "category_id": 16,
      "name": "Non-profit"
    },
    {
      "category_id": 17,
      "name": "Photography"
    },
    {
      "category_id": 18,
      "name": "Real Estate"
    },
    {
      "category_id": 10,
      "name": "Restaurant/Food"
    },
    {
      "category_id": 21,
      "name": "Sports"
    },
    {
      "category_id": 22,
      "name": "Stationery"
    }
  ]
}
```


### <a name="get_specific_email_template_category"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Specific Email Template Category") `GET` /email/master-templates-categories/{category_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| category_id | `string` |  ``` Required ```  | Your category id. | `25` | 

#### Responses
**200** 

Body (_Get Specific Email Template Category response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "List of Email Categories",
  "data": {
    "category_id": 4,
    "name": "Birthday"
  }
}
```


### <a name="get_all_templates_for_category"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get All Templates For Category") `GET` /email/master-templates-categories/{category_id}/master-templates

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| category_id | `string` |  ``` Required ```  | Your category id. | `1` | 

#### Responses
**200** 

Body (_Get All Templates For Category response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "List of Email Templates By Category",
  "data": [
    {
      "template_id_master": 1,
      "category_id": 1,
      "template_name": "Minty",
      "body": "<!DOCTYPE html PUBLIC \"-//W3C//DTD XHTML 1.0 Transitional//EN\" ...\n                     </tr>\n                  </tbody>\n               </table>\n            </td>\n         </tr>\n      </tbody>\n   </table>\n</body>\n</html>",
      "date_added": "1445848821",
      "thumbnail": {
        "small": "https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_email-marketing/_templates-master/minty/thumb-small.jpg",
        "large": "https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_email-marketing/_templates-master/minty/thumb-large.jpg"
      }
    }
  ]
}
```


### <a name="upload_image_to_specific_template"></a>![Endpoint: ](https://apidocs.io/img/method.png "Upload Image to Specific Template") `POST` /email/templates-images/{template_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| template_id | `string` |  ``` Required ```  | Your template id. | `1` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `upload image to specific template request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "image": "image.png",
  "url": "http://www.downloadimg.from/here.png"
}
``` 

#### Responses
**200** 

Body (_Upload Image to Specific Template response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here is your uploaded image.",
  "data": "https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_email-marketing/_templates-user/BEC51696-E923-4998-9249-C9B49DB7571A/2056F933-9C64-4E57-AB19-01F65EBB7C0A.png"
}
```


[Back to API Reference](#api_reference)

## <a name="email_to_sms_allowed_address"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Email-to-SMS Allowed Address") Email-to-SMS Allowed Address


### <a name="list_of_email_to_sms_allowed_address"></a>![Endpoint: ](https://apidocs.io/img/method.png "List of Email-to-SMS Allowed Address") `GET` /sms/email-sms

> Get list of allowed email addresses.



#### Responses
**200** 

Body (_List of Email-to-SMS Allowed Address response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are some data.",
  "data": {
    "total": 25,
    "per_page": 15,
    "current_page": 1,
    "last_page": 2,
    "next_page_url": "https://rest.clicksend.com/v3/sms/email-sms/?page=2",
    "prev_page_url": null,
    "from": 1,
    "to": 15,
    "data": [
      {
        "email_address_id": 84,
        "email_address": "my@email.com",
        "from": "+13523944199"
      },
      {
        "email_address_id": 85,
        "email_address": "my@email.com",
        "from": "+13523944199"
      },
      {
        "email_address_id": 86,
        "email_address": "my@email.com",
        "from": "+13523944199"
      },
      {
        "email_address_id": 87,
        "email_address": "my@email.com",
        "from": "+13523944199"
      },
      {
        "email_address_id": 88,
        "email_address": "my@email.com",
        "from": "+13523944199"
      },
      {
        "email_address_id": 89,
        "email_address": "my@email.com",
        "from": "+13523944199"
      },
      {
        "email_address_id": 90,
        "email_address": "my@email.com",
        "from": "+13523944199"
      },
      {
        "email_address_id": 91,
        "email_address": "my@email.com",
        "from": "+13523944199"
      },
      {
        "email_address_id": 92,
        "email_address": "my@email.com",
        "from": "+13523944199"
      },
      {
        "email_address_id": 93,
        "email_address": "*@clickssend.com",
        "from": "+13523944199"
      },
      {
        "email_address_id": 94,
        "email_address": "my@email.com.com",
        "from": "+13523944199"
      },
      {
        "email_address_id": 95,
        "email_address": "my@email.com",
        "from": "+17128848693"
      },
      {
        "email_address_id": 96,
        "email_address": "lOWAW@gmail.com",
        "from": "+17128848252"
      },
      {
        "email_address_id": 97,
        "email_address": "munPM@gmail.com",
        "from": "+17128848867"
      },
      {
        "email_address_id": 98,
        "email_address": "XZKK9@gmail.com",
        "from": "+17128847113"
      }
    ]
  }
}
```


### <a name="create_email_to_sms_allowed_address"></a>![Endpoint: ](https://apidocs.io/img/method.png "Create Email to SMS Allowed Address") `POST` /sms/email-sms

> Create an allowed email address.



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `create email to sms allowed address request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "email_address": "Cv3p0@gmail.com",
  "from": "+17128845887"
}
``` 

#### Responses
**200** 

Body (_Create Email to SMS Allowed Address response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "New data has been saved.",
  "data": {
    "email_address_id": 107,
    "email_address": "Cv3p0@gmail.com",
    "from": "+17128845887"
  }
}
```


### <a name="get_specific_email_to_sms_allowed_address"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get specific Email-to-SMS Allowed Address") `GET` /sms/email-sms/{email_address_id}

> Get a specific allowed email address.



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| email_address_id | `precision` |  ``` Required ```  | Your email address id. | `113` | 

#### Responses
**200** 

Body (_Get specific Email-to-SMS Allowed Address response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are some data.",
  "data": {
    "email_address_id": 113,
    "email_address": "RXcMn@gmail.com",
    "from": "+17128843729"
  }
}
```


### <a name="update_email_to_sms_allowed_address"></a>![Endpoint: ](https://apidocs.io/img/method.png "Update Email-to-SMS Allowed Address") `PUT` /sms/email-sms/{email_address_id}

> Update a specific allowed email address.



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| email_address_id | `precision` |  ``` Required ```  | Your email address id. | `107` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `update email-to-sms allowed address request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "email_address": "pfvRZ@gmail.com",
  "from": "+17128842283"
}
``` 

#### Responses
**200** 

Body (_Update Email-to-SMS Allowed Address response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your data has been updated.",
  "data": {
    "email_address_id": 107,
    "email_address": "pfvRZ@gmail.com",
    "from": "+17128842283"
  }
}
```


### <a name="delete_email_to_sms_allowed_address"></a>![Endpoint: ](https://apidocs.io/img/method.png "Delete Email-to-SMS Allowed Address") `DELETE` /sms/email-sms/{email_address_id}

> Delete a specific allowed email address.



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| email_address_id | `precision` |  ``` Required ```  | Your email address id. | `107` | 

#### Responses
**200** 

Body (_Delete Email-to-SMS Allowed Address response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Allowed email address was deleted.",
  "data": []
}
```


[Back to API Reference](#api_reference)

## <a name="email_to_sms_stripped_strings"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Email-to-SMS Stripped Strings") Email-to-SMS Stripped Strings


### <a name="list_stripped_strings"></a>![Endpoint: ](https://apidocs.io/img/method.png "List Stripped Strings") `GET` /sms/email-sms-stripped-strings

> TODO: Add a method description



#### Responses
**200** 

Body (_List Stripped Strings response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here is your result.",
  "data": {
    "total": 2,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 2,
    "data": [
      {
        "rule_id": 18,
        "strip_string": "This is a test1."
      },
      {
        "rule_id": 19,
        "strip_string": "This is a test2."
      }
    ]
  }
}
```


### <a name="find_specific_stripped_string"></a>![Endpoint: ](https://apidocs.io/img/method.png "Find Specific Stripped String") `GET` /sms/email-sms-stripped-strings/{rule_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| rule_id | `precision` |  ``` Required ```  | The rule id you want to access. | `18` | 

#### Responses
**200** 

Body (_Find Specific Stripped String response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here is your result.",
  "data": {
    "rule_id": 18,
    "strip_string": "You've received a reply from."
  }
}
```


### <a name="create_stripped_string"></a>![Endpoint: ](https://apidocs.io/img/method.png "Create Stripped String") `POST` /sms/email-sms-stripped-strings

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `create stripped string request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "strip_string": "~~~test~~~"
}
``` 

#### Responses
**200** 

Body (_Create Stripped String response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Strip string has been created.",
  "data": {
    "rule_id": 20,
    "strip_string": "~~~~test~~~~"
  }
}
```


### <a name="update_stripped_string"></a>![Endpoint: ](https://apidocs.io/img/method.png "Update Stripped String") `PUT` /sms/email-sms-stripped-strings/{rule_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| rule_id | `precision` |  ``` Required ```  | The rule id you want to access. | `20` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `update stripped string request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "strip_string": "~~~test1~~~"
}
``` 

#### Responses
**200** 

Body (_Update Stripped String response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Strip string has been updated.",
  "data": {
    "rule_id": 20,
    "strip_string": "~~~~test1~~~~"
  }
}
```


### <a name="delete_stripped_string"></a>![Endpoint: ](https://apidocs.io/img/method.png "Delete Stripped String") `DELETE` /sms/email-sms-stripped-strings/{rule_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| rule_id | `precision` |  ``` Required ```  | The rule id you want to access. | `20` | 

#### Responses
**200** 

Body (_Delete Stripped String response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Strip string has been deleted.",
  "data": true
}
```


[Back to API Reference](#api_reference)

## <a name="fax"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Fax") Fax


### <a name="send_fax"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send Fax") `POST` /fax/send

> **Letter File Options**
> **Use existing URL**
> With this option, you can use an existing URL to a PDF document. For example, you might generate the pdf on your server.
> **Upload File to Our Server**
> With this option, you can use the `/uploads` endpoint to upload the document. The `/uploads` endpoint returns a URL that can be used in the `/fax/send` endpoint.



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `send fax request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "file_url": "file_url",
  "messages": [
    "messages"
  ],
  "to": "to",
  "source": "source",
  "list_id": 195.190037407535,
  "from": "from",
  "schedule": 195.190037407535,
  "custom_string": "custom_string",
  "country": "country",
  "from_email": "from_email"
}
``` 

#### Responses
**200** 

Body (_Send Fax response_) 
```
{
  "http_code": 195,
  "response_code": "response_code",
  "response_msg": "response_msg",
  "data": {}
}
```


### <a name="calculate_price"></a>![Endpoint: ](https://apidocs.io/img/method.png "Calculate Price") `POST` /fax/price

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `calculate price request132` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "file_url": "file_url",
  "messages": [
    "messages"
  ],
  "to": "to",
  "source": "source",
  "list_id": 195.190037407535,
  "from": "from",
  "schedule": 195.190037407535,
  "custom_string": "custom_string",
  "country": "country",
  "from_email": "from_email"
}
``` 

#### Responses
**200** 

Body (_Calculate Price response_) 
```
{
  "http_code": 195,
  "response_code": "response_code",
  "response_msg": "response_msg",
  "data": {}
}
```


### <a name="get_fax_history"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Fax History") `GET` /fax/history?date_from={date_from}&date_to={date_to}&q={q}&order_by={order_by}

> Get a list of Fax History.



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| date_from | `precision` |  ``` Optional ```  | Customize result by setting from date (timestsamp) | `1457572619` | 
| date_to | `precision` |  ``` Optional ```  | Customize result by setting to date (timestamp) | `1457573000` | 
| q | `string` |  ``` Optional ```  | Custom query | `status:Sent,status_code:201` | 
| order_by | `string` |  ``` Optional ```  | Order result by | `subject:desc` | 

#### Responses
**200** 

Body (_Get Fax History response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here is your history.",
  "data": {
    "total": 2,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 2,
    "data": [
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": null,
        "message_id": "2FDA7622-FC6E-4D21-B335-32FF860D7E19",
        "to": "+61261111115",
        "from": "+61267132168",
        "carrier": "",
        "country": "AU",
        "custom_string": "custom_string",
        "schedule": "1436874701",
        "message_pages": "6.00",
        "message_price": "13.2000",
        "status": "Sent",
        "status_code": "201",
        "status_text": "Sent",
        "date_added": 1457572619,
        "from_email": null,
        "_file_url": "https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/document.pdf",
        "date": null,
        "_api_username": "username"
      },
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": null,
        "message_id": "A6A20382-8211-46B9-8F09-E7337AE6626D",
        "to": "+61261111115",
        "from": "+61267132168",
        "carrier": "",
        "country": "AU",
        "custom_string": "custom_string",
        "schedule": "1436874701",
        "message_pages": "6.00",
        "message_price": "13.2000",
        "status": "Queued",
        "status_code": null,
        "status_text": null,
        "date_added": 1457586514,
        "from_email": null,
        "_file_url": "https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/document.pdf",
        "date": null,
        "_api_username": "username"
      }
    ]
  }
}
```


### <a name="list_of_fax_delivery_receipts"></a>![Endpoint: ](https://apidocs.io/img/method.png "List of Fax Delivery Receipts") `GET` /fax/receipts

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



#### Responses
**200** 

Body (_List of Fax Delivery Receipts response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are your delivery receipts.",
  "data": {
    "total": 1,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 1,
    "data": [
      {
        "timestamp_send": "1450854013",
        "timestamp": "1451200622",
        "message_id": "88AB118E-EB1B-478C-98CE-6C73ABA23F67",
        "status_code": "Completed",
        "status_text": "",
        "error_code": "",
        "error_text": "",
        "custom_string": "",
        "subaccount_id": 1,
        "message_type": "fax"
      }
    ]
  }
}
```


### <a name="get_a_specific_fax_delivery_receipt"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get a Specific Fax Delivery Receipt") `GET` /fax/receipts/{message_id}

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



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| message_id | `string` |  ``` Required ```  | D2AF-479B-8955-6395D561DEF4" (required, number) - Message ID. | `"3FAC74F1` | 

#### Responses
**200** 

Body (_Get a Specific Fax Delivery Receipt response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here is your fax receipt.",
  "data": {
    "user_id": 1,
    "subaccount_id": 1,
    "list_id": null,
    "message_id": "3FAC74F1-D2AF-479B-8955-6395D561DEF4",
    "to": "+61267132168",
    "from": "+61267132168",
    "carrier": "",
    "country": "AU",
    "custom_string": "custom_string",
    "schedule": "1436874701",
    "message_pages": "1.00",
    "message_price": "1.000000",
    "status": "WaitApproval",
    "status_code": null,
    "status_text": null,
    "date_added": 1454394659
  }
}
```


### <a name="mark_fax_delivery_receipts_as_read"></a>![Endpoint: ](https://apidocs.io/img/method.png "Mark Fax Delivery Receipts as read") `PUT` /fax/receipts-read

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



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `mark fax delivery receipts as read request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "date_before": 1441958441
}
``` 

#### Responses
**200** 

Body (_Mark Fax Delivery Receipts as read response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Receipts has been marked as read.",
  "data": []
}
```


### <a name="add_a_test_delivery_receipt"></a>![Endpoint: ](https://apidocs.io/img/method.png "Add a Test Delivery Receipt") `POST` /fax/receipts

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



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `add a test delivery receipt request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "url": "http://yourUrl.com"
}
``` 

#### Responses
**200** 

Body (_Add a Test Delivery Receipt response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Receipt has been added",
  "data": {
    "timestamp": "1441958441",
    "message_id": "493FFB41-9733-4641-985F-BD79A067B58F",
    "status_code": "201",
    "status_text": "Success: Message received on handset.",
    "error_code": null,
    "error_text": null,
    "custom_string": null
  }
}
```


[Back to API Reference](#api_reference)

## <a name="forgot_account"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Forgot Account") Forgot Account


### <a name="forgot_username"></a>![Endpoint: ](https://apidocs.io/img/method.png "Forgot Username") `PUT` /forgot-username

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `forgot username request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "email": "email",
  "phone_number": 31.6853192991974,
  "country": "country"
}
``` 

#### Responses
**200** 

Body (_Forgot Username response_) 
```
{
  "http_code": 31,
  "response_code": "response_code",
  "response_msg": "response_msg",
  "data": [
    "data"
  ]
}
```


### <a name="forgot_password"></a>![Endpoint: ](https://apidocs.io/img/method.png "Forgot Password") `PUT` /forgot-password

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `forgot password request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "username": "0F6pKiiuca"
}
``` 

#### Responses
**200** 

Body (_Forgot Password response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "An email notification has been sent.",
  "data": []
}
```


### <a name="verify_forgot_password"></a>![Endpoint: ](https://apidocs.io/img/method.png "Verify Forgot Password") `PUT` /forgot-password/verify

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `verify forgot password request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "subaccount_id": 54,
  "activation_token": "9C648BAD-EB7F-4E7E-96BC-B433140C4F1F",
  "password": "0F6pKiiuca"
}
``` 

#### Responses
**200** 

Body (_Verify Forgot Password response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your password has been updated.",
  "data": []
}
```


[Back to API Reference](#api_reference)

## <a name="mms"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "MMS") MMS


### <a name="send_mms"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send MMS") `POST` /mms/send

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `send mms request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "media_file": "media_file",
  "to": "to",
  "subject": "subject",
  "body": "body",
  "source": "source",
  "list_id": 31.6853192991974,
  "from": "from",
  "schedule": 31.6853192991974,
  "custom_string": "custom_string",
  "country": "country",
  "from_email": "from_email"
}
``` 

#### Responses
**200** 

Body (_Send MMS response_) 
```
{
  "http_code": 31,
  "response_code": "response_code",
  "response_msg": "response_msg",
  "data": {}
}
```


### <a name="get_price"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Price") `POST` /mms/price

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `get price request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "media_file": "media_file",
  "to": "to",
  "subject": "subject",
  "body": "body",
  "source": "source",
  "list_id": 31.6853192991974,
  "from": "from",
  "schedule": 31.6853192991974,
  "custom_string": "custom_string",
  "country": "country",
  "from_email": "from_email"
}
``` 

#### Responses
**200** 

Body (_Get Price response_) 
```
{
  "http_code": 31,
  "response_code": "response_code",
  "response_msg": "response_msg",
  "data": {}
}
```


### <a name="get_mms_history"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get MMS History") `GET` /mms/history?q={q}&order_by={order_by}&date_from={date_from}&date_to={date_to}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| q | `string` |  ``` Optional ```  | A custom query. | `list_id:429,direction:out` | 
| order_by | `string` |  ``` Optional ```  | Sort records by. | `subject:desc` | 
| date_from | `number` |  ``` Optional ```  | Timestamp (from) used to show records by date. | `1443501617` | 
| date_to | `number` |  ``` Optional ```  | Timestamp (to) used to show records by date. | `1443501727` | 

#### Responses
**200** 

Body (_Get MMS History response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here is your history.",
  "data": {
    "total": 31,
    "per_page": 15,
    "current_page": 1,
    "last_page": 3,
    "next_page_url": "/?page=2",
    "prev_page_url": null,
    "from": 1,
    "to": 15,
    "data": [
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": 429,
        "contact_id": 7,
        "message_id": "2453E085-C1F8-47EC-AD35-B793960B1313",
        "direction": "out",
        "to": "+61298444214",
        "subject": "This is a subject",
        "from": "+61298444213",
        "body": "John This is a test message.",
        "carrier": "",
        "country": "AU",
        "custom_string": "",
        "schedule": "1467356623",
        "from_email": null,
        "message_parts": "1.00",
        "message_price": "2.4200",
        "priority": 10,
        "status": "Failed",
        "status_code": "301",
        "status_text": "Unable to process your MMS for sending.",
        "date_added": 1467356623,
        "_media_file_url": "https://disk.domain.com/_mms/2D789145-3E66-4038-9BA5-EF3DEEE82386.gif",
        "_api_username": "my_api_username"
      },
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": 429,
        "contact_id": 8,
        "message_id": "54889DC7-A840-4A21-A977-EBE8C51FC2F8",
        "direction": "out",
        "to": "+61298444214",
        "subject": "This is a subject",
        "from": "+61298444213",
        "body": "John This is a test message.",
        "carrier": "",
        "country": "AU",
        "custom_string": "",
        "schedule": "1467356623",
        "from_email": null,
        "message_parts": "1.00",
        "message_price": "2.4200",
        "priority": 10,
        "status": "Queued:WaitSend",
        "status_code": null,
        "status_text": null,
        "date_added": 1467356623,
        "_media_file_url": "https://disk.domain.com/_mms/2D789145-3E66-4038-9BA5-EF3DEEE82386.gif",
        "_api_username": "my_api_username"
      },
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": 429,
        "contact_id": 9,
        "message_id": "F2E75443-35A4-4300-9D12-E67682E762DB",
        "direction": "out",
        "to": "+61298444214",
        "subject": "This is a subject",
        "from": "+61298444213",
        "body": "John This is a test message.",
        "carrier": "",
        "country": "AU",
        "custom_string": "",
        "schedule": "1467356623",
        "from_email": null,
        "message_parts": "1.00",
        "message_price": "2.4200",
        "priority": 10,
        "status": "Queued:WaitSend",
        "status_code": null,
        "status_text": null,
        "date_added": 1467356623,
        "_media_file_url": "https://disk.domain.com/_mms/2D789145-3E66-4038-9BA5-EF3DEEE82386.gif",
        "_api_username": "my_api_username"
      },
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": 429,
        "contact_id": 10,
        "message_id": "26B77CD6-5C98-46C7-A6DF-F76F29B7E09F",
        "direction": "out",
        "to": "+61298444214",
        "subject": "This is a subject",
        "from": "+61298444213",
        "body": "John This is a test message.",
        "carrier": "",
        "country": "AU",
        "custom_string": "",
        "schedule": "1467356623",
        "from_email": null,
        "message_parts": "1.00",
        "message_price": "2.4200",
        "priority": 10,
        "status": "Queued:WaitSend",
        "status_code": null,
        "status_text": null,
        "date_added": 1467356623,
        "_media_file_url": "https://disk.domain.com/_mms/2D789145-3E66-4038-9BA5-EF3DEEE82386.gif",
        "_api_username": "my_api_username"
      },
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": 429,
        "contact_id": 11,
        "message_id": "70BAB69D-8EA5-417C-A8EA-7F0D843E30F3",
        "direction": "out",
        "to": "+61298444214",
        "subject": "This is a subject",
        "from": "+61298444213",
        "body": "John This is a test message.",
        "carrier": "",
        "country": "AU",
        "custom_string": "",
        "schedule": "1467356623",
        "from_email": null,
        "message_parts": "1.00",
        "message_price": "2.4200",
        "priority": 10,
        "status": "Sent",
        "status_code": "200",
        "status_text": "Sent",
        "date_added": 1467356623,
        "_media_file_url": "https://disk.domain.com/_mms/2D789145-3E66-4038-9BA5-EF3DEEE82386.gif",
        "_api_username": "my_api_username"
      },
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": 429,
        "contact_id": 4,
        "message_id": "42E3C025-FD9D-4C9F-B374-C7DF5337F6AF",
        "direction": "out",
        "to": "+61298444214",
        "subject": "This is a subject",
        "from": "+61298444213",
        "body": "John This is a test message.",
        "carrier": "",
        "country": "AU",
        "custom_string": "",
        "schedule": "1467358732",
        "from_email": null,
        "message_parts": "1.00",
        "message_price": "2.4200",
        "priority": 10,
        "status": "Queued",
        "status_code": null,
        "status_text": null,
        "date_added": 1467358732,
        "_media_file_url": "https://disk.domain.com/_mms/601D3E45-49FD-4653-B8F7-ED70B5CB9A43.gif",
        "_api_username": "my_api_username"
      },
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": 429,
        "contact_id": 5,
        "message_id": "218D5034-89A0-4C6C-B8F9-006BEF50B92B",
        "direction": "out",
        "to": "+61298444214",
        "subject": "This is a subject",
        "from": "+61298444213",
        "body": "John This is a test message.",
        "carrier": "",
        "country": "AU",
        "custom_string": "",
        "schedule": "1467358732",
        "from_email": null,
        "message_parts": "1.00",
        "message_price": "2.4200",
        "priority": 10,
        "status": "Queued",
        "status_code": null,
        "status_text": null,
        "date_added": 1467358732,
        "_media_file_url": "https://disk.domain.com/_mms/601D3E45-49FD-4653-B8F7-ED70B5CB9A43.gif",
        "_api_username": "my_api_username"
      },
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": 429,
        "contact_id": 6,
        "message_id": "EFCF9FAA-1BCA-4C58-884A-257C0D87124E",
        "direction": "out",
        "to": "+61298444214",
        "subject": "This is a subject",
        "from": "+61298444213",
        "body": "John This is a test message.",
        "carrier": "",
        "country": "AU",
        "custom_string": "",
        "schedule": "1467358732",
        "from_email": null,
        "message_parts": "1.00",
        "message_price": "2.4200",
        "priority": 10,
        "status": "Queued",
        "status_code": null,
        "status_text": null,
        "date_added": 1467358732,
        "_media_file_url": "https://disk.domain.com/_mms/601D3E45-49FD-4653-B8F7-ED70B5CB9A43.gif",
        "_api_username": "my_api_username"
      },
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": 429,
        "contact_id": 7,
        "message_id": "3E0DC217-7D0F-4C20-A3F2-E3362B938CAF",
        "direction": "out",
        "to": "+61298444214",
        "subject": "This is a subject",
        "from": "+61298444213",
        "body": "John This is a test message.",
        "carrier": "",
        "country": "AU",
        "custom_string": "",
        "schedule": "1467358732",
        "from_email": null,
        "message_parts": "1.00",
        "message_price": "2.4200",
        "priority": 10,
        "status": "Queued",
        "status_code": null,
        "status_text": null,
        "date_added": 1467358732,
        "_media_file_url": "https://disk.domain.com/_mms/601D3E45-49FD-4653-B8F7-ED70B5CB9A43.gif",
        "_api_username": "my_api_username"
      },
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": 429,
        "contact_id": 8,
        "message_id": "7827223E-0D73-49A1-95D0-8B85C3F5CC71",
        "direction": "out",
        "to": "+61298444214",
        "subject": "This is a subject",
        "from": "+61298444213",
        "body": "John This is a test message.",
        "carrier": "",
        "country": "AU",
        "custom_string": "",
        "schedule": "1467358732",
        "from_email": null,
        "message_parts": "1.00",
        "message_price": "2.4200",
        "priority": 10,
        "status": "Queued",
        "status_code": null,
        "status_text": null,
        "date_added": 1467358732,
        "_media_file_url": "https://disk.domain.com/_mms/601D3E45-49FD-4653-B8F7-ED70B5CB9A43.gif",
        "_api_username": "my_api_username"
      },
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": 429,
        "contact_id": 9,
        "message_id": "0D902342-3873-4EE9-A86A-CA1B0B755BBA",
        "direction": "out",
        "to": "+61298444214",
        "subject": "This is a subject",
        "from": "+61298444213",
        "body": "John This is a test message.",
        "carrier": "",
        "country": "AU",
        "custom_string": "",
        "schedule": "1467358732",
        "from_email": null,
        "message_parts": "1.00",
        "message_price": "2.4200",
        "priority": 10,
        "status": "Queued",
        "status_code": null,
        "status_text": null,
        "date_added": 1467358732,
        "_media_file_url": "https://disk.domain.com/_mms/601D3E45-49FD-4653-B8F7-ED70B5CB9A43.gif",
        "_api_username": "my_api_username"
      },
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": 429,
        "contact_id": 10,
        "message_id": "0549ADFD-9D70-4B1A-B62F-875A05B481D9",
        "direction": "out",
        "to": "+61298444214",
        "subject": "This is a subject",
        "from": "+61298444213",
        "body": "John This is a test message.",
        "carrier": "",
        "country": "AU",
        "custom_string": "",
        "schedule": "1467358732",
        "from_email": null,
        "message_parts": "1.00",
        "message_price": "2.4200",
        "priority": 10,
        "status": "Queued",
        "status_code": null,
        "status_text": null,
        "date_added": 1467358732,
        "_media_file_url": "https://disk.domain.com/_mms/601D3E45-49FD-4653-B8F7-ED70B5CB9A43.gif",
        "_api_username": "my_api_username"
      },
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": 429,
        "contact_id": 11,
        "message_id": "1327677D-D2EF-4442-A0F3-B480C7E94359",
        "direction": "out",
        "to": "+61298444214",
        "subject": "This is a subject",
        "from": "+61298444213",
        "body": "John This is a test message.",
        "carrier": "",
        "country": "AU",
        "custom_string": "",
        "schedule": "1467358732",
        "from_email": null,
        "message_parts": "1.00",
        "message_price": "2.4200",
        "priority": 10,
        "status": "Queued",
        "status_code": null,
        "status_text": null,
        "date_added": 1467358732,
        "_media_file_url": "https://disk.domain.com/_mms/601D3E45-49FD-4653-B8F7-ED70B5CB9A43.gif",
        "_api_username": "my_api_username"
      },
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": null,
        "contact_id": null,
        "message_id": "42ABDB50-3DAE-41B5-8F48-6F227F38DB2E",
        "direction": "out",
        "to": "+61437887633",
        "subject": "This is a subject",
        "from": "",
        "body": "This is a test message.",
        "carrier": "Telstra",
        "country": "AU",
        "custom_string": "",
        "schedule": "1467363093",
        "from_email": null,
        "message_parts": "1.00",
        "message_price": "2.4200",
        "priority": 10,
        "status": "Queued",
        "status_code": null,
        "status_text": null,
        "date_added": 1467363093,
        "_media_file_url": "https://disk.domain.com/_mms/C755FD73-AD7A-4EB8-A521-FC10BB37F3B7.gif",
        "_api_username": "my_api_username"
      },
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": null,
        "contact_id": null,
        "message_id": "53271F40-EEB2-4DE9-A525-F0620211A4C9",
        "direction": "out",
        "to": "+61437887633",
        "subject": "This is a subject",
        "from": "",
        "body": "This is a test message.",
        "carrier": "Telstra",
        "country": "AU",
        "custom_string": "",
        "schedule": "1467363210",
        "from_email": null,
        "message_parts": "1.00",
        "message_price": "2.4200",
        "priority": 10,
        "status": "Queued",
        "status_code": null,
        "status_text": null,
        "date_added": 1467363210,
        "_media_file_url": "https://disk.domain.com/_mms/2289C892-7518-4FBB-9A1C-7C34A93F6328.gif",
        "_api_username": "my_api_username"
      }
    ]
  }
}
```


### <a name="export_mms_history"></a>![Endpoint: ](https://apidocs.io/img/method.png "Export MMS History") `GET` /mms/history/export?filename={filename}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| filename | `string` |  ``` Required ```  | Your export filename. | `export.csv` | 

#### Responses
**200** 

Body (_Export MMS History response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Download your file here.",
  "data": {
    "url": "http://disk.domain.com/files/22D55AF9-6CF0-476D-A8B3-82A998FD2738?filename=export.csv"
  }
}
```


### <a name="cancel_mms"></a>![Endpoint: ](https://apidocs.io/img/method.png "Cancel MMS") `PUT` /mms/{message_id}/cancel

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| message_id | `string` |  ``` Required ```  | Message ID. | `52E3C025-FD9D-4C9F-B374-C7DF5337F6AF` | 

#### Responses
**200** 

Body (_Cancel MMS response_) 
```
{
  "http_code": 31,
  "response_code": "response_code",
  "response_msg": "response_msg",
  "data": "data"
}
```


### <a name="cancel_all_mms"></a>![Endpoint: ](https://apidocs.io/img/method.png "Cancel All MMS") `PUT` /mms/cancel-all

> TODO: Add a method description



#### Responses
**200** 

Body (_Cancel All MMS response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "2 MMS have been cancelled.",
  "data": {
    "count": 2
  }
}
```


### <a name="get_all_delivery_receipts"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get all Delivery Receipts") `GET` /mms/receipts

> TODO: Add a method description



#### Responses
**200** 

Body (_Get all Delivery Receipts response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are your delivery receipts.",
  "data": {
    "total": 3,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 3,
    "data": [
      {
        "timestamp_send": "1450854013",
        "timestamp": "1451200622",
        "message_id": "88AB118E-EB1B-478C-98CE-6C73ABA23F67",
        "status_code": "Completed",
        "status_text": "",
        "error_code": "",
        "error_text": "",
        "custom_string": "",
        "subaccount_id": 1,
        "message_type": "mms"
      },
      {
        "timestamp_send": "1450854013",
        "timestamp": "1451200622",
        "message_id": "88AB118E-EB1B-478C-98CE-6C73ABA23F67",
        "status_code": "Completed",
        "status_text": "",
        "error_code": "",
        "error_text": "",
        "custom_string": "",
        "subaccount_id": 1,
        "message_type": "mms"
      },
      {
        "timestamp_send": "1450854013",
        "timestamp": "1451200622",
        "message_id": "88AB118E-EB1B-478C-98CE-6C73ABA23F67",
        "status_code": "Completed",
        "status_text": "",
        "error_code": "",
        "error_text": "",
        "custom_string": "",
        "subaccount_id": 1,
        "message_type": "mms"
      }
    ]
  }
}
```


### <a name="get_delivery_receipt"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Delivery Receipt") `GET` /mms/receipts/{message_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| message_id | `string` |  ``` Required ```  | Message ID. | `3E0DC217-7D0F-4C20-A3F2-E3362B938CAF` | 

#### Responses
**200** 

Body (_Get Delivery Receipt response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here is your MMS receipt.",
  "data": {
    "user_id": 1,
    "subaccount_id": 1,
    "list_id": 429,
    "contact_id": 7,
    "message_id": "3E0DC217-7D0F-4C20-A3F2-E3362B938CAF",
    "direction": "out",
    "to": "+61298444214",
    "subject": "This is a subject",
    "from": "+61298444213",
    "body": "John This is a test message.",
    "carrier": "",
    "country": "AU",
    "custom_string": "",
    "schedule": "1467358732",
    "from_email": null,
    "message_parts": "1.00",
    "message_price": "2.420000",
    "priority": 10,
    "status": "Queued",
    "status_code": null,
    "status_text": null,
    "date_added": 1467358732,
    "_media_file_url": "https://disk.domain.com/_mms/601D3E45-49FD-4653-B8F7-ED70B5CB9A43.gif"
  }
}
```


### <a name="mark_receipts_as_read"></a>![Endpoint: ](https://apidocs.io/img/method.png "Mark Receipts As Read") `PUT` /mms/receipts-read

> TODO: Add a method description



#### Responses
**200** 

Body (_Mark Receipts As Read response_) 
```
{
  "http_code": 31,
  "response_code": "response_code",
  "response_msg": "response_msg",
  "data": "data"
}
```


### <a name="get_all_inbound_sms___pull"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get all Inbound SMS - Pull") `GET` /sms/inbound

> Inbound MMS shares the same rules/settings/endpoints as SMS. Any attachments will be converted to a URL.
> **Push Inbound SMS**
> If you prefer, we can push message replies to your server as they arrive with us.
> Refer to SMS->Inbound SMS in the docs.
> **Pull Inbound SMS**
> Receive SMS by polling your Inbox.
> Refer to SMS->Inbound SMS in the docs.



#### Responses
**200** 

Body 
```
{}
```


[Back to API Reference](#api_reference)

## <a name="numbers"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Numbers") Numbers


### <a name="get_all_dedicated_numbers"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get all Dedicated Numbers") `GET` /numbers

> TODO: Add a method description



#### Responses
**200** 

Body (_Get all Dedicated Numbers response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are you dedicated numbers.",
  "data": {
    "total": 22,
    "per_page": 15,
    "current_page": 1,
    "last_page": 2,
    "next_page_url": "https://rest.clicksend.com/v3/numbers/?page=2",
    "prev_page_url": null,
    "from": 1,
    "to": 15,
    "data": [
      {
        "dedicated_number": "+61481070206",
        "country": "AU",
        "price": "18.59",
        "_country_name": "Australia"
      },
      {
        "dedicated_number": "+61437887639",
        "country": "AU",
        "price": "18.59",
        "_country_name": "Australia"
      },
      {
        "dedicated_number": "+61481070206",
        "country": "AU",
        "price": "18.59",
        "_country_name": "Australia"
      },
      {
        "dedicated_number": "+61287265298",
        "country": "AU",
        "price": "18.59",
        "_country_name": "Australia"
      },
      {
        "dedicated_number": "+19403944918",
        "country": "US",
        "price": "26.94",
        "_country_name": "United States of America"
      },
      {
        "dedicated_number": "+61287265842",
        "country": "AU",
        "price": "26.94",
        "_country_name": "Australia"
      },
      {
        "dedicated_number": "+61287265371",
        "country": "AU",
        "price": "26.94",
        "_country_name": "Australia"
      },
      {
        "dedicated_number": "+61287265372",
        "country": "AU",
        "price": "26.94",
        "_country_name": "Australia"
      },
      {
        "dedicated_number": "+16062191029",
        "country": "US",
        "price": "26.94",
        "_country_name": "United States of America"
      },
      {
        "dedicated_number": "+12282060588",
        "country": "US",
        "price": "26.94",
        "_country_name": "United States of America"
      },
      {
        "dedicated_number": "+12282060587",
        "country": "US",
        "price": "26.94",
        "_country_name": "United States of America"
      },
      {
        "dedicated_number": "+12282060586",
        "country": "US",
        "price": "26.94",
        "_country_name": "United States of America"
      },
      {
        "dedicated_number": "+12282060585",
        "country": "US",
        "price": "26.94",
        "_country_name": "United States of America"
      },
      {
        "dedicated_number": "+12282060584",
        "country": "US",
        "price": "26.94",
        "_country_name": "United States of America"
      },
      {
        "dedicated_number": "+12282060583",
        "country": "US",
        "price": "26.94",
        "_country_name": "United States of America"
      }
    ],
    "_currency": {
      "currency_name_short": "USD",
      "currency_prefix_d": "$",
      "currency_prefix_c": "¢",
      "currency_name_long": "US Dollars"
    }
  }
}
```


### <a name="buy_dedicated_number"></a>![Endpoint: ](https://apidocs.io/img/method.png "Buy dedicated number") `POST` /numbers/buy/{dedicated_number}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| dedicated_number | `string` |  ``` Required ```  | Your phone number in E.164 format. | `+12282060576` | 

#### Responses
**200** 

Body (_Buy dedicated number response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here is your new number.",
  "data": {
    "dedicated_number": "+12282060576",
    "country": "US",
    "price_total": "8.98",
    "_price_setup": "22.22",
    "_price_monthly": "11.11",
    "_currency": {
      "currency_name_short": "USD",
      "currency_prefix_d": "$",
      "currency_prefix_c": "¢",
      "currency_name_long": "US Dollars"
    }
  }
}
```


### <a name="search_dedicated_numbers_by_country"></a>![Endpoint: ](https://apidocs.io/img/method.png "Search Dedicated Numbers by Country") `GET` /numbers/search/{country}?{search}=1&{search_type}=2

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| country | `string` |  ``` Required ```  | Your preferred country. | `US` | 
| search | `string` |  ``` Optional ```  | Your search pattern or query. | `88` | 
| search_type | `precision` |  ``` Optional ```  | Your strategy for searching, 0 = starts with, 1 = anywhere, 2 = ends with. | `1` | 

#### Responses
**200** 

Body (_Search Dedicated Numbers by Country response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are your data.",
  "data": {
    "total": 22346,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1490,
    "next_page_url": "/?page=2",
    "prev_page_url": null,
    "from": 1,
    "to": 15,
    "data": [
      {
        "country": "US",
        "country_name": "United States of America",
        "dedicated_number": "+12132633745",
        "price": "26.94",
        "currency": "USD"
      },
      {
        "country": "US",
        "country_name": "United States of America",
        "dedicated_number": "+12134657532",
        "price": "26.94",
        "currency": "USD"
      },
      {
        "country": "US",
        "country_name": "United States of America",
        "dedicated_number": "+12134657538",
        "price": "26.94",
        "currency": "USD"
      },
      {
        "country": "US",
        "country_name": "United States of America",
        "dedicated_number": "+13235777962",
        "price": "26.94",
        "currency": "USD"
      },
      {
        "country": "US",
        "country_name": "United States of America",
        "dedicated_number": "+13235777963",
        "price": "26.94",
        "currency": "USD"
      },
      {
        "country": "US",
        "country_name": "United States of America",
        "dedicated_number": "+13235777965",
        "price": "26.94",
        "currency": "USD"
      },
      {
        "country": "US",
        "country_name": "United States of America",
        "dedicated_number": "+13235777967",
        "price": "26.94",
        "currency": "USD"
      },
      {
        "country": "US",
        "country_name": "United States of America",
        "dedicated_number": "+13235777968",
        "price": "26.94",
        "currency": "USD"
      },
      {
        "country": "US",
        "country_name": "United States of America",
        "dedicated_number": "+13235777971",
        "price": "26.94",
        "currency": "USD"
      },
      {
        "country": "US",
        "country_name": "United States of America",
        "dedicated_number": "+13235777973",
        "price": "26.94",
        "currency": "USD"
      },
      {
        "country": "US",
        "country_name": "United States of America",
        "dedicated_number": "+13235777974",
        "price": "26.94",
        "currency": "USD"
      },
      {
        "country": "US",
        "country_name": "United States of America",
        "dedicated_number": "+13235777975",
        "price": "26.94",
        "currency": "USD"
      },
      {
        "country": "US",
        "country_name": "United States of America",
        "dedicated_number": "+13235777976",
        "price": "26.94",
        "currency": "USD"
      },
      {
        "country": "US",
        "country_name": "United States of America",
        "dedicated_number": "+13235777978",
        "price": "26.94",
        "currency": "USD"
      },
      {
        "country": "US",
        "country_name": "United States of America",
        "dedicated_number": "+13235777979",
        "price": "26.94",
        "currency": "USD"
      }
    ]
  }
}
```


[Back to API Reference](#api_reference)

## <a name="pricing"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Pricing") Pricing


### <a name="get_country_pricing"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Country Pricing") `GET` /pricing/{country}?currency={currency}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| country | `string` |  ``` Required ```  | Two-letter representation of the country. | `AU` | 
| currency | `string` |  ``` Optional ```  | Three-letter representation of the currency. | `AUD` | 

#### Responses
**200** 

Body (_Get Country Pricing response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Price Lists.",
  "data": {
    "country": "AU",
    "sms": {
      "price_rate_0": "0.0700",
      "price_rate_1": "0.0650",
      "price_rate_2": "0.0600",
      "price_rate_3": "0.0550",
      "dedicated_number_monthly": "19.0000",
      "dedicated_number_setup": "20.0000",
      "dedicated_number_shortcode_monthly": "0.0000",
      "dedicated_number_shortcode_setup": "0.0000"
    },
    "voice": {
      "price_landline": "0.0530",
      "price_mobile": "0.1730"
    },
    "fax": {
      "price_fax": "0.2000",
      "dedicated_number_monthly": "30.0000",
      "dedicated_number_setup": "40.0000"
    },
    "post": {
      "price_letter_black": "1.2700",
      "price_letter_colour": "1.4700",
      "price_letter_page_black": "0.1000",
      "price_letter_page_colour": "0.2400",
      "price_letter_large_surcharge": "1.5000",
      "price_letter_large_surcharge_sheet": "0.0400",
      "price_direct_mail_dl": "0.1200",
      "price_direct_mail_a5": "0.1200",
      "direct_mail_min_quantity": 5000
    },
    "email": {
      "price_rate_0": "0.0100",
      "price_rate_1": "0.0080",
      "price_rate_2": "0.0040",
      "price_rate_3": "0.0010"
    },
    "mms": {
      "price_mms": "0.4500",
      "dedicated_number_monthly": "10.0000",
      "dedicated_number_setup": "20.0000"
    },
    "postcard": {
      "price_postcard": "10.0000"
    },
    "_currency": {
      "currency_name_short": "AUD",
      "currency_prefix_d": "$",
      "currency_prefix_c": "c",
      "currency_name_long": "Australian Dollars"
    }
  }
}
```


[Back to API Reference](#api_reference)

## <a name="post_direct_mail"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Post Direct Mail") Post Direct Mail


### <a name="search_locations"></a>![Endpoint: ](https://apidocs.io/img/method.png "Search Locations") `GET` /post/direct-mail/locations/search/{country}/?q={query}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| country | `string` |  ``` Required ```  | Country code. | `AD` | 
| query | `string` |  ``` Required ```  | A postal code or place name. | `AD100` | 

#### Responses
**200** 

Body (_Search Locations response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here's your result.",
  "data": {
    "total": 1,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 1,
    "data": [
      {
        "location_id": 1,
        "country_code": "AD",
        "postal_code": "AD100",
        "place_name": "Canillo",
        "admin_name1": "",
        "admin_code1": "",
        "admin_name2": "",
        "admin_code2": "",
        "admin_name3": "",
        "admin_code3": "",
        "latitude": "42.583300",
        "longitude": "1.666700",
        "accuracy": 6
      }
    ]
  }
}
```


### <a name="create_new_campaign"></a>![Endpoint: ](https://apidocs.io/img/method.png "Create New Campaign") `POST` /post/direct-mail/campaigns/send

> Create new direct mail campaign.



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `create new campaign request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "name": "name",
  "size": "size",
  "file_urls": [
    "file_urls"
  ],
  "schedule": 31.6853192991974,
  "source": "source",
  "areas": [
    "areas"
  ]
}
``` 

#### Responses
**200** 

Body (_Create New Campaign response_) 
```
{
  "http_code": 31,
  "response_code": "response_code",
  "response_msg": "response_msg",
  "data": {}
}
```


### <a name="calculate_direct_mail_campaign_price"></a>![Endpoint: ](https://apidocs.io/img/method.png "Calculate Direct Mail Campaign Price") `POST` /post/direct-mail/campaigns/price

> Calculate direct mail campaign price.



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `calculate direct mail campaign price request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "name": "name",
  "size": "size",
  "file_urls": [
    "file_urls"
  ],
  "schedule": 31.6853192991974,
  "source": "source",
  "areas": [
    "areas"
  ]
}
``` 

#### Responses
**200** 

Body (_Calculate Direct Mail Campaign Price response_) 
```
{
  "http_code": 31,
  "response_code": "response_code",
  "response_msg": "response_msg",
  "data": {}
}
```


### <a name="list_direct_mail_campaigns"></a>![Endpoint: ](https://apidocs.io/img/method.png "List Direct Mail Campaigns") `GET` /post/direct-mail/campaigns

> Get list of direct mail campaigns.



#### Responses
**200** 

Body (_List Direct Mail Campaigns response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are your results.",
  "data": {
    "total": 69,
    "per_page": 15,
    "current_page": 3,
    "last_page": 5,
    "next_page_url": "https://rest.clicksend.com/v3/post/direct-mail/campaigns?page=4",
    "prev_page_url": "https://rest.clicksend.com/v3/post/direct-mail/campaigns?page=2",
    "from": 31,
    "to": 45,
    "data": [
      {
        "campaign_id": 34,
        "user_id": 1,
        "name": "My Campaign",
        "status": null,
        "date_added": 1477040355,
        "schedule": 1477032023,
        "custom_string": null,
        "message_id": null,
        "_total_quantity": "250",
        "_areas": [
          {
            "campaign_id": 34,
            "location_id": 1,
            "quantity": 100,
            "status": null,
            "price": null
          },
          {
            "campaign_id": 34,
            "location_id": 2,
            "quantity": 100,
            "status": null,
            "price": null
          },
          {
            "campaign_id": 34,
            "location_id": 3,
            "quantity": 50,
            "status": null,
            "price": null
          }
        ]
      },
      {
        "campaign_id": 35,
        "user_id": 1,
        "name": "My Campaign",
        "status": null,
        "date_added": 1477040625,
        "schedule": 1477032023,
        "custom_string": null,
        "message_id": null,
        "_total_quantity": "250",
        "_areas": [
          {
            "campaign_id": 35,
            "location_id": 1,
            "quantity": 100,
            "status": null,
            "price": null
          },
          {
            "campaign_id": 35,
            "location_id": 2,
            "quantity": 100,
            "status": null,
            "price": null
          },
          {
            "campaign_id": 35,
            "location_id": 3,
            "quantity": 50,
            "status": null,
            "price": null
          }
        ]
      },
      {
        "campaign_id": 37,
        "user_id": 1,
        "name": "My Campaign",
        "status": null,
        "date_added": 1477040829,
        "schedule": 1477032023,
        "custom_string": null,
        "message_id": null,
        "_total_quantity": 0,
        "_areas": []
      },
      {
        "campaign_id": 38,
        "user_id": 1,
        "name": "My Campaign",
        "status": null,
        "date_added": 1477040843,
        "schedule": 1477032023,
        "custom_string": null,
        "message_id": null,
        "_total_quantity": "250",
        "_areas": [
          {
            "campaign_id": 38,
            "location_id": 1,
            "quantity": 100,
            "status": null,
            "price": null
          },
          {
            "campaign_id": 38,
            "location_id": 2,
            "quantity": 100,
            "status": null,
            "price": null
          },
          {
            "campaign_id": 38,
            "location_id": 3,
            "quantity": 50,
            "status": null,
            "price": null
          }
        ]
      },
      {
        "campaign_id": 39,
        "user_id": 1,
        "name": "My Campaign",
        "status": null,
        "date_added": 1477275714,
        "schedule": 1477032023,
        "custom_string": null,
        "message_id": null,
        "_total_quantity": "250",
        "_areas": [
          {
            "campaign_id": 39,
            "location_id": 1,
            "quantity": 100,
            "status": null,
            "price": null
          },
          {
            "campaign_id": 39,
            "location_id": 2,
            "quantity": 100,
            "status": null,
            "price": null
          },
          {
            "campaign_id": 39,
            "location_id": 3,
            "quantity": 50,
            "status": null,
            "price": null
          }
        ]
      },
      {
        "campaign_id": 40,
        "user_id": 1,
        "name": "My Campaign",
        "status": null,
        "date_added": 1477275760,
        "schedule": 1477032023,
        "custom_string": "Custom String",
        "message_id": null,
        "_total_quantity": "250",
        "_areas": [
          {
            "campaign_id": 40,
            "location_id": 1,
            "quantity": 100,
            "status": null,
            "price": null
          },
          {
            "campaign_id": 40,
            "location_id": 2,
            "quantity": 100,
            "status": null,
            "price": null
          },
          {
            "campaign_id": 40,
            "location_id": 3,
            "quantity": 50,
            "status": null,
            "price": null
          }
        ]
      },
      {
        "campaign_id": 42,
        "user_id": 1,
        "name": "My Campaign",
        "status": null,
        "date_added": 1477276756,
        "schedule": 1477032023,
        "custom_string": "Custom String",
        "message_id": null,
        "_total_quantity": "250",
        "_areas": [
          {
            "campaign_id": 42,
            "location_id": 1,
            "quantity": 100,
            "status": null,
            "price": null
          },
          {
            "campaign_id": 42,
            "location_id": 2,
            "quantity": 100,
            "status": null,
            "price": null
          },
          {
            "campaign_id": 42,
            "location_id": 3,
            "quantity": 50,
            "status": null,
            "price": null
          }
        ]
      },
      {
        "campaign_id": 43,
        "user_id": 1,
        "name": "My Campaign",
        "status": null,
        "date_added": 1477276830,
        "schedule": 1477032023,
        "custom_string": "Custom String",
        "message_id": null,
        "_total_quantity": "250",
        "_areas": [
          {
            "campaign_id": 43,
            "location_id": 1,
            "quantity": 100,
            "status": null,
            "price": null
          },
          {
            "campaign_id": 43,
            "location_id": 2,
            "quantity": 100,
            "status": null,
            "price": null
          },
          {
            "campaign_id": 43,
            "location_id": 3,
            "quantity": 50,
            "status": null,
            "price": null
          }
        ]
      },
      {
        "campaign_id": 49,
        "user_id": 1,
        "name": "My Campaign",
        "status": null,
        "date_added": 1477279662,
        "schedule": 1477032023,
        "custom_string": "Custom String",
        "message_id": null,
        "_total_quantity": "250",
        "_areas": [
          {
            "campaign_id": 49,
            "location_id": 1,
            "quantity": 100,
            "status": null,
            "price": null
          },
          {
            "campaign_id": 49,
            "location_id": 2,
            "quantity": 100,
            "status": null,
            "price": null
          },
          {
            "campaign_id": 49,
            "location_id": 3,
            "quantity": 50,
            "status": null,
            "price": null
          }
        ]
      },
      {
        "campaign_id": 51,
        "user_id": 1,
        "name": "My Campaign",
        "status": null,
        "date_added": 1477279949,
        "schedule": 1477032023,
        "custom_string": "Custom String",
        "message_id": null,
        "_total_quantity": "250",
        "_areas": [
          {
            "campaign_id": 51,
            "location_id": 1,
            "quantity": 100,
            "status": null,
            "price": null
          },
          {
            "campaign_id": 51,
            "location_id": 2,
            "quantity": 100,
            "status": null,
            "price": null
          },
          {
            "campaign_id": 51,
            "location_id": 3,
            "quantity": 50,
            "status": null,
            "price": null
          }
        ]
      },
      {
        "campaign_id": 52,
        "user_id": 1,
        "name": "My Campaign",
        "status": null,
        "date_added": 1477280021,
        "schedule": 1477032023,
        "custom_string": "Custom String",
        "message_id": null,
        "_total_quantity": "250",
        "_areas": [
          {
            "campaign_id": 52,
            "location_id": 1,
            "quantity": 100,
            "status": null,
            "price": null
          },
          {
            "campaign_id": 52,
            "location_id": 2,
            "quantity": 100,
            "status": null,
            "price": null
          },
          {
            "campaign_id": 52,
            "location_id": 3,
            "quantity": 50,
            "status": null,
            "price": null
          }
        ]
      },
      {
        "campaign_id": 53,
        "user_id": 1,
        "name": "My Campaign",
        "status": null,
        "date_added": 1477280780,
        "schedule": 1477032023,
        "custom_string": "Custom String",
        "message_id": null,
        "_total_quantity": "250",
        "_areas": [
          {
            "campaign_id": 53,
            "location_id": 1,
            "quantity": 100,
            "status": null,
            "price": "222.00"
          },
          {
            "campaign_id": 53,
            "location_id": 2,
            "quantity": 100,
            "status": null,
            "price": "222.00"
          },
          {
            "campaign_id": 53,
            "location_id": 3,
            "quantity": 50,
            "status": null,
            "price": "111.00"
          }
        ]
      },
      {
        "campaign_id": 54,
        "user_id": 1,
        "name": "My Campaign",
        "status": null,
        "date_added": 1477281977,
        "schedule": 1477032023,
        "custom_string": "Custom String",
        "message_id": null,
        "_total_quantity": "250",
        "_areas": [
          {
            "campaign_id": 54,
            "location_id": 1,
            "quantity": 100,
            "status": null,
            "price": "222.00"
          },
          {
            "campaign_id": 54,
            "location_id": 2,
            "quantity": 100,
            "status": null,
            "price": "222.00"
          },
          {
            "campaign_id": 54,
            "location_id": 3,
            "quantity": 50,
            "status": null,
            "price": "111.00"
          }
        ]
      },
      {
        "campaign_id": 55,
        "user_id": 1,
        "name": "My Campaign",
        "status": "Queued",
        "date_added": 1477284216,
        "schedule": 1477032023,
        "custom_string": "Custom String",
        "message_id": null,
        "_total_quantity": "250",
        "_areas": [
          {
            "campaign_id": 55,
            "location_id": 1,
            "quantity": 100,
            "status": "Queued",
            "price": "222.00"
          },
          {
            "campaign_id": 55,
            "location_id": 2,
            "quantity": 100,
            "status": "Queued",
            "price": "222.00"
          },
          {
            "campaign_id": 55,
            "location_id": 3,
            "quantity": 50,
            "status": "Queued",
            "price": "111.00"
          }
        ]
      },
      {
        "campaign_id": 56,
        "user_id": 1,
        "name": "My Campaign",
        "status": "Scheduled",
        "date_added": 1477284517,
        "schedule": 1477384503,
        "custom_string": "Custom String",
        "message_id": null,
        "_total_quantity": "250",
        "_areas": [
          {
            "campaign_id": 56,
            "location_id": 1,
            "quantity": 100,
            "status": "Scheduled",
            "price": "222.00"
          },
          {
            "campaign_id": 56,
            "location_id": 2,
            "quantity": 100,
            "status": "Scheduled",
            "price": "222.00"
          },
          {
            "campaign_id": 56,
            "location_id": 3,
            "quantity": 50,
            "status": "Scheduled",
            "price": "111.00"
          }
        ]
      }
    ]
  }
}
```


[Back to API Reference](#api_reference)

## <a name="post_letter"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Post Letter") Post Letter


### <a name="send_post_letter"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send Post Letter") `POST` /post/letters/send

> **Supported File Types**
> We support `pdf`, `docx` and `doc` files. Contact us to add support for any other file type. If you're using `docx` or `doc` files, you'll need to convert the file first using our uploads endpoint with the querystring parameter `convert=post` e.g. `POST /uploads?convert=post`. This will return a URL to the converted pdf file that can be used in the `/post/letters/send` endpoint.
> **Letter File Options**
> **Use existing URL**
> With this option, you can use an existing URL to a `pdf` document. For example, you might generate the `pdf` on your server.
> **Upload File to Our Server**
> With this option, you can use the `/uploads` endpoint to upload the document. The `/uploads` endpoint returns a URL that can be used in the `/post/letters/send` endpoint.



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `send post letter request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "file_url": "http://server.com/file.pdf",
  "template_used": 1,
  "colour": 1,
  "duplex": 0,
  "recipients": [
    {
      "address_name": "My Home Address",
      "address_line_1": "Address 1",
      "address_line_2": "Address 2",
      "address_city": "CITY",
      "address_state": "State",
      "address_postal_code": 123456,
      "address_country": "AU",
      "return_address_id": 1,
      "schedule": 1449573604
    }
  ]
}
``` 

#### Responses
**200** 

Body (_Send Post Letter response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Letters queued for delivery.",
  "data": {
    "total_price": 13.42,
    "total_count": 1,
    "queued_count": 1,
    "recipients": [
      {
        "user_id": 1,
        "subaccount_id": 1,
        "message_id": "A00A1066-BBAE-432B-9B2D-E88969B12C46",
        "address_name": "My Home Address",
        "address_line_1": "Address 1",
        "address_line_2": "",
        "address_city": "CITY",
        "address_state": "State",
        "address_postal_code": "123456",
        "address_country": "AU",
        "return_address_id": 1,
        "schedule": 1449573604,
        "source": ".rest.v3",
        "colour": 1,
        "duplex": 0,
        "post_pages": 7,
        "post_price": "13.4200",
        "date_added": 1459131623,
        "status": "SUCCESS",
        "_file_url": "http://server.com/file.pdf",
        "_return_address": {
          "return_address_id": 1,
          "user_id": 1,
          "address_name": "My Home Address",
          "address_line_1": "Maritime Avenue",
          "address_line_2": "",
          "address_city": "Flynn",
          "address_state": "WA",
          "address_postal_code": "6302",
          "address_country": "AU"
        },
        "_api_username": "my_api_username"
      }
    ],
    "_currency": {
      "currency_name_short": "AUD",
      "currency_prefix_d": "$",
      "currency_prefix_c": "c",
      "currency_name_long": "Australian Dollars"
    }
  }
}
```


### <a name="calculate_price"></a>![Endpoint: ](https://apidocs.io/img/method.png "Calculate Price") `POST` /post/letters/price

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `calculate price request170` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "file_url": "http://server.com/file.pdf",
  "template_used": 1,
  "colour": 1,
  "duplex": 0,
  "recipients": [
    "[]"
  ],
  "Body": ""
}
``` 

#### Responses
**200** 

Body (_Calculate Price response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are some results.",
  "data": {
    "total_price": 1.87,
    "total_cost": 1,
    "recipients": [
      {
        "user_id": 1,
        "subaccount_id": 1,
        "message_id": "06FAD39C-78FD-4D2F-B606-9846D1979F35",
        "address_name": "My Home Address",
        "address_line_1": "131",
        "address_line_2": "Scheuvront Drive",
        "address_city": "DENVER",
        "address_state": "CO",
        "address_postal_code": "80202",
        "address_country": "AU",
        "return_address_id": 1,
        "schedule": 1449573604,
        "post_pages": 3,
        "post_price": "1.8700",
        "status": "SUCCESS",
        "date_added": 1449662203
      }
    ]
  }
}
```


### <a name="get_post_letter_history"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Post Letter History") `GET` /post/letters/history

> TODO: Add a method description



#### Responses
**200** 

Body (_Get Post Letter History response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here is your history.",
  "data": {
    "total": 6,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 6,
    "data": [
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": null,
        "message_id": "7C0CF79F-F6E0-471D-8CC8-D7AB34A4D423",
        "address_name": "My Home Address",
        "address_line_1": "130 Scheuvront Drive",
        "address_line_2": null,
        "address_city": "DENVER",
        "address_state": "CO",
        "address_postal_code": "80202",
        "address_country": "AU",
        "return_address_id": 4,
        "custom_string": null,
        "schedule": null,
        "source": null,
        "colour": 0,
        "duplex": 0,
        "post_pages": 1,
        "post_price": "1.100000",
        "status": "Queued:Stamped",
        "status_code": "",
        "status_text": "",
        "date_added": 1447642486
      },
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": null,
        "message_id": "D7E64413-EE22-4E75-9D7D-1653AE5625CB",
        "address_name": "My Home Address",
        "address_line_1": "130 Scheuvront Drive",
        "address_line_2": null,
        "address_city": "DENVER",
        "address_state": "CO",
        "address_postal_code": "80202",
        "address_country": "AU",
        "return_address_id": 4,
        "custom_string": null,
        "schedule": null,
        "source": null,
        "colour": 0,
        "duplex": 0,
        "post_pages": 1,
        "post_price": "1.100000",
        "status": "Queued:Stamped",
        "status_code": "",
        "status_text": "",
        "date_added": 1447645676
      },
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": null,
        "message_id": "0AE161A5-8054-4E4C-B4CC-82E1CAE25D92",
        "address_name": "My Home Address",
        "address_line_1": "130 Scheuvront Drive",
        "address_line_2": null,
        "address_city": "DENVER",
        "address_state": "CO",
        "address_postal_code": "80202",
        "address_country": "AU",
        "return_address_id": 4,
        "custom_string": null,
        "schedule": null,
        "source": null,
        "colour": 0,
        "duplex": 0,
        "post_pages": 1,
        "post_price": "1.100000",
        "status": "Queued",
        "status_code": null,
        "status_text": null,
        "date_added": 1447742914
      },
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": null,
        "message_id": "F18B4ECD-7508-4694-814C-BC87028A8AAE",
        "address_name": "My Home Address",
        "address_line_1": "130 Scheuvront Drive",
        "address_line_2": null,
        "address_city": "DENVER",
        "address_state": "CO",
        "address_postal_code": "80202",
        "address_country": "AU",
        "return_address_id": 4,
        "custom_string": null,
        "schedule": null,
        "source": null,
        "colour": 0,
        "duplex": 0,
        "post_pages": 1,
        "post_price": "1.100000",
        "status": "Queued",
        "status_code": null,
        "status_text": null,
        "date_added": 1447745108
      },
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": null,
        "message_id": "8849F629-F9DB-499E-B084-5088399A51E9",
        "address_name": "My Home Address",
        "address_line_1": "130 Scheuvront Drive",
        "address_line_2": null,
        "address_city": "DENVER",
        "address_state": "CO",
        "address_postal_code": "80202",
        "address_country": "AU",
        "return_address_id": 4,
        "custom_string": null,
        "schedule": null,
        "source": null,
        "colour": 0,
        "duplex": 0,
        "post_pages": 1,
        "post_price": "1.100000",
        "status": "Queued",
        "status_code": null,
        "status_text": null,
        "date_added": 1447745144
      },
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": null,
        "message_id": "3095F46F-8ED2-49A2-B4CC-DC20786A6209",
        "address_name": "My Home Address",
        "address_line_1": "130 Scheuvront Drive",
        "address_line_2": null,
        "address_city": "DENVER",
        "address_state": "CO",
        "address_postal_code": "80202",
        "address_country": "AU",
        "return_address_id": 4,
        "custom_string": null,
        "schedule": null,
        "source": null,
        "colour": 0,
        "duplex": 0,
        "post_pages": 1,
        "post_price": "1.100000",
        "status": "Queued",
        "status_code": null,
        "status_text": null,
        "date_added": 1447745652
      }
    ]
  }
}
```


### <a name="export_post_letter_history"></a>![Endpoint: ](https://apidocs.io/img/method.png "Export Post Letter History") `GET` /post/letters/export?filename={filename}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| filename | `string` |  ``` Required ```  | Filename for the export file. | `myexport.csv` | 

#### Responses
**200** 

Body (_Export Post Letter History response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Download your file here.",
  "data": {
    "url": "https://rest.clicksend.com/files/705F80D0-D044-4F85-8617-081988B398E4?filename=myexport.csv"
  }
}
```


### <a name="create_a_post_return_address"></a>![Endpoint: ](https://apidocs.io/img/method.png "Create a Post Return Address") `POST` /post/return-addresses

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `create a post return address request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "address_name": "My Home Address",
  "address_line_1": "Maritime Avenue",
  "address_line_2": "",
  "address_city": "Flynn",
  "address_state": "WA",
  "address_postal_code": 6302,
  "address_country": "Australia"
}
``` 

#### Responses
**200** 

Body (_Create a Post Return Address response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "New return address has been added.",
  "data": {
    "return_address_id": 14,
    "user_id": 1,
    "address_name": "My Home Address",
    "address_line_1": "Maritime Avenue",
    "address_line_2": "",
    "address_city": "Flynn",
    "address_state": "WA",
    "address_postal_code": "6302",
    "address_country": "Australia"
  }
}
```


### <a name="get_list_of_post_return_addresses"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get List of Post Return Addresses") `GET` /post/return-addresses

> TODO: Add a method description



#### Responses
**200** 

Body (_Get List of Post Return Addresses response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are your records.",
  "data": {
    "total": 10,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 10,
    "data": [
      {
        "return_address_id": 4,
        "user_id": 1,
        "address_name": "My Address",
        "address_line_1": "Maritime Avenue",
        "address_line_2": "",
        "address_city": "Flynn",
        "address_state": "WA",
        "address_postal_code": "6302",
        "address_country": "AU"
      },
      {
        "return_address_id": 5,
        "user_id": 1,
        "address_name": "My Address",
        "address_line_1": "Maritime Avenue",
        "address_line_2": "",
        "address_city": "Flynn",
        "address_state": "WA",
        "address_postal_code": "6302",
        "address_country": "AU"
      },
      {
        "return_address_id": 6,
        "user_id": 1,
        "address_name": "My Address",
        "address_line_1": "Maritime Avenue",
        "address_line_2": "",
        "address_city": "Flynn",
        "address_state": "WA",
        "address_postal_code": "6302",
        "address_country": "AU"
      },
      {
        "return_address_id": 7,
        "user_id": 1,
        "address_name": "My Address",
        "address_line_1": "Maritime Avenue",
        "address_line_2": "",
        "address_city": "Flynn",
        "address_state": "WA",
        "address_postal_code": "6302",
        "address_country": "AU"
      },
      {
        "return_address_id": 8,
        "user_id": 1,
        "address_name": "My Address",
        "address_line_1": "Maritime Avenue",
        "address_line_2": "",
        "address_city": "Flynn",
        "address_state": "WA",
        "address_postal_code": "6302",
        "address_country": "AU"
      },
      {
        "return_address_id": 9,
        "user_id": 1,
        "address_name": "My Address",
        "address_line_1": "Maritime Avenue",
        "address_line_2": "",
        "address_city": "Flynn",
        "address_state": "WA",
        "address_postal_code": "6302",
        "address_country": "AU"
      },
      {
        "return_address_id": 10,
        "user_id": 1,
        "address_name": "My Address",
        "address_line_1": "Maritime Avenue",
        "address_line_2": "",
        "address_city": "Flynn",
        "address_state": "WA",
        "address_postal_code": "6302",
        "address_country": "AU"
      },
      {
        "return_address_id": 11,
        "user_id": 1,
        "address_name": "My Address",
        "address_line_1": "Maritime Avenue",
        "address_line_2": "",
        "address_city": "Flynn",
        "address_state": "WA",
        "address_postal_code": "6302",
        "address_country": "AU"
      },
      {
        "return_address_id": 12,
        "user_id": 1,
        "address_name": "My Address",
        "address_line_1": "Maritime Avenue",
        "address_line_2": "",
        "address_city": "Flynn",
        "address_state": "WA",
        "address_postal_code": "6302",
        "address_country": "AU"
      },
      {
        "return_address_id": 14,
        "user_id": 1,
        "address_name": "My Home Address",
        "address_line_1": "Maritime Avenue",
        "address_line_2": "",
        "address_city": "Flynn",
        "address_state": "WA",
        "address_postal_code": "6302",
        "address_country": "Australia"
      }
    ]
  }
}
```


### <a name="get_post_return_address"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Post Return Address") `GET` /post/return-addresses/{return_address_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| return_address_id | `precision` |  ``` Required ```  | Your return address id. | `14` | 

#### Responses
**200** 

Body (_Get Post Return Address response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here is your data.",
  "data": {
    "return_address_id": 14,
    "user_id": 1,
    "address_name": "My Home Address",
    "address_line_1": "Maritime Avenue",
    "address_line_2": "",
    "address_city": "Flynn",
    "address_state": "WA",
    "address_postal_code": "6302",
    "address_country": "Australia"
  }
}
```


### <a name="update_post_return_address"></a>![Endpoint: ](https://apidocs.io/img/method.png "Update Post Return Address") `PUT` /post/return-addresses/{return_address_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| return_address_id | `precision` |  ``` Required ```  | Your return address id. | `14` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `update post return address request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "address_name": "My Home Address",
  "address_line_1": "Maritime Avenue",
  "address_line_2": "",
  "address_city": "Flynn",
  "address_state": "WA",
  "address_postal_code": 6302,
  "address_country": "Australia"
}
``` 

#### Responses
**200** 

Body (_Update Post Return Address response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your return address has been updated.",
  "data": {
    "return_address_id": 14,
    "user_id": 1,
    "address_name": "My Home Address",
    "address_line_1": "Maritime Avenue",
    "address_line_2": "",
    "address_city": "Flynn",
    "address_state": "WA",
    "address_postal_code": 6302,
    "address_country": "Australia"
  }
}
```


### <a name="delete_post_return_address"></a>![Endpoint: ](https://apidocs.io/img/method.png "Delete Post Return Address") `DELETE` /post/return-addresses/{return_address_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| return_address_id | `precision` |  ``` Required ```  | Your return address id. | `12` | 

#### Responses
**200** 

Body (_Delete Post Return Address response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your return address has been deleted.",
  "data": []
}
```


[Back to API Reference](#api_reference)

## <a name="postcards"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Postcards") Postcards


### <a name="send_postcard"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send Postcard") `POST` /post/postcards/send

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



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `send postcard request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "file_urls": [
    "https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_front.pdf",
    "https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_back.pdf"
  ],
  "recipients": [
    {
      "address_name": "My Home Address",
      "address_line_1": "Address 1",
      "address_line_2": "",
      "address_city": "City",
      "address_state": "State",
      "address_postal_code": "123456",
      "address_country": "AU",
      "return_address_id": 1
    }
  ]
}
``` 

#### Responses
**200** 

Body (_Send Postcard response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Postcard queued for delivery.",
  "data": {
    "total_price": 11,
    "total_count": 1,
    "queued_count": 1,
    "recipients": [
      {
        "user_id": 1,
        "subaccount_id": 13,
        "message_id": "C8CAA97A-905A-4A31-99CB-A92C7BA05A97",
        "address_name": "My Home Address",
        "address_line_1": "Address 1",
        "address_line_2": "",
        "address_city": "CITY",
        "address_state": "State",
        "address_postal_code": "123456",
        "address_country": "AU",
        "return_address_id": 1,
        "letter_file_name": "6A559A74-486D-4012-84D7-F3FE11904CB1.pdf",
        "schedule": 1482473172,
        "ip_address": "127.0.0.1",
        "source": ".rest.v3",
        "post_price": 11,
        "priority": 32,
        "status": "SUCCESS",
        "date_added": 1482473172,
        "_file_url": "https://rest.clicksend.com/files/6A559A74-486D-4012-84D7-F3FE11904CB1.pdf",
        "_return_address": {
          "return_address_id": 1,
          "user_id": 1,
          "address_name": "John Doe",
          "address_line_1": "5/30 Leonora St",
          "address_line_2": "",
          "address_city": "Como",
          "address_state": "WA",
          "address_postal_code": "6152",
          "address_country": "AU"
        },
        "_api_username": "johndoe"
      }
    ],
    "_currency": {
      "currency_name_short": "AUD",
      "currency_prefix_d": "$",
      "currency_prefix_c": "c",
      "currency_name_long": "Australian Dollars"
    }
  }
}
```


### <a name="calculate_pricing"></a>![Endpoint: ](https://apidocs.io/img/method.png "Calculate Pricing") `POST` /post/postcards/price

> For `file_urls` field. You can attach at least 1 and max of 2 PDF file urls.
> - Supply a single pdf with 2 pages (front and back)
> - Supply 2 urls to seperate PDFs



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `calculate pricing request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "file_urls": [
    "https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_front.pdf",
    "https://s3-ap-southeast-2.amazonaws.com/clicksend-api-downloads/_public/_examples/a5_back.pdf"
  ],
  "recipients": [
    {
      "address_name": "My Home Address",
      "address_line_1": "Address 1",
      "address_line_2": "",
      "address_city": "City",
      "address_state": "State",
      "address_postal_code": "123456",
      "address_country": "AU",
      "return_address_id": 1
    }
  ]
}
``` 

#### Responses
**200** 

Body (_Calculate Pricing response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Postcard queued for delivery.",
  "data": {
    "total_price": 11,
    "total_count": 1,
    "queued_count": 1,
    "recipients": [
      {
        "user_id": 1,
        "subaccount_id": 13,
        "message_id": "C8CAA97A-905A-4A31-99CB-A92C7BA05A97",
        "address_name": "My Home Address",
        "address_line_1": "Address 1",
        "address_line_2": "",
        "address_city": "CITY",
        "address_state": "State",
        "address_postal_code": "123456",
        "address_country": "AU",
        "return_address_id": 1,
        "letter_file_name": "6A559A74-486D-4012-84D7-F3FE11904CB1.pdf",
        "schedule": 1482473172,
        "ip_address": "127.0.0.1",
        "source": ".rest.v3",
        "post_price": 11,
        "priority": 32,
        "status": "SUCCESS",
        "date_added": 1482473172,
        "_file_url": "https://rest.clicksend.com/files/6A559A74-486D-4012-84D7-F3FE11904CB1.pdf",
        "_return_address": {
          "return_address_id": 1,
          "user_id": 1,
          "address_name": "John Doe",
          "address_line_1": "5/30 Leonora St",
          "address_line_2": "",
          "address_city": "Como",
          "address_state": "WA",
          "address_postal_code": "6152",
          "address_country": "AU"
        },
        "_api_username": "johndoe"
      }
    ],
    "_currency": {
      "currency_name_short": "AUD",
      "currency_prefix_d": "$",
      "currency_prefix_c": "c",
      "currency_name_long": "Australian Dollars"
    }
  }
}
```


### <a name="get_postcard_history"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Postcard History") `GET` /post/postcards/history

> TODO: Add a method description



#### Responses
**200** 

Body (_Get Postcard History response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here is your history.",
  "data": {
    "total": 32,
    "per_page": 15,
    "current_page": 1,
    "last_page": 3,
    "next_page_url": "https://rest.clicksend.com/v3/post/postcards/history?page=2",
    "prev_page_url": null,
    "from": 1,
    "to": 15,
    "data": [
      {
        "user_id": 1,
        "subaccount_id": 13,
        "list_id": null,
        "message_id": "909D6F4F-FC88-4BB8-AD96-D2F4B3139301",
        "message_id_supplier": "2RXWRVFFG3G8D6TB6V6P6VX7RHR7",
        "address_name": "My Home Address",
        "address_line_1": "Address 1",
        "address_line_2": "",
        "address_city": "CITY",
        "address_state": "State",
        "address_postal_code": "123456",
        "address_country": "AU",
        "return_address_id": 1,
        "letter_file_name": "65889986-E306-4309-B229-FD9215EE1013A.pdf",
        "custom_string": null,
        "schedule": "1482308357",
        "ip_address": "127.0.0.1",
        "source": ".rest.v3",
        "post_price": "1.710000",
        "post_price_supplier": "0.000000",
        "priority": 32,
        "status": "Sent",
        "date_added": 1482308357,
        "_file_url": "https://rest.clicksend.com/files/65889986-E306-4309-B229-FD9215EE1013A.pdf",
        "_return_address": {
          "return_address_id": 1,
          "user_id": 1,
          "address_name": "John Doe",
          "address_line_1": "3/28 Leonora St",
          "address_line_2": "",
          "address_city": "Como",
          "address_state": "WA",
          "address_postal_code": "6152",
          "address_country": "AU"
        },
        "_api_username": "johndoe"
      },
      {
        "user_id": 1,
        "subaccount_id": 13,
        "list_id": null,
        "message_id": "E4FBBB5F-9E05-45D8-93AF-2C1A3BFD5284",
        "message_id_supplier": "3HKQX79D2CT6DXDRQVRHPW7GDTM6",
        "address_name": "My Home Address",
        "address_line_1": "Address 1",
        "address_line_2": "",
        "address_city": "CITY",
        "address_state": "State",
        "address_postal_code": "123456",
        "address_country": "AU",
        "return_address_id": 1,
        "letter_file_name": "2B306DC3-FD44-488B-92B2-D895934289FCA.pdf",
        "custom_string": null,
        "schedule": "1482308357",
        "ip_address": "127.0.0.1",
        "source": ".rest.v3",
        "post_price": "1.710000",
        "post_price_supplier": "0.000000",
        "priority": 32,
        "status": "Sent",
        "date_added": 1482308357,
        "_file_url": "https://rest.clicksend.com/files/2B306DC3-FD44-488B-92B2-D895934289FCA.pdf",
        "_return_address": {
          "return_address_id": 1,
          "user_id": 1,
          "address_name": "John Doe",
          "address_line_1": "3/28 Leonora St",
          "address_line_2": "",
          "address_city": "Como",
          "address_state": "WA",
          "address_postal_code": "6152",
          "address_country": "AU"
        },
        "_api_username": "johndoe"
      },
      {
        "user_id": 1,
        "subaccount_id": 13,
        "list_id": null,
        "message_id": "550CB11B-2D75-4851-8E2C-798F67A0BF9D",
        "message_id_supplier": "B3YCJJRHQ2WD3CJFXKWB4BTFVYW8",
        "address_name": "My Home Address",
        "address_line_1": "Address 1",
        "address_line_2": "",
        "address_city": "CITY",
        "address_state": "State",
        "address_postal_code": "123456",
        "address_country": "AU",
        "return_address_id": 1,
        "letter_file_name": "81D66A74-E41A-4C9B-AD51-CC932051F486A.pdf",
        "custom_string": null,
        "schedule": "1482308357",
        "ip_address": "127.0.0.1",
        "source": ".rest.v3",
        "post_price": "1.710000",
        "post_price_supplier": "0.000000",
        "priority": 32,
        "status": "Sent",
        "date_added": 1482308357,
        "_file_url": "https://rest.clicksend.com/files/81D66A74-E41A-4C9B-AD51-CC932051F486A.pdf",
        "_return_address": {
          "return_address_id": 1,
          "user_id": 1,
          "address_name": "John Doe",
          "address_line_1": "3/28 Leonora St",
          "address_line_2": "",
          "address_city": "Como",
          "address_state": "WA",
          "address_postal_code": "6152",
          "address_country": "AU"
        },
        "_api_username": "johndoe"
      },
      {
        "user_id": 1,
        "subaccount_id": 13,
        "list_id": null,
        "message_id": "65C65D93-C327-45BD-BD6D-3C9682C88533",
        "message_id_supplier": "R8CR92RVJH2Y8JC9JJCGT8RWH8B2",
        "address_name": "My Home Address",
        "address_line_1": "Address 1",
        "address_line_2": "",
        "address_city": "CITY",
        "address_state": "State",
        "address_postal_code": "123456",
        "address_country": "AU",
        "return_address_id": 2,
        "letter_file_name": "80686068-68A5-42C6-8CD3-DE2FF5914D81A.pdf",
        "custom_string": null,
        "schedule": "1482308357",
        "ip_address": "127.0.0.1",
        "source": ".rest.v3",
        "post_price": "1.710000",
        "post_price_supplier": "0.000000",
        "priority": 32,
        "status": "Sent",
        "date_added": 1482308357,
        "_file_url": "https://rest.clicksend.com/files/80686068-68A5-42C6-8CD3-DE2FF5914D81A.pdf",
        "_return_address": {
          "return_address_id": 2,
          "user_id": 1,
          "address_name": "My Home Address",
          "address_line_1": "Maritime Avenue",
          "address_line_2": "",
          "address_city": "Flynn",
          "address_state": "WA",
          "address_postal_code": "6302",
          "address_country": "AU"
        },
        "_api_username": "johndoe"
      },
      {
        "user_id": 1,
        "subaccount_id": 13,
        "list_id": null,
        "message_id": "B4E256A5-1D25-45D7-9DB5-EEC17761372A",
        "message_id_supplier": "V88MF93C9TVG2VF83T6K2GQVD6DJ",
        "address_name": "My Home Address",
        "address_line_1": "Address 1",
        "address_line_2": "",
        "address_city": "CITY",
        "address_state": "State",
        "address_postal_code": "123456",
        "address_country": "AU",
        "return_address_id": 2,
        "letter_file_name": "DD750F79-A44F-4729-AC35-9267FE5AB2EFA.pdf",
        "custom_string": null,
        "schedule": "1482308357",
        "ip_address": "127.0.0.1",
        "source": ".rest.v3",
        "post_price": "1.710000",
        "post_price_supplier": "0.000000",
        "priority": 32,
        "status": "Sent",
        "date_added": 1482308357,
        "_file_url": "https://rest.clicksend.com/files/DD750F79-A44F-4729-AC35-9267FE5AB2EFA.pdf",
        "_return_address": {
          "return_address_id": 2,
          "user_id": 1,
          "address_name": "My Home Address",
          "address_line_1": "Maritime Avenue",
          "address_line_2": "",
          "address_city": "Flynn",
          "address_state": "WA",
          "address_postal_code": "6302",
          "address_country": "AU"
        },
        "_api_username": "johndoe"
      },
      {
        "user_id": 1,
        "subaccount_id": 13,
        "list_id": null,
        "message_id": "4BF01D93-8BE5-42E4-AEAF-C9D1B27DCA23",
        "message_id_supplier": "CQK8KTHP3J2B2WG2DW86C2DDH6WW",
        "address_name": "My Home Address",
        "address_line_1": "Address 1",
        "address_line_2": "",
        "address_city": "CITY",
        "address_state": "State",
        "address_postal_code": "123456",
        "address_country": "AU",
        "return_address_id": 1,
        "letter_file_name": "BB141DB5-57DF-4FA5-A9E4-A13E5AC716E7A.pdf",
        "custom_string": null,
        "schedule": "1482311889",
        "ip_address": "127.0.0.1",
        "source": ".rest.v3",
        "post_price": "1.370000",
        "post_price_supplier": "0.000000",
        "priority": 32,
        "status": "Sent",
        "date_added": 1482311889,
        "_file_url": "https://rest.clicksend.com/files/BB141DB5-57DF-4FA5-A9E4-A13E5AC716E7A.pdf",
        "_return_address": {
          "return_address_id": 1,
          "user_id": 1,
          "address_name": "John Doe",
          "address_line_1": "3/28 Leonora St",
          "address_line_2": "",
          "address_city": "Como",
          "address_state": "WA",
          "address_postal_code": "6152",
          "address_country": "AU"
        },
        "_api_username": "johndoe"
      },
      {
        "user_id": 1,
        "subaccount_id": 13,
        "list_id": null,
        "message_id": "BBA4C1F0-5C7C-4A58-9B93-C48FAB2DA649",
        "message_id_supplier": "X9FBM27WHPJJW9JWT2XVJTYXVDY2",
        "address_name": "My Home Address",
        "address_line_1": "Address 1",
        "address_line_2": "",
        "address_city": "CITY",
        "address_state": "State",
        "address_postal_code": "123456",
        "address_country": "AU",
        "return_address_id": 1,
        "letter_file_name": "BF430552-0581-42DD-BA00-B2228E7FE34BA.pdf",
        "custom_string": null,
        "schedule": "1482311889",
        "ip_address": "127.0.0.1",
        "source": ".rest.v3",
        "post_price": "1.370000",
        "post_price_supplier": "0.000000",
        "priority": 32,
        "status": "Sent",
        "date_added": 1482311889,
        "_file_url": "https://rest.clicksend.com/files/BF430552-0581-42DD-BA00-B2228E7FE34BA.pdf",
        "_return_address": {
          "return_address_id": 1,
          "user_id": 1,
          "address_name": "John Doe",
          "address_line_1": "3/28 Leonora St",
          "address_line_2": "",
          "address_city": "Como",
          "address_state": "WA",
          "address_postal_code": "6152",
          "address_country": "AU"
        },
        "_api_username": "johndoe"
      },
      {
        "user_id": 1,
        "subaccount_id": 13,
        "list_id": null,
        "message_id": "5BC692D1-EC43-4C4F-9E83-8543B52F8B7B",
        "message_id_supplier": "7VW44YDFPJB7WWDRTXPKK9F7Q4RJ",
        "address_name": "My Home Address",
        "address_line_1": "Address 1",
        "address_line_2": "",
        "address_city": "CITY",
        "address_state": "State",
        "address_postal_code": "123456",
        "address_country": "AU",
        "return_address_id": 1,
        "letter_file_name": "13BB1876-E421-4B5A-8017-81E7F9598FE5A.pdf",
        "custom_string": null,
        "schedule": "1482311889",
        "ip_address": "127.0.0.1",
        "source": ".rest.v3",
        "post_price": "1.370000",
        "post_price_supplier": "0.000000",
        "priority": 32,
        "status": "Sent",
        "date_added": 1482311889,
        "_file_url": "https://rest.clicksend.com/files/13BB1876-E421-4B5A-8017-81E7F9598FE5AA.pdf",
        "_return_address": {
          "return_address_id": 1,
          "user_id": 1,
          "address_name": "John Doe",
          "address_line_1": "3/28 Leonora St",
          "address_line_2": "",
          "address_city": "Como",
          "address_state": "WA",
          "address_postal_code": "6152",
          "address_country": "AU"
        },
        "_api_username": "johndoe"
      },
      {
        "user_id": 1,
        "subaccount_id": 13,
        "list_id": null,
        "message_id": "CD2C87AA-D352-4998-BE7F-5EBDF089AF61",
        "message_id_supplier": "GQ8MJ4DBRGQFPQ9K9M239CBVKDP2",
        "address_name": "My Home Address",
        "address_line_1": "Address 1",
        "address_line_2": "",
        "address_city": "CITY",
        "address_state": "State",
        "address_postal_code": "123456",
        "address_country": "AU",
        "return_address_id": 2,
        "letter_file_name": "77A18FEA-8935-430E-B14A-7EBF5E1E19C8AA.pdf",
        "custom_string": null,
        "schedule": "1482311889",
        "ip_address": "127.0.0.1",
        "source": ".rest.v3",
        "post_price": "1.370000",
        "post_price_supplier": "0.000000",
        "priority": 32,
        "status": "Sent",
        "date_added": 1482311889,
        "_file_url": "https://rest.clicksend.com/files/77A18FEA-8935-430E-B14A-7EBF5E1E19C8AA.pdf",
        "_return_address": {
          "return_address_id": 2,
          "user_id": 1,
          "address_name": "My Home Address",
          "address_line_1": "Maritime Avenue",
          "address_line_2": "",
          "address_city": "Flynn",
          "address_state": "WA",
          "address_postal_code": "6302",
          "address_country": "AU"
        },
        "_api_username": "johndoe"
      },
      {
        "user_id": 1,
        "subaccount_id": 13,
        "list_id": null,
        "message_id": "17CD0519-4E91-4EC0-B9AF-F1BE3BC7A485",
        "message_id_supplier": "GFJKTT8CJBCYR3DFFMPPBDQJQP32",
        "address_name": "My Home Address",
        "address_line_1": "Address 1",
        "address_line_2": "",
        "address_city": "CITY",
        "address_state": "State",
        "address_postal_code": "123456",
        "address_country": "AU",
        "return_address_id": 2,
        "letter_file_name": "21837EDA-1167-4104-A4D3-4A22FA0585E4AA.pdf",
        "custom_string": null,
        "schedule": "1482311889",
        "ip_address": "127.0.0.1",
        "source": ".rest.v3",
        "post_price": "1.370000",
        "post_price_supplier": "0.000000",
        "priority": 32,
        "status": "Sent",
        "date_added": 1482311889,
        "_file_url": "https://rest.clicksend.com/files/21837EDA-1167-4104-A4D3-4A22FA0585E4A.pdf",
        "_return_address": {
          "return_address_id": 2,
          "user_id": 1,
          "address_name": "My Home Address",
          "address_line_1": "Maritime Avenue",
          "address_line_2": "",
          "address_city": "Flynn",
          "address_state": "WA",
          "address_postal_code": "6302",
          "address_country": "AU"
        },
        "_api_username": "johndoe"
      },
      {
        "user_id": 1,
        "subaccount_id": 13,
        "list_id": null,
        "message_id": "8A2DAFE7-130F-4F9A-820B-85D79F874E05",
        "message_id_supplier": "4F2JH87CP3PX22WRRYWVK8JJKXR2",
        "address_name": "My Home Address",
        "address_line_1": "Address 1",
        "address_line_2": "",
        "address_city": "CITY",
        "address_state": "State",
        "address_postal_code": "123456",
        "address_country": "AU",
        "return_address_id": 1,
        "letter_file_name": "C738FB89-750F-45E4-9E0A-EBD19A8B2884A.pdf",
        "custom_string": null,
        "schedule": "1482313126",
        "ip_address": "127.0.0.1",
        "source": ".rest.v3",
        "post_price": "1.370000",
        "post_price_supplier": "0.000000",
        "priority": 32,
        "status": "Sent",
        "date_added": 1482313126,
        "_file_url": "https://rest.clicksend.com/files/C738FB89-750F-45E4-9E0A-EBD19A8B2884A.pdf",
        "_return_address": {
          "return_address_id": 1,
          "user_id": 1,
          "address_name": "John Doe",
          "address_line_1": "3/28 Leonora St",
          "address_line_2": "",
          "address_city": "Como",
          "address_state": "WA",
          "address_postal_code": "6152",
          "address_country": "AU"
        },
        "_api_username": "johndoe"
      },
      {
        "user_id": 1,
        "subaccount_id": 13,
        "list_id": null,
        "message_id": "047CDB95-6C9D-4485-962F-EA28FFD7C0D9",
        "message_id_supplier": "MHPDXPKFJFR9H677TQM8PH4YDMHP",
        "address_name": "My Home Address",
        "address_line_1": "Address 1",
        "address_line_2": "",
        "address_city": "CITY",
        "address_state": "State",
        "address_postal_code": "123456",
        "address_country": "AU",
        "return_address_id": 1,
        "letter_file_name": "5089F9FC-0179-44E8-AC5E-225932FE9500A.pdf",
        "custom_string": null,
        "schedule": "1482313126",
        "ip_address": "127.0.0.1",
        "source": ".rest.v3",
        "post_price": "1.370000",
        "post_price_supplier": "0.000000",
        "priority": 32,
        "status": "Sent",
        "date_added": 1482313126,
        "_file_url": "https://rest.clicksend.com/files/5089F9FC-0179-44E8-AC5E-225932FE9500A.pdf",
        "_return_address": {
          "return_address_id": 1,
          "user_id": 1,
          "address_name": "John Doe",
          "address_line_1": "3/28 Leonora St",
          "address_line_2": "",
          "address_city": "Como",
          "address_state": "WA",
          "address_postal_code": "6152",
          "address_country": "AU"
        },
        "_api_username": "johndoe"
      },
      {
        "user_id": 1,
        "subaccount_id": 13,
        "list_id": null,
        "message_id": "653C5ED0-5AAD-4946-8E72-8152E23A6AA5",
        "message_id_supplier": "JYPVGC83PH68XX64QYBHQXRD4V2G",
        "address_name": "My Home Address",
        "address_line_1": "Address 1",
        "address_line_2": "",
        "address_city": "CITY",
        "address_state": "State",
        "address_postal_code": "123456",
        "address_country": "AU",
        "return_address_id": 1,
        "letter_file_name": "E17C7CE6-C2C9-476D-8886-E2B8CA6C30E3A.pdf",
        "custom_string": null,
        "schedule": "1482313126",
        "ip_address": "127.0.0.1",
        "source": ".rest.v3",
        "post_price": "1.370000",
        "post_price_supplier": "0.000000",
        "priority": 32,
        "status": "Sent",
        "date_added": 1482313126,
        "_file_url": "https://rest.clicksend.com/files/E17C7CE6-C2C9-476D-8886-E2B8CA6C30E3A.pdf",
        "_return_address": {
          "return_address_id": 1,
          "user_id": 1,
          "address_name": "John Doe",
          "address_line_1": "3/28 Leonora St",
          "address_line_2": "",
          "address_city": "Como",
          "address_state": "WA",
          "address_postal_code": "6152",
          "address_country": "AU"
        },
        "_api_username": "johndoe"
      },
      {
        "user_id": 1,
        "subaccount_id": 13,
        "list_id": null,
        "message_id": "EF4177A7-AE6D-4035-9052-10B2C9DF4564",
        "message_id_supplier": "68TC768BG42TK6Q83VBFVKY87D99",
        "address_name": "My Home Address",
        "address_line_1": "Address 1",
        "address_line_2": "",
        "address_city": "CITY",
        "address_state": "State",
        "address_postal_code": "123456",
        "address_country": "AU",
        "return_address_id": 2,
        "letter_file_name": "252678EE-C597-4D20-B1DE-F21629E77831A.pdf",
        "custom_string": null,
        "schedule": "1482313126",
        "ip_address": "127.0.0.1",
        "source": ".rest.v3",
        "post_price": "1.370000",
        "post_price_supplier": "0.000000",
        "priority": 32,
        "status": "Sent",
        "date_added": 1482313126,
        "_file_url": "https://rest.clicksend.com/files/252678EE-C597-4D20-B1DE-F21629E77831A.pdf",
        "_return_address": {
          "return_address_id": 2,
          "user_id": 1,
          "address_name": "My Home Address",
          "address_line_1": "Maritime Avenue",
          "address_line_2": "",
          "address_city": "Flynn",
          "address_state": "WA",
          "address_postal_code": "6302",
          "address_country": "AU"
        },
        "_api_username": "johndoe"
      },
      {
        "user_id": 1,
        "subaccount_id": 13,
        "list_id": null,
        "message_id": "E196E8B4-1233-4EF4-8689-C296D55B9DAE",
        "message_id_supplier": "8BF2H8CCDJMHCMCKR3THJ6XDDJ9K",
        "address_name": "My Home Address",
        "address_line_1": "Address 1",
        "address_line_2": "",
        "address_city": "CITY",
        "address_state": "State",
        "address_postal_code": "123456",
        "address_country": "AU",
        "return_address_id": 2,
        "letter_file_name": "8B2A85E1-D092-47DC-B70B-983B10AD83D6A.pdf",
        "custom_string": null,
        "schedule": "1482313126",
        "ip_address": "127.0.0.1",
        "source": ".rest.v3",
        "post_price": "1.370000",
        "post_price_supplier": "0.000000",
        "priority": 32,
        "status": "Sent",
        "date_added": 1482313126,
        "_file_url": "https://rest.clicksend.com/files/8B2A85E1-D092-47DC-B70B-983B10AD83D6A.pdf",
        "_return_address": {
          "return_address_id": 2,
          "user_id": 1,
          "address_name": "My Home Address",
          "address_line_1": "Maritime Avenue",
          "address_line_2": "",
          "address_city": "Flynn",
          "address_state": "WA",
          "address_postal_code": "6302",
          "address_country": "AU"
        },
        "_api_username": "johndoe"
      }
    ]
  }
}
```


### <a name="export_postcard_history"></a>![Endpoint: ](https://apidocs.io/img/method.png "Export Postcard History") `GET` /post/postcards/export?filename={filename}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| filename | `string` |  ``` Required ```  | Filename for the export file. | `myexport.csv` | 

#### Responses
**200** 

Body (_Export Postcard History response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Download your file here.",
  "data": {
    "url": "https://rest.clicksend.com/files/705F80D0-D044-4F85-8617-081988B398E5?filename=myexport.csv"
  }
}
```


[Back to API Reference](#api_reference)

## <a name="referral_accounts"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Referral Accounts") Referral Accounts


### <a name="get_list_of_referral_accounts"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get List of Referral Accounts") `GET` /referral/accounts

> TODO: Add a method description



#### Responses
**200** 

Body (_Get List of Referral Accounts response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are your referrals.",
  "data": {
    "total": 5,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 5,
    "data": [
      {
        "referral_rule_id": 1,
        "refered_user_id": 24,
        "date_referred": 1438260940,
        "percentage_referral": 5
      },
      {
        "referral_rule_id": 2,
        "refered_user_id": 25,
        "date_referred": 1438260989,
        "percentage_referral": 5
      },
      {
        "referral_rule_id": 3,
        "refered_user_id": 26,
        "date_referred": 1438260992,
        "percentage_referral": 5
      },
      {
        "referral_rule_id": 4,
        "refered_user_id": 27,
        "date_referred": 1438260994,
        "percentage_referral": 5
      },
      {
        "referral_rule_id": 5,
        "refered_user_id": 28,
        "date_referred": 1438260997,
        "percentage_referral": 5
      }
    ]
  }
}
```


[Back to API Reference](#api_reference)

## <a name="reseller"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Reseller") Reseller


### <a name="get_reseller_setting"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Reseller Setting") `GET` /reseller

> Get reseller setting.



#### Responses
**200** 

Body (_Get Reseller Setting response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your result.",
  "data": [
    {
      "reseller_user_id": 1,
      "allow_public_signups": 1,
      "default_margin": 10,
      "default_margin_numbers": 20,
      "trial_balance": "500.00",
      "subdomain": "subdomain",
      "colour_navigation": "#9999FF",
      "logo_url": "http://url.com"
    }
  ]
}
```


### <a name="update_reseller_setting"></a>![Endpoint: ](https://apidocs.io/img/method.png "Update Reseller Setting") `PUT` /reseller

> Update a specific reseller setting.



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `update reseller setting request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "allow_public_signups": 1,
  "default_margin": 100,
  "default_margin_numbers": 150,
  "trial_balance": 50,
  "subdomain": "subdomain",
  "colour_navigation": "#9999FF",
  "logo_url_light": "http://url.com/light",
  "logo_url_dark": "http://url.com/dark",
  "company_name": "MyCompany"
}
``` 

#### Responses
**200** 

Body (_Update Reseller Setting response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your setting has been updated.",
  "data": {
    "reseller_user_id": 1,
    "allow_public_signups": 1,
    "default_margin": 100,
    "default_margin_numbers": 150,
    "trial_balance": 50,
    "subdomain": "subdomain",
    "colour_navigation": "#9999FF",
    "logo_url_light": "http://url.com/light",
    "logo_url_dark": "http://url.com/dark",
    "company_name": "MyCompany"
  }
}
```


### <a name="reseller_by_subdomain"></a>![Endpoint: ](https://apidocs.io/img/method.png "Reseller By Subdomain") `GET` /reseller/{subdomain}

> Get reseller setting by subdomin.



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| subdomain | `string` |  ``` Required ```  | Subdomain | `mysubdomain` | 

#### Responses
**200** 

Body (_Reseller By Subdomain response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here's your result.",
  "data": {
    "reseller_user_id": 1,
    "allow_public_signups": 1,
    "colour_navigation": "#9999FF",
    "logo_url_light": "http://url.com/light",
    "logo_url_dark": "http://url.com/dark",
    "company_name": "MyCompany"
  }
}
```


[Back to API Reference](#api_reference)

## <a name="reseller_accounts"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Reseller Accounts") Reseller Accounts


### <a name="list_of_reseller_accounts"></a>![Endpoint: ](https://apidocs.io/img/method.png "List of Reseller Accounts") `GET` /reseller/accounts

> Get list of Reseller Accounts



#### Responses
**200** 

Body (_List of Reseller Accounts response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are you data.",
  "data": {
    "total": 11,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 11,
    "data": [
      {
        "user_id": 24,
        "username": "username75897",
        "user_email": "email86363@gmail.com",
        "active": 1,
        "banned": 0,
        "balance": "115.000000",
        "user_phone": "+61261063776",
        "reply_to": "originalemail",
        "delivery_to": "+61261086832",
        "user_first_name": "Firstname30529",
        "user_last_name": "Lastname83402",
        "account": 0,
        "account_name": "Johnn99YH",
        "account_billing_email": "AIYkwXgB2c@CzrJB.com",
        "account_billing_mobile": "+61353787961",
        "country": "AU",
        "default_country_sms": "AU",
        "unsubscribe_mail": 1,
        "auto_recharge": 0,
        "auto_recharge_amount": "20.00",
        "low_credit_amount": "1.50",
        "setting_unicode_sms": 1,
        "setting_beta": 1,
        "setting_email_sms_subject": 0,
        "setting_fix_sender_id": 26979,
        "setting_sms_message_char_limit": 140,
        "_currency": {
          "currency_name_short": "AUD",
          "currency_prefix_d": "$",
          "currency_prefix_c": "c",
          "currency_name_long": "Australian Dollars"
        },
        "_subaccount": {
          "subaccount_id": 54,
          "api_username": "Y3c5zm7z97",
          "email": "oNEDu5ffl8@BP8lY.com",
          "phone_number": "+61353787526",
          "first_name": "JohnNyZWy",
          "last_name": "Doe8ozHX",
          "api_key": "D683D2C1-8AAE-881A-78FF-E8577D7BED2D",
          "access_users": 1,
          "access_billing": 1,
          "access_reporting": 1,
          "access_contacts": 0,
          "access_settings": 1,
          "access_sms": 1,
          "access_email": 0,
          "access_voice": 0,
          "access_fax": 0,
          "access_post": 0,
          "access_reseller": 0
        }
      },
      {
        "user_id": 60,
        "username": "FHJatAkKXD",
        "user_email": "MEynjL6C3A@2YtIn.com",
        "active": 0,
        "banned": 0,
        "balance": "2273.435000",
        "user_phone": "+61353787971",
        "reply_to": "originalemail",
        "delivery_to": "I1hq9xrvmcNO24sf",
        "user_first_name": "JohnjRk3I",
        "user_last_name": "Doe1uWR5",
        "account": 0,
        "account_name": "JohnkMJLv",
        "account_billing_email": "fZpbUQfzE0@NQ9Nt.com",
        "account_billing_mobile": "+61353787898",
        "country": "AU",
        "default_country_sms": "AU",
        "unsubscribe_mail": 0,
        "auto_recharge": 0,
        "auto_recharge_amount": "20.00",
        "low_credit_amount": "1.50",
        "setting_unicode_sms": 0,
        "setting_beta": 0,
        "setting_email_sms_subject": 0,
        "setting_fix_sender_id": 0,
        "setting_sms_message_char_limit": 140,
        "_currency": {
          "currency_name_short": "AUD",
          "currency_prefix_d": "$",
          "currency_prefix_c": "c",
          "currency_name_long": "Australian Dollars"
        },
        "_subaccount": {
          "subaccount_id": 70,
          "api_username": "a4CQgqG4lS",
          "email": "fZpbUQfzE0@NQ9Nt.com",
          "phone_number": "+61353787898",
          "first_name": "John19k46",
          "last_name": "DoexkI6a",
          "api_key": "C9B4AFBA-BDBA-E343-950B-2C63BF6E7901",
          "access_users": 1,
          "access_billing": 1,
          "access_reporting": 1,
          "access_contacts": 0,
          "access_settings": 1,
          "access_sms": 0,
          "access_email": 0,
          "access_voice": 0,
          "access_fax": 0,
          "access_post": 0,
          "access_reseller": 0
        }
      },
      {
        "user_id": 61,
        "username": "e10GrL9GUw",
        "user_email": "eThbkhkjwi@El2xE.com",
        "active": 0,
        "banned": 0,
        "balance": "115.000000",
        "user_phone": "+61353787600",
        "reply_to": "originalemail",
        "delivery_to": "iBX9lNMRLM1Dp5QN",
        "user_first_name": "JohnTW9sV",
        "user_last_name": "DoeBQhRS",
        "account": 0,
        "account_name": "JohnwjvLq",
        "account_billing_email": "alKdHhfzXI@MvAvZ.com",
        "account_billing_mobile": "+61353787282",
        "country": "AU",
        "default_country_sms": "AU",
        "unsubscribe_mail": 0,
        "auto_recharge": 0,
        "auto_recharge_amount": "20.00",
        "low_credit_amount": "1.50",
        "setting_unicode_sms": 0,
        "setting_beta": 0,
        "setting_email_sms_subject": 0,
        "setting_fix_sender_id": 0,
        "setting_sms_message_char_limit": 140,
        "_currency": {
          "currency_name_short": "AUD",
          "currency_prefix_d": "$",
          "currency_prefix_c": "c",
          "currency_name_long": "Australian Dollars"
        },
        "_subaccount": {
          "subaccount_id": 71,
          "api_username": "zOgiEZ1TK7",
          "email": "alKdHhfzXI@MvAvZ.com",
          "phone_number": "+61353787282",
          "first_name": "JohnufkdZ",
          "last_name": "DoevmQ93",
          "api_key": "2E829F76-FB67-D2D6-637E-7DB511D98A85",
          "access_users": 1,
          "access_billing": 1,
          "access_reporting": 1,
          "access_contacts": 0,
          "access_settings": 1,
          "access_sms": 0,
          "access_email": 0,
          "access_voice": 0,
          "access_fax": 0,
          "access_post": 0,
          "access_reseller": 0
        }
      },
      {
        "user_id": 62,
        "username": "FYuLNmYf8K",
        "user_email": "J6tOUnclVo@vmAV6.com",
        "active": 0,
        "banned": 0,
        "balance": "115.000000",
        "user_phone": "+61353787970",
        "reply_to": "originalemail",
        "delivery_to": "WrDhMU4CAwsGvoBn",
        "user_first_name": "JohnsIbLF",
        "user_last_name": "DoeWhrkh",
        "account": 0,
        "account_name": "JohnCEUiT",
        "account_billing_email": "Y6Q8mpg5PM@DxhTZ.com",
        "account_billing_mobile": "+61353787685",
        "country": "AU",
        "default_country_sms": "AU",
        "unsubscribe_mail": 0,
        "auto_recharge": 0,
        "auto_recharge_amount": "20.00",
        "low_credit_amount": "1.50",
        "setting_unicode_sms": 0,
        "setting_beta": 0,
        "setting_email_sms_subject": 0,
        "setting_fix_sender_id": 8,
        "setting_sms_message_char_limit": 140,
        "_currency": {
          "currency_name_short": "AUD",
          "currency_prefix_d": "$",
          "currency_prefix_c": "c",
          "currency_name_long": "Australian Dollars"
        },
        "_subaccount": {
          "subaccount_id": 72,
          "api_username": "lDcRBjpvzc",
          "email": "Y6Q8mpg5PM@DxhTZ.com",
          "phone_number": "+61353787685",
          "first_name": "JohnpIh23",
          "last_name": "Doen7y2c",
          "api_key": "E0D3BF7C-F51A-95BF-F80C-A90C546A3AF7",
          "access_users": 1,
          "access_billing": 1,
          "access_reporting": 1,
          "access_contacts": 0,
          "access_settings": 1,
          "access_sms": 0,
          "access_email": 0,
          "access_voice": 0,
          "access_fax": 0,
          "access_post": 0,
          "access_reseller": 0
        }
      },
      {
        "user_id": 70,
        "username": "username_62220",
        "user_email": "email_96752@gmail.com",
        "active": 0,
        "banned": 0,
        "balance": "115.000000",
        "user_phone": "+61261061361",
        "reply_to": "originalemail",
        "delivery_to": null,
        "user_first_name": "Firstname6663",
        "user_last_name": "Lastname95048",
        "account": 0,
        "account_name": "Company 99550",
        "account_billing_email": "email_96752@gmail.com",
        "account_billing_mobile": "+61261061361",
        "country": "AU",
        "default_country_sms": "AU",
        "unsubscribe_mail": 0,
        "auto_recharge": 0,
        "auto_recharge_amount": "20.00",
        "low_credit_amount": "1.50",
        "setting_unicode_sms": 0,
        "setting_beta": 0,
        "setting_email_sms_subject": 0,
        "setting_fix_sender_id": 2147483647,
        "setting_sms_message_char_limit": 140,
        "_currency": {
          "currency_name_short": "AUD",
          "currency_prefix_d": "$",
          "currency_prefix_c": "c",
          "currency_name_long": "Australian Dollars"
        },
        "_subaccount": {
          "subaccount_id": 80,
          "api_username": "username_62220",
          "email": "email_96752@gmail.com",
          "phone_number": "+61261061361",
          "first_name": "Firstname6663",
          "last_name": "Lastname95048",
          "api_key": "DD87E68D-73B9-91AF-8EEE-F1D3C8FA40F5",
          "access_users": 1,
          "access_billing": 1,
          "access_reporting": 1,
          "access_contacts": 0,
          "access_settings": 1,
          "access_sms": 0,
          "access_email": 0,
          "access_voice": 0,
          "access_fax": 0,
          "access_post": 0,
          "access_reseller": 0
        }
      },
      {
        "user_id": 71,
        "username": "username_38270",
        "user_email": "email_66764@gmail.com",
        "active": 0,
        "banned": 0,
        "balance": "115.000000",
        "user_phone": "+61261063404",
        "reply_to": "originalemail",
        "delivery_to": "+61261089282",
        "user_first_name": "Firstname1371",
        "user_last_name": "Lastname50417",
        "account": 0,
        "account_name": "Company 50249",
        "account_billing_email": "email_66764@gmail.com",
        "account_billing_mobile": "+61261063404",
        "country": "AU",
        "default_country_sms": "AU",
        "unsubscribe_mail": 0,
        "auto_recharge": 0,
        "auto_recharge_amount": "20.00",
        "low_credit_amount": "1.50",
        "setting_unicode_sms": 1,
        "setting_beta": 1,
        "setting_email_sms_subject": 0,
        "setting_fix_sender_id": 2147483647,
        "setting_sms_message_char_limit": 140,
        "_currency": {
          "currency_name_short": "AUD",
          "currency_prefix_d": "$",
          "currency_prefix_c": "c",
          "currency_name_long": "Australian Dollars"
        },
        "_subaccount": {
          "subaccount_id": 81,
          "api_username": "username_38270",
          "email": "email_66764@gmail.com",
          "phone_number": "+61261063404",
          "first_name": "Firstname1371",
          "last_name": "Lastname50417",
          "api_key": "1219277F-5111-C884-DEE1-7C16681A3655",
          "access_users": 1,
          "access_billing": 1,
          "access_reporting": 1,
          "access_contacts": 0,
          "access_settings": 1,
          "access_sms": 0,
          "access_email": 0,
          "access_voice": 0,
          "access_fax": 0,
          "access_post": 0,
          "access_reseller": 0
        }
      },
      {
        "user_id": 72,
        "username": "username_39016",
        "user_email": "email_67772@gmail.com",
        "active": 1,
        "banned": 0,
        "balance": "115.000000",
        "user_phone": "+61261061316",
        "reply_to": "originalemail",
        "delivery_to": "+61261087712",
        "user_first_name": "Firstname26535",
        "user_last_name": "Lastname36882",
        "account": 0,
        "account_name": "Company 26794",
        "account_billing_email": "email_67772@gmail.com",
        "account_billing_mobile": "+61261061316",
        "country": "AU",
        "default_country_sms": "AU",
        "unsubscribe_mail": 0,
        "auto_recharge": 0,
        "auto_recharge_amount": "20.00",
        "low_credit_amount": "1.50",
        "setting_unicode_sms": 0,
        "setting_beta": 0,
        "setting_email_sms_subject": 1,
        "setting_fix_sender_id": 87404,
        "setting_sms_message_char_limit": 140,
        "_currency": {
          "currency_name_short": "AUD",
          "currency_prefix_d": "$",
          "currency_prefix_c": "c",
          "currency_name_long": "Australian Dollars"
        },
        "_subaccount": {
          "subaccount_id": 82,
          "api_username": "username_39016",
          "email": "email_67772@gmail.com",
          "phone_number": "+61261061316",
          "first_name": "Firstname26535",
          "last_name": "Lastname36882",
          "api_key": "631D0E3C-CA0A-E224-BF1B-0070FDACF775",
          "access_users": 1,
          "access_billing": 1,
          "access_reporting": 1,
          "access_contacts": 0,
          "access_settings": 1,
          "access_sms": 0,
          "access_email": 0,
          "access_voice": 0,
          "access_fax": 0,
          "access_post": 0,
          "access_reseller": 0
        }
      },
      {
        "user_id": 73,
        "username": "username_10832",
        "user_email": "email_28172@gmail.com",
        "active": 1,
        "banned": 0,
        "balance": "115.000000",
        "user_phone": "+61261064026",
        "reply_to": "originalemail",
        "delivery_to": "+61261088320",
        "user_first_name": "Firstname10383",
        "user_last_name": "Lastname11110",
        "account": 0,
        "account_name": "Company 28247",
        "account_billing_email": "email_28172@gmail.com",
        "account_billing_mobile": "+61261064026",
        "country": "AU",
        "default_country_sms": "AU",
        "unsubscribe_mail": 0,
        "auto_recharge": 0,
        "auto_recharge_amount": "20.00",
        "low_credit_amount": "1.50",
        "setting_unicode_sms": 1,
        "setting_beta": 0,
        "setting_email_sms_subject": 1,
        "setting_fix_sender_id": 67684,
        "setting_sms_message_char_limit": 140,
        "_currency": {
          "currency_name_short": "AUD",
          "currency_prefix_d": "$",
          "currency_prefix_c": "c",
          "currency_name_long": "Australian Dollars"
        },
        "_subaccount": {
          "subaccount_id": 83,
          "api_username": "username_10832",
          "email": "email_28172@gmail.com",
          "phone_number": "+61261064026",
          "first_name": "Firstname10383",
          "last_name": "Lastname11110",
          "api_key": "E236FDFF-4730-F719-85B9-2AC0D4D192F5",
          "access_users": 1,
          "access_billing": 1,
          "access_reporting": 1,
          "access_contacts": 0,
          "access_settings": 1,
          "access_sms": 0,
          "access_email": 0,
          "access_voice": 0,
          "access_fax": 0,
          "access_post": 0,
          "access_reseller": 0
        }
      },
      {
        "user_id": 74,
        "username": "username65302",
        "user_email": "email1024@gmail.com",
        "active": 1,
        "banned": 0,
        "balance": "115.000000",
        "user_phone": "+61261067753",
        "reply_to": "originalemail",
        "delivery_to": "+61261087647",
        "user_first_name": "Firstname42348",
        "user_last_name": "Lastname45055",
        "account": 0,
        "account_name": "Company88867",
        "account_billing_email": "email1024@gmail.com",
        "account_billing_mobile": "+61261067753",
        "country": "AU",
        "default_country_sms": "AU",
        "unsubscribe_mail": 1,
        "auto_recharge": 0,
        "auto_recharge_amount": "20.00",
        "low_credit_amount": "1.50",
        "setting_unicode_sms": 1,
        "setting_beta": 0,
        "setting_email_sms_subject": 1,
        "setting_fix_sender_id": 93951,
        "setting_sms_message_char_limit": 140,
        "_currency": {
          "currency_name_short": "AUD",
          "currency_prefix_d": "$",
          "currency_prefix_c": "c",
          "currency_name_long": "Australian Dollars"
        },
        "_subaccount": {
          "subaccount_id": 84,
          "api_username": "username65302",
          "email": "email1024@gmail.com",
          "phone_number": "+61261067753",
          "first_name": "Firstname42348",
          "last_name": "Lastname45055",
          "api_key": "98AE5B58-141B-1310-AC66-45D34D56CA4C",
          "access_users": 1,
          "access_billing": 1,
          "access_reporting": 1,
          "access_contacts": 0,
          "access_settings": 1,
          "access_sms": 0,
          "access_email": 0,
          "access_voice": 0,
          "access_fax": 0,
          "access_post": 0,
          "access_reseller": 0
        }
      },
      {
        "user_id": 75,
        "username": "username67428",
        "user_email": "email13820@gmail.com",
        "active": 0,
        "banned": 0,
        "balance": "115.000000",
        "user_phone": "+61261062260",
        "reply_to": "originalemail",
        "delivery_to": "+61261088951",
        "user_first_name": "Firstname70051",
        "user_last_name": "Lastname35293",
        "account": 0,
        "account_name": "Company13805",
        "account_billing_email": "email13820@gmail.com",
        "account_billing_mobile": "+61261062260",
        "country": "AU",
        "default_country_sms": "AU",
        "unsubscribe_mail": 1,
        "auto_recharge": 0,
        "auto_recharge_amount": "20.00",
        "low_credit_amount": "1.50",
        "setting_unicode_sms": 0,
        "setting_beta": 0,
        "setting_email_sms_subject": 0,
        "setting_fix_sender_id": 35625,
        "setting_sms_message_char_limit": 140,
        "_currency": {
          "currency_name_short": "AUD",
          "currency_prefix_d": "$",
          "currency_prefix_c": "c",
          "currency_name_long": "Australian Dollars"
        },
        "_subaccount": {
          "subaccount_id": 85,
          "api_username": "username67428",
          "email": "email13820@gmail.com",
          "phone_number": "+61261062260",
          "first_name": "Firstname70051",
          "last_name": "Lastname35293",
          "api_key": "C9E22A8E-88B2-0077-3445-F95A5D501FEA",
          "access_users": 1,
          "access_billing": 1,
          "access_reporting": 1,
          "access_contacts": 0,
          "access_settings": 1,
          "access_sms": 0,
          "access_email": 0,
          "access_voice": 0,
          "access_fax": 0,
          "access_post": 0,
          "access_reseller": 0
        }
      },
      {
        "user_id": 76,
        "username": "username59",
        "user_email": "email52313@gmail.com",
        "active": 0,
        "banned": 0,
        "balance": "115.000000",
        "user_phone": "+61261069962",
        "reply_to": "originalemail",
        "delivery_to": "+61261083784",
        "user_first_name": "Firstname49996",
        "user_last_name": "Lastname22152",
        "account": 0,
        "account_name": "Company23060",
        "account_billing_email": "email52313@gmail.com",
        "account_billing_mobile": "+61261069962",
        "country": "AU",
        "default_country_sms": "AU",
        "unsubscribe_mail": 1,
        "auto_recharge": 0,
        "auto_recharge_amount": "20.00",
        "low_credit_amount": "1.50",
        "setting_unicode_sms": 1,
        "setting_beta": 0,
        "setting_email_sms_subject": 0,
        "setting_fix_sender_id": 44842,
        "setting_sms_message_char_limit": 140,
        "_currency": {
          "currency_name_short": "AUD",
          "currency_prefix_d": "$",
          "currency_prefix_c": "c",
          "currency_name_long": "Australian Dollars"
        },
        "_subaccount": {
          "subaccount_id": 86,
          "api_username": "username59",
          "email": "email52313@gmail.com",
          "phone_number": "+61261069962",
          "first_name": "Firstname49996",
          "last_name": "Lastname22152",
          "api_key": "BBD918C1-DD00-FFFB-CF53-4C3AB9E15F5C",
          "access_users": 1,
          "access_billing": 1,
          "access_reporting": 1,
          "access_contacts": 0,
          "access_settings": 1,
          "access_sms": 0,
          "access_email": 0,
          "access_voice": 0,
          "access_fax": 0,
          "access_post": 0,
          "access_reseller": 0
        }
      }
    ]
  }
}
```


### <a name="get_reseller_account"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Reseller Account") `GET` /reseller/accounts/{client_user_id}

> Get a specific reseller account.



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| client_user_id | `precision` |  ``` Required ```  | The client user id. | `24` | 

#### Responses
**200** 

Body (_Get Reseller Account response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are your data.",
  "data": {
    "user_id": 24,
    "username": "username75897",
    "user_email": "email86363@gmail.com",
    "active": 1,
    "banned": 0,
    "balance": "115.000000",
    "user_phone": "+61261063776",
    "reply_to": "originalemail",
    "delivery_to": "+61261086832",
    "user_first_name": "Firstname30529",
    "user_last_name": "Lastname83402",
    "account": 0,
    "account_name": "Johnn99YH",
    "account_billing_email": "AIYkwXgB2c@CzrJB.com",
    "account_billing_mobile": "+61353787961",
    "country": "AU",
    "default_country_sms": "AU",
    "unsubscribe_mail": 1,
    "auto_recharge": 0,
    "auto_recharge_amount": "20.00",
    "low_credit_amount": "1.50",
    "setting_unicode_sms": 1,
    "setting_beta": 1,
    "setting_email_sms_subject": 0,
    "setting_fix_sender_id": 26979,
    "setting_sms_message_char_limit": 140,
    "_currency": {
      "currency_name_short": "AUD",
      "currency_prefix_d": "$",
      "currency_prefix_c": "c",
      "currency_name_long": "Australian Dollars"
    },
    "_subaccount": {
      "subaccount_id": 54,
      "api_username": "Y3c5zm7z97",
      "email": "oNEDu5ffl8@BP8lY.com",
      "phone_number": "+61353787526",
      "first_name": "JohnNyZWy",
      "last_name": "Doe8ozHX",
      "api_key": "D683D2C1-8AAE-881A-78FF-E8577D7BED2D",
      "access_users": 1,
      "access_billing": 1,
      "access_reporting": 1,
      "access_contacts": 0,
      "access_settings": 1,
      "access_sms": 1,
      "access_email": 0,
      "access_voice": 0,
      "access_fax": 0,
      "access_post": 0,
      "access_reseller": 0
    }
  }
}
```


### <a name="create_reseller_account"></a>![Endpoint: ](https://apidocs.io/img/method.png "Create Reseller Account") `POST` /reseller/accounts

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `create reseller account request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "username": "johndoe2",
  "user_email": "johndoe2@awesome.com",
  "user_phone": "518-481-1002",
  "user_first_name": "John",
  "user_last_name": "Doe",
  "country": "US",
  "password": "pass",
  "account_name": "The Awesome Company"
}
``` 

#### Responses
**200** 

Body (_Create Reseller Account response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "New reseller has been added.",
  "data": {
    "user_id": 117,
    "username": "johndoe2",
    "user_email": "johndoe2@awesome.com",
    "active": 0,
    "banned": 0,
    "balance": "0.000000",
    "user_phone": "+15184811002",
    "reply_to": "originalemail",
    "delivery_to": null,
    "user_first_name": "John",
    "user_last_name": "Doe",
    "account": 0,
    "account_name": "The Awesome Company",
    "account_billing_email": "johndoe2@awesome.com",
    "account_billing_mobile": "+15184811002",
    "country": "US",
    "default_country_sms": "US",
    "auto_recharge": 0,
    "auto_recharge_amount": "20.00",
    "low_credit_amount": "0.00",
    "setting_unicode_sms": 0,
    "setting_email_sms_subject": 0,
    "setting_fix_sender_id": 0,
    "setting_sms_message_char_limit": 6,
    "old_dashboard": 0,
    "balance_commission": "0.299954",
    "timezone": "Australia/Melbourne",
    "_currency": {
      "currency_name_short": "USD",
      "currency_prefix_d": "$",
      "currency_prefix_c": "¢",
      "currency_name_long": "US Dollars"
    },
    "_subaccount": {
      "subaccount_id": 127,
      "api_username": "johndoe2",
      "email": "johndoe2@awesome.com",
      "phone_number": "+15184811002",
      "first_name": "John",
      "last_name": "Doe",
      "api_key": "A724C6A4-1D1A-93E8-5FB8-62DC1D153CE4",
      "access_users": 1,
      "access_billing": 1,
      "access_reporting": 1,
      "access_contacts": 0,
      "access_settings": 1,
      "access_sms": 0,
      "access_email": 0,
      "access_voice": 0,
      "access_fax": 0,
      "access_post": 0,
      "access_reseller": 0
    }
  }
}
```


### <a name="create_reseller_account___public"></a>![Endpoint: ](https://apidocs.io/img/method.png "Create Reseller Account - Public") `POST` /reseller/accounts-public

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `create reseller account - public request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "reseller_user_id": 1,
  "username": "john_awesome",
  "user_email": "johnis@awesome.com",
  "user_phone": "+61261063270",
  "user_first_name": "John",
  "user_last_name": "Awesome",
  "country": "AU",
  "password": "pass",
  "account_name": "The Awesome Company"
}
``` 

#### Responses
**200** 

Body (_Create Reseller Account - Public response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "New reseller has been added.",
  "data": {
    "user_id": 130,
    "username": "john_awesome",
    "user_email": "johnis@awesome.com",
    "active": 0,
    "banned": 0,
    "balance": "0.000000",
    "user_phone": "+61261063270",
    "reply_to": "originalemail",
    "delivery_to": null,
    "user_first_name": "John",
    "user_last_name": "Awesome",
    "account": 0,
    "account_name": "The Awesome Company",
    "account_billing_email": "johnis@awesome.com",
    "account_billing_mobile": "+61261063270",
    "country": "AU",
    "default_country_sms": "AU",
    "auto_recharge": 0,
    "auto_recharge_amount": "20.00",
    "low_credit_amount": "0.00",
    "setting_unicode_sms": 0,
    "setting_email_sms_subject": 0,
    "setting_fix_sender_id": 0,
    "setting_sms_message_char_limit": 8,
    "old_dashboard": 0,
    "balance_commission": "0.299954",
    "timezone": "Australia/Melbourne",
    "_currency": {
      "currency_name_short": "AUD",
      "currency_prefix_d": "$",
      "currency_prefix_c": "c",
      "currency_name_long": "Australian Dollars"
    },
    "_subaccount": {
      "subaccount_id": 146,
      "api_username": "john_awesome",
      "email": "johnis@awesome.com",
      "phone_number": "+61261063270",
      "first_name": "John",
      "last_name": "Awesome",
      "api_key": "A144E6D3-3FF9-F3BF-4495-80AE75A0BF88",
      "access_users": 1,
      "access_billing": 1,
      "access_reporting": 1,
      "access_contacts": 0,
      "access_settings": 1,
      "access_sms": 0,
      "access_email": 0,
      "access_voice": 0,
      "access_fax": 0,
      "access_post": 0,
      "access_reseller": 0,
      "notes": null
    }
  }
}
```


### <a name="update_reseller_account"></a>![Endpoint: ](https://apidocs.io/img/method.png "Update Reseller Account") `PUT` /reseller/accounts/{client_user_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| client_user_id | `precision` |  ``` Required ```  | Your client user id. | `24` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `update reseller account request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "username": "johndoe2",
  "user_email": "johndoe2@awesome.com",
  "user_phone": "518-481-1002",
  "user_first_name": "John",
  "user_last_name": "Doe",
  "country": "US",
  "password": "pass",
  "account_name": "The Awesome Company"
}
``` 

#### Responses
**200** 

Body (_Update Reseller Account response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Reseller account has been updated.",
  "data": {
    "user_id": 117,
    "username": "johndoe2",
    "user_email": "johndoe2@awesome.com",
    "active": 0,
    "banned": 0,
    "balance": "199.997000",
    "user_phone": "518-481-1002",
    "reply_to": "originalemail",
    "delivery_to": null,
    "user_first_name": "John",
    "user_last_name": "Doe",
    "account": 0,
    "account_name": "The Awesome Company",
    "account_billing_email": "johndoe2@awesome.com",
    "account_billing_mobile": "+15184811002",
    "country": "US",
    "default_country_sms": "US",
    "auto_recharge": 0,
    "auto_recharge_amount": "20.00",
    "low_credit_amount": "0.00",
    "setting_unicode_sms": 0,
    "setting_email_sms_subject": 0,
    "setting_fix_sender_id": 0,
    "setting_sms_message_char_limit": 6,
    "old_dashboard": 0,
    "balance_commission": "0.299954",
    "timezone": "Australia/Melbourne",
    "_currency": {
      "currency_name_short": "USD",
      "currency_prefix_d": "$",
      "currency_prefix_c": "¢",
      "currency_name_long": "US Dollars"
    },
    "_subaccount": null
  }
}
```


### <a name="transfer_credit"></a>![Endpoint: ](https://apidocs.io/img/method.png "Transfer Credit") `PUT` /reseller/transfer-credit

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `transfer credit request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "client_user_id": "client_user_id",
  "balance": 244.962146072631,
  "currency": "currency"
}
``` 

#### Responses
**200** 

Body (_Transfer Credit response_) 
```
{
  "http_code": 244,
  "response_code": "response_code",
  "response_msg": "response_msg",
  "data": {}
}
```


[Back to API Reference](#api_reference)

## <a name="sdk"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "SDK") SDK


### <a name="sdk_download"></a>![Endpoint: ](https://apidocs.io/img/method.png "SDK Download") `GET` /sdk-download/{type}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| type | `string` |  ``` Required ```  | Supported types. | `cs, java, android, objectivec, angular, ruby, python, php, nodejs, go` | 

#### Responses
**200** 

Body


[Back to API Reference](#api_reference)

## <a name="search"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Search") Search


### <a name="search_contacts_lists"></a>![Endpoint: ](https://apidocs.io/img/method.png "Search Contacts-Lists") `GET` /search/contacts-lists?q={q}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| q | `string` |  ``` Required ```  | Your keyword or query. | `Gorne` | 

#### Responses
**200** 

Body (_Search Contacts-Lists response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are some search result.",
  "data": {
    "total": 2,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 2,
    "data": [
      {
        "id": 552807,
        "name": "Gorne",
        "contact": "+16783270696",
        "type": "contact",
        "contacts_count": null
      },
      {
        "id": 428,
        "name": "Gorne",
        "contact": "GHPAJCCVGMTD9BLA",
        "type": "list",
        "contacts_count": 3
      }
    ]
  }
}
```


[Back to API Reference](#api_reference)

## <a name="sms"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "SMS") SMS


### <a name="send_an_sms"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send an SMS") `POST` /sms/send

> You can post **up to 1000 messages** with each API call.



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `send an sms request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "to": "to",
  "body": "body",
  "source": "source",
  "list_id": 81.4574279642931,
  "from": "from",
  "schedule": 81.4574279642931,
  "custom_string": "custom_string",
  "country": "country",
  "from_email": "from_email"
}
``` 

#### Responses
**200** 

Body (_Send an SMS response_) 
```
{
  "http_code": 81,
  "response_code": "response_code",
  "response_msg": "response_msg",
  "data": {}
}
```


### <a name="calculate_price"></a>![Endpoint: ](https://apidocs.io/img/method.png "Calculate Price") `POST` /sms/price

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `calculate price request205` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "to": "to",
  "body": "body",
  "source": "source",
  "list_id": 81.4574279642931,
  "from": "from",
  "schedule": 81.4574279642931,
  "custom_string": "custom_string",
  "country": "country"
}
``` 

#### Responses
**200** 

Body (_Calculate Price response_) 
```
{
  "http_code": 81,
  "response_code": "response_code",
  "response_msg": "response_msg",
  "data": {}
}
```


### <a name="get_all_history"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get all History") `GET` /sms/history?date_from={date_from}&date_to={date_to}

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



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| date_from | `number` |  ``` Optional ```  | Timestamp (from) used to show records by date. | `1449459940` | 
| date_to | `number` |  ``` Optional ```  | Timestamp (to) used to show recrods by date. | `1449659940` | 

#### Responses
**200** 

Body (_Get all History response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are your data.",
  "data": {
    "total": 6,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 6,
    "data": [
      {
        "direction": "out",
        "date": "1436932432",
        "to": "+16783270696",
        "body": "Chocolate bar icing icing oat cake carrot cake jelly cotton 1iQByXxdLN.",
        "status": "Completed",
        "from": "sendlist",
        "schedule": "1436879372",
        "status_code": null,
        "status_text": null,
        "error_code": null,
        "error_text": null,
        "message_id": "4E90F4C3-43A3-489D-9AB8-DA1F4332A0C3",
        "message_parts": "1.00",
        "message_price": "0.070000",
        "from_email": null,
        "list_id": null,
        "custom_string": "this is a test",
        "contact_id": 0,
        "user_id": 1,
        "subaccount_id": 1,
        "country": "US",
        "carrier": "",
        "first_name": "John",
        "last_name": "Doe",
        "_api_username": "johndoe"
      },
      {
        "direction": "out",
        "date": "1436932432",
        "to": "+16783275492",
        "body": "Chocolate bar icing icing oat cake carrot cake jelly cotton 1iQByXxdLN.",
        "status": "Completed",
        "from": "sendlist",
        "schedule": "1436879372",
        "status_code": null,
        "status_text": null,
        "error_code": null,
        "error_text": null,
        "message_id": "7DA5EB64-29FF-4E8A-AB6B-FE945EC9B45E",
        "message_parts": "1.00",
        "message_price": "0.070000",
        "from_email": null,
        "list_id": null,
        "custom_string": "this is a test",
        "contact_id": 0,
        "user_id": 1,
        "subaccount_id": 1,
        "country": "US",
        "carrier": "",
        "first_name": "John",
        "last_name": "Doe",
        "_api_username": "johndoe"
      },
      {
        "direction": "out",
        "date": "1436932503",
        "to": "+61411111111",
        "body": "Jelly liquorice marshmallow candy carrot cake fgzOlMXuOI.",
        "status": "Completed",
        "from": "sendmobile",
        "schedule": "1436871976",
        "status_code": null,
        "status_text": null,
        "error_code": null,
        "error_text": null,
        "message_id": "064AF521-2A27-4B2A-9AB5-C45F555024EA",
        "message_parts": "1.00",
        "message_price": "0.070000",
        "from_email": null,
        "list_id": null,
        "custom_string": "this is a test",
        "contact_id": 0,
        "user_id": 1,
        "subaccount_id": 1,
        "country": "AU",
        "carrier": "Telstra",
        "_api_username": "johndoe"
      },
      {
        "direction": "out",
        "date": "1436932503",
        "to": "+61411111111",
        "body": "Chocolate bar icing icing oat cake carrot cake jelly cotton 1iQByXxdLN.",
        "status": "Completed",
        "from": "sendlist",
        "schedule": "1436879372",
        "status_code": null,
        "status_text": null,
        "error_code": null,
        "error_text": null,
        "message_id": "25DD465D-2286-45AF-AE25-D7AB36587B57",
        "message_parts": "1.00",
        "message_price": "0.070000",
        "from_email": null,
        "list_id": null,
        "custom_string": "this is a test",
        "contact_id": 0,
        "user_id": 1,
        "subaccount_id": 1,
        "country": "AU",
        "carrier": "Telstra",
        "_api_username": "johndoe"
      },
      {
        "direction": "out",
        "date": "1436932503",
        "to": "+16783270696",
        "body": "Chocolate bar icing icing oat cake carrot cake jelly cotton 1iQByXxdLN.",
        "status": "Completed",
        "from": "sendlist",
        "schedule": "1436879372",
        "status_code": null,
        "status_text": null,
        "error_code": null,
        "error_text": null,
        "message_id": "CBC8FCF2-78B2-4C7B-ABFB-76B7AC5CB558",
        "message_parts": "1.00",
        "message_price": "0.070000",
        "from_email": null,
        "list_id": null,
        "custom_string": "this is a test",
        "contact_id": 0,
        "user_id": 1,
        "subaccount_id": 1,
        "country": "US",
        "carrier": "",
        "first_name": "John",
        "last_name": "Doe",
        "_api_username": "johndoe"
      },
      {
        "direction": "out",
        "date": "1436932503",
        "to": "+16783275492",
        "body": "Chocolate bar icing icing oat cake carrot cake jelly cotton 1iQByXxdLN.",
        "status": "Completed",
        "from": "sendlist",
        "schedule": "1436879372",
        "status_code": null,
        "status_text": null,
        "error_code": null,
        "error_text": null,
        "message_id": "39266530-5430-44AA-B620-FDFC7D4A9184",
        "message_parts": "1.00",
        "message_price": "0.070000",
        "from_email": null,
        "list_id": null,
        "custom_string": "this is a test",
        "contact_id": 0,
        "user_id": 1,
        "subaccount_id": 1,
        "country": "US",
        "carrier": "",
        "first_name": "John",
        "last_name": "Doe",
        "_api_username": "johndoe"
      }
    ]
  }
}
```


### <a name="export_sms_history"></a>![Endpoint: ](https://apidocs.io/img/method.png "Export SMS History") `GET` /sms/history/export

> TODO: Add a method description



#### Responses
**200** 

Body (_Export SMS History response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Download your file here.",
  "data": {
    "url": "https://rest.clicksend.com/files/811F1369-B602-4526-A70C-C9951EC49272"
  }
}
```


### <a name="get_all_delivery_receipts"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get all Delivery Receipts") `GET` /sms/receipts

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



#### Responses
**200** 

Body (_Get all Delivery Receipts response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are your delivery receipts.",
  "data": {
    "total": 3,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 3,
    "data": [
      {
        "timestamp_send": "1442381791",
        "timestamp": "1442381791",
        "message_id": "31BC271B-1E0C-45F6-9E7E-97186C46BB82",
        "status_code": "201",
        "status_text": "Success: Message received on handset.",
        "error_code": null,
        "error_text": null,
        "custom_string": null,
        "_message_type": "sms"
      },
      {
        "timestamp_send": "1442381829",
        "timestamp": "1442381829",
        "message_id": "23C8ADA3-FD8B-420B-801A-F829BB87AC6F",
        "status_code": "201",
        "status_text": "Success: Message received on handset.",
        "error_code": null,
        "error_text": null,
        "custom_string": null,
        "_message_type": "sms"
      },
      {
        "timestamp_send": "1442381861",
        "timestamp": "1442381861",
        "message_id": "3BD22FAD-A5D3-4D99-B4C0-16BF65BE052C",
        "status_code": "201",
        "status_text": "Success: Message received on handset.",
        "error_code": null,
        "error_text": null,
        "custom_string": null,
        "_message_type": "sms"
      }
    ]
  }
}
```


### <a name="get_a_specific_delivery_receipt"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get a Specific Delivery Receipt") `GET` /sms/receipts/{message_id}

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



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| message_id | `string` |  ``` Required ```  | Your message id. | `88AB118E EB1B 478C 98CE 6C73ABA23F67` | 

#### Responses
**200** 

Body (_Get a Specific Delivery Receipt response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your receipt.",
  "data": {
    "timestamp_send": "1450854013",
    "timestamp": "1451200622",
    "message_id": "88AB118E-EB1B-478C-98CE-6C73ABA23F67",
    "status_code": "Completed",
    "status_text": "statustext",
    "error_code": "errorcode",
    "error_text": "errortext",
    "custom_string": "",
    "message_type": "sms"
  }
}
```


### <a name="add_a_test_delivery_receipt"></a>![Endpoint: ](https://apidocs.io/img/method.png "Add a Test Delivery Receipt") `POST` /sms/receipts

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



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `add a test delivery receipt request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "url": "http://yourUrl.com"
}
``` 

#### Responses
**200** 

Body (_Add a Test Delivery Receipt response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Receipt has been added",
  "data": {
    "timestamp": "1441958441",
    "message_id": "493FFB41-9733-4641-985F-BD79A067B58F",
    "status_code": "201",
    "status_text": "Success: Message received on handset.",
    "error_code": null,
    "error_text": null,
    "custom_string": null
  }
}
```


### <a name="mark_delivery_receipts_as_read"></a>![Endpoint: ](https://apidocs.io/img/method.png "Mark Delivery Receipts as read") `PUT` /sms/receipts-read

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



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `mark delivery receipts as read request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "date_before": 1441958441
}
``` 

#### Responses
**200** 

Body (_Mark Delivery Receipts as read response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Receipts has been marked as read.",
  "data": []
}
```


### <a name="get_all_inbound_sms___pull"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get all Inbound SMS - Pull") `GET` /sms/inbound

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



#### Responses
**200** 

Body (_Get all Inbound SMS - Pull response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are your data.",
  "data": {
    "total": 3,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 3,
    "data": [
      {
        "timestamp": "1436174407",
        "from": "+61411111111",
        "body": "Liquorice sweet roll fruitcake gummies. ",
        "original_body": "Liquorice sweet roll fruitcake gummies. ",
        "original_message_id": "C557B56E-83C0-4070-A74C-9BF05474B418",
        "to": "SC557B56E-83C0-4070-A74C-9BF05474B418",
        "custom_string": "22PKU978RF",
        "message_id": "C557B56E-83C0-4070-A74C-9BF05474B418",
        "_keyword": "liquorice"
      },
      {
        "timestamp": "1436174406",
        "from": "Lemon drops brownie pie chocolate bar pie swe",
        "body": "Lemon drops brownie pie chocolate bar pie sweet jelly-o chocolate.",
        "original_body": "Lemon drops brownie pie chocolate bar pie sweet jelly-o chocolate.",
        "original_message_id": "373F7121-8089-42FA-8F5C-8F8F7C18DFAA",
        "to": "S373F7121-8089-42FA-8F5C-8F8F7C18DFAA",
        "custom_string": "2ATQKLETYX",
        "message_id": "C557B56E-83C0-4070-A74C-9BF05474B418",
        "_keyword": "lemon"
      },
      {
        "timestamp": "1436174405",
        "from": "Jelly beans jelly cupcake bear claw gummies.",
        "body": "Jelly beans jelly cupcake bear claw gummies.",
        "original_body": "Jelly beans jelly cupcake bear claw gummies.",
        "original_message_id": "A9F3863C-D88E-4A54-BEF1-BD73A6E42E2E",
        "to": "SA9F3863C-D88E-4A54-BEF1-BD73A6E42E2E",
        "custom_string": "0PZCOGJP0A",
        "message_id": "C557B56E-83C0-4070-A74C-9BF05474B418",
        "_keyword": "jelly"
      }
    ]
  }
}
```


### <a name="get_specific_inbound___pull"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Specific Inbound - Pull") `GET` /sms/inbound/{message_id}

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



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| message_id | `string` |  ``` Required ```  | Message ID. Must be a valid GUID. | `5D420421-8715-4461-A9A2-C8F569E41835` | 

#### Responses
**200** 

Body (_Get Specific Inbound - Pull response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here's your result.",
  "data": {
    "timestamp": "1457947468",
    "from": "+61410926433",
    "body": "This is a test incoming SMS. IWXTUW9DCH.",
    "original_body": "This is the original message. 0CSO0ITKJM.",
    "original_message_id": "5D420421-8715-4461-A9A2-C8F569E41835",
    "to": "+61411111111",
    "custom_string": "custom_string",
    "message_id": "C557B56E-83C0-4070-A74C-9BF05474B418",
    "_keyword": "this"
  }
}
```


### <a name="add_a_test_inbound_sms"></a>![Endpoint: ](https://apidocs.io/img/method.png "Add a Test Inbound SMS") `POST` /sms/inbound

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



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `add a test inbound sms request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "url": "http://yourUrl.com"
}
``` 

#### Responses
**200** 

Body (_Add a Test Inbound SMS response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are your incoming messages.",
  "data": {
    "timestamp": "1442398236",
    "from": "+61468460249",
    "body": "This is a test incoming SMS. 5IHHOWWZTB.",
    "original_body": "This is the original message. AA4NN45X7J.",
    "original_message_id": "F35B6DF1-0C9E-488F-954E-2F603B6192F5",
    "to": "+61411111111",
    "custom_string": null,
    "message_id": "C557B56E-83C0-4070-A74C-9BF05474B418",
    "_keyword": "this"
  }
}
```


### <a name="mark_a_specific_inbound_sms_as_read"></a>![Endpoint: ](https://apidocs.io/img/method.png "Mark a specific Inbound SMS as read") `PUT` /sms/inbound-read/{message_id}

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



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| message_id | `string` |  ``` Required ```  | B7CE432193CD-0753597B7293 (string, required) - The message ID you want to mark as read. | `307EF035` | 

#### Responses
**200** 

Body (_Mark a specific Inbound SMS as read response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Inbound messages have been marked as read.",
  "data": []
}
```


### <a name="mark_all_inbound_sms_as_read"></a>![Endpoint: ](https://apidocs.io/img/method.png "Mark all Inbound SMS as read") `PUT` /sms/inbound-read

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



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `mark all inbound sms as read request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "date_before": 1442398100
}
``` 

#### Responses
**200** 

Body (_Mark all Inbound SMS as read response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Inbound messages have been marked as read.",
  "data": []
}
```


### <a name="cancel_a_scheduled_message"></a>![Endpoint: ](https://apidocs.io/img/method.png "Cancel a Scheduled Message") `PUT` /sms/{message_id}/cancel

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| message_id | `string` |  ``` Required ```  | B7CE432193CD-0753597B7293 (string, required) - The message ID you want to cancel. | `307EF035` | 

#### Responses
**200** 

Body (_Cancel a Scheduled Message response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Message 307EF035-B7CE-4321-93CD-0753597B7293 has been cancelled.",
  "data": []
}
```


### <a name="cancel_all_scheduled_messages"></a>![Endpoint: ](https://apidocs.io/img/method.png "Cancel all Scheduled Messages") `PUT` /sms/cancel-all

> TODO: Add a method description



#### Responses
**200** 

Body (_Cancel all Scheduled Messages response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "5 messages has been cancelled.",
  "data": {
    "count": 5
  }
}
```


[Back to API Reference](#api_reference)

## <a name="sms_campaigns"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "SMS Campaigns") SMS Campaigns


### <a name="create_sms_campaign"></a>![Endpoint: ](https://apidocs.io/img/method.png "Create SMS Campaign") `POST` /sms-campaigns/send

> You can post to a list with **up to 20000 recipients** with each API call.



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `create sms campaign request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "list_id": 428,
  "name": "My Campaign 1",
  "from": "+61353787448",
  "body": "This is my new campaign message.",
  "schedule": 1444821615
}
``` 

#### Responses
**200** 

Body (_Create SMS Campaign response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your new campaign has been added.",
  "data": {
    "sms_campaign_id": 7,
    "name": "My Campaign 1",
    "user_id": 1,
    "subaccount_id": 1,
    "list_id": 428,
    "from": "+61353787448",
    "body": "This is my new campaign message.",
    "schedule": "1444821615",
    "status": "Queued",
    "date_added": "1444962630",
    "ip_address": "192.168.10.1",
    "custom_string": null,
    "source": null
  }
}
```


### <a name="calculate_price_for_sms_campaign"></a>![Endpoint: ](https://apidocs.io/img/method.png "Calculate Price for SMS Campaign") `POST` /sms-campaigns/price

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `calculate price for sms campaign request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "list_id": 428,
  "name": "My Campaign 1",
  "from": "+61353787448",
  "body": "(First Name), this is your new campaign message."
}
``` 

#### Responses
**200** 

Body (_Calculate Price for SMS Campaign response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here is your price for your SMS Campaign.",
  "data": {
    "total_count": 1,
    "total_price": "0.035",
    "data": {
      "from": "+61353787448",
      "body": "John, this is your new campaign message.",
      "schedule": 1444381346
    },
    "currency": {
      "currency_name_short": "GBP",
      "currency_prefix_d": "£",
      "currency_prefix_c": "p",
      "currency_name_long": "British Pounds"
    }
  }
}
```


### <a name="update_an_sms_campaign"></a>![Endpoint: ](https://apidocs.io/img/method.png "Update an SMS Campaign") `PUT` /sms-campaigns/{sms_campaign_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| sms_campaign_id | `precision` |  ``` Required ```  | Your SMS Campaign id. | `1` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `update an sms campaign request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "list_id": 428,
  "name": "Awesome campaign.",
  "from": "+61353787447",
  "body": "his is an awesome message.",
  "schedule": 1444821615
}
``` 

#### Responses
**200** 

Body (_Update an SMS Campaign response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your SMS Campaign has been updated.",
  "data": {
    "sms_campaign_id": 1,
    "name": "Awesome campaign.",
    "user_id": 1,
    "subaccount_id": 1,
    "list_id": 428,
    "from": "+61353787447",
    "body": "This is an awesome message.",
    "schedule": "1444821615",
    "status": "Queued",
    "date_added": "1444962803",
    "ip_address": "192.168.10.1",
    "custom_string": null,
    "source": null
  }
}
```


### <a name="get_sms_campaign"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get SMS Campaign") `GET` /sms-campaigns/{sms_campaign_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| sms_campaign_id | `precision` |  ``` Required ```  | Your SMS campaign id. | `1` | 

#### Responses
**200** 

Body (_Get SMS Campaign response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your SMS Campaign.",
  "data": {
    "sms_campaign_id": 2,
    "name": "My Campaign 1",
    "user_id": 1,
    "subaccount_id": 1,
    "list_id": 428,
    "from": "+61353787448",
    "body": "This is my new campaign message.",
    "schedule": "1444821615",
    "status": "Sent",
    "date_added": "1444882068",
    "ip_address": "192.168.10.1",
    "custom_string": null,
    "source": null,
    "_total_count": 10
  }
}
```


### <a name="cancel_an_sms_campaign"></a>![Endpoint: ](https://apidocs.io/img/method.png "Cancel an SMS Campaign") `PUT` /sms-campaigns/{sms_campaign_id}/cancel

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| sms_campaign_id | `precision` |  ``` Required ```  | Your SMS Campaign id. | `1` | 

#### Responses
**200** 

Body (_Cancel an SMS Campaign response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your SMS Campaign has been cancelled.",
  "data": {
    "sms_campaign_id": 1,
    "name": "Awesome campaign.",
    "user_id": 1,
    "subaccount_id": 1,
    "list_id": 428,
    "from": "+61353787447",
    "body": "This is an awesome message.",
    "schedule": "1444821615",
    "status": "Cancelled",
    "date_added": "1444959876",
    "ip_address": "192.168.10.1",
    "custom_string": null,
    "source": null
  }
}
```


### <a name="get_list_of_sms_campaigns"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get list of SMS Campaigns") `GET` /sms-campaigns

> TODO: Add a method description



#### Responses
**200** 

Body (_Get list of SMS Campaigns response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are your SMS campaigns.",
  "data": {
    "total": 7,
    "per_page": 20,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 7,
    "data": [
      {
        "sms_campaign_id": 1,
        "name": "This is my awesome campaign.",
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": 428,
        "from": "+61353787447",
        "body": "This is my new campaign message.",
        "schedule": "1444821615",
        "status": "Cancelled",
        "date_added": "1444962803",
        "ip_address": "192.168.10.1",
        "custom_string": null,
        "source": null,
        "_total_count": 10
      },
      {
        "sms_campaign_id": 7,
        "name": "My Campaign 1",
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": 428,
        "from": "+61353787448",
        "body": "This is my new campaign message.",
        "schedule": "1444821615",
        "status": "Queued",
        "date_added": "1444962630",
        "ip_address": "192.168.10.1",
        "custom_string": null,
        "source": null,
        "_total_count": 10
      },
      {
        "sms_campaign_id": 6,
        "name": "My Campaign 1",
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": 428,
        "from": "+61353787448",
        "body": "This is my new campaign message.",
        "schedule": "1444821615",
        "status": "Queued",
        "date_added": "1444893067",
        "ip_address": "192.168.10.1",
        "custom_string": null,
        "source": null,
        "_total_count": 10
      },
      {
        "sms_campaign_id": 5,
        "name": "My Campaign 1",
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": 428,
        "from": "+61353787448",
        "body": "This is my new campaign message.",
        "schedule": "1444821615",
        "status": "Sent",
        "date_added": "1444891837",
        "ip_address": "192.168.10.1",
        "custom_string": null,
        "source": null,
        "_total_count": 10
      },
      {
        "sms_campaign_id": 4,
        "name": "My Campaign 1",
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": 428,
        "from": "+61353787448",
        "body": "This is my new campaign message.",
        "schedule": "1444821615",
        "status": "Sent",
        "date_added": "1444888498",
        "ip_address": "192.168.10.1",
        "custom_string": null,
        "source": null,
        "_total_count": 10
      },
      {
        "sms_campaign_id": 3,
        "name": "My Campaign 1",
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": 428,
        "from": "+61353787448",
        "body": "This is my new campaign message.",
        "schedule": "1444821615",
        "status": "Sent",
        "date_added": "1444882130",
        "ip_address": "192.168.10.1",
        "custom_string": null,
        "source": null,
        "_total_count": 10
      },
      {
        "sms_campaign_id": 2,
        "name": "My Campaign 1",
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": 428,
        "from": "+61353787448",
        "body": "This is my new campaign message.",
        "schedule": "1444821615",
        "status": "Sent",
        "date_added": "1444882068",
        "ip_address": "192.168.10.1",
        "custom_string": null,
        "source": null,
        "_total_count": 10
      }
    ]
  }
}
```


[Back to API Reference](#api_reference)

## <a name="sms_templates"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "SMS Templates") SMS Templates


### <a name="list_of_templates"></a>![Endpoint: ](https://apidocs.io/img/method.png "List of Templates") `GET` /sms/templates

> Get list of templates.



#### Responses
**200** 

Body (_List of Templates response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are your data.",
  "data": {
    "total": 10,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 10,
    "data": [
      {
        "template_id": 1,
        "body": "This is a sample template.",
        "template_name": "My Awesome Template"
      },
      {
        "template_id": 2,
        "body": "This is a sample template.",
        "template_name": "My Awesome Template"
      },
      {
        "template_id": 3,
        "body": "This is a sample template.",
        "template_name": "My Awesome Template"
      },
      {
        "template_id": 4,
        "body": "This is a sample template.",
        "template_name": "My Awesome Template"
      },
      {
        "template_id": 5,
        "body": "This is a sample template.",
        "template_name": "My Awesome Template"
      },
      {
        "template_id": 6,
        "body": "This is a sample template.",
        "template_name": "My Awesome Template"
      },
      {
        "template_id": 7,
        "body": "This is a sample template.",
        "template_name": "My Awesome Template"
      },
      {
        "template_id": 8,
        "body": "This is a sample template.",
        "template_name": "My Awesome Template"
      },
      {
        "template_id": 9,
        "body": "This is a sample template.",
        "template_name": "My Awesome Template"
      },
      {
        "template_id": 10,
        "body": "This is a sample template.",
        "template_name": "My Awesome Template"
      }
    ]
  }
}
```


### <a name="create_a_template"></a>![Endpoint: ](https://apidocs.io/img/method.png "Create a Template") `POST` /sms/templates

> Create new template.



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `create a template request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "template_name": "Template 501916",
  "body": "This is a sample content: H7YI68B3yk for this template."
}
``` 

#### Responses
**200** 

Body (_Create a Template response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "New template has been saved.",
  "data": {
    "template_id": 25,
    "body": "This is a sample content: H7YI68B3yk for this template.",
    "template_name": "Template 501916"
  }
}
```


### <a name="update_a_template"></a>![Endpoint: ](https://apidocs.io/img/method.png "Update a Template") `PUT` /sms/templates/{template_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| template_id | `string` |  ``` Required ```  | Your template id. | `25` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `update a template request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "template_name": "I am updated",
  "body": "This is a sample content: Sc0KNWgSMG for this template."
}
``` 

#### Responses
**200** 

Body (_Update a Template response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your template has been updated.",
  "data": {
    "template_id": 25,
    "body": "This is a sample content: Sc0KNWgSMG for this template.",
    "template_name": "I am updated"
  }
}
```


### <a name="delete_a_template"></a>![Endpoint: ](https://apidocs.io/img/method.png "Delete a Template") `DELETE` /sms/templates/{template_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| template_id | `string` |  ``` Required ```  | Your template id. | `25` | 

#### Responses
**200** 

Body (_Delete a Template response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your template has been deleted.",
  "data": []
}
```


[Back to API Reference](#api_reference)

## <a name="statistics"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Statistics") Statistics


### <a name="get_sms_statistics"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get SMS Statistics") `GET` /statistics/sms

> TODO: Add a method description



#### Responses
**200** 

Body (_Get SMS Statistics response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are your data.",
  "data": {
    "total": {
      "outbound": {
        "count": 132,
        "price": 9.24
      },
      "inbound": {
        "count": 0
      },
      "bounced": {
        "count": 0
      }
    },
    "stat": [
      {
        "date": 1434412800,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1434499200,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1434585600,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1434672000,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1434758400,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1434844800,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1434931200,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1435017600,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1435104000,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1435190400,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1435276800,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1435363200,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1435449600,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1435536000,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1435622400,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1435708800,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1435795200,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1435881600,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1435968000,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1436054400,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1436140800,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1436227200,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1436313600,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1436400000,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1436486400,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1436572800,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1436659200,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1436745600,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1436832000,
        "outbound": {
          "count": 49,
          "price": 3.43
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1436918400,
        "outbound": {
          "count": 83,
          "price": 5.81
        },
        "inbound": {
          "count": 0
        },
        "bounced": {
          "count": 0
        }
      }
    ],
    "currency": {
      "currency_name_short": "AUD",
      "currency_prefix_d": "$",
      "currency_prefix_c": "c",
      "currency_name_long": "Australian Dollars"
    }
  }
}
```


### <a name="get_voice_statistics"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Voice Statistics") `GET` /statistics/voice

> TODO: Add a method description



#### Responses
**200** 

Body (_Get Voice Statistics response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are your statistics.",
  "data": {
    "total": {
      "outbound": {
        "count": 4,
        "price": 0.6600252
      },
      "bounced": {
        "count": 0
      }
    },
    "stats": [
      {
        "date": 1441065600,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1441152000,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1441238400,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1441324800,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1441411200,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1441497600,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1441584000,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1441670400,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1441756800,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1441843200,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1441929600,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1442016000,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1442102400,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1442188800,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1442275200,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1442361600,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1442448000,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1442534400,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1442620800,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1442707200,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1442793600,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1442880000,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1442966400,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1443052800,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1443139200,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1443225600,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1443312000,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1443398400,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1443484800,
        "outbound": {
          "count": 4,
          "price": 0.6600252
        },
        "bounced": {
          "count": 0
        }
      },
      {
        "date": 1443571200,
        "outbound": {
          "count": 0,
          "price": 0
        },
        "bounced": {
          "count": 0
        }
      }
    ],
    "currency": {
      "currency_name_short": "USD",
      "currency_prefix_d": "$",
      "currency_prefix_c": "¢",
      "currency_name_long": "US Dollars"
    }
  }
}
```


[Back to API Reference](#api_reference)

## <a name="subaccounts"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Subaccounts") Subaccounts


### <a name="get_all_subaccounts"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get all Subaccounts") `GET` /subaccounts

> TODO: Add a method description



#### Responses
**200** 

Body (_Get all Subaccounts response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "SUCCESS",
  "data": {
    "total": 8,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 8,
    "data": [
      {
        "subaccount_id": 1,
        "api_username": "johndoe",
        "email": "john@doe.com",
        "phone_number": "+13523944199",
        "first_name": "John",
        "last_name": "Doe",
        "api_key": "E72D09F6-AC80-0A5C-F7F0-1A244A377A5C",
        "access_users": 1,
        "access_billing": 1,
        "access_reporting": 1,
        "access_contacts": 1,
        "access_settings": 1,
        "access_sms": 1,
        "access_email": 1,
        "access_voice": 1,
        "access_fax": 1,
        "access_post": 1,
        "access_reseller": 1,
        "access_mms": 1,
        "share_campaigns": 0,
        "notes": null
      },
      {
        "subaccount_id": 27,
        "api_username": "name9Fb",
        "email": "testvT9@gmail.com",
        "phone_number": "+19417516953",
        "first_name": "Firstname7JiPG",
        "last_name": "Lastname2olB1",
        "api_key": "B7825E96-6A67-1275-0F35-8DB8AC743B2C",
        "access_users": 1,
        "access_billing": 1,
        "access_reporting": 1,
        "access_contacts": 1,
        "access_settings": 1,
        "access_sms": 1,
        "access_email": 1,
        "access_voice": 1,
        "access_fax": 1,
        "access_post": 1,
        "access_reseller": 1,
        "access_mms": 1,
        "share_campaigns": 0,
        "notes": null
      },
      {
        "subaccount_id": 28,
        "api_username": "nameLXD",
        "email": "testIiq@gmail.com",
        "phone_number": "+19417519130",
        "first_name": "FirstnameSA3tA",
        "last_name": "Lastname22Pam",
        "api_key": "D09BA7BC-546A-C951-6D3D-DAE3FEE6D848",
        "access_users": 1,
        "access_billing": 1,
        "access_reporting": 1,
        "access_contacts": 1,
        "access_settings": 1,
        "access_sms": 1,
        "access_email": 1,
        "access_voice": 1,
        "access_fax": 1,
        "access_post": 1,
        "access_reseller": 1,
        "access_mms": 1,
        "share_campaigns": 0,
        "notes": null
      },
      {
        "subaccount_id": 29,
        "api_username": "nameh7m",
        "email": "testxQv.updated@gmail.com",
        "phone_number": "+19417519640",
        "first_name": "Firstname5dgZw Updated",
        "last_name": "Lastname0voRd Updated",
        "api_key": "9415E584-794E-4F90-699D-7ECEF7290E51",
        "access_users": 1,
        "access_billing": 1,
        "access_reporting": 1,
        "access_contacts": 1,
        "access_settings": 1,
        "access_sms": 1,
        "access_email": 1,
        "access_voice": 1,
        "access_fax": 1,
        "access_post": 1,
        "access_reseller": 1,
        "access_mms": 1,
        "share_campaigns": 0,
        "notes": null
      },
      {
        "subaccount_id": 30,
        "api_username": "name5XC",
        "email": "testaLj.updated@gmail.com",
        "phone_number": "+19417514461",
        "first_name": "FirstnameZcMSS Updated",
        "last_name": "LastnameDLmEB Updated",
        "api_key": "6E1491FC-797E-3011-1274-595EAFDE06EE",
        "access_users": 1,
        "access_billing": 1,
        "access_reporting": 1,
        "access_contacts": 1,
        "access_settings": 1,
        "access_sms": 1,
        "access_email": 1,
        "access_voice": 1,
        "access_fax": 1,
        "access_post": 1,
        "access_reseller": 1,
        "access_mms": 1,
        "share_campaigns": 0,
        "notes": null
      },
      {
        "subaccount_id": 47,
        "api_username": "franklinew5",
        "email": "frank@test.com",
        "phone_number": "+13108147982",
        "first_name": "John",
        "last_name": "Doe",
        "api_key": "2C3B97DD-6C61-94BF-7886-9CA11DF550AF",
        "access_users": 1,
        "access_billing": 1,
        "access_reporting": 1,
        "access_contacts": 1,
        "access_settings": 1,
        "access_sms": 1,
        "access_email": 1,
        "access_voice": 1,
        "access_fax": 1,
        "access_post": 1,
        "access_reseller": 1,
        "access_mms": 1,
        "share_campaigns": 0,
        "notes": null
      },
      {
        "subaccount_id": 48,
        "api_username": "franklinew6",
        "email": "frank@test.com",
        "phone_number": "+13108147982",
        "first_name": "John",
        "last_name": "Doe",
        "api_key": "DE5F8C8F-E939-941B-C9E0-2BD542C3FFE3",
        "access_users": 1,
        "access_billing": 1,
        "access_reporting": 1,
        "access_contacts": 1,
        "access_settings": 1,
        "access_sms": 1,
        "access_email": 1,
        "access_voice": 1,
        "access_fax": 1,
        "access_post": 1,
        "access_reseller": 1,
        "access_mms": 1,
        "share_campaigns": 0,
        "notes": null
      },
      {
        "subaccount_id": 49,
        "api_username": "franklinew7",
        "email": "frank@test.com",
        "phone_number": "+13108147982",
        "first_name": "John",
        "last_name": "Doe",
        "api_key": "6279E8E9-8D02-72AE-9824-BF7C0C2E4FE7",
        "access_users": 1,
        "access_billing": 1,
        "access_reporting": 1,
        "access_contacts": 1,
        "access_settings": 1,
        "access_sms": 0,
        "access_email": 0,
        "access_voice": 0,
        "access_fax": 0,
        "access_post": 0,
        "access_reseller": 0,
        "access_mms": 0,
        "share_campaigns": 0,
        "notes": null
      }
    ]
  }
}
```


### <a name="create_a_new_subaccount"></a>![Endpoint: ](https://apidocs.io/img/method.png "Create a new subaccount") `POST` /subaccounts

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `create a new subaccount request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "api_username": "nameP99",
  "password": "pass",
  "email": "testvrq@gmail.com",
  "phone_number": "941-751-3278",
  "first_name": "FirstnameeGPqV",
  "last_name": "LastnamePvjJp"
}
``` 

#### Responses
**200** 

Body (_Create a new subaccount response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "New account has been created.",
  "data": {
    "subaccount_id": 59,
    "api_username": "nameP99",
    "email": "testvrq@gmail.com",
    "phone_number": "+619417513278",
    "first_name": "FirstnameeGPqV",
    "last_name": "LastnamePvjJp",
    "api_key": "367C506E-FBCA-1EDA-E8E0-1384F9F196D5",
    "access_users": 1,
    "access_billing": 1,
    "access_reporting": 1,
    "access_contacts": 1,
    "access_settings": 1,
    "access_sms": 1,
    "access_email": 1,
    "access_voice": 1,
    "access_fax": 1,
    "access_post": 1,
    "access_reseller": 1,
    "access_mms": 1,
    "share_campaigns": 0,
    "notes": null
  }
}
```


### <a name="get_a_specific_subaccount"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get a specific subaccount") `GET` /subaccounts/{subaccount_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| subaccount_id | `precision` |  ``` Required ```  | The subaccount ID you want to access. | `59` | 

#### Responses
**200** 

Body (_Get a specific subaccount response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are your data.",
  "data": {
    "subaccount_id": 59,
    "api_username": "nameP99",
    "email": "testvrq@gmail.com",
    "phone_number": "+619417513278",
    "first_name": "FirstnameeGPqV",
    "last_name": "LastnamePvjJp",
    "api_key": "367C506E-FBCA-1EDA-E8E0-1384F9F196D5",
    "access_users": 1,
    "access_billing": 1,
    "access_reporting": 1,
    "access_contacts": 1,
    "access_settings": 1,
    "access_sms": 1,
    "access_email": 1,
    "access_voice": 1,
    "access_fax": 1,
    "access_post": 1,
    "access_reseller": 1,
    "access_mms": 1,
    "share_campaigns": 0,
    "notes": null
  }
}
```


### <a name="update_a_specific_subaccount"></a>![Endpoint: ](https://apidocs.io/img/method.png "Update a specific subaccount") `PUT` /subaccounts/{subaccount_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| subaccount_id | `precision` |  ``` Required ```  | The subaccount ID you want to access. | `59` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `update a specific subaccount request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "password": "pass",
  "email": "testfP0.updated@gmail.com",
  "phone_number": "+19417519130",
  "first_name": "FirstnameKvdRZUpdated",
  "last_name": "LastnameHUPYGUpdated",
  "access_users": 1,
  "access_billing": 1,
  "access_reporting": 1,
  "access_contacts": 1,
  "access_settings": 1,
  "access_sms": 1,
  "access_email": 1,
  "access_voice": 1,
  "access_fax": 1,
  "access_post": 1,
  "access_reseller": 1,
  "access_mms": 1,
  "share_campaigns": 0,
  "notes": null
}
``` 

#### Responses
**200** 

Body (_Update a specific subaccount response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Subaccount #59 has been updated.",
  "data": {
    "subaccount_id": 59,
    "api_username": "nameP99",
    "email": "testfP0.updated@gmail.com",
    "phone_number": "+619417513065",
    "first_name": "FirstnameKvdRZ Updated",
    "last_name": "LastnameHUPYG Updated",
    "api_key": "367C506E-FBCA-1EDA-E8E0-1384F9F196D5",
    "access_users": 1,
    "access_billing": 1,
    "access_reporting": 1,
    "access_contacts": 1,
    "access_settings": 1,
    "access_sms": 1,
    "access_email": 1,
    "access_voice": 1,
    "access_fax": 1,
    "access_post": 1,
    "access_reseller": 1,
    "access_mms": 1,
    "share_campaigns": 0,
    "notes": null
  }
}
```


### <a name="delete_a_specific_subaccount"></a>![Endpoint: ](https://apidocs.io/img/method.png "Delete a specific subaccount") `DELETE` /subaccounts/{subaccount_id}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| subaccount_id | `precision` |  ``` Required ```  | The subaccount ID you want to access. | `59` | 

#### Responses
**200** 

Body (_Delete a specific subaccount response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Subaccount #59 has been deleted",
  "data": true
}
```


### <a name="regenerate_api_key"></a>![Endpoint: ](https://apidocs.io/img/method.png "Regenerate API Key") `PUT` /subaccounts/{subaccount_id}/regen-api-key

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| subaccount_id | `precision` |  ``` Required ```  | The subaccount ID you want to access. | `59` | 

#### Responses
**200** 

Body (_Regenerate API Key response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Your API Key has been regenerated.",
  "data": {
    "api_key": "E72D09F6-AC80-0A5C-F7F0-1A244A377A5C"
  }
}
```


[Back to API Reference](#api_reference)

## <a name="timezones"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Timezones") Timezones


### <a name="get_timezones"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Timezones") `GET` /timezones

> Get supported list of timezones.



#### Responses
**200** 

Body (_Get Timezones response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "List of timezones.",
  "data": [
    "Africa/Abidjan",
    "Africa/Accra",
    "Africa/Addis_Ababa",
    "Africa/Algiers",
    "Africa/Asmara",
    "Africa/Bamako",
    "Africa/Bangui",
    "Africa/Banjul",
    "Africa/Bissau",
    "Africa/Blantyre",
    "Africa/Brazzaville",
    "Africa/Bujumbura",
    "Africa/Cairo",
    "Africa/Casablanca",
    "Africa/Ceuta",
    "Africa/Conakry",
    "Africa/Dakar",
    "Africa/Dar_es_Salaam",
    "Africa/Djibouti",
    "Africa/Douala",
    "Africa/El_Aaiun",
    "Africa/Freetown",
    "Africa/Gaborone",
    "Africa/Harare",
    "Africa/Johannesburg",
    "Africa/Juba",
    "Africa/Kampala",
    "Africa/Khartoum",
    "Africa/Kigali",
    "Africa/Kinshasa",
    "Africa/Lagos",
    "Africa/Libreville",
    "Africa/Lome",
    "Africa/Luanda",
    "Africa/Lubumbashi",
    "Africa/Lusaka",
    "Africa/Malabo",
    "Africa/Maputo",
    "Africa/Maseru",
    "Africa/Mbabane",
    "Africa/Mogadishu",
    "Africa/Monrovia",
    "Africa/Nairobi",
    "Africa/Ndjamena",
    "Africa/Niamey",
    "Africa/Nouakchott",
    "Africa/Ouagadougou",
    "Africa/Porto-Novo",
    "Africa/Sao_Tome",
    "Africa/Tripoli",
    "Africa/Tunis",
    "Africa/Windhoek",
    "America/Adak",
    "America/Anchorage",
    "America/Anguilla",
    "America/Antigua",
    "America/Araguaina",
    "America/Argentina/Buenos_Aires",
    "America/Argentina/Catamarca",
    "America/Argentina/Cordoba",
    "America/Argentina/Jujuy",
    "America/Argentina/La_Rioja",
    "America/Argentina/Mendoza",
    "America/Argentina/Rio_Gallegos",
    "America/Argentina/Salta",
    "America/Argentina/San_Juan",
    "America/Argentina/San_Luis",
    "America/Argentina/Tucuman",
    "America/Argentina/Ushuaia",
    "America/Aruba",
    "America/Asuncion",
    "America/Atikokan",
    "America/Bahia",
    "America/Bahia_Banderas",
    "America/Barbados",
    "America/Belem",
    "America/Belize",
    "America/Blanc-Sablon",
    "America/Boa_Vista",
    "America/Bogota",
    "America/Boise",
    "America/Cambridge_Bay",
    "America/Campo_Grande",
    "America/Cancun",
    "America/Caracas",
    "America/Cayenne",
    "America/Cayman",
    "America/Chicago",
    "America/Chihuahua",
    "America/Costa_Rica",
    "America/Creston",
    "America/Cuiaba",
    "America/Curacao",
    "America/Danmarkshavn",
    "America/Dawson",
    "America/Dawson_Creek",
    "America/Denver",
    "America/Detroit",
    "America/Dominica",
    "America/Edmonton",
    "America/Eirunepe",
    "America/El_Salvador",
    "America/Fort_Nelson",
    "America/Fortaleza",
    "America/Glace_Bay",
    "America/Godthab",
    "America/Goose_Bay",
    "America/Grand_Turk",
    "America/Grenada",
    "America/Guadeloupe",
    "America/Guatemala",
    "America/Guayaquil",
    "America/Guyana",
    "America/Halifax",
    "America/Havana",
    "America/Hermosillo",
    "America/Indiana/Indianapolis",
    "America/Indiana/Knox",
    "America/Indiana/Marengo",
    "America/Indiana/Petersburg",
    "America/Indiana/Tell_City",
    "America/Indiana/Vevay",
    "America/Indiana/Vincennes",
    "America/Indiana/Winamac",
    "America/Inuvik",
    "America/Iqaluit",
    "America/Jamaica",
    "America/Juneau",
    "America/Kentucky/Louisville",
    "America/Kentucky/Monticello",
    "America/Kralendijk",
    "America/La_Paz",
    "America/Lima",
    "America/Los_Angeles",
    "America/Lower_Princes",
    "America/Maceio",
    "America/Managua",
    "America/Manaus",
    "America/Marigot",
    "America/Martinique",
    "America/Matamoros",
    "America/Mazatlan",
    "America/Menominee",
    "America/Merida",
    "America/Metlakatla",
    "America/Mexico_City",
    "America/Miquelon",
    "America/Moncton",
    "America/Monterrey",
    "America/Montevideo",
    "America/Montserrat",
    "America/Nassau",
    "America/New_York",
    "America/Nipigon",
    "America/Nome",
    "America/Noronha",
    "America/North_Dakota/Beulah",
    "America/North_Dakota/Center",
    "America/North_Dakota/New_Salem",
    "America/Ojinaga",
    "America/Panama",
    "America/Pangnirtung",
    "America/Paramaribo",
    "America/Phoenix",
    "America/Port-au-Prince",
    "America/Port_of_Spain",
    "America/Porto_Velho",
    "America/Puerto_Rico",
    "America/Rainy_River",
    "America/Rankin_Inlet",
    "America/Recife",
    "America/Regina",
    "America/Resolute",
    "America/Rio_Branco",
    "America/Santarem",
    "America/Santiago",
    "America/Santo_Domingo",
    "America/Sao_Paulo",
    "America/Scoresbysund",
    "America/Sitka",
    "America/St_Barthelemy",
    "America/St_Johns",
    "America/St_Kitts",
    "America/St_Lucia",
    "America/St_Thomas",
    "America/St_Vincent",
    "America/Swift_Current",
    "America/Tegucigalpa",
    "America/Thule",
    "America/Thunder_Bay",
    "America/Tijuana",
    "America/Toronto",
    "America/Tortola",
    "America/Vancouver",
    "America/Whitehorse",
    "America/Winnipeg",
    "America/Yakutat",
    "America/Yellowknife",
    "Antarctica/Casey",
    "Antarctica/Davis",
    "Antarctica/DumontDUrville",
    "Antarctica/Macquarie",
    "Antarctica/Mawson",
    "Antarctica/McMurdo",
    "Antarctica/Palmer",
    "Antarctica/Rothera",
    "Antarctica/Syowa",
    "Antarctica/Troll",
    "Antarctica/Vostok",
    "Arctic/Longyearbyen",
    "Asia/Aden",
    "Asia/Almaty",
    "Asia/Amman",
    "Asia/Anadyr",
    "Asia/Aqtau",
    "Asia/Aqtobe",
    "Asia/Ashgabat",
    "Asia/Baghdad",
    "Asia/Bahrain",
    "Asia/Baku",
    "Asia/Bangkok",
    "Asia/Barnaul",
    "Asia/Beirut",
    "Asia/Bishkek",
    "Asia/Brunei",
    "Asia/Chita",
    "Asia/Choibalsan",
    "Asia/Colombo",
    "Asia/Damascus",
    "Asia/Dhaka",
    "Asia/Dili",
    "Asia/Dubai",
    "Asia/Dushanbe",
    "Asia/Gaza",
    "Asia/Hebron",
    "Asia/Ho_Chi_Minh",
    "Asia/Hong_Kong",
    "Asia/Hovd",
    "Asia/Irkutsk",
    "Asia/Jakarta",
    "Asia/Jayapura",
    "Asia/Jerusalem",
    "Asia/Kabul",
    "Asia/Kamchatka",
    "Asia/Karachi",
    "Asia/Kathmandu",
    "Asia/Khandyga",
    "Asia/Kolkata",
    "Asia/Krasnoyarsk",
    "Asia/Kuala_Lumpur",
    "Asia/Kuching",
    "Asia/Kuwait",
    "Asia/Macau",
    "Asia/Magadan",
    "Asia/Makassar",
    "Asia/Manila",
    "Asia/Muscat",
    "Asia/Nicosia",
    "Asia/Novokuznetsk",
    "Asia/Novosibirsk",
    "Asia/Omsk",
    "Asia/Oral",
    "Asia/Phnom_Penh",
    "Asia/Pontianak",
    "Asia/Pyongyang",
    "Asia/Qatar",
    "Asia/Qyzylorda",
    "Asia/Rangoon",
    "Asia/Riyadh",
    "Asia/Sakhalin",
    "Asia/Samarkand",
    "Asia/Seoul",
    "Asia/Shanghai",
    "Asia/Singapore",
    "Asia/Srednekolymsk",
    "Asia/Taipei",
    "Asia/Tashkent",
    "Asia/Tbilisi",
    "Asia/Tehran",
    "Asia/Thimphu",
    "Asia/Tokyo",
    "Asia/Tomsk",
    "Asia/Ulaanbaatar",
    "Asia/Urumqi",
    "Asia/Ust-Nera",
    "Asia/Vientiane",
    "Asia/Vladivostok",
    "Asia/Yakutsk",
    "Asia/Yekaterinburg",
    "Asia/Yerevan",
    "Atlantic/Azores",
    "Atlantic/Bermuda",
    "Atlantic/Canary",
    "Atlantic/Cape_Verde",
    "Atlantic/Faroe",
    "Atlantic/Madeira",
    "Atlantic/Reykjavik",
    "Atlantic/South_Georgia",
    "Atlantic/St_Helena",
    "Atlantic/Stanley",
    "Australia/Adelaide",
    "Australia/Brisbane",
    "Australia/Broken_Hill",
    "Australia/Currie",
    "Australia/Darwin",
    "Australia/Eucla",
    "Australia/Hobart",
    "Australia/Lindeman",
    "Australia/Lord_Howe",
    "Australia/Melbourne",
    "Australia/Perth",
    "Australia/Sydney",
    "Europe/Amsterdam",
    "Europe/Andorra",
    "Europe/Astrakhan",
    "Europe/Athens",
    "Europe/Belgrade",
    "Europe/Berlin",
    "Europe/Bratislava",
    "Europe/Brussels",
    "Europe/Bucharest",
    "Europe/Budapest",
    "Europe/Busingen",
    "Europe/Chisinau",
    "Europe/Copenhagen",
    "Europe/Dublin",
    "Europe/Gibraltar",
    "Europe/Guernsey",
    "Europe/Helsinki",
    "Europe/Isle_of_Man",
    "Europe/Istanbul",
    "Europe/Jersey",
    "Europe/Kaliningrad",
    "Europe/Kiev",
    "Europe/Kirov",
    "Europe/Lisbon",
    "Europe/Ljubljana",
    "Europe/London",
    "Europe/Luxembourg",
    "Europe/Madrid",
    "Europe/Malta",
    "Europe/Mariehamn",
    "Europe/Minsk",
    "Europe/Monaco",
    "Europe/Moscow",
    "Europe/Oslo",
    "Europe/Paris",
    "Europe/Podgorica",
    "Europe/Prague",
    "Europe/Riga",
    "Europe/Rome",
    "Europe/Samara",
    "Europe/San_Marino",
    "Europe/Sarajevo",
    "Europe/Simferopol",
    "Europe/Skopje",
    "Europe/Sofia",
    "Europe/Stockholm",
    "Europe/Tallinn",
    "Europe/Tirane",
    "Europe/Ulyanovsk",
    "Europe/Uzhgorod",
    "Europe/Vaduz",
    "Europe/Vatican",
    "Europe/Vienna",
    "Europe/Vilnius",
    "Europe/Volgograd",
    "Europe/Warsaw",
    "Europe/Zagreb",
    "Europe/Zaporozhye",
    "Europe/Zurich",
    "Indian/Antananarivo",
    "Indian/Chagos",
    "Indian/Christmas",
    "Indian/Cocos",
    "Indian/Comoro",
    "Indian/Kerguelen",
    "Indian/Mahe",
    "Indian/Maldives",
    "Indian/Mauritius",
    "Indian/Mayotte",
    "Indian/Reunion",
    "Pacific/Apia",
    "Pacific/Auckland",
    "Pacific/Bougainville",
    "Pacific/Chatham",
    "Pacific/Chuuk",
    "Pacific/Easter",
    "Pacific/Efate",
    "Pacific/Enderbury",
    "Pacific/Fakaofo",
    "Pacific/Fiji",
    "Pacific/Funafuti",
    "Pacific/Galapagos",
    "Pacific/Gambier",
    "Pacific/Guadalcanal",
    "Pacific/Guam",
    "Pacific/Honolulu",
    "Pacific/Johnston",
    "Pacific/Kiritimati",
    "Pacific/Kosrae",
    "Pacific/Kwajalein",
    "Pacific/Majuro",
    "Pacific/Marquesas",
    "Pacific/Midway",
    "Pacific/Nauru",
    "Pacific/Niue",
    "Pacific/Norfolk",
    "Pacific/Noumea",
    "Pacific/Pago_Pago",
    "Pacific/Palau",
    "Pacific/Pitcairn",
    "Pacific/Pohnpei",
    "Pacific/Port_Moresby",
    "Pacific/Rarotonga",
    "Pacific/Saipan",
    "Pacific/Tahiti",
    "Pacific/Tarawa",
    "Pacific/Tongatapu",
    "Pacific/Wake",
    "Pacific/Wallis",
    "UTC"
  ]
}
```


[Back to API Reference](#api_reference)

## <a name="transactional_email"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Transactional Email") Transactional Email


### <a name="email_send"></a>![Endpoint: ](https://apidocs.io/img/method.png "Email Send") `POST` /email/send

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `email send request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "to": [
    "to"
  ],
  "subject": "subject",
  "from.email_address_id": 172.952709855955,
  "body": "body",
  "attachments": [
    "attachments"
  ],
  "cc": [
    "cc"
  ],
  "bcc": [
    "bcc"
  ],
  "from.name": "from.name"
}
``` 

#### Responses
**200** 

Body (_Email Send response_) 
```
{
  "http_code": 172,
  "response_code": "response_code",
  "response_msg": "response_msg",
  "data": {}
}
```


### <a name="email_price"></a>![Endpoint: ](https://apidocs.io/img/method.png "Email Price") `POST` /email/price

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `email price request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "to": [
    "to"
  ],
  "subject": "subject",
  "from.email_address_id": 172.952709855955,
  "body": "body",
  "attachments": [
    "attachments"
  ],
  "cc": [
    "cc"
  ],
  "bcc": [
    "bcc"
  ],
  "from.name": "from.name"
}
``` 

#### Responses
**200** 

Body (_Email Price response_) 
```
{
  "http_code": 172,
  "response_code": "response_code",
  "response_msg": "response_msg",
  "data": {}
}
```


### <a name="email_history"></a>![Endpoint: ](https://apidocs.io/img/method.png "Email History") `GET` /email/history

> TODO: Add a method description



#### Responses
**200** 

Body (_Email History response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here is your result.",
  "data": {
    "total": 2,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 15,
    "data": [
      {
        "user_id": 1201,
        "subaccount_id": 1039,
        "from_email_address_id": 2,
        "from_name": "test",
        "to": [
          {
            "email": "test1@user.com"
          }
        ],
        "cc": null,
        "bcc": null,
        "subject": "test email transaction",
        "body": "This is a test content <img src=\"cid:7c65ccc4a134a809db09a839df9b75f055afcb62@click-send.com\" />",
        "body_plain_text": "This is a test content <img src=\"cid:7c65ccc4a134a809db09a839df9b75f055afcb62@click-send.com\" />",
        "schedule": "1469001353",
        "message_id": "BCEBC89E-6993-4F13-B485-942440C62915",
        "status": "Sent",
        "status_text": "Email added to outgoing mail queue for delivery",
        "soft_bounce_count": 0,
        "hard_bounce_count": 0,
        "price": "0.0000",
        "date_added": "1469001354",
        "custom_string": null,
        "_attachments": [],
        "_currency": {
          "currency_name_short": "PHP",
          "currency_prefix_d": "?",
          "currency_prefix_c": "c",
          "currency_name_long": "Philippine Peso"
        }
      },
      {
        "user_id": 1201,
        "subaccount_id": 1039,
        "from_email_address_id": 2,
        "from_name": "test",
        "to": [
          {
            "email": "test1@user.com"
          }
        ],
        "cc": null,
        "bcc": null,
        "subject": "test email transaction",
        "body": "This is a test content",
        "body_plain_text": "This is a test content",
        "schedule": "1469002942",
        "message_id": "988067DE-9318-448F-B225-7A5A695B23D1",
        "status": "Queued:WaitSend",
        "status_text": null,
        "soft_bounce_count": 0,
        "hard_bounce_count": 0,
        "price": "0.0822",
        "date_added": "1469002942",
        "custom_string": null,
        "_attachments": [
          {
            "file_name": "test.jpg",
            "content_type": "image/jpeg",
            "content_disposition": "attachment",
            "content_id": "<cid:PHP-CID-5b3eb73f50a7cf7f423dc97070bb3b5280312308>",
            "_attachment_file_url": "http://api.clicksend.local/files/B5664FA5-CEBD-40B0-BED1-5CFF0CA027BD.jpg"
          }
        ],
        "_currency": {
          "currency_name_short": "PHP",
          "currency_prefix_d": "?",
          "currency_prefix_c": "c",
          "currency_name_long": "Philippine Peso"
        }
      }
    ]
  }
}
```


### <a name="export_history"></a>![Endpoint: ](https://apidocs.io/img/method.png "Export History") `GET` /email/history/export?filename={filename}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| filename | `string` |  ``` Required ```  | File name for the export file. | `myexport.csv` | 

#### Responses
**200** 

Body (_Export History response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Download your file here.",
  "data": {
    "url": "https://rest.clicksend.com/files/705F80D0-D044-4F85-8617-081988B398E4?filename=myexport.csv"
  }
}
```


### <a name="add_a_test_delivery_receipt"></a>![Endpoint: ](https://apidocs.io/img/method.png "Add a Test Delivery Receipt") `POST` /email/receipts

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



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `add a test delivery receipt request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "url": "http://yourUrl.com"
}
``` 

#### Responses
**200** 

Body (_Add a Test Delivery Receipt response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Receipt has been added.",
  "data": {
    "email": "john_doe@user.com",
    "timestamp": 1476870832,
    "message_id": "73A80623-CFC3-4E7F-856A-880B289242D7@clicksend.com",
    "status": "Delivered"
  }
}
```


[Back to API Reference](#api_reference)

## <a name="uploads"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Uploads") Uploads


### <a name="upload_a_file"></a>![Endpoint: ](https://apidocs.io/img/method.png "Upload a file") `POST` /uploads?convert={convert}

> The `upload` endpoint provides a method for converting files from an unspported format to a format that one of our endpoints can handle.
> Files can be submitted two ways:
> 1. Using `base64` encoding in an `application/json` request. In this case, submit the `base64`-encoded file contents in the `content` field of the request body, and `convert` can be specified either also in the body or as part of the query string.
> 2. Using `multipart/form-data` encoding, in the same way it would be submitted using a HTML form. You may find cURL useful for this. For an example of how to do this, see one of our [SDKs](https://dashboard.clicksend.com/#/libraries-sdk/main). In this case, specify `convert` in the query string.
> Note that `convert` specifies the conversion to take place - that is, what the result should be compatible with - and can be any of `fax`, `mms`, `csv` or `post`.
> All files have 10 minutes expiry.



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| convert | `string` |  ``` Optional ```  | TODO: Add a parameter description | `"convert"` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `upload a file request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "content": "content",
  "convert": "convert"
}
``` 

#### Responses
**200** 

Body (_Upload a file response_) 
```
{
  "http_code": 172,
  "response_code": "response_code",
  "response_msg": "response_msg",
  "data": {}
}
```


[Back to API Reference](#api_reference)

## <a name="voice"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Voice") Voice


### <a name="send_a_voice_call"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send a Voice Call") `POST` /voice/send

> You can post **up to 1000 messages** with each API call.



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `send a voice call request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "to": "to",
  "body": "body",
  "voice": "voice",
  "source": "source",
  "list_id": 172.952709855955,
  "lang": "lang",
  "schedule": 172.952709855955,
  "custom_string": "custom_string",
  "country": "country",
  "require_input": 172.952709855955
}
``` 

#### Responses
**200** 

Body (_Send a Voice Call response_) 
```
{
  "http_code": 172,
  "response_code": "response_code",
  "response_msg": "response_msg",
  "data": {}
}
```


### <a name="calculate_price"></a>![Endpoint: ](https://apidocs.io/img/method.png "Calculate Price") `POST` /voice/price

> TODO: Add a method description



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `calculate price request263` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "to": "to",
  "body": "body",
  "voice": "voice",
  "source": "source",
  "list_id": 172.952709855955,
  "lang": "lang",
  "schedule": 172.952709855955,
  "custom_string": "custom_string",
  "country": "country",
  "require_input": 172.952709855955
}
``` 

#### Responses
**200** 

Body (_Calculate Price response_) 
```
{
  "http_code": 172,
  "response_code": "response_code",
  "response_msg": "response_msg",
  "data": {}
}
```


### <a name="voice_languages"></a>![Endpoint: ](https://apidocs.io/img/method.png "Voice Languages") `GET` /voice/lang

> TODO: Add a method description



#### Responses
**200** 

Body (_Voice Languages response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are the possible languages.",
  "data": [
    {
      "code": "en-us",
      "country": "English, US",
      "gender": [
        "female",
        "male"
      ]
    },
    {
      "code": "en-au",
      "country": "English, Australia",
      "gender": [
        "female",
        "male"
      ]
    },
    {
      "code": "en-gb",
      "country": "English, UK",
      "gender": [
        "female",
        "male"
      ]
    },
    {
      "code": "en-in",
      "country": "English, India",
      "gender": "female"
    },
    {
      "code": "de-de",
      "country": "German, Germany",
      "gender": [
        "female",
        "male"
      ]
    },
    {
      "code": "es-es",
      "country": "Spanish, Spain",
      "gender": [
        "female",
        "male"
      ]
    },
    {
      "code": "es-us",
      "country": "Spanish, US",
      "gender": [
        "female",
        "male"
      ]
    },
    {
      "code": "fr-ca",
      "country": "French, Canada",
      "gender": "female"
    },
    {
      "code": "fr-fr",
      "country": "French, France",
      "gender": [
        "female",
        "male"
      ]
    },
    {
      "code": "is-is",
      "country": "Icelandic, Iceland",
      "gender": [
        "female",
        "male"
      ]
    },
    {
      "code": "it-it",
      "country": "Italian, Italy",
      "gender": [
        "female",
        "male"
      ]
    },
    {
      "code": "nl-nl",
      "country": "Dutch, Netherlands",
      "gender": [
        "female",
        "male"
      ]
    },
    {
      "code": "pl-pl",
      "country": "Polish-Poland",
      "gender": [
        "female",
        "male"
      ]
    },
    {
      "code": "pt-pt",
      "country": "Portuguese, Portugal",
      "gender": "male"
    },
    {
      "code": "pt-br",
      "country": "Portuguese, Brazil",
      "gender": [
        "female",
        "male"
      ]
    },
    {
      "code": "ro-ro",
      "country": "Romanian, Romania",
      "gender": "female"
    },
    {
      "code": "ru-ru",
      "country": "Russian, Russia",
      "gender": [
        "female",
        "male"
      ]
    },
    {
      "code": "sv-se",
      "country": "Swedish, Sweden",
      "gender": "female"
    },
    {
      "code": "tr-tr",
      "country": "Turkish, Turkey",
      "gender": "female"
    },
    {
      "code": "en-gb-wls",
      "country": "English, Wales",
      "gender": [
        "female",
        "male"
      ]
    },
    {
      "code": "cy-gb-wls",
      "country": "Celtic, Wales",
      "gender": [
        "female",
        "male"
      ]
    },
    {
      "code": "nb-no",
      "country": "Norwegian, Norway",
      "gender": "female"
    },
    {
      "code": "da-dk",
      "country": "Danish, Denmark",
      "gender": [
        "female",
        "male"
      ]
    }
  ]
}
```


### <a name="get_voice_history"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Voice History") `GET` /voice/history?date_from={date_from}&date_to={date_to}

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| date_from | `number` |  ``` Optional ```  | Timestamp (from) used to show records by date. | `1443501617` | 
| date_to | `number` |  ``` Optional ```  | Timestamp (to) used to show recrods by date. | `1443501727` | 

#### Responses
**200** 

Body (_Get Voice History response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here is your history.",
  "data": {
    "total": 4,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 4,
    "data": [
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": null,
        "message_id": "D6456F8A-9DF9-46EC-8014-BFE87860F65C",
        "to": "+15184811537",
        "to_type": "mobile",
        "from": "+19403944918",
        "voice": "female",
        "lang": "en-us",
        "body": "this is a test.",
        "carrier": "",
        "country": "US",
        "custom_string": "mystring",
        "schedule": "1538672470",
        "message_parts": "1.00",
        "message_price": "0.17",
        "status": "WaitApproval",
        "status_code": null,
        "status_text": null,
        "date_added": 1443501617
      },
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": null,
        "message_id": "25304958-15F2-41D9-8716-CF1F28EF506B",
        "to": "+15184811537",
        "to_type": "mobile",
        "from": "+19403944918",
        "voice": "female",
        "lang": "en-us",
        "body": "this is a test.",
        "carrier": "",
        "country": "US",
        "custom_string": "mystring",
        "schedule": "1538672470",
        "message_parts": "1.00",
        "message_price": "0.17",
        "status": "WaitApproval",
        "status_code": null,
        "status_text": null,
        "date_added": 1443501727
      },
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": null,
        "message_id": "0B474459-B75F-4180-9567-7ECA3FC56BD7",
        "to": "+15184811538",
        "to_type": "mobile",
        "from": "+19403944918",
        "voice": "female",
        "lang": "en-us",
        "body": "this is a test.",
        "carrier": "",
        "country": "US",
        "custom_string": "mystring",
        "schedule": "1538672470",
        "message_parts": "1.00",
        "message_price": "0.17",
        "status": "WaitApproval",
        "status_code": null,
        "status_text": null,
        "date_added": 1443501727
      },
      {
        "user_id": 1,
        "subaccount_id": 1,
        "list_id": null,
        "message_id": "A991556C-D4A5-47D5-A5E5-C9D251C8743A",
        "to": "+15184811539",
        "to_type": "mobile",
        "from": "+19403944918",
        "voice": "female",
        "lang": "en-us",
        "body": "this is a test.",
        "carrier": "",
        "country": "US",
        "custom_string": "mystring",
        "schedule": "1538672470",
        "message_parts": "1.00",
        "message_price": "0.17",
        "status": "WaitApproval",
        "status_code": null,
        "status_text": null,
        "date_added": 1443501727
      }
    ]
  }
}
```


### <a name="export_voice_history"></a>![Endpoint: ](https://apidocs.io/img/method.png "Export Voice History") `GET` /voice/history/export

> TODO: Add a method description



#### Responses
**200** 

Body (_Export Voice History response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Download your file here.",
  "data": {
    "url": "https://rest.clicksend.com/files/24E25B4B-CB69-4BA3-8D4E-7ABA92124722?filename=export.csv"
  }
}
```


### <a name="get_voice_receipts"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Voice receipts") `GET` /voice/receipts

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



#### Responses
**200** 

Body (_Get Voice receipts response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here are your delivery receipts.",
  "data": {
    "total": 2,
    "per_page": 15,
    "current_page": 1,
    "last_page": 1,
    "next_page_url": null,
    "prev_page_url": null,
    "from": 1,
    "to": 2,
    "data": [
      {
        "timestamp_send": "1442381791",
        "timestamp": "1442381791",
        "message_id": "31BC271B-1E0C-45F6-9E7E-97186C46BB82",
        "status_code": "201",
        "status_text": "Success: Message received on handset.",
        "error_code": null,
        "error_text": null,
        "custom_string": null,
        "message_type": "voice",
        "digits": "2"
      },
      {
        "timestamp_send": "1442381829",
        "timestamp": "1442381829",
        "message_id": "23C8ADA3-FD8B-420B-801A-F829BB87AC6F",
        "status_code": "201",
        "status_text": "Success: Message received on handset.",
        "error_code": null,
        "error_text": null,
        "custom_string": null,
        "message_type": "voice",
        "digits": "5"
      }
    ]
  }
}
```


### <a name="add_a_test_delivery_receipt"></a>![Endpoint: ](https://apidocs.io/img/method.png "Add a Test Delivery Receipt") `POST` /voice/receipts

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



#### Request Headers
>Accept=application/json;
>Content-Type=application/json;charset=utf-8;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| `add a test delivery receipt request` |  ``` Required ```  | TODO: Add a parameter description | 

 Example 
``` 
{
  "url": "http://yourUrl.com"
}
``` 

#### Responses
**200** 

Body (_Add a Test Delivery Receipt response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Test receipt has been added.",
  "data": {
    "timestamp_send": "1489730505",
    "timestamp": "1489730505",
    "message_id": "CEA5E06A-F4BF-4EC6-8315-B25087352DFA",
    "status_code": "201",
    "status_text": "Success: Message received on handset.",
    "error_code": null,
    "error_text": null,
    "custom_string": null,
    "subaccount_id": 1746,
    "message_type": "voice",
    "digits": "2"
  }
}
```


### <a name="get_specific_voice_receipt"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Specific Voice Receipt") `GET` /voice/receipts/{message_id}

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



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| message_id | `string` |  ``` Required ```  | 3055-45F1-9B79-F2C43509FD16 (string, required) - The voice receipt message id. | `28DD2718` | 

#### Responses
**200** 

Body (_Get Specific Voice Receipt response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Here is your result.",
  "data": {
    "timestamp_send": "1461658202",
    "timestamp": "1461658202",
    "message_id": "1FCFEBBF-90F5-4198-AEBD-5DAEDBA3D7B1",
    "status_code": "Sent",
    "status_text": "Sent",
    "error_code": "",
    "error_text": "",
    "custom_string": "custom string test",
    "subaccount_id": 1039,
    "message_type": "voice",
    "digits": "6"
  }
}
```


### <a name="marked_voice_receipts_as_read"></a>![Endpoint: ](https://apidocs.io/img/method.png "Marked Voice Receipts as Read") `PUT` /voice/receipts-read?date_before={date_before}

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



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| date_before | `precision` |  ``` Required ```  | An optional timestamp - mark all as read before this timestamp. If not given, all receipts will be marked as read. | `1461897483` | 

#### Responses
**200** 

Body (_Marked Voice Receipts as Read response_) 
```
{
  "http_code": 172,
  "response_code": "response_code",
  "response_msg": "response_msg",
  "data": "data"
}
```


### <a name="cancel_a_specific_voice_call"></a>![Endpoint: ](https://apidocs.io/img/method.png "Cancel a Specific Voice Call") `PUT` /voice/{message_id}/cancel

> TODO: Add a method description



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| message_id | `string` |  ``` Required ```  | Your voice message id. | `7B5BFC19 06B7 49C1 8DCDFB011600E12B` | 

#### Responses
**200** 

Body (_Cancel a Specific Voice Call response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "Voice have been cancelled.",
  "data": []
}
```


### <a name="cancel_all_voice_calls"></a>![Endpoint: ](https://apidocs.io/img/method.png "Cancel all Voice Calls") `PUT` /voice/cancel-all

> TODO: Add a method description



#### Responses
**200** 

Body (_Cancel all Voice Calls response_) 
```
{
  "http_code": 200,
  "response_code": "SUCCESS",
  "response_msg": "5 messages have been cancelled.",
  "data": {
    "count": 5
  }
}
```


[Back to API Reference](#api_reference)

