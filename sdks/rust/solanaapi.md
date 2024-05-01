# \SolanaApi

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                                  | HTTP request                           | Description |
| ----------------------------------------------------------------------- | -------------------------------------- | ----------- |
| [**create\_solana\_account**](solanaapi.md#create\_solana\_account)     | **POST** /solana                       |             |
| [**get\_solana\_account**](solanaapi.md#get\_solana\_account)           | **GET** /solana/{accountName}          |             |
| [**list\_solana\_accounts**](solanaapi.md#list\_solana\_accounts)       | **GET** /solana                        |             |
| [**sign\_solana\_transaction**](solanaapi.md#sign\_solana\_transaction) | **POST** /solana/{accountName}/sign-tx |             |

## create\_solana\_account

> crate::models::AccountApiResponse create\_solana\_account(authorization, solana\_input)

### Parameters

| Name              | Type                              | Description | Required    | Notes |
| ----------------- | --------------------------------- | ----------- | ----------- | ----- |
| **authorization** | **String**                        |             | \[required] |       |
| **solana\_input** | [**SolanaInput**](solanainput.md) |             | \[required] |       |

### Return type

[**crate::models::AccountApiResponse**](../../rust/docs/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](solanaapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## get\_solana\_account

> crate::models::AccountApiResponse get\_solana\_account(authorization, account\_name)

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

[\[Back to top\]](solanaapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## list\_solana\_accounts

> crate::models::AccountApiResponse list\_solana\_accounts(authorization)

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

[\[Back to top\]](solanaapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## sign\_solana\_transaction

> crate::models::SolanaApiResponse sign\_solana\_transaction(authorization, account\_name, solana\_transaction\_input)

### Parameters

| Name                           | Type                                                    | Description | Required    | Notes |
| ------------------------------ | ------------------------------------------------------- | ----------- | ----------- | ----- |
| **authorization**              | **String**                                              |             | \[required] |       |
| **account\_name**              | **String**                                              |             | \[required] |       |
| **solana\_transaction\_input** | [**SolanaTransactionInput**](solanatransactioninput.md) |             | \[required] |       |

### Return type

[**crate::models::SolanaApiResponse**](../../rust/docs/SolanaAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](solanaapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
