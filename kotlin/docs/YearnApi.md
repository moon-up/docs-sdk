# YearnApi

All URIs are relative to *https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addLiquidity**](YearnApi.md#addLiquidity) | **POST** /yearn/{name}/add-liquidity | 
[**addLiquidityWeth**](YearnApi.md#addLiquidityWeth) | **POST** /yearn/{name}/add-liquidity-weth | 
[**removeLiquidity**](YearnApi.md#removeLiquidity) | **POST** /yearn/{name}/remove-liquidity | 
[**removeLiquidityWeth**](YearnApi.md#removeLiquidityWeth) | **POST** /yearn/{name}/remove-liquidity-weth | 


<a id="addLiquidity"></a>
# **addLiquidity**
> TransactionAPIResponse addLiquidity(authorization, name, inputBody)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = YearnApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val inputBody : InputBody =  // InputBody | 
try {
    val result : TransactionAPIResponse = apiInstance.addLiquidity(authorization, name, inputBody)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling YearnApi#addLiquidity")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling YearnApi#addLiquidity")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **name** | **kotlin.String**|  |
 **inputBody** | [**InputBody**](InputBody.md)|  |

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

<a id="addLiquidityWeth"></a>
# **addLiquidityWeth**
> TransactionAPIResponse addLiquidityWeth(authorization, name, inputBody)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = YearnApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val inputBody : InputBody =  // InputBody | 
try {
    val result : TransactionAPIResponse = apiInstance.addLiquidityWeth(authorization, name, inputBody)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling YearnApi#addLiquidityWeth")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling YearnApi#addLiquidityWeth")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **name** | **kotlin.String**|  |
 **inputBody** | [**InputBody**](InputBody.md)|  |

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
> TransactionAPIResponse removeLiquidity(authorization, name, inputBody)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = YearnApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val inputBody : InputBody =  // InputBody | 
try {
    val result : TransactionAPIResponse = apiInstance.removeLiquidity(authorization, name, inputBody)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling YearnApi#removeLiquidity")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling YearnApi#removeLiquidity")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **name** | **kotlin.String**|  |
 **inputBody** | [**InputBody**](InputBody.md)|  |

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

<a id="removeLiquidityWeth"></a>
# **removeLiquidityWeth**
> TransactionAPIResponse removeLiquidityWeth(authorization, name, inputBody)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = YearnApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val inputBody : InputBody =  // InputBody | 
try {
    val result : TransactionAPIResponse = apiInstance.removeLiquidityWeth(authorization, name, inputBody)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling YearnApi#removeLiquidityWeth")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling YearnApi#removeLiquidityWeth")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **name** | **kotlin.String**|  |
 **inputBody** | [**InputBody**](InputBody.md)|  |

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

