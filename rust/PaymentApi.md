# \PaymentApi

All URIs are relative to _https://vault-api.usemoon.ai_

| Method                                                                                       | HTTP request                         | Description |
| -------------------------------------------------------------------------------------------- | ------------------------------------ | ----------- |
| [**create\_payment\_intent\_config**](PaymentApi.md#create\_payment\_intent\_config)         | **POST** /payment/config             |             |
| [**delete\_payment\_intent\_config**](PaymentApi.md#delete\_payment\_intent\_config)         | **DELETE** /payment/config/{id}      |             |
| [**get\_all\_payment\_intent\_configs**](PaymentApi.md#get\_all\_payment\_intent\_configs)   | **GET** /payment/config              |             |
| [**get\_one\_payment\_intent\_configs**](PaymentApi.md#get\_one\_payment\_intent\_configs)   | **GET** /payment/config/{id}         |             |
| [**moralis\_webhook**](PaymentApi.md#moralis\_webhook)                                       | **POST** /payment/webhook/{id}       |             |
| [**payment\_create\_payment\_intent**](PaymentApi.md#payment\_create\_payment\_intent)       | **POST** /payment                    |             |
| [**payment\_delete\_payment\_intent**](PaymentApi.md#payment\_delete\_payment\_intent)       | **DELETE** /payment/{id}             |             |
| [**payment\_get\_all\_payment\_intents**](PaymentApi.md#payment\_get\_all\_payment\_intents) | **GET** /payment                     |             |
| [**payment\_get\_available\_chains**](PaymentApi.md#payment\_get\_available\_chains)         | **GET** /payment/chains              |             |
| [**payment\_get\_payment\_intent**](PaymentApi.md#payment\_get\_payment\_intent)             | **GET** /payment/{id}                |             |
| [**payment\_update\_payment\_intent**](PaymentApi.md#payment\_update\_payment\_intent)       | **PUT** /payment/{id}                |             |
| [**tatum\_webhook**](PaymentApi.md#tatum\_webhook)                                           | **POST** /payment/webhook/tatum/{id} |             |
| [**update\_payment\_intent\_config**](PaymentApi.md#update\_payment\_intent\_config)         | **PUT** /payment/config/{id}         |             |

## create\_payment\_intent\_config

> serde\_json::Value create\_payment\_intent\_config(authorization, body)

### Parameters

| Name              | Type                           | Description | Required    | Notes |
| ----------------- | ------------------------------ | ----------- | ----------- | ----- |
| **authorization** | **String**                     |             | \[required] |       |
| **body**          | Option<**serde\_json::Value**> |             | \[required] |       |

### Return type

[**serde\_json::Value**](docs/serde\_json::Value.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](PaymentApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## delete\_payment\_intent\_config

> crate::models::PaymentIntentResponse delete\_payment\_intent\_config(authorization, id)

### Parameters

| Name              | Type       | Description | Required    | Notes |
| ----------------- | ---------- | ----------- | ----------- | ----- |
| **authorization** | **String** |             | \[required] |       |
| **id**            | **String** |             | \[required] |       |

### Return type

[**crate::models::PaymentIntentResponse**](PaymentIntentResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](PaymentApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## get\_all\_payment\_intent\_configs

> Vec[crate::models::PaymentIntentResponse](crate::models::PaymentIntentResponse) get\_all\_payment\_intent\_configs(authorization)

### Parameters

| Name              | Type       | Description | Required    | Notes |
| ----------------- | ---------- | ----------- | ----------- | ----- |
| **authorization** | **String** |             | \[required] |       |

### Return type

[**Vec**](PaymentIntentResponse.md)[**crate::models::PaymentIntentResponse**](crate::models::PaymentIntentResponse)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](PaymentApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## get\_one\_payment\_intent\_configs

> crate::models::PaymentIntentResponse get\_one\_payment\_intent\_configs(authorization, id)

### Parameters

| Name              | Type       | Description | Required    | Notes |
| ----------------- | ---------- | ----------- | ----------- | ----- |
| **authorization** | **String** |             | \[required] |       |
| **id**            | **String** |             | \[required] |       |

### Return type

[**crate::models::PaymentIntentResponse**](PaymentIntentResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](PaymentApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## moralis\_webhook

> serde\_json::Value moralis\_webhook(id, i\_webhook)

### Parameters

| Name           | Type                        | Description | Required    | Notes |
| -------------- | --------------------------- | ----------- | ----------- | ----- |
| **id**         | **String**                  |             | \[required] |       |
| **i\_webhook** | [**IWebhook**](IWebhook.md) |             | \[required] |       |

### Return type

[**serde\_json::Value**](docs/serde\_json::Value.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](PaymentApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## payment\_create\_payment\_intent

> crate::models::PaymentIntentResponse payment\_create\_payment\_intent(authorization, create\_payment\_intent\_input)

### Parameters

| Name                               | Type                                                        | Description | Required    | Notes |
| ---------------------------------- | ----------------------------------------------------------- | ----------- | ----------- | ----- |
| **authorization**                  | **String**                                                  |             | \[required] |       |
| **create\_payment\_intent\_input** | [**CreatePaymentIntentInput**](CreatePaymentIntentInput.md) |             | \[required] |       |

### Return type

[**crate::models::PaymentIntentResponse**](PaymentIntentResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](PaymentApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## payment\_delete\_payment\_intent

> crate::models::PaymentIntentResponse payment\_delete\_payment\_intent(authorization, id)

### Parameters

| Name              | Type       | Description | Required    | Notes |
| ----------------- | ---------- | ----------- | ----------- | ----- |
| **authorization** | **String** |             | \[required] |       |
| **id**            | **String** |             | \[required] |       |

### Return type

[**crate::models::PaymentIntentResponse**](PaymentIntentResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](PaymentApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## payment\_get\_all\_payment\_intents

> Vec[crate::models::PaymentIntentResponse](crate::models::PaymentIntentResponse) payment\_get\_all\_payment\_intents(authorization)

### Parameters

| Name              | Type       | Description | Required    | Notes |
| ----------------- | ---------- | ----------- | ----------- | ----- |
| **authorization** | **String** |             | \[required] |       |

### Return type

[**Vec**](PaymentIntentResponse.md)[**crate::models::PaymentIntentResponse**](crate::models::PaymentIntentResponse)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](PaymentApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## payment\_get\_available\_chains

> Vec payment\_get\_available\_chains()

### Parameters

This endpoint does not need any parameter.

### Return type

**Vec**

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](PaymentApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## payment\_get\_payment\_intent

> crate::models::PaymentIntentResponse payment\_get\_payment\_intent(authorization, id)

### Parameters

| Name              | Type       | Description | Required    | Notes |
| ----------------- | ---------- | ----------- | ----------- | ----- |
| **authorization** | **String** |             | \[required] |       |
| **id**            | **String** |             | \[required] |       |

### Return type

[**crate::models::PaymentIntentResponse**](PaymentIntentResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](PaymentApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## payment\_update\_payment\_intent

> crate::models::PaymentIntentResponse payment\_update\_payment\_intent(authorization, id, create\_payment\_intent\_input)

### Parameters

| Name                               | Type                                                        | Description | Required    | Notes |
| ---------------------------------- | ----------------------------------------------------------- | ----------- | ----------- | ----- |
| **authorization**                  | **String**                                                  |             | \[required] |       |
| **id**                             | **String**                                                  |             | \[required] |       |
| **create\_payment\_intent\_input** | [**CreatePaymentIntentInput**](CreatePaymentIntentInput.md) |             | \[required] |       |

### Return type

[**crate::models::PaymentIntentResponse**](PaymentIntentResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](PaymentApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## tatum\_webhook

> serde\_json::Value tatum\_webhook(id, tatum\_transaction\_event)

### Parameters

| Name                          | Type                                                  | Description | Required    | Notes |
| ----------------------------- | ----------------------------------------------------- | ----------- | ----------- | ----- |
| **id**                        | **String**                                            |             | \[required] |       |
| **tatum\_transaction\_event** | [**TatumTransactionEvent**](TatumTransactionEvent.md) |             | \[required] |       |

### Return type

[**serde\_json::Value**](docs/serde\_json::Value.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](PaymentApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## update\_payment\_intent\_config

> crate::models::PaymentIntentResponse update\_payment\_intent\_config(authorization, id, body)

### Parameters

| Name              | Type                           | Description | Required    | Notes |
| ----------------- | ------------------------------ | ----------- | ----------- | ----- |
| **authorization** | **String**                     |             | \[required] |       |
| **id**            | **String**                     |             | \[required] |       |
| **body**          | Option<**serde\_json::Value**> |             | \[required] |       |

### Return type

[**crate::models::PaymentIntentResponse**](PaymentIntentResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](PaymentApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
