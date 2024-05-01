# \AccountsApi

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                    | HTTP request                                      | Description |
| --------------------------------------------------------- | ------------------------------------------------- | ----------- |
| [**broadcast\_tx**](AccountsApi.md#broadcast\_tx)         | **POST** /accounts/{accountName}/broadcast-tx     |             |
| [**create\_account**](AccountsApi.md#create\_account)     | **POST** /accounts                                |             |
| [**delete\_account**](AccountsApi.md#delete\_account)     | **DELETE** /accounts/{accountName}                |             |
| [**deploy\_contract**](AccountsApi.md#deploy\_contract)   | **POST** /accounts/{accountName}/deploy           |             |
| [**get\_account**](AccountsApi.md#get\_account)           | **GET** /accounts/{accountName}                   |             |
| [**get\_balance**](AccountsApi.md#get\_balance)           | **GET** /accounts/{accountName}/balance           |             |
| [**get\_nonce**](AccountsApi.md#get\_nonce)               | **GET** /accounts/{accountName}/nonce             |             |
| [**list\_accounts**](AccountsApi.md#list\_accounts)       | **GET** /accounts                                 |             |
| [**sign\_message**](AccountsApi.md#sign\_message)         | **POST** /accounts/{accountName}/sign-message     |             |
| [**sign\_transaction**](AccountsApi.md#sign\_transaction) | **POST** /accounts/{accountName}/sign-transaction |             |
| [**sign\_typed\_data**](AccountsApi.md#sign\_typed\_data) | **POST** /accounts/{accountName}/sign-typed-data  |             |
| [**transfer\_eth**](AccountsApi.md#transfer\_eth)         | **POST** /accounts/{accountName}/transfer-eth     |             |

## broadcast\_tx

> crate::models::BroadCastRawTransactionApiResponse broadcast\_tx(authorization, account\_name, broadcast\_input)

### Parameters

| Name                 | Type                                    | Description | Required    | Notes |
| -------------------- | --------------------------------------- | ----------- | ----------- | ----- |
| **authorization**    | **String**                              |             | \[required] |       |
| **account\_name**    | **String**                              |             | \[required] |       |
| **broadcast\_input** | [**BroadcastInput**](BroadcastInput.md) |             | \[required] |       |

### Return type

[**crate::models::BroadCastRawTransactionApiResponse**](docs/BroadCastRawTransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](AccountsApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## create\_account

> crate::models::AccountApiResponse create\_account(authorization, create\_account\_input)

### Parameters

| Name                       | Type                                            | Description | Required    | Notes |
| -------------------------- | ----------------------------------------------- | ----------- | ----------- | ----- |
| **authorization**          | **String**                                      |             | \[required] |       |
| **create\_account\_input** | [**CreateAccountInput**](CreateAccountInput.md) |             | \[required] |       |

### Return type

[**crate::models::AccountApiResponse**](docs/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](AccountsApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## delete\_account

> crate::models::AccountApiResponse delete\_account(authorization, account\_name)

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

[\[Back to top\]](AccountsApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## deploy\_contract

> crate::models::TransactionApiResponse deploy\_contract(authorization, account\_name, deploy\_input)

### Parameters

| Name              | Type                              | Description | Required    | Notes |
| ----------------- | --------------------------------- | ----------- | ----------- | ----- |
| **authorization** | **String**                        |             | \[required] |       |
| **account\_name** | **String**                        |             | \[required] |       |
| **deploy\_input** | [**DeployInput**](DeployInput.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](AccountsApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## get\_account

> crate::models::AccountApiResponse get\_account(authorization, account\_name)

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

[\[Back to top\]](AccountsApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## get\_balance

> crate::models::BalanceApiResponse get\_balance(account\_name, authorization, chain\_id)

### Parameters

| Name              | Type       | Description | Required    | Notes |
| ----------------- | ---------- | ----------- | ----------- | ----- |
| **account\_name** | **String** |             | \[required] |       |
| **authorization** | **String** |             | \[required] |       |
| **chain\_id**     | **String** |             | \[required] |       |

### Return type

[**crate::models::BalanceApiResponse**](docs/BalanceAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](AccountsApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## get\_nonce

> crate::models::NonceApiResponse get\_nonce(account\_name, authorization)

### Parameters

| Name              | Type       | Description | Required    | Notes |
| ----------------- | ---------- | ----------- | ----------- | ----- |
| **account\_name** | **String** |             | \[required] |       |
| **authorization** | **String** |             | \[required] |       |

### Return type

[**crate::models::NonceApiResponse**](docs/NonceAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](AccountsApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## list\_accounts

> crate::models::AccountApiResponse list\_accounts(authorization)

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

[\[Back to top\]](AccountsApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## sign\_message

> crate::models::SignMessageApiResponse sign\_message(account\_name, authorization, sign\_message)

### Parameters

| Name              | Type                              | Description | Required    | Notes |
| ----------------- | --------------------------------- | ----------- | ----------- | ----- |
| **account\_name** | **String**                        |             | \[required] |       |
| **authorization** | **String**                        |             | \[required] |       |
| **sign\_message** | [**SignMessage**](SignMessage.md) |             | \[required] |       |

### Return type

[**crate::models::SignMessageApiResponse**](docs/SignMessageAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](AccountsApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## sign\_transaction

> crate::models::TransactionApiResponse sign\_transaction(account\_name, authorization, input\_body)

### Parameters

| Name              | Type                          | Description | Required    | Notes |
| ----------------- | ----------------------------- | ----------- | ----------- | ----- |
| **account\_name** | **String**                    |             | \[required] |       |
| **authorization** | **String**                    |             | \[required] |       |
| **input\_body**   | [**InputBody**](InputBody.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](AccountsApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## sign\_typed\_data

> crate::models::SignMessageApiResponse sign\_typed\_data(account\_name, authorization, sign\_typed\_data)

### Parameters

| Name                  | Type                                  | Description | Required    | Notes |
| --------------------- | ------------------------------------- | ----------- | ----------- | ----- |
| **account\_name**     | **String**                            |             | \[required] |       |
| **authorization**     | **String**                            |             | \[required] |       |
| **sign\_typed\_data** | [**SignTypedData**](SignTypedData.md) |             | \[required] |       |

### Return type

[**crate::models::SignMessageApiResponse**](docs/SignMessageAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](AccountsApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## transfer\_eth

> crate::models::TransactionApiResponse transfer\_eth(account\_name, authorization, input\_body)

### Parameters

| Name              | Type                          | Description | Required    | Notes |
| ----------------- | ----------------------------- | ----------- | ----------- | ----- |
| **account\_name** | **String**                    |             | \[required] |       |
| **authorization** | **String**                    |             | \[required] |       |
| **input\_body**   | [**InputBody**](InputBody.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](AccountsApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
