# OneinchApi

All URIs are relative to *https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**approveCallData**](OneinchApi.md#approveCallData) | **POST** /oneinch/approve-call-data | 
[**approveSpender**](OneinchApi.md#approveSpender) | **POST** /oneinch/approve-spender | 
[**protocols**](OneinchApi.md#protocols) | **POST** /oneinch/protocols | 
[**quote**](OneinchApi.md#quote) | **POST** /oneinch/quote | 
[**swap**](OneinchApi.md#swap) | **POST** /oneinch/{accountName}/swap | 
[**tokens**](OneinchApi.md#tokens) | **POST** /oneinch/tokens | 


<a id="approveCallData"></a>
# **approveCallData**
> kotlin.Any approveCallData(body)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = OneinchApi()
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.approveCallData(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OneinchApi#approveCallData")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OneinchApi#approveCallData")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **kotlin.Any**|  |

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

<a id="approveSpender"></a>
# **approveSpender**
> kotlin.Any approveSpender(body)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = OneinchApi()
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.approveSpender(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OneinchApi#approveSpender")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OneinchApi#approveSpender")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **kotlin.Any**|  |

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

<a id="protocols"></a>
# **protocols**
> kotlin.Any protocols(body)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = OneinchApi()
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.protocols(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OneinchApi#protocols")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OneinchApi#protocols")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **kotlin.Any**|  |

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

<a id="quote"></a>
# **quote**
> kotlin.Any quote(body)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = OneinchApi()
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.quote(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OneinchApi#quote")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OneinchApi#quote")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **kotlin.Any**|  |

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

<a id="swap"></a>
# **swap**
> kotlin.Any swap(accountName, authorization, getSwapDto)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = OneinchApi()
val accountName : kotlin.String = accountName_example // kotlin.String | 
val authorization : kotlin.String = authorization_example // kotlin.String | 
val getSwapDto : GetSwapDto =  // GetSwapDto | 
try {
    val result : kotlin.Any = apiInstance.swap(accountName, authorization, getSwapDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OneinchApi#swap")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OneinchApi#swap")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accountName** | **kotlin.String**|  |
 **authorization** | **kotlin.String**|  |
 **getSwapDto** | [**GetSwapDto**](GetSwapDto.md)|  |

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

<a id="tokens"></a>
# **tokens**
> kotlin.Any tokens(body)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = OneinchApi()
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.tokens(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OneinchApi#tokens")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OneinchApi#tokens")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **kotlin.Any**|  |

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

