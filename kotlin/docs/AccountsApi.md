# AccountsApi

All URIs are relative to *https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app*

Method | HTTP request | Description
------------- | ------------- | -------------
[**broadcastTx**](AccountsApi.md#broadcastTx) | **POST** /accounts/{accountName}/broadcast-tx | 
[**createAccount**](AccountsApi.md#createAccount) | **POST** /accounts | 
[**deleteAccount**](AccountsApi.md#deleteAccount) | **DELETE** /accounts/{accountName} | 
[**deployContract**](AccountsApi.md#deployContract) | **POST** /accounts/{accountName}/deploy | 
[**getAccount**](AccountsApi.md#getAccount) | **GET** /accounts/{accountName} | 
[**getBalance**](AccountsApi.md#getBalance) | **GET** /accounts/{accountName}/balance | 
[**getNonce**](AccountsApi.md#getNonce) | **GET** /accounts/{accountName}/nonce | 
[**listAccounts**](AccountsApi.md#listAccounts) | **GET** /accounts | 
[**signMessage**](AccountsApi.md#signMessage) | **POST** /accounts/{accountName}/sign-message | 
[**signTransaction**](AccountsApi.md#signTransaction) | **POST** /accounts/{accountName}/sign-transaction | 
[**signTypedData**](AccountsApi.md#signTypedData) | **POST** /accounts/{accountName}/sign-typed-data | 
[**transferEth**](AccountsApi.md#transferEth) | **POST** /accounts/{accountName}/transfer-eth | 


<a id="broadcastTx"></a>
# **broadcastTx**
> BroadCastRawTransactionAPIResponse broadcastTx(authorization, accountName, broadcastInput)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = AccountsApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val accountName : kotlin.String = accountName_example // kotlin.String | 
val broadcastInput : BroadcastInput =  // BroadcastInput | 
try {
    val result : BroadCastRawTransactionAPIResponse = apiInstance.broadcastTx(authorization, accountName, broadcastInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountsApi#broadcastTx")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountsApi#broadcastTx")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **accountName** | **kotlin.String**|  |
 **broadcastInput** | [**BroadcastInput**](BroadcastInput.md)|  |

### Return type

[**BroadCastRawTransactionAPIResponse**](BroadCastRawTransactionAPIResponse.md)

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

<a id="createAccount"></a>
# **createAccount**
> AccountAPIResponse createAccount(authorization, createAccountInput)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = AccountsApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val createAccountInput : CreateAccountInput =  // CreateAccountInput | 
try {
    val result : AccountAPIResponse = apiInstance.createAccount(authorization, createAccountInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountsApi#createAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountsApi#createAccount")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **createAccountInput** | [**CreateAccountInput**](CreateAccountInput.md)|  |

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

<a id="deleteAccount"></a>
# **deleteAccount**
> AccountAPIResponse deleteAccount(authorization, accountName)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = AccountsApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val accountName : kotlin.String = accountName_example // kotlin.String | 
try {
    val result : AccountAPIResponse = apiInstance.deleteAccount(authorization, accountName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountsApi#deleteAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountsApi#deleteAccount")
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

<a id="deployContract"></a>
# **deployContract**
> TransactionAPIResponse deployContract(authorization, accountName, deployInput)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = AccountsApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val accountName : kotlin.String = accountName_example // kotlin.String | 
val deployInput : DeployInput =  // DeployInput | 
try {
    val result : TransactionAPIResponse = apiInstance.deployContract(authorization, accountName, deployInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountsApi#deployContract")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountsApi#deployContract")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **kotlin.String**|  |
 **accountName** | **kotlin.String**|  |
 **deployInput** | [**DeployInput**](DeployInput.md)|  |

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

<a id="getAccount"></a>
# **getAccount**
> AccountAPIResponse getAccount(authorization, accountName)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = AccountsApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val accountName : kotlin.String = accountName_example // kotlin.String | 
try {
    val result : AccountAPIResponse = apiInstance.getAccount(authorization, accountName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountsApi#getAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountsApi#getAccount")
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

<a id="getBalance"></a>
# **getBalance**
> BalanceAPIResponse getBalance(accountName, authorization, chainId)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = AccountsApi()
val accountName : kotlin.String = accountName_example // kotlin.String | 
val authorization : kotlin.String = authorization_example // kotlin.String | 
val chainId : kotlin.String = chainId_example // kotlin.String | 
try {
    val result : BalanceAPIResponse = apiInstance.getBalance(accountName, authorization, chainId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountsApi#getBalance")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountsApi#getBalance")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accountName** | **kotlin.String**|  |
 **authorization** | **kotlin.String**|  |
 **chainId** | **kotlin.String**|  |

### Return type

[**BalanceAPIResponse**](BalanceAPIResponse.md)

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

<a id="getNonce"></a>
# **getNonce**
> NonceAPIResponse getNonce(accountName, authorization)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = AccountsApi()
val accountName : kotlin.String = accountName_example // kotlin.String | 
val authorization : kotlin.String = authorization_example // kotlin.String | 
try {
    val result : NonceAPIResponse = apiInstance.getNonce(accountName, authorization)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountsApi#getNonce")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountsApi#getNonce")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accountName** | **kotlin.String**|  |
 **authorization** | **kotlin.String**|  |

### Return type

[**NonceAPIResponse**](NonceAPIResponse.md)

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

<a id="listAccounts"></a>
# **listAccounts**
> AccountAPIResponse listAccounts(authorization)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = AccountsApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
try {
    val result : AccountAPIResponse = apiInstance.listAccounts(authorization)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountsApi#listAccounts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountsApi#listAccounts")
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

<a id="signMessage"></a>
# **signMessage**
> SignMessageAPIResponse signMessage(accountName, authorization, signMessage)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = AccountsApi()
val accountName : kotlin.String = accountName_example // kotlin.String | 
val authorization : kotlin.String = authorization_example // kotlin.String | 
val signMessage : SignMessage =  // SignMessage | 
try {
    val result : SignMessageAPIResponse = apiInstance.signMessage(accountName, authorization, signMessage)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountsApi#signMessage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountsApi#signMessage")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accountName** | **kotlin.String**|  |
 **authorization** | **kotlin.String**|  |
 **signMessage** | [**SignMessage**](SignMessage.md)|  |

### Return type

[**SignMessageAPIResponse**](SignMessageAPIResponse.md)

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

<a id="signTransaction"></a>
# **signTransaction**
> TransactionAPIResponse signTransaction(accountName, authorization, inputBody)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = AccountsApi()
val accountName : kotlin.String = accountName_example // kotlin.String | 
val authorization : kotlin.String = authorization_example // kotlin.String | 
val inputBody : InputBody =  // InputBody | 
try {
    val result : TransactionAPIResponse = apiInstance.signTransaction(accountName, authorization, inputBody)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountsApi#signTransaction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountsApi#signTransaction")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accountName** | **kotlin.String**|  |
 **authorization** | **kotlin.String**|  |
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

<a id="signTypedData"></a>
# **signTypedData**
> SignMessageAPIResponse signTypedData(accountName, authorization, signTypedData)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = AccountsApi()
val accountName : kotlin.String = accountName_example // kotlin.String | 
val authorization : kotlin.String = authorization_example // kotlin.String | 
val signTypedData : SignTypedData =  // SignTypedData | 
try {
    val result : SignMessageAPIResponse = apiInstance.signTypedData(accountName, authorization, signTypedData)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountsApi#signTypedData")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountsApi#signTypedData")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accountName** | **kotlin.String**|  |
 **authorization** | **kotlin.String**|  |
 **signTypedData** | [**SignTypedData**](SignTypedData.md)|  |

### Return type

[**SignMessageAPIResponse**](SignMessageAPIResponse.md)

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

<a id="transferEth"></a>
# **transferEth**
> TransactionAPIResponse transferEth(accountName, authorization, inputBody)



### Example
```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = AccountsApi()
val accountName : kotlin.String = accountName_example // kotlin.String | 
val authorization : kotlin.String = authorization_example // kotlin.String | 
val inputBody : InputBody =  // InputBody | 
try {
    val result : TransactionAPIResponse = apiInstance.transferEth(accountName, authorization, inputBody)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountsApi#transferEth")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountsApi#transferEth")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accountName** | **kotlin.String**|  |
 **authorization** | **kotlin.String**|  |
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

