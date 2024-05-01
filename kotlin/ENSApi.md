# ENSApi

All URIs are relative to *https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**resolve**](ENSApi.md#resolve) | **POST** /ens/resolve | 


<a id="resolve"></a>
# **resolve**
> EnsResolveAPIResponse resolve(authorization, ensResolveInput)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = ENSApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val ensResolveInput : EnsResolveInput =  // EnsResolveInput | 
try {
    val result : EnsResolveAPIResponse = apiInstance.resolve(authorization, ensResolveInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ENSApi#resolve")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ENSApi#resolve")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **ensResolveInput** | [**EnsResolveInput**](EnsResolveInput.md)|  |

### Return type

[**EnsResolveAPIResponse**](EnsResolveAPIResponse.md)

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

