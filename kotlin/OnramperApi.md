# OnramperApi

All URIs are relative to *https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**onRamperCheckout**](OnramperApi.md#onRamperCheckout) | **POST** /onramper/fund/${accountName} | 
[**onRamperGetQuotesBuy**](OnramperApi.md#onRamperGetQuotesBuy) | **GET** /onramper/quotes/buy | 
[**onRamperGetQuotesSell**](OnramperApi.md#onRamperGetQuotesSell) | **GET** /onramper/quotes/sell | 
[**onRamperGetSupportedAssets**](OnramperApi.md#onRamperGetSupportedAssets) | **GET** /onramper/assets | 
[**onRamperGetSupportedCurrencies**](OnramperApi.md#onRamperGetSupportedCurrencies) | **GET** /onramper/currencies | 
[**onRamperGetSupportedDefaultsAll**](OnramperApi.md#onRamperGetSupportedDefaultsAll) | **GET** /onramper/defaults | 
[**onRamperGetSupportedOnRampsAll**](OnramperApi.md#onRamperGetSupportedOnRampsAll) | **GET** /onramper/onramps | 
[**onRamperGetSupportedPaymentTypes**](OnramperApi.md#onRamperGetSupportedPaymentTypes) | **GET** /onramper/payment-types | 
[**onRamperGetSupportedPaymentTypesFiat**](OnramperApi.md#onRamperGetSupportedPaymentTypesFiat) | **GET** /onramper/payment-types/fiat | 


<a id="onRamperCheckout"></a>
# **onRamperCheckout**
> kotlin.Any onRamperCheckout(authorization, accountName, transactionInput)



### Example
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

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **accountName** | **kotlin.String**|  |
 **transactionInput** | [**TransactionInput**](TransactionInput.md)|  |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.apiKey["x-api-key"] = ""
    ApiClient.apiKeyPrefix["x-api-key"] = ""
Configure BearerAuth:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="onRamperGetQuotesBuy"></a>
# **onRamperGetQuotesBuy**
> kotlin.collections.List&lt;Quote&gt; onRamperGetQuotesBuy(authorization, fiat, crypto, amount, paymentMethod, uuid, clientName, country)



### Example
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

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **fiat** | **kotlin.String**|  |
 **crypto** | **kotlin.String**|  |
 **amount** | **kotlin.Double**|  |
 **paymentMethod** | **kotlin.String**|  | [optional] [default to &quot;creditcard&quot;]
 **uuid** | **kotlin.String**|  | [optional] [default to &quot;&quot;]
 **clientName** | **kotlin.String**|  | [optional] [default to &quot;&quot;]
 **country** | **kotlin.String**|  | [optional] [default to &quot;&quot;]

### Return type

[**kotlin.collections.List&lt;Quote&gt;**](Quote.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.apiKey["x-api-key"] = ""
    ApiClient.apiKeyPrefix["x-api-key"] = ""
Configure BearerAuth:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="onRamperGetQuotesSell"></a>
# **onRamperGetQuotesSell**
> kotlin.collections.List&lt;SellQuote&gt; onRamperGetQuotesSell(authorization, fiat, crypto, amount, paymentMethod, uuid, clientName, country)



### Example
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

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **fiat** | **kotlin.String**|  |
 **crypto** | **kotlin.String**|  |
 **amount** | **kotlin.Double**|  |
 **paymentMethod** | **kotlin.String**|  | [optional] [default to &quot;creditcard&quot;]
 **uuid** | **kotlin.String**|  | [optional] [default to &quot;&quot;]
 **clientName** | **kotlin.String**|  | [optional] [default to &quot;&quot;]
 **country** | **kotlin.String**|  | [optional] [default to &quot;&quot;]

### Return type

[**kotlin.collections.List&lt;SellQuote&gt;**](SellQuote.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.apiKey["x-api-key"] = ""
    ApiClient.apiKeyPrefix["x-api-key"] = ""
Configure BearerAuth:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="onRamperGetSupportedAssets"></a>
# **onRamperGetSupportedAssets**
> SupportedAssetResponse onRamperGetSupportedAssets(authorization, source, country)



### Example
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

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **source** | **kotlin.String**|  |
 **country** | **kotlin.String**|  |

### Return type

[**SupportedAssetResponse**](SupportedAssetResponse.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.apiKey["x-api-key"] = ""
    ApiClient.apiKeyPrefix["x-api-key"] = ""
Configure BearerAuth:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="onRamperGetSupportedCurrencies"></a>
# **onRamperGetSupportedCurrencies**
> SupportedCurrenciesResponse onRamperGetSupportedCurrencies(authorization, type)



### Example
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

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **type** | **kotlin.String**|  |

### Return type

[**SupportedCurrenciesResponse**](SupportedCurrenciesResponse.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.apiKey["x-api-key"] = ""
    ApiClient.apiKeyPrefix["x-api-key"] = ""
Configure BearerAuth:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="onRamperGetSupportedDefaultsAll"></a>
# **onRamperGetSupportedDefaultsAll**
> SupportedDefaultResponse onRamperGetSupportedDefaultsAll(authorization, country, type)



### Example
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

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **country** | **kotlin.String**|  |
 **type** | **kotlin.String**|  |

### Return type

[**SupportedDefaultResponse**](SupportedDefaultResponse.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.apiKey["x-api-key"] = ""
    ApiClient.apiKeyPrefix["x-api-key"] = ""
Configure BearerAuth:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="onRamperGetSupportedOnRampsAll"></a>
# **onRamperGetSupportedOnRampsAll**
> GetSupportedOnRampsResponse onRamperGetSupportedOnRampsAll(authorization)



### Example
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

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |

### Return type

[**GetSupportedOnRampsResponse**](GetSupportedOnRampsResponse.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.apiKey["x-api-key"] = ""
    ApiClient.apiKeyPrefix["x-api-key"] = ""
Configure BearerAuth:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="onRamperGetSupportedPaymentTypes"></a>
# **onRamperGetSupportedPaymentTypes**
> SupportedPaymentTypesCurrencyResponse onRamperGetSupportedPaymentTypes(authorization, fiat, country, type)



### Example
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

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **fiat** | **kotlin.String**|  |
 **country** | **kotlin.String**|  |
 **type** | **kotlin.String**|  |

### Return type

[**SupportedPaymentTypesCurrencyResponse**](SupportedPaymentTypesCurrencyResponse.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.apiKey["x-api-key"] = ""
    ApiClient.apiKeyPrefix["x-api-key"] = ""
Configure BearerAuth:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="onRamperGetSupportedPaymentTypesFiat"></a>
# **onRamperGetSupportedPaymentTypesFiat**
> SupportedPaymentTypesCurrencyResponse onRamperGetSupportedPaymentTypesFiat(authorization, fiat, country)



### Example
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

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **fiat** | **kotlin.String**|  |
 **country** | **kotlin.String**|  |

### Return type

[**SupportedPaymentTypesCurrencyResponse**](SupportedPaymentTypesCurrencyResponse.md)

### Authorization


Configure ApiKeyAuth:
    ApiClient.apiKey["x-api-key"] = ""
    ApiClient.apiKeyPrefix["x-api-key"] = ""
Configure BearerAuth:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

