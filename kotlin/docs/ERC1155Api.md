# ERC1155Api

All URIs are relative to *https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**balanceOf**](ERC1155Api.md#balanceOf) | **POST** /erc1155/{name}/balance-of | 
[**balanceOfBatch**](ERC1155Api.md#balanceOfBatch) | **POST** /erc1155/{name}/balance-of-batch | 
[**isApprovedForAll**](ERC1155Api.md#isApprovedForAll) | **POST** /erc1155/{name}/is-approved-for-all | 
[**safeBatchTransferFrom**](ERC1155Api.md#safeBatchTransferFrom) | **POST** /erc1155/{name}/safe-batch-transfer-from | 
[**safeTransferFrom**](ERC1155Api.md#safeTransferFrom) | **POST** /erc1155/{name}/safe-transfer-from | 
[**setApprovalForAll**](ERC1155Api.md#setApprovalForAll) | **POST** /erc1155/{name}/set-approval-for-all | 


<a id="balanceOf"></a>
# **balanceOf**
> TransactionAPIResponse balanceOf(name, authorization, erc1155Request)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = ERC1155Api()
val name : kotlin.String = name_example // kotlin.String | 
val authorization : kotlin.String = authorization_example // kotlin.String | 
val erc1155Request : Erc1155Request =  // Erc1155Request | 
try {
    val result : TransactionAPIResponse = apiInstance.balanceOf(name, authorization, erc1155Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ERC1155Api#balanceOf")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ERC1155Api#balanceOf")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **kotlin.String**|  |
 **authorization** | **kotlin.String**|  |
 **erc1155Request** | [**Erc1155Request**](Erc1155Request.md)|  |

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

<a id="balanceOfBatch"></a>
# **balanceOfBatch**
> TransactionAPIResponse balanceOfBatch(name, authorization, erc1155Request)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = ERC1155Api()
val name : kotlin.String = name_example // kotlin.String | 
val authorization : kotlin.String = authorization_example // kotlin.String | 
val erc1155Request : Erc1155Request =  // Erc1155Request | 
try {
    val result : TransactionAPIResponse = apiInstance.balanceOfBatch(name, authorization, erc1155Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ERC1155Api#balanceOfBatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ERC1155Api#balanceOfBatch")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **kotlin.String**|  |
 **authorization** | **kotlin.String**|  |
 **erc1155Request** | [**Erc1155Request**](Erc1155Request.md)|  |

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

<a id="isApprovedForAll"></a>
# **isApprovedForAll**
> TransactionAPIResponse isApprovedForAll(name, authorization, erc1155Request)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = ERC1155Api()
val name : kotlin.String = name_example // kotlin.String | 
val authorization : kotlin.String = authorization_example // kotlin.String | 
val erc1155Request : Erc1155Request =  // Erc1155Request | 
try {
    val result : TransactionAPIResponse = apiInstance.isApprovedForAll(name, authorization, erc1155Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ERC1155Api#isApprovedForAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ERC1155Api#isApprovedForAll")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **kotlin.String**|  |
 **authorization** | **kotlin.String**|  |
 **erc1155Request** | [**Erc1155Request**](Erc1155Request.md)|  |

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

<a id="safeBatchTransferFrom"></a>
# **safeBatchTransferFrom**
> TransactionAPIResponse safeBatchTransferFrom(name, authorization, erc1155Request)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = ERC1155Api()
val name : kotlin.String = name_example // kotlin.String | 
val authorization : kotlin.String = authorization_example // kotlin.String | 
val erc1155Request : Erc1155Request =  // Erc1155Request | 
try {
    val result : TransactionAPIResponse = apiInstance.safeBatchTransferFrom(name, authorization, erc1155Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ERC1155Api#safeBatchTransferFrom")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ERC1155Api#safeBatchTransferFrom")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **kotlin.String**|  |
 **authorization** | **kotlin.String**|  |
 **erc1155Request** | [**Erc1155Request**](Erc1155Request.md)|  |

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

<a id="safeTransferFrom"></a>
# **safeTransferFrom**
> TransactionAPIResponse safeTransferFrom(name, authorization, erc1155Request)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = ERC1155Api()
val name : kotlin.String = name_example // kotlin.String | 
val authorization : kotlin.String = authorization_example // kotlin.String | 
val erc1155Request : Erc1155Request =  // Erc1155Request | 
try {
    val result : TransactionAPIResponse = apiInstance.safeTransferFrom(name, authorization, erc1155Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ERC1155Api#safeTransferFrom")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ERC1155Api#safeTransferFrom")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **kotlin.String**|  |
 **authorization** | **kotlin.String**|  |
 **erc1155Request** | [**Erc1155Request**](Erc1155Request.md)|  |

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

<a id="setApprovalForAll"></a>
# **setApprovalForAll**
> TransactionAPIResponse setApprovalForAll(name, authorization, erc1155Request)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = ERC1155Api()
val name : kotlin.String = name_example // kotlin.String | 
val authorization : kotlin.String = authorization_example // kotlin.String | 
val erc1155Request : Erc1155Request =  // Erc1155Request | 
try {
    val result : TransactionAPIResponse = apiInstance.setApprovalForAll(name, authorization, erc1155Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ERC1155Api#setApprovalForAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ERC1155Api#setApprovalForAll")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **kotlin.String**|  |
 **authorization** | **kotlin.String**|  |
 **erc1155Request** | [**Erc1155Request**](Erc1155Request.md)|  |

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

