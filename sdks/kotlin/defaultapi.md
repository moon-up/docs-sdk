# DefaultApi

## DefaultApi

All URIs are relative to _https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app_

| Method                                     | HTTP request  | Description |
| ------------------------------------------ | ------------- | ----------- |
| [**getMessage**](defaultapi.md#getMessage) | **GET** /ping |             |

## **getMessage**

> PingResponse getMessage()

#### Example

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

#### Parameters

This endpoint does not need any parameter.

#### Return type

[**PingResponse**](pingresponse.md)

#### Authorization

No authorization required

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json
