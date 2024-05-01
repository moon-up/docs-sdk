# DefaultApi

All URIs are relative to *https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getMessage**](DefaultApi.md#getMessage) | **GET** /ping | 


<a id="getMessage"></a>
# **getMessage**
> PingResponse getMessage()



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = DefaultApi()
try {
    val result : PingResponse = apiInstance.getMessage()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DefaultApi#getMessage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DefaultApi#getMessage")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PingResponse**](PingResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

