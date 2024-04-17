# LitecoinApi

All URIs are relative to *https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createLitecoinAccount**](LitecoinApi.md#createLitecoinAccount) | **POST** /litecoin | 
[**getLitecoinAccount**](LitecoinApi.md#getLitecoinAccount) | **GET** /litecoin/{accountName} | 
[**listLitecoinAccounts**](LitecoinApi.md#listLitecoinAccounts) | **GET** /litecoin | 
[**signLitecoinTransaction**](LitecoinApi.md#signLitecoinTransaction) | **POST** /litecoin/{accountName}/sign-tx | 


<a id="createLitecoinAccount"></a>
# **createLitecoinAccount**
> AccountAPIResponse createLitecoinAccount(authorization, litecoinInput)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = LitecoinApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val litecoinInput : LitecoinInput =  // LitecoinInput | 
try {
    val result : AccountAPIResponse = apiInstance.createLitecoinAccount(authorization, litecoinInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LitecoinApi#createLitecoinAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LitecoinApi#createLitecoinAccount")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **litecoinInput** | [**LitecoinInput**](LitecoinInput.md)|  |

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

<a id="getLitecoinAccount"></a>
# **getLitecoinAccount**
> AccountAPIResponse getLitecoinAccount(authorization, accountName)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = LitecoinApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val accountName : kotlin.String = accountName_example // kotlin.String | 
try {
    val result : AccountAPIResponse = apiInstance.getLitecoinAccount(authorization, accountName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LitecoinApi#getLitecoinAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LitecoinApi#getLitecoinAccount")
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

<a id="listLitecoinAccounts"></a>
# **listLitecoinAccounts**
> AccountAPIResponse listLitecoinAccounts(authorization)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = LitecoinApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
try {
    val result : AccountAPIResponse = apiInstance.listLitecoinAccounts(authorization)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LitecoinApi#listLitecoinAccounts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LitecoinApi#listLitecoinAccounts")
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

<a id="signLitecoinTransaction"></a>
# **signLitecoinTransaction**
> LitecoinAPIResponse signLitecoinTransaction(authorization, accountName, litecoinTransactionInput)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = LitecoinApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val accountName : kotlin.String = accountName_example // kotlin.String | 
val litecoinTransactionInput : LitecoinTransactionInput =  // LitecoinTransactionInput | 
try {
    val result : LitecoinAPIResponse = apiInstance.signLitecoinTransaction(authorization, accountName, litecoinTransactionInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LitecoinApi#signLitecoinTransaction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LitecoinApi#signLitecoinTransaction")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **accountName** | **kotlin.String**|  |
 **litecoinTransactionInput** | [**LitecoinTransactionInput**](LitecoinTransactionInput.md)|  |

### Return type

[**LitecoinAPIResponse**](LitecoinAPIResponse.md)

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

