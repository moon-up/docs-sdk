# Erc721Api

All URIs are relative to *https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**approve**](Erc721Api.md#approve) | **POST** /erc721/{name}/approve | 
[**balanceOf**](Erc721Api.md#balanceOf) | **POST** /erc721/{name}/balance-of | 
[**getApproved**](Erc721Api.md#getApproved) | **POST** /erc721/{name}/get-approved | 
[**isApprovedForAll**](Erc721Api.md#isApprovedForAll) | **POST** /erc721/{name}/is-approved-for-all | 
[**name**](Erc721Api.md#name) | **POST** /erc721/{name}/name | 
[**ownerOf**](Erc721Api.md#ownerOf) | **POST** /erc721/{name}/owner-of | 
[**safeTransferFrom**](Erc721Api.md#safeTransferFrom) | **POST** /erc721/{name}/safe-transfer-from | 
[**setApprovalForAll**](Erc721Api.md#setApprovalForAll) | **POST** /erc721/{name}/set-approval-for-all | 
[**symbol**](Erc721Api.md#symbol) | **POST** /erc721/{name}/symbol | 
[**tokenUri**](Erc721Api.md#tokenUri) | **POST** /erc721/{name}/token-uri | 
[**transfer**](Erc721Api.md#transfer) | **POST** /erc721/{name}/transfer | 
[**transferFrom**](Erc721Api.md#transferFrom) | **POST** /erc721/{name}/transfer-from | 


<a id="approve"></a>
# **approve**
> TransactionAPIResponse approve(authorization, name, erc721Request)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = Erc721Api()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val erc721Request : Erc721Request =  // Erc721Request | 
try {
    val result : TransactionAPIResponse = apiInstance.approve(authorization, name, erc721Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling Erc721Api#approve")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling Erc721Api#approve")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **name** | **kotlin.String**|  |
 **erc721Request** | [**Erc721Request**](Erc721Request.md)|  |

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

<a id="balanceOf"></a>
# **balanceOf**
> TransactionAPIResponse balanceOf(authorization, name, erc721Request)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = Erc721Api()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val erc721Request : Erc721Request =  // Erc721Request | 
try {
    val result : TransactionAPIResponse = apiInstance.balanceOf(authorization, name, erc721Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling Erc721Api#balanceOf")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling Erc721Api#balanceOf")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **name** | **kotlin.String**|  |
 **erc721Request** | [**Erc721Request**](Erc721Request.md)|  |

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

<a id="getApproved"></a>
# **getApproved**
> TransactionAPIResponse getApproved(authorization, name, erc721Request)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = Erc721Api()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val erc721Request : Erc721Request =  // Erc721Request | 
try {
    val result : TransactionAPIResponse = apiInstance.getApproved(authorization, name, erc721Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling Erc721Api#getApproved")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling Erc721Api#getApproved")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **name** | **kotlin.String**|  |
 **erc721Request** | [**Erc721Request**](Erc721Request.md)|  |

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
> TransactionAPIResponse isApprovedForAll(authorization, name, erc721Request)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = Erc721Api()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val erc721Request : Erc721Request =  // Erc721Request | 
try {
    val result : TransactionAPIResponse = apiInstance.isApprovedForAll(authorization, name, erc721Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling Erc721Api#isApprovedForAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling Erc721Api#isApprovedForAll")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **name** | **kotlin.String**|  |
 **erc721Request** | [**Erc721Request**](Erc721Request.md)|  |

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

<a id="name"></a>
# **name**
> TransactionAPIResponse name(authorization, name, erc721Request)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = Erc721Api()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val erc721Request : Erc721Request =  // Erc721Request | 
try {
    val result : TransactionAPIResponse = apiInstance.name(authorization, name, erc721Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling Erc721Api#name")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling Erc721Api#name")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **name** | **kotlin.String**|  |
 **erc721Request** | [**Erc721Request**](Erc721Request.md)|  |

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

<a id="ownerOf"></a>
# **ownerOf**
> TransactionAPIResponse ownerOf(authorization, name, erc721Request)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = Erc721Api()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val erc721Request : Erc721Request =  // Erc721Request | 
try {
    val result : TransactionAPIResponse = apiInstance.ownerOf(authorization, name, erc721Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling Erc721Api#ownerOf")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling Erc721Api#ownerOf")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **name** | **kotlin.String**|  |
 **erc721Request** | [**Erc721Request**](Erc721Request.md)|  |

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
> TransactionAPIResponse safeTransferFrom(authorization, name, erc721Request)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = Erc721Api()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val erc721Request : Erc721Request =  // Erc721Request | 
try {
    val result : TransactionAPIResponse = apiInstance.safeTransferFrom(authorization, name, erc721Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling Erc721Api#safeTransferFrom")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling Erc721Api#safeTransferFrom")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **name** | **kotlin.String**|  |
 **erc721Request** | [**Erc721Request**](Erc721Request.md)|  |

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
> TransactionAPIResponse setApprovalForAll(authorization, name, erc721Request)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = Erc721Api()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val erc721Request : Erc721Request =  // Erc721Request | 
try {
    val result : TransactionAPIResponse = apiInstance.setApprovalForAll(authorization, name, erc721Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling Erc721Api#setApprovalForAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling Erc721Api#setApprovalForAll")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **name** | **kotlin.String**|  |
 **erc721Request** | [**Erc721Request**](Erc721Request.md)|  |

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

<a id="symbol"></a>
# **symbol**
> TransactionAPIResponse symbol(authorization, name, erc721Request)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = Erc721Api()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val erc721Request : Erc721Request =  // Erc721Request | 
try {
    val result : TransactionAPIResponse = apiInstance.symbol(authorization, name, erc721Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling Erc721Api#symbol")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling Erc721Api#symbol")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **name** | **kotlin.String**|  |
 **erc721Request** | [**Erc721Request**](Erc721Request.md)|  |

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

<a id="tokenUri"></a>
# **tokenUri**
> TransactionAPIResponse tokenUri(authorization, name, erc721Request)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = Erc721Api()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val erc721Request : Erc721Request =  // Erc721Request | 
try {
    val result : TransactionAPIResponse = apiInstance.tokenUri(authorization, name, erc721Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling Erc721Api#tokenUri")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling Erc721Api#tokenUri")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **name** | **kotlin.String**|  |
 **erc721Request** | [**Erc721Request**](Erc721Request.md)|  |

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

<a id="transfer"></a>
# **transfer**
> TransactionAPIResponse transfer(authorization, name, erc721Request)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = Erc721Api()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val erc721Request : Erc721Request =  // Erc721Request | 
try {
    val result : TransactionAPIResponse = apiInstance.transfer(authorization, name, erc721Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling Erc721Api#transfer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling Erc721Api#transfer")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **name** | **kotlin.String**|  |
 **erc721Request** | [**Erc721Request**](Erc721Request.md)|  |

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

<a id="transferFrom"></a>
# **transferFrom**
> TransactionAPIResponse transferFrom(authorization, name, erc721Request)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = Erc721Api()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val erc721Request : Erc721Request =  // Erc721Request | 
try {
    val result : TransactionAPIResponse = apiInstance.transferFrom(authorization, name, erc721Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling Erc721Api#transferFrom")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling Erc721Api#transferFrom")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **name** | **kotlin.String**|  |
 **erc721Request** | [**Erc721Request**](Erc721Request.md)|  |

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

