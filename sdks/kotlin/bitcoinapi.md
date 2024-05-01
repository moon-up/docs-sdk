# BitcoinApi

## BitcoinApi

All URIs are relative to _https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app_

| Method                                                             | HTTP request                            | Description |
| ------------------------------------------------------------------ | --------------------------------------- | ----------- |
| [**createBitcoinAccount**](bitcoinapi.md#createBitcoinAccount)     | **POST** /bitcoin                       |             |
| [**getBitcoinAccount**](bitcoinapi.md#getBitcoinAccount)           | **GET** /bitcoin/{accountName}          |             |
| [**listBitcoinAccounts**](bitcoinapi.md#listBitcoinAccounts)       | **GET** /bitcoin                        |             |
| [**signBitcoinTransaction**](bitcoinapi.md#signBitcoinTransaction) | **POST** /bitcoin/{accountName}/sign-tx |             |

## **createBitcoinAccount**

> AccountAPIResponse createBitcoinAccount(authorization, bitcoinInput)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = BitcoinApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val bitcoinInput : BitcoinInput =  // BitcoinInput | 
try {
    val result : AccountAPIResponse = apiInstance.createBitcoinAccount(authorization, bitcoinInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BitcoinApi#createBitcoinAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BitcoinApi#createBitcoinAccount")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                                | Description | Notes |
| ----------------- | ----------------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**                   |             |       |
| **bitcoinInput**  | [**BitcoinInput**](bitcoininput.md) |             |       |

#### Return type

[**AccountAPIResponse**](accountapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **getBitcoinAccount**

> AccountAPIResponse getBitcoinAccount(authorization, accountName)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = BitcoinApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val accountName : kotlin.String = accountName_example // kotlin.String | 
try {
    val result : AccountAPIResponse = apiInstance.getBitcoinAccount(authorization, accountName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BitcoinApi#getBitcoinAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BitcoinApi#getBitcoinAccount")
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

## **listBitcoinAccounts**

> AccountAPIResponse listBitcoinAccounts(authorization)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = BitcoinApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
try {
    val result : AccountAPIResponse = apiInstance.listBitcoinAccounts(authorization)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BitcoinApi#listBitcoinAccounts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BitcoinApi#listBitcoinAccounts")
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

## **signBitcoinTransaction**

> BitcoinAPIResponse signBitcoinTransaction(authorization, accountName, bitcoinTransactionInput)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = BitcoinApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val accountName : kotlin.String = accountName_example // kotlin.String | 
val bitcoinTransactionInput : BitcoinTransactionInput =  // BitcoinTransactionInput | 
try {
    val result : BitcoinAPIResponse = apiInstance.signBitcoinTransaction(authorization, accountName, bitcoinTransactionInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BitcoinApi#signBitcoinTransaction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BitcoinApi#signBitcoinTransaction")
    e.printStackTrace()
}
```

#### Parameters

| Name                        | Type                                                      | Description | Notes |
| --------------------------- | --------------------------------------------------------- | ----------- | ----- |
| **authorization**           | **kotlin.String**                                         |             |       |
| **accountName**             | **kotlin.String**                                         |             |       |
| **bitcoinTransactionInput** | [**BitcoinTransactionInput**](bitcointransactioninput.md) |             |       |

#### Return type

[**BitcoinAPIResponse**](bitcoinapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json
