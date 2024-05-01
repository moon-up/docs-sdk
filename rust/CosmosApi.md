# \CosmosApi

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                                  | HTTP request                           | Description |
| ----------------------------------------------------------------------- | -------------------------------------- | ----------- |
| [**create\_cosmos\_account**](CosmosApi.md#create\_cosmos\_account)     | **POST** /cosmos                       |             |
| [**get\_cosmos\_account**](CosmosApi.md#get\_cosmos\_account)           | **GET** /cosmos/{accountName}          |             |
| [**list\_cosmos\_accounts**](CosmosApi.md#list\_cosmos\_accounts)       | **GET** /cosmos                        |             |
| [**sign\_cosmos\_transaction**](CosmosApi.md#sign\_cosmos\_transaction) | **POST** /cosmos/{accountName}/sign-tx |             |

## create\_cosmos\_account

> crate::models::AccountApiResponse create\_cosmos\_account(authorization, cosmos\_input)

### Parameters

| Name              | Type                              | Description | Required    | Notes |
| ----------------- | --------------------------------- | ----------- | ----------- | ----- |
| **authorization** | **String**                        |             | \[required] |       |
| **cosmos\_input** | [**CosmosInput**](CosmosInput.md) |             | \[required] |       |

### Return type

[**crate::models::AccountApiResponse**](docs/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](CosmosApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## get\_cosmos\_account

> crate::models::AccountApiResponse get\_cosmos\_account(authorization, account\_name)

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

[\[Back to top\]](CosmosApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## list\_cosmos\_accounts

> crate::models::AccountApiResponse list\_cosmos\_accounts(authorization)

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

[\[Back to top\]](CosmosApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## sign\_cosmos\_transaction

> crate::models::CosmosApiResponse sign\_cosmos\_transaction(authorization, account\_name, cosmos\_transaction\_input)

### Parameters

| Name                           | Type                                                    | Description | Required    | Notes |
| ------------------------------ | ------------------------------------------------------- | ----------- | ----------- | ----- |
| **authorization**              | **String**                                              |             | \[required] |       |
| **account\_name**              | **String**                                              |             | \[required] |       |
| **cosmos\_transaction\_input** | [**CosmosTransactionInput**](CosmosTransactionInput.md) |             | \[required] |       |

### Return type

[**crate::models::CosmosApiResponse**](docs/CosmosAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](CosmosApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
