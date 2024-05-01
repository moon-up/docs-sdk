# OnramperApi

## OnramperApi

All URIs are relative to _https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app_

| Method                                                                                          | HTTP request                           | Description |
| ----------------------------------------------------------------------------------------------- | -------------------------------------- | ----------- |
| [**onRamperCheckout**](onramperapi.md#onRamperCheckout)                                         | **POST** /onramper/fund/${accountName} |             |
| [**onRamperGetQuotesBuy**](onramperapi.md#onRamperGetQuotesBuy)                                 | **GET** /onramper/quotes/buy           |             |
| [**onRamperGetQuotesSell**](onramperapi.md#onRamperGetQuotesSell)                               | **GET** /onramper/quotes/sell          |             |
| [**onRamperGetSupportedAssets**](onramperapi.md#onRamperGetSupportedAssets)                     | **GET** /onramper/assets               |             |
| [**onRamperGetSupportedCurrencies**](onramperapi.md#onRamperGetSupportedCurrencies)             | **GET** /onramper/currencies           |             |
| [**onRamperGetSupportedDefaultsAll**](onramperapi.md#onRamperGetSupportedDefaultsAll)           | **GET** /onramper/defaults             |             |
| [**onRamperGetSupportedOnRampsAll**](onramperapi.md#onRamperGetSupportedOnRampsAll)             | **GET** /onramper/onramps              |             |
| [**onRamperGetSupportedPaymentTypes**](onramperapi.md#onRamperGetSupportedPaymentTypes)         | **GET** /onramper/payment-types        |             |
| [**onRamperGetSupportedPaymentTypesFiat**](onramperapi.md#onRamperGetSupportedPaymentTypesFiat) | **GET** /onramper/payment-types/fiat   |             |

## **onRamperCheckout**

> kotlin.Any onRamperCheckout(authorization, accountName, transactionInput)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = OnramperApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val accountName : kotlin.String = accountName_example // kotlin.String | 
val transactionInput : TransactionInput =  // TransactionInput | 
try {
    val result : kotlin.Any = apiInstance.onRamperCheckout(authorization, accountName, transactionInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OnramperApi#onRamperCheckout")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OnramperApi#onRamperCheckout")
    e.printStackTrace()
}
```

#### Parameters

| Name                 | Type                                        | Description | Notes |
| -------------------- | ------------------------------------------- | ----------- | ----- |
| **authorization**    | **kotlin.String**                           |             |       |
| **accountName**      | **kotlin.String**                           |             |       |
| **transactionInput** | [**TransactionInput**](transactioninput.md) |             |       |

#### Return type

[**kotlin.Any**](../../kotlin/docs/kotlin.Any.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **onRamperGetQuotesBuy**

> kotlin.collections.List\<Quote> onRamperGetQuotesBuy(authorization, fiat, crypto, amount, paymentMethod, uuid, clientName, country)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = OnramperApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val fiat : kotlin.String = fiat_example // kotlin.String | 
val crypto : kotlin.String = crypto_example // kotlin.String | 
val amount : kotlin.Double = 1.2 // kotlin.Double | 
val paymentMethod : kotlin.String = paymentMethod_example // kotlin.String | 
val uuid : kotlin.String = uuid_example // kotlin.String | 
val clientName : kotlin.String = clientName_example // kotlin.String | 
val country : kotlin.String = country_example // kotlin.String | 
try {
    val result : kotlin.collections.List<Quote> = apiInstance.onRamperGetQuotesBuy(authorization, fiat, crypto, amount, paymentMethod, uuid, clientName, country)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OnramperApi#onRamperGetQuotesBuy")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OnramperApi#onRamperGetQuotesBuy")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type              | Description | Notes                                  |
| ----------------- | ----------------- | ----------- | -------------------------------------- |
| **authorization** | **kotlin.String** |             |                                        |
| **fiat**          | **kotlin.String** |             |                                        |
| **crypto**        | **kotlin.String** |             |                                        |
| **amount**        | **kotlin.Double** |             |                                        |
| **paymentMethod** | **kotlin.String** |             | \[optional] \[default to "creditcard"] |
| **uuid**          | **kotlin.String** |             | \[optional] \[default to ""]           |
| **clientName**    | **kotlin.String** |             | \[optional] \[default to ""]           |
| **country**       | **kotlin.String** |             | \[optional] \[default to ""]           |

#### Return type

[**kotlin.collections.List\<Quote>**](quote.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

## **onRamperGetQuotesSell**

> kotlin.collections.List\<SellQuote> onRamperGetQuotesSell(authorization, fiat, crypto, amount, paymentMethod, uuid, clientName, country)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = OnramperApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val fiat : kotlin.String = fiat_example // kotlin.String | 
val crypto : kotlin.String = crypto_example // kotlin.String | 
val amount : kotlin.Double = 1.2 // kotlin.Double | 
val paymentMethod : kotlin.String = paymentMethod_example // kotlin.String | 
val uuid : kotlin.String = uuid_example // kotlin.String | 
val clientName : kotlin.String = clientName_example // kotlin.String | 
val country : kotlin.String = country_example // kotlin.String | 
try {
    val result : kotlin.collections.List<SellQuote> = apiInstance.onRamperGetQuotesSell(authorization, fiat, crypto, amount, paymentMethod, uuid, clientName, country)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OnramperApi#onRamperGetQuotesSell")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OnramperApi#onRamperGetQuotesSell")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type              | Description | Notes                                  |
| ----------------- | ----------------- | ----------- | -------------------------------------- |
| **authorization** | **kotlin.String** |             |                                        |
| **fiat**          | **kotlin.String** |             |                                        |
| **crypto**        | **kotlin.String** |             |                                        |
| **amount**        | **kotlin.Double** |             |                                        |
| **paymentMethod** | **kotlin.String** |             | \[optional] \[default to "creditcard"] |
| **uuid**          | **kotlin.String** |             | \[optional] \[default to ""]           |
| **clientName**    | **kotlin.String** |             | \[optional] \[default to ""]           |
| **country**       | **kotlin.String** |             | \[optional] \[default to ""]           |

#### Return type

[**kotlin.collections.List\<SellQuote>**](sellquote.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

## **onRamperGetSupportedAssets**

> SupportedAssetResponse onRamperGetSupportedAssets(authorization, source, country)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = OnramperApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val source : kotlin.String = source_example // kotlin.String | 
val country : kotlin.String = country_example // kotlin.String | 
try {
    val result : SupportedAssetResponse = apiInstance.onRamperGetSupportedAssets(authorization, source, country)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OnramperApi#onRamperGetSupportedAssets")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OnramperApi#onRamperGetSupportedAssets")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type              | Description | Notes |
| ----------------- | ----------------- | ----------- | ----- |
| **authorization** | **kotlin.String** |             |       |
| **source**        | **kotlin.String** |             |       |
| **country**       | **kotlin.String** |             |       |

#### Return type

[**SupportedAssetResponse**](supportedassetresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

## **onRamperGetSupportedCurrencies**

> SupportedCurrenciesResponse onRamperGetSupportedCurrencies(authorization, type)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = OnramperApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val type : kotlin.String = type_example // kotlin.String | 
try {
    val result : SupportedCurrenciesResponse = apiInstance.onRamperGetSupportedCurrencies(authorization, type)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OnramperApi#onRamperGetSupportedCurrencies")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OnramperApi#onRamperGetSupportedCurrencies")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type              | Description | Notes |
| ----------------- | ----------------- | ----------- | ----- |
| **authorization** | **kotlin.String** |             |       |
| **type**          | **kotlin.String** |             |       |

#### Return type

[**SupportedCurrenciesResponse**](supportedcurrenciesresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

## **onRamperGetSupportedDefaultsAll**

> SupportedDefaultResponse onRamperGetSupportedDefaultsAll(authorization, country, type)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = OnramperApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val country : kotlin.String = country_example // kotlin.String | 
val type : kotlin.String = type_example // kotlin.String | 
try {
    val result : SupportedDefaultResponse = apiInstance.onRamperGetSupportedDefaultsAll(authorization, country, type)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OnramperApi#onRamperGetSupportedDefaultsAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OnramperApi#onRamperGetSupportedDefaultsAll")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type              | Description | Notes |
| ----------------- | ----------------- | ----------- | ----- |
| **authorization** | **kotlin.String** |             |       |
| **country**       | **kotlin.String** |             |       |
| **type**          | **kotlin.String** |             |       |

#### Return type

[**SupportedDefaultResponse**](supporteddefaultresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

## **onRamperGetSupportedOnRampsAll**

> GetSupportedOnRampsResponse onRamperGetSupportedOnRampsAll(authorization)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = OnramperApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
try {
    val result : GetSupportedOnRampsResponse = apiInstance.onRamperGetSupportedOnRampsAll(authorization)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OnramperApi#onRamperGetSupportedOnRampsAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OnramperApi#onRamperGetSupportedOnRampsAll")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type              | Description | Notes |
| ----------------- | ----------------- | ----------- | ----- |
| **authorization** | **kotlin.String** |             |       |

#### Return type

[**GetSupportedOnRampsResponse**](getsupportedonrampsresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

## **onRamperGetSupportedPaymentTypes**

> SupportedPaymentTypesCurrencyResponse onRamperGetSupportedPaymentTypes(authorization, fiat, country, type)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = OnramperApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val fiat : kotlin.String = fiat_example // kotlin.String | 
val country : kotlin.String = country_example // kotlin.String | 
val type : kotlin.String = type_example // kotlin.String | 
try {
    val result : SupportedPaymentTypesCurrencyResponse = apiInstance.onRamperGetSupportedPaymentTypes(authorization, fiat, country, type)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OnramperApi#onRamperGetSupportedPaymentTypes")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OnramperApi#onRamperGetSupportedPaymentTypes")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type              | Description | Notes |
| ----------------- | ----------------- | ----------- | ----- |
| **authorization** | **kotlin.String** |             |       |
| **fiat**          | **kotlin.String** |             |       |
| **country**       | **kotlin.String** |             |       |
| **type**          | **kotlin.String** |             |       |

#### Return type

[**SupportedPaymentTypesCurrencyResponse**](supportedpaymenttypescurrencyresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

## **onRamperGetSupportedPaymentTypesFiat**

> SupportedPaymentTypesCurrencyResponse onRamperGetSupportedPaymentTypesFiat(authorization, fiat, country)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = OnramperApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val fiat : kotlin.String = fiat_example // kotlin.String | 
val country : kotlin.String = country_example // kotlin.String | 
try {
    val result : SupportedPaymentTypesCurrencyResponse = apiInstance.onRamperGetSupportedPaymentTypesFiat(authorization, fiat, country)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OnramperApi#onRamperGetSupportedPaymentTypesFiat")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OnramperApi#onRamperGetSupportedPaymentTypesFiat")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type              | Description | Notes |
| ----------------- | ----------------- | ----------- | ----- |
| **authorization** | **kotlin.String** |             |       |
| **fiat**          | **kotlin.String** |             |       |
| **country**       | **kotlin.String** |             |       |

#### Return type

[**SupportedPaymentTypesCurrencyResponse**](supportedpaymenttypescurrencyresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json
