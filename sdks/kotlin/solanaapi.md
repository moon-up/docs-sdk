# SolanaApi

## SolanaApi

All URIs are relative to _https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app_

| Method                                                          | HTTP request                           | Description |
| --------------------------------------------------------------- | -------------------------------------- | ----------- |
| [**createSolanaAccount**](solanaapi.md#createSolanaAccount)     | **POST** /solana                       |             |
| [**getSolanaAccount**](solanaapi.md#getSolanaAccount)           | **GET** /solana/{accountName}          |             |
| [**listSolanaAccounts**](solanaapi.md#listSolanaAccounts)       | **GET** /solana                        |             |
| [**signSolanaTransaction**](solanaapi.md#signSolanaTransaction) | **POST** /solana/{accountName}/sign-tx |             |

## **createSolanaAccount**

> AccountAPIResponse createSolanaAccount(authorization, solanaInput)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = SolanaApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val solanaInput : SolanaInput =  // SolanaInput | 
try {
    val result : AccountAPIResponse = apiInstance.createSolanaAccount(authorization, solanaInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SolanaApi#createSolanaAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SolanaApi#createSolanaAccount")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                              | Description | Notes |
| ----------------- | --------------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**                 |             |       |
| **solanaInput**   | [**SolanaInput**](solanainput.md) |             |       |

#### Return type

[**AccountAPIResponse**](accountapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **getSolanaAccount**

> AccountAPIResponse getSolanaAccount(authorization, accountName)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = SolanaApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val accountName : kotlin.String = accountName_example // kotlin.String | 
try {
    val result : AccountAPIResponse = apiInstance.getSolanaAccount(authorization, accountName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SolanaApi#getSolanaAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SolanaApi#getSolanaAccount")
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

## **listSolanaAccounts**

> AccountAPIResponse listSolanaAccounts(authorization)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = SolanaApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
try {
    val result : AccountAPIResponse = apiInstance.listSolanaAccounts(authorization)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SolanaApi#listSolanaAccounts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SolanaApi#listSolanaAccounts")
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

## **signSolanaTransaction**

> SolanaAPIResponse signSolanaTransaction(authorization, accountName, solanaTransactionInput)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = SolanaApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val accountName : kotlin.String = accountName_example // kotlin.String | 
val solanaTransactionInput : SolanaTransactionInput =  // SolanaTransactionInput | 
try {
    val result : SolanaAPIResponse = apiInstance.signSolanaTransaction(authorization, accountName, solanaTransactionInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SolanaApi#signSolanaTransaction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SolanaApi#signSolanaTransaction")
    e.printStackTrace()
}
```

#### Parameters

| Name                       | Type                                                    | Description | Notes |
| -------------------------- | ------------------------------------------------------- | ----------- | ----- |
| **authorization**          | **kotlin.String**                                       |             |       |
| **accountName**            | **kotlin.String**                                       |             |       |
| **solanaTransactionInput** | [**SolanaTransactionInput**](solanatransactioninput.md) |             |       |

#### Return type

[**SolanaAPIResponse**](solanaapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json
