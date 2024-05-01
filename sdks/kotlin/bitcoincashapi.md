# BitcoincashApi

## BitcoincashApi

All URIs are relative to _https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app_

| Method                                                                         | HTTP request                                | Description |
| ------------------------------------------------------------------------------ | ------------------------------------------- | ----------- |
| [**createBitcoinCashAccount**](bitcoincashapi.md#createBitcoinCashAccount)     | **POST** /bitcoincash                       |             |
| [**getBitcoinCashAccount**](bitcoincashapi.md#getBitcoinCashAccount)           | **GET** /bitcoincash/{accountName}          |             |
| [**listBitcoinCashAccounts**](bitcoincashapi.md#listBitcoinCashAccounts)       | **GET** /bitcoincash                        |             |
| [**signBitcoinCashTransaction**](bitcoincashapi.md#signBitcoinCashTransaction) | **POST** /bitcoincash/{accountName}/sign-tx |             |

## **createBitcoinCashAccount**

> AccountAPIResponse createBitcoinCashAccount(authorization, bitcoinCashInput)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = BitcoincashApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val bitcoinCashInput : BitcoinCashInput =  // BitcoinCashInput | 
try {
    val result : AccountAPIResponse = apiInstance.createBitcoinCashAccount(authorization, bitcoinCashInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BitcoincashApi#createBitcoinCashAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BitcoincashApi#createBitcoinCashAccount")
    e.printStackTrace()
}
```

#### Parameters

| Name                 | Type                                        | Description | Notes |
| -------------------- | ------------------------------------------- | ----------- | ----- |
| **authorization**    | **kotlin.String**                           |             |       |
| **bitcoinCashInput** | [**BitcoinCashInput**](bitcoincashinput.md) |             |       |

#### Return type

[**AccountAPIResponse**](accountapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **getBitcoinCashAccount**

> AccountAPIResponse getBitcoinCashAccount(authorization, accountName)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = BitcoincashApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val accountName : kotlin.String = accountName_example // kotlin.String | 
try {
    val result : AccountAPIResponse = apiInstance.getBitcoinCashAccount(authorization, accountName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BitcoincashApi#getBitcoinCashAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BitcoincashApi#getBitcoinCashAccount")
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

## **listBitcoinCashAccounts**

> AccountAPIResponse listBitcoinCashAccounts(authorization)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = BitcoincashApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
try {
    val result : AccountAPIResponse = apiInstance.listBitcoinCashAccounts(authorization)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BitcoincashApi#listBitcoinCashAccounts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BitcoincashApi#listBitcoinCashAccounts")
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

## **signBitcoinCashTransaction**

> BitcoinCashAPIResponse signBitcoinCashTransaction(authorization, accountName, bitcoinCashTransactionInput)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = BitcoincashApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val accountName : kotlin.String = accountName_example // kotlin.String | 
val bitcoinCashTransactionInput : BitcoinCashTransactionInput =  // BitcoinCashTransactionInput | 
try {
    val result : BitcoinCashAPIResponse = apiInstance.signBitcoinCashTransaction(authorization, accountName, bitcoinCashTransactionInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BitcoincashApi#signBitcoinCashTransaction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BitcoincashApi#signBitcoinCashTransaction")
    e.printStackTrace()
}
```

#### Parameters

| Name                            | Type                                                              | Description | Notes |
| ------------------------------- | ----------------------------------------------------------------- | ----------- | ----- |
| **authorization**               | **kotlin.String**                                                 |             |       |
| **accountName**                 | **kotlin.String**                                                 |             |       |
| **bitcoinCashTransactionInput** | [**BitcoinCashTransactionInput**](bitcoincashtransactioninput.md) |             |       |

#### Return type

[**BitcoinCashAPIResponse**](bitcoincashapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json
