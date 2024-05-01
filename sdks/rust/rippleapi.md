# \RippleApi

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                                  | HTTP request                           | Description |
| ----------------------------------------------------------------------- | -------------------------------------- | ----------- |
| [**create\_ripple\_account**](rippleapi.md#create\_ripple\_account)     | **POST** /ripple                       |             |
| [**get\_ripple\_account**](rippleapi.md#get\_ripple\_account)           | **GET** /ripple/{accountName}          |             |
| [**list\_ripple\_accounts**](rippleapi.md#list\_ripple\_accounts)       | **GET** /ripple                        |             |
| [**sign\_ripple\_transaction**](rippleapi.md#sign\_ripple\_transaction) | **POST** /ripple/{accountName}/sign-tx |             |

## create\_ripple\_account

> crate::models::AccountApiResponse create\_ripple\_account(authorization, ripple\_input)

### Parameters

| Name              | Type                              | Description | Required    | Notes |
| ----------------- | --------------------------------- | ----------- | ----------- | ----- |
| **authorization** | **String**                        |             | \[required] |       |
| **ripple\_input** | [**RippleInput**](rippleinput.md) |             | \[required] |       |

### Return type

[**crate::models::AccountApiResponse**](../../rust/docs/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](rippleapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## get\_ripple\_account

> crate::models::AccountApiResponse get\_ripple\_account(authorization, account\_name)

### Parameters

| Name              | Type       | Description | Required    | Notes |
| ----------------- | ---------- | ----------- | ----------- | ----- |
| **authorization** | **String** |             | \[required] |       |
| **account\_name** | **String** |             | \[required] |       |

### Return type

[**crate::models::AccountApiResponse**](../../rust/docs/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](rippleapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## list\_ripple\_accounts

> crate::models::AccountApiResponse list\_ripple\_accounts(authorization)

### Parameters

| Name              | Type       | Description | Required    | Notes |
| ----------------- | ---------- | ----------- | ----------- | ----- |
| **authorization** | **String** |             | \[required] |       |

### Return type

[**crate::models::AccountApiResponse**](../../rust/docs/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](rippleapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## sign\_ripple\_transaction

> crate::models::RippleApiResponse sign\_ripple\_transaction(authorization, account\_name, ripple\_transaction\_input)

### Parameters

| Name                           | Type                                                    | Description | Required    | Notes |
| ------------------------------ | ------------------------------------------------------- | ----------- | ----------- | ----- |
| **authorization**              | **String**                                              |             | \[required] |       |
| **account\_name**              | **String**                                              |             | \[required] |       |
| **ripple\_transaction\_input** | [**RippleTransactionInput**](rippletransactioninput.md) |             | \[required] |       |

### Return type

[**crate::models::RippleApiResponse**](../../rust/docs/RippleAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](rippleapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
