# \EosApi

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                         | HTTP request                        | Description |
| -------------------------------------------------------------- | ----------------------------------- | ----------- |
| [**create\_eos\_account**](EosApi.md#create\_eos\_account)     | **POST** /eos                       |             |
| [**get\_eos\_account**](EosApi.md#get\_eos\_account)           | **GET** /eos/{accountName}          |             |
| [**list\_eos\_accounts**](EosApi.md#list\_eos\_accounts)       | **GET** /eos                        |             |
| [**sign\_eos\_transaction**](EosApi.md#sign\_eos\_transaction) | **POST** /eos/{accountName}/sign-tx |             |

## create\_eos\_account

> crate::models::AccountApiResponse create\_eos\_account(authorization, eos\_input)

### Parameters

| Name              | Type                        | Description | Required    | Notes |
| ----------------- | --------------------------- | ----------- | ----------- | ----- |
| **authorization** | **String**                  |             | \[required] |       |
| **eos\_input**    | [**EosInput**](EosInput.md) |             | \[required] |       |

### Return type

[**crate::models::AccountApiResponse**](docs/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](EosApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## get\_eos\_account

> crate::models::AccountApiResponse get\_eos\_account(authorization, account\_name)

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

[\[Back to top\]](EosApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## list\_eos\_accounts

> crate::models::AccountApiResponse list\_eos\_accounts(authorization)

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

[\[Back to top\]](EosApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## sign\_eos\_transaction

> crate::models::EosApiResponse sign\_eos\_transaction(authorization, account\_name, eos\_transaction\_input)

### Parameters

| Name                        | Type                                              | Description | Required    | Notes |
| --------------------------- | ------------------------------------------------- | ----------- | ----------- | ----- |
| **authorization**           | **String**                                        |             | \[required] |       |
| **account\_name**           | **String**                                        |             | \[required] |       |
| **eos\_transaction\_input** | [**EosTransactionInput**](EosTransactionInput.md) |             | \[required] |       |

### Return type

[**crate::models::EosApiResponse**](docs/EosAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](EosApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
