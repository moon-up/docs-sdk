# \OnramperApi

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                                                                                  | HTTP request                           | Description |
| ----------------------------------------------------------------------------------------------------------------------- | -------------------------------------- | ----------- |
| [**on\_ramper\_checkout**](onramperapi.md#on\_ramper\_checkout)                                                         | **POST** /onramper/fund/${accountName} |             |
| [**on\_ramper\_get\_quotes\_buy**](onramperapi.md#on\_ramper\_get\_quotes\_buy)                                         | **GET** /onramper/quotes/buy           |             |
| [**on\_ramper\_get\_quotes\_sell**](onramperapi.md#on\_ramper\_get\_quotes\_sell)                                       | **GET** /onramper/quotes/sell          |             |
| [**on\_ramper\_get\_supported\_assets**](onramperapi.md#on\_ramper\_get\_supported\_assets)                             | **GET** /onramper/assets               |             |
| [**on\_ramper\_get\_supported\_currencies**](onramperapi.md#on\_ramper\_get\_supported\_currencies)                     | **GET** /onramper/currencies           |             |
| [**on\_ramper\_get\_supported\_defaults\_all**](onramperapi.md#on\_ramper\_get\_supported\_defaults\_all)               | **GET** /onramper/defaults             |             |
| [**on\_ramper\_get\_supported\_on\_ramps\_all**](onramperapi.md#on\_ramper\_get\_supported\_on\_ramps\_all)             | **GET** /onramper/onramps              |             |
| [**on\_ramper\_get\_supported\_payment\_types**](onramperapi.md#on\_ramper\_get\_supported\_payment\_types)             | **GET** /onramper/payment-types        |             |
| [**on\_ramper\_get\_supported\_payment\_types\_fiat**](onramperapi.md#on\_ramper\_get\_supported\_payment\_types\_fiat) | **GET** /onramper/payment-types/fiat   |             |

## on\_ramper\_checkout

> serde\_json::Value on\_ramper\_checkout(authorization, account\_name, transaction\_input)

### Parameters

| Name                   | Type                                        | Description | Required    | Notes |
| ---------------------- | ------------------------------------------- | ----------- | ----------- | ----- |
| **authorization**      | **String**                                  |             | \[required] |       |
| **account\_name**      | **String**                                  |             | \[required] |       |
| **transaction\_input** | [**TransactionInput**](transactioninput.md) |             | \[required] |       |

### Return type

[**serde\_json::Value**](../../rust/docs/serde\_json::Value.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](onramperapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## on\_ramper\_get\_quotes\_buy

> Vec[crate::models::Quote](crate::models::Quote) on\_ramper\_get\_quotes\_buy(authorization, fiat, crypto, amount, payment\_method, uuid, client\_name, country)

### Parameters

| Name                | Type               | Description | Required    | Notes                    |
| ------------------- | ------------------ | ----------- | ----------- | ------------------------ |
| **authorization**   | **String**         |             | \[required] |                          |
| **fiat**            | **String**         |             | \[required] |                          |
| **crypto**          | **String**         |             | \[required] |                          |
| **amount**          | **f64**            |             | \[required] |                          |
| **payment\_method** | Option<**String**> |             |             | \[default to creditcard] |
| **uuid**            | Option<**String**> |             |             | \[default to ]           |
| **client\_name**    | Option<**String**> |             |             | \[default to ]           |
| **country**         | Option<**String**> |             |             | \[default to ]           |

### Return type

[**Vec**](quote.md)[**crate::models::Quote**](crate::models::Quote)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](onramperapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## on\_ramper\_get\_quotes\_sell

> Vec[crate::models::SellQuote](crate::models::SellQuote) on\_ramper\_get\_quotes\_sell(authorization, fiat, crypto, amount, payment\_method, uuid, client\_name, country)

### Parameters

| Name                | Type               | Description | Required    | Notes                    |
| ------------------- | ------------------ | ----------- | ----------- | ------------------------ |
| **authorization**   | **String**         |             | \[required] |                          |
| **fiat**            | **String**         |             | \[required] |                          |
| **crypto**          | **String**         |             | \[required] |                          |
| **amount**          | **f64**            |             | \[required] |                          |
| **payment\_method** | Option<**String**> |             |             | \[default to creditcard] |
| **uuid**            | Option<**String**> |             |             | \[default to ]           |
| **client\_name**    | Option<**String**> |             |             | \[default to ]           |
| **country**         | Option<**String**> |             |             | \[default to ]           |

### Return type

[**Vec**](sellquote.md)[**crate::models::SellQuote**](crate::models::SellQuote)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](onramperapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## on\_ramper\_get\_supported\_assets

> crate::models::SupportedAssetResponse on\_ramper\_get\_supported\_assets(authorization, source, country)

### Parameters

| Name              | Type       | Description | Required    | Notes |
| ----------------- | ---------- | ----------- | ----------- | ----- |
| **authorization** | **String** |             | \[required] |       |
| **source**        | **String** |             | \[required] |       |
| **country**       | **String** |             | \[required] |       |

### Return type

[**crate::models::SupportedAssetResponse**](supportedassetresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](onramperapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## on\_ramper\_get\_supported\_currencies

> crate::models::SupportedCurrenciesResponse on\_ramper\_get\_supported\_currencies(authorization, r#type)

### Parameters

| Name              | Type       | Description | Required    | Notes |
| ----------------- | ---------- | ----------- | ----------- | ----- |
| **authorization** | **String** |             | \[required] |       |
| **r#type**        | **String** |             | \[required] |       |

### Return type

[**crate::models::SupportedCurrenciesResponse**](supportedcurrenciesresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](onramperapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## on\_ramper\_get\_supported\_defaults\_all

> crate::models::SupportedDefaultResponse on\_ramper\_get\_supported\_defaults\_all(authorization, country, r#type)

### Parameters

| Name              | Type       | Description | Required    | Notes |
| ----------------- | ---------- | ----------- | ----------- | ----- |
| **authorization** | **String** |             | \[required] |       |
| **country**       | **String** |             | \[required] |       |
| **r#type**        | **String** |             | \[required] |       |

### Return type

[**crate::models::SupportedDefaultResponse**](supporteddefaultresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](onramperapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## on\_ramper\_get\_supported\_on\_ramps\_all

> crate::models::GetSupportedOnRampsResponse on\_ramper\_get\_supported\_on\_ramps\_all(authorization)

### Parameters

| Name              | Type       | Description | Required    | Notes |
| ----------------- | ---------- | ----------- | ----------- | ----- |
| **authorization** | **String** |             | \[required] |       |

### Return type

[**crate::models::GetSupportedOnRampsResponse**](getsupportedonrampsresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](onramperapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## on\_ramper\_get\_supported\_payment\_types

> crate::models::SupportedPaymentTypesCurrencyResponse on\_ramper\_get\_supported\_payment\_types(authorization, fiat, country, r#type)

### Parameters

| Name              | Type       | Description | Required    | Notes |
| ----------------- | ---------- | ----------- | ----------- | ----- |
| **authorization** | **String** |             | \[required] |       |
| **fiat**          | **String** |             | \[required] |       |
| **country**       | **String** |             | \[required] |       |
| **r#type**        | **String** |             | \[required] |       |

### Return type

[**crate::models::SupportedPaymentTypesCurrencyResponse**](supportedpaymenttypescurrencyresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](onramperapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## on\_ramper\_get\_supported\_payment\_types\_fiat

> crate::models::SupportedPaymentTypesCurrencyResponse on\_ramper\_get\_supported\_payment\_types\_fiat(authorization, fiat, country)

### Parameters

| Name              | Type       | Description | Required    | Notes |
| ----------------- | ---------- | ----------- | ----------- | ----- |
| **authorization** | **String** |             | \[required] |       |
| **fiat**          | **String** |             | \[required] |       |
| **country**       | **String** |             | \[required] |       |

### Return type

[**crate::models::SupportedPaymentTypesCurrencyResponse**](supportedpaymenttypescurrencyresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](onramperapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
