# CosmosApi

## CosmosApi

All URIs are relative to _https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app_

| Method                                                          | HTTP request                           | Description |
| --------------------------------------------------------------- | -------------------------------------- | ----------- |
| [**createCosmosAccount**](cosmosapi.md#createCosmosAccount)     | **POST** /cosmos                       |             |
| [**getCosmosAccount**](cosmosapi.md#getCosmosAccount)           | **GET** /cosmos/{accountName}          |             |
| [**listCosmosAccounts**](cosmosapi.md#listCosmosAccounts)       | **GET** /cosmos                        |             |
| [**signCosmosTransaction**](cosmosapi.md#signCosmosTransaction) | **POST** /cosmos/{accountName}/sign-tx |             |

## **createCosmosAccount**

> AccountAPIResponse createCosmosAccount(authorization, cosmosInput)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = CosmosApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val cosmosInput : CosmosInput =  // CosmosInput | 
try {
    val result : AccountAPIResponse = apiInstance.createCosmosAccount(authorization, cosmosInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CosmosApi#createCosmosAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CosmosApi#createCosmosAccount")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                              | Description | Notes |
| ----------------- | --------------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**                 |             |       |
| **cosmosInput**   | [**CosmosInput**](cosmosinput.md) |             |       |

#### Return type

[**AccountAPIResponse**](accountapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **getCosmosAccount**

> AccountAPIResponse getCosmosAccount(authorization, accountName)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = CosmosApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val accountName : kotlin.String = accountName_example // kotlin.String | 
try {
    val result : AccountAPIResponse = apiInstance.getCosmosAccount(authorization, accountName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CosmosApi#getCosmosAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CosmosApi#getCosmosAccount")
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

## **listCosmosAccounts**

> AccountAPIResponse listCosmosAccounts(authorization)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = CosmosApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
try {
    val result : AccountAPIResponse = apiInstance.listCosmosAccounts(authorization)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CosmosApi#listCosmosAccounts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CosmosApi#listCosmosAccounts")
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

## **signCosmosTransaction**

> CosmosAPIResponse signCosmosTransaction(authorization, accountName, cosmosTransactionInput)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = CosmosApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val accountName : kotlin.String = accountName_example // kotlin.String | 
val cosmosTransactionInput : CosmosTransactionInput =  // CosmosTransactionInput | 
try {
    val result : CosmosAPIResponse = apiInstance.signCosmosTransaction(authorization, accountName, cosmosTransactionInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CosmosApi#signCosmosTransaction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CosmosApi#signCosmosTransaction")
    e.printStackTrace()
}
```

#### Parameters

| Name                       | Type                                                    | Description | Notes |
| -------------------------- | ------------------------------------------------------- | ----------- | ----- |
| **authorization**          | **kotlin.String**                                       |             |       |
| **accountName**            | **kotlin.String**                                       |             |       |
| **cosmosTransactionInput** | [**CosmosTransactionInput**](cosmostransactioninput.md) |             |       |

#### Return type

[**CosmosAPIResponse**](cosmosapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json
