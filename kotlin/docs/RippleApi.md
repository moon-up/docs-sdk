# RippleApi

All URIs are relative to *https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createRippleAccount**](RippleApi.md#createRippleAccount) | **POST** /ripple | 
[**getRippleAccount**](RippleApi.md#getRippleAccount) | **GET** /ripple/{accountName} | 
[**listRippleAccounts**](RippleApi.md#listRippleAccounts) | **GET** /ripple | 
[**signRippleTransaction**](RippleApi.md#signRippleTransaction) | **POST** /ripple/{accountName}/sign-tx | 


<a id="createRippleAccount"></a>
# **createRippleAccount**
> AccountAPIResponse createRippleAccount(authorization, rippleInput)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = RippleApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val rippleInput : RippleInput =  // RippleInput | 
try {
    val result : AccountAPIResponse = apiInstance.createRippleAccount(authorization, rippleInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RippleApi#createRippleAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RippleApi#createRippleAccount")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **rippleInput** | [**RippleInput**](RippleInput.md)|  |

### Return type

[**AccountAPIResponse**](AccountAPIResponse.md)

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

<a id="getRippleAccount"></a>
# **getRippleAccount**
> AccountAPIResponse getRippleAccount(authorization, accountName)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = RippleApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val accountName : kotlin.String = accountName_example // kotlin.String | 
try {
    val result : AccountAPIResponse = apiInstance.getRippleAccount(authorization, accountName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RippleApi#getRippleAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RippleApi#getRippleAccount")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **accountName** | **kotlin.String**|  |

### Return type

[**AccountAPIResponse**](AccountAPIResponse.md)

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

<a id="listRippleAccounts"></a>
# **listRippleAccounts**
> AccountAPIResponse listRippleAccounts(authorization)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = RippleApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
try {
    val result : AccountAPIResponse = apiInstance.listRippleAccounts(authorization)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RippleApi#listRippleAccounts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RippleApi#listRippleAccounts")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |

### Return type

[**AccountAPIResponse**](AccountAPIResponse.md)

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

<a id="signRippleTransaction"></a>
# **signRippleTransaction**
> RippleAPIResponse signRippleTransaction(authorization, accountName, rippleTransactionInput)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = RippleApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val accountName : kotlin.String = accountName_example // kotlin.String | 
val rippleTransactionInput : RippleTransactionInput =  // RippleTransactionInput | 
try {
    val result : RippleAPIResponse = apiInstance.signRippleTransaction(authorization, accountName, rippleTransactionInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RippleApi#signRippleTransaction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RippleApi#signRippleTransaction")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **accountName** | **kotlin.String**|  |
 **rippleTransactionInput** | [**RippleTransactionInput**](RippleTransactionInput.md)|  |

### Return type

[**RippleAPIResponse**](RippleAPIResponse.md)

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

