# \LitecoinApi

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                                        | HTTP request                             | Description |
| ----------------------------------------------------------------------------- | ---------------------------------------- | ----------- |
| [**create\_litecoin\_account**](litecoinapi.md#create\_litecoin\_account)     | **POST** /litecoin                       |             |
| [**get\_litecoin\_account**](litecoinapi.md#get\_litecoin\_account)           | **GET** /litecoin/{accountName}          |             |
| [**list\_litecoin\_accounts**](litecoinapi.md#list\_litecoin\_accounts)       | **GET** /litecoin                        |             |
| [**sign\_litecoin\_transaction**](litecoinapi.md#sign\_litecoin\_transaction) | **POST** /litecoin/{accountName}/sign-tx |             |

## create\_litecoin\_account

> crate::models::AccountApiResponse create\_litecoin\_account(authorization, litecoin\_input)

### Parameters

| Name                | Type                                  | Description | Required    | Notes |
| ------------------- | ------------------------------------- | ----------- | ----------- | ----- |
| **authorization**   | **String**                            |             | \[required] |       |
| **litecoin\_input** | [**LitecoinInput**](litecoininput.md) |             | \[required] |       |

### Return type

[**crate::models::AccountApiResponse**](../../rust/docs/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](litecoinapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## get\_litecoin\_account

> crate::models::AccountApiResponse get\_litecoin\_account(authorization, account\_name)

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

[\[Back to top\]](litecoinapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## list\_litecoin\_accounts

> crate::models::AccountApiResponse list\_litecoin\_accounts(authorization)

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

[\[Back to top\]](litecoinapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## sign\_litecoin\_transaction

> crate::models::LitecoinApiResponse sign\_litecoin\_transaction(authorization, account\_name, litecoin\_transaction\_input)

### Parameters

| Name                             | Type                                                        | Description | Required    | Notes |
| -------------------------------- | ----------------------------------------------------------- | ----------- | ----------- | ----- |
| **authorization**                | **String**                                                  |             | \[required] |       |
| **account\_name**                | **String**                                                  |             | \[required] |       |
| **litecoin\_transaction\_input** | [**LitecoinTransactionInput**](litecointransactioninput.md) |             | \[required] |       |

### Return type

[**crate::models::LitecoinApiResponse**](../../rust/docs/LitecoinAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](litecoinapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
