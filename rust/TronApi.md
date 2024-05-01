# \TronApi

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                            | HTTP request                         | Description |
| ----------------------------------------------------------------- | ------------------------------------ | ----------- |
| [**create\_tron\_account**](TronApi.md#create\_tron\_account)     | **POST** /tron                       |             |
| [**get\_tron\_account**](TronApi.md#get\_tron\_account)           | **GET** /tron/{accountName}          |             |
| [**list\_tron\_accounts**](TronApi.md#list\_tron\_accounts)       | **GET** /tron                        |             |
| [**sign\_tron\_transaction**](TronApi.md#sign\_tron\_transaction) | **POST** /tron/{accountName}/sign-tx |             |

## create\_tron\_account

> crate::models::AccountApiResponse create\_tron\_account(authorization, tron\_input)

### Parameters

| Name              | Type                          | Description | Required    | Notes |
| ----------------- | ----------------------------- | ----------- | ----------- | ----- |
| **authorization** | **String**                    |             | \[required] |       |
| **tron\_input**   | [**TronInput**](TronInput.md) |             | \[required] |       |

### Return type

[**crate::models::AccountApiResponse**](docs/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](TronApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## get\_tron\_account

> crate::models::AccountApiResponse get\_tron\_account(authorization, account\_name)

### Parameters

| Name              | Type       | Description | Required    | Notes |
| ----------------- | ---------- | ----------- | ----------- | ----- |
| **authorization** | **String** |             | \[required] |       |
| **account\_name** | **String** |             | \[required] |       |

### Return type

[**crate::models::AccountApiResponse**](docs/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](TronApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## list\_tron\_accounts

> crate::models::AccountApiResponse list\_tron\_accounts(authorization)

### Parameters

| Name              | Type       | Description | Required    | Notes |
| ----------------- | ---------- | ----------- | ----------- | ----- |
| **authorization** | **String** |             | \[required] |       |

### Return type

[**crate::models::AccountApiResponse**](docs/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](TronApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## sign\_tron\_transaction

> crate::models::TronApiResponse sign\_tron\_transaction(authorization, account\_name, tron\_transaction\_input)

### Parameters

| Name                         | Type                                                | Description | Required    | Notes |
| ---------------------------- | --------------------------------------------------- | ----------- | ----------- | ----- |
| **authorization**            | **String**                                          |             | \[required] |       |
| **account\_name**            | **String**                                          |             | \[required] |       |
| **tron\_transaction\_input** | [**TronTransactionInput**](TronTransactionInput.md) |             | \[required] |       |

### Return type

[**crate::models::TronApiResponse**](docs/TronAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](TronApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
