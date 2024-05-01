# UniSwapApi

All URIs are relative to *https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addLiquidity**](UniSwapApi.md#addLiquidity) | **POST** /uniswap/{name}/add-liquidity | 
[**removeLiquidity**](UniSwapApi.md#removeLiquidity) | **POST** /uniswap/{name}/remove-liquidity | 
[**swapExactETHForTokens**](UniSwapApi.md#swapExactETHForTokens) | **POST** /uniswap/{name}/swap-exact-eth-for-tokens | 
[**swapExactTokensForTokens**](UniSwapApi.md#swapExactTokensForTokens) | **POST** /uniswap/{name}/swap-exact-tokens-for-tokens | 


<a id="addLiquidity"></a>
# **addLiquidity**
> TransactionAPIResponse addLiquidity(authorization, name, uniswapInput)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = UniSwapApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val uniswapInput : UniswapInput =  // UniswapInput | 
try {
    val result : TransactionAPIResponse = apiInstance.addLiquidity(authorization, name, uniswapInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UniSwapApi#addLiquidity")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UniSwapApi#addLiquidity")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **name** | **kotlin.String**|  |
 **uniswapInput** | [**UniswapInput**](UniswapInput.md)|  |

### Return type

[**TransactionAPIResponse**](TransactionAPIResponse.md)

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

<a id="removeLiquidity"></a>
# **removeLiquidity**
> TransactionAPIResponse removeLiquidity(authorization, name, uniswapInput)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = UniSwapApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val uniswapInput : UniswapInput =  // UniswapInput | 
try {
    val result : TransactionAPIResponse = apiInstance.removeLiquidity(authorization, name, uniswapInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UniSwapApi#removeLiquidity")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UniSwapApi#removeLiquidity")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **name** | **kotlin.String**|  |
 **uniswapInput** | [**UniswapInput**](UniswapInput.md)|  |

### Return type

[**TransactionAPIResponse**](TransactionAPIResponse.md)

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

<a id="swapExactETHForTokens"></a>
# **swapExactETHForTokens**
> TransactionAPIResponse swapExactETHForTokens(authorization, name, uniswapInput)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = UniSwapApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val uniswapInput : UniswapInput =  // UniswapInput | 
try {
    val result : TransactionAPIResponse = apiInstance.swapExactETHForTokens(authorization, name, uniswapInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UniSwapApi#swapExactETHForTokens")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UniSwapApi#swapExactETHForTokens")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **name** | **kotlin.String**|  |
 **uniswapInput** | [**UniswapInput**](UniswapInput.md)|  |

### Return type

[**TransactionAPIResponse**](TransactionAPIResponse.md)

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

<a id="swapExactTokensForTokens"></a>
# **swapExactTokensForTokens**
> TransactionAPIResponse swapExactTokensForTokens(authorization, name, uniswapInput)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = UniSwapApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val uniswapInput : UniswapInput =  // UniswapInput | 
try {
    val result : TransactionAPIResponse = apiInstance.swapExactTokensForTokens(authorization, name, uniswapInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UniSwapApi#swapExactTokensForTokens")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UniSwapApi#swapExactTokensForTokens")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **name** | **kotlin.String**|  |
 **uniswapInput** | [**UniswapInput**](UniswapInput.md)|  |

### Return type

[**TransactionAPIResponse**](TransactionAPIResponse.md)

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

