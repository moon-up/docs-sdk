# LitecoinApi

## LitecoinApi

All URIs are relative to _https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app_

| Method                                                                | HTTP request                             | Description |
| --------------------------------------------------------------------- | ---------------------------------------- | ----------- |
| [**createLitecoinAccount**](litecoinapi.md#createLitecoinAccount)     | **POST** /litecoin                       |             |
| [**getLitecoinAccount**](litecoinapi.md#getLitecoinAccount)           | **GET** /litecoin/{accountName}          |             |
| [**listLitecoinAccounts**](litecoinapi.md#listLitecoinAccounts)       | **GET** /litecoin                        |             |
| [**signLitecoinTransaction**](litecoinapi.md#signLitecoinTransaction) | **POST** /litecoin/{accountName}/sign-tx |             |

## **createLitecoinAccount**

> AccountAPIResponse createLitecoinAccount(authorization, litecoinInput)

#### Example

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

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**                     |             |       |
| **litecoinInput** | [**LitecoinInput**](litecoininput.md) |             |       |

#### Return type

[**AccountAPIResponse**](accountapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **getLitecoinAccount**

> AccountAPIResponse getLitecoinAccount(authorization, accountName)

#### Example

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

## **listLitecoinAccounts**

> AccountAPIResponse listLitecoinAccounts(authorization)

#### Example

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

## **signLitecoinTransaction**

> LitecoinAPIResponse signLitecoinTransaction(authorization, accountName, litecoinTransactionInput)

#### Example

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

#### Parameters

| Name                         | Type                                                        | Description | Notes |
| ---------------------------- | ----------------------------------------------------------- | ----------- | ----- |
| **authorization**            | **kotlin.String**                                           |             |       |
| **accountName**              | **kotlin.String**                                           |             |       |
| **litecoinTransactionInput** | [**LitecoinTransactionInput**](litecointransactioninput.md) |             |       |

#### Return type

[**LitecoinAPIResponse**](litecoinapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json
