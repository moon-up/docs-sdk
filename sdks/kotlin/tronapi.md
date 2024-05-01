# TronApi

## TronApi

All URIs are relative to _https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app_

| Method                                                    | HTTP request                         | Description |
| --------------------------------------------------------- | ------------------------------------ | ----------- |
| [**createTronAccount**](tronapi.md#createTronAccount)     | **POST** /tron                       |             |
| [**getTronAccount**](tronapi.md#getTronAccount)           | **GET** /tron/{accountName}          |             |
| [**listTronAccounts**](tronapi.md#listTronAccounts)       | **GET** /tron                        |             |
| [**signTronTransaction**](tronapi.md#signTronTransaction) | **POST** /tron/{accountName}/sign-tx |             |

## **createTronAccount**

> AccountAPIResponse createTronAccount(authorization, tronInput)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = TronApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val tronInput : TronInput =  // TronInput | 
try {
    val result : AccountAPIResponse = apiInstance.createTronAccount(authorization, tronInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TronApi#createTronAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TronApi#createTronAccount")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                          | Description | Notes |
| ----------------- | ----------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**             |             |       |
| **tronInput**     | [**TronInput**](troninput.md) |             |       |

#### Return type

[**AccountAPIResponse**](accountapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **getTronAccount**

> AccountAPIResponse getTronAccount(authorization, accountName)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = TronApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val accountName : kotlin.String = accountName_example // kotlin.String | 
try {
    val result : AccountAPIResponse = apiInstance.getTronAccount(authorization, accountName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TronApi#getTronAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TronApi#getTronAccount")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type              | Description | Notes |
| ----------------- | ----------------- | ----------- | ----- |
| **authorization** | **kotlin.String** |             |       |
| **accountName**   | **kotlin.String** |             |       |

#### Return type

[**AccountAPIResponse**](accountapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

## **listTronAccounts**

> AccountAPIResponse listTronAccounts(authorization)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = TronApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
try {
    val result : AccountAPIResponse = apiInstance.listTronAccounts(authorization)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TronApi#listTronAccounts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TronApi#listTronAccounts")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type              | Description | Notes |
| ----------------- | ----------------- | ----------- | ----- |
| **authorization** | **kotlin.String** |             |       |

#### Return type

[**AccountAPIResponse**](accountapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

## **signTronTransaction**

> TronAPIResponse signTronTransaction(authorization, accountName, tronTransactionInput)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = TronApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val accountName : kotlin.String = accountName_example // kotlin.String | 
val tronTransactionInput : TronTransactionInput =  // TronTransactionInput | 
try {
    val result : TronAPIResponse = apiInstance.signTronTransaction(authorization, accountName, tronTransactionInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TronApi#signTronTransaction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TronApi#signTronTransaction")
    e.printStackTrace()
}
```

#### Parameters

| Name                     | Type                                                | Description | Notes |
| ------------------------ | --------------------------------------------------- | ----------- | ----- |
| **authorization**        | **kotlin.String**                                   |             |       |
| **accountName**          | **kotlin.String**                                   |             |       |
| **tronTransactionInput** | [**TronTransactionInput**](trontransactioninput.md) |             |       |

#### Return type

[**TronAPIResponse**](tronapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json
