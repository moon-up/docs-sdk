# \AccountsApi

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                    | HTTP request                                      | Description |
| --------------------------------------------------------- | ------------------------------------------------- | ----------- |
| [**broadcast\_tx**](accountsapi.md#broadcast\_tx)         | **POST** /accounts/{accountName}/broadcast-tx     |             |
| [**create\_account**](accountsapi.md#create\_account)     | **POST** /accounts                                |             |
| [**delete\_account**](accountsapi.md#delete\_account)     | **DELETE** /accounts/{accountName}                |             |
| [**deploy\_contract**](accountsapi.md#deploy\_contract)   | **POST** /accounts/{accountName}/deploy           |             |
| [**get\_account**](accountsapi.md#get\_account)           | **GET** /accounts/{accountName}                   |             |
| [**get\_balance**](accountsapi.md#get\_balance)           | **GET** /accounts/{accountName}/balance           |             |
| [**get\_nonce**](accountsapi.md#get\_nonce)               | **GET** /accounts/{accountName}/nonce             |             |
| [**list\_accounts**](accountsapi.md#list\_accounts)       | **GET** /accounts                                 |             |
| [**sign\_message**](accountsapi.md#sign\_message)         | **POST** /accounts/{accountName}/sign-message     |             |
| [**sign\_transaction**](accountsapi.md#sign\_transaction) | **POST** /accounts/{accountName}/sign-transaction |             |
| [**sign\_typed\_data**](accountsapi.md#sign\_typed\_data) | **POST** /accounts/{accountName}/sign-typed-data  |             |
| [**transfer\_eth**](accountsapi.md#transfer\_eth)         | **POST** /accounts/{accountName}/transfer-eth     |             |

## broadcast\_tx

> crate::models::BroadCastRawTransactionApiResponse broadcast\_tx(authorization, account\_name, broadcast\_input)

### Parameters

| Name                 | Type                                    | Description | Required    | Notes |
| -------------------- | --------------------------------------- | ----------- | ----------- | ----- |
| **authorization**    | **String**                              |             | \[required] |       |
| **account\_name**    | **String**                              |             | \[required] |       |
| **broadcast\_input** | [**BroadcastInput**](broadcastinput.md) |             | \[required] |       |

### Return type

[**crate::models::BroadCastRawTransactionApiResponse**](../../rust/docs/BroadCastRawTransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## create\_account

> crate::models::AccountApiResponse create\_account(authorization, create\_account\_input)

### Parameters

| Name                       | Type                                            | Description | Required    | Notes |
| -------------------------- | ----------------------------------------------- | ----------- | ----------- | ----- |
| **authorization**          | **String**                                      |             | \[required] |       |
| **create\_account\_input** | [**CreateAccountInput**](createaccountinput.md) |             | \[required] |       |

### Return type

[**crate::models::AccountApiResponse**](../../rust/docs/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## delete\_account

> crate::models::AccountApiResponse delete\_account(authorization, account\_name)

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

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## deploy\_contract

> crate::models::TransactionApiResponse deploy\_contract(authorization, account\_name, deploy\_input)

### Parameters

| Name              | Type                              | Description | Required    | Notes |
| ----------------- | --------------------------------- | ----------- | ----------- | ----- |
| **authorization** | **String**                        |             | \[required] |       |
| **account\_name** | **String**                        |             | \[required] |       |
| **deploy\_input** | [**DeployInput**](deployinput.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](../../rust/docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## get\_account

> crate::models::AccountApiResponse get\_account(authorization, account\_name)

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

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## get\_balance

> crate::models::BalanceApiResponse get\_balance(account\_name, authorization, chain\_id)

### Parameters

| Name              | Type       | Description | Required    | Notes |
| ----------------- | ---------- | ----------- | ----------- | ----- |
| **account\_name** | **String** |             | \[required] |       |
| **authorization** | **String** |             | \[required] |       |
| **chain\_id**     | **String** |             | \[required] |       |

### Return type

[**crate::models::BalanceApiResponse**](../../rust/docs/BalanceAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## get\_nonce

> crate::models::NonceApiResponse get\_nonce(account\_name, authorization)

### Parameters

| Name              | Type       | Description | Required    | Notes |
| ----------------- | ---------- | ----------- | ----------- | ----- |
| **account\_name** | **String** |             | \[required] |       |
| **authorization** | **String** |             | \[required] |       |

### Return type

[**crate::models::NonceApiResponse**](../../rust/docs/NonceAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## list\_accounts

> crate::models::AccountApiResponse list\_accounts(authorization)

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

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## sign\_message

> crate::models::SignMessageApiResponse sign\_message(account\_name, authorization, sign\_message)

### Parameters

| Name              | Type                              | Description | Required    | Notes |
| ----------------- | --------------------------------- | ----------- | ----------- | ----- |
| **account\_name** | **String**                        |             | \[required] |       |
| **authorization** | **String**                        |             | \[required] |       |
| **sign\_message** | [**SignMessage**](signmessage.md) |             | \[required] |       |

### Return type

[**crate::models::SignMessageApiResponse**](../../rust/docs/SignMessageAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## sign\_transaction

> crate::models::TransactionApiResponse sign\_transaction(account\_name, authorization, input\_body)

### Parameters

| Name              | Type                          | Description | Required    | Notes |
| ----------------- | ----------------------------- | ----------- | ----------- | ----- |
| **account\_name** | **String**                    |             | \[required] |       |
| **authorization** | **String**                    |             | \[required] |       |
| **input\_body**   | [**InputBody**](inputbody.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](../../rust/docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## sign\_typed\_data

> crate::models::SignMessageApiResponse sign\_typed\_data(account\_name, authorization, sign\_typed\_data)

### Parameters

| Name                  | Type                                  | Description | Required    | Notes |
| --------------------- | ------------------------------------- | ----------- | ----------- | ----- |
| **account\_name**     | **String**                            |             | \[required] |       |
| **authorization**     | **String**                            |             | \[required] |       |
| **sign\_typed\_data** | [**SignTypedData**](signtypeddata.md) |             | \[required] |       |

### Return type

[**crate::models::SignMessageApiResponse**](../../rust/docs/SignMessageAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## transfer\_eth

> crate::models::TransactionApiResponse transfer\_eth(account\_name, authorization, input\_body)

### Parameters

| Name              | Type                          | Description | Required    | Notes |
| ----------------- | ----------------------------- | ----------- | ----------- | ----- |
| **account\_name** | **String**                    |             | \[required] |       |
| **authorization** | **String**                    |             | \[required] |       |
| **input\_body**   | [**InputBody**](inputbody.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](../../rust/docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
