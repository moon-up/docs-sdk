# EosApi

## EosApi

All URIs are relative to _https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app_

| Method                                                 | HTTP request                        | Description |
| ------------------------------------------------------ | ----------------------------------- | ----------- |
| [**createEosAccount**](eosapi.md#createEosAccount)     | **POST** /eos                       |             |
| [**getEosAccount**](eosapi.md#getEosAccount)           | **GET** /eos/{accountName}          |             |
| [**listEosAccounts**](eosapi.md#listEosAccounts)       | **GET** /eos                        |             |
| [**signEosTransaction**](eosapi.md#signEosTransaction) | **POST** /eos/{accountName}/sign-tx |             |

## **createEosAccount**

> AccountAPIResponse createEosAccount(authorization, eosInput)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = EosApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val eosInput : EosInput =  // EosInput | 
try {
    val result : AccountAPIResponse = apiInstance.createEosAccount(authorization, eosInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EosApi#createEosAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EosApi#createEosAccount")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                        | Description | Notes |
| ----------------- | --------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**           |             |       |
| **eosInput**      | [**EosInput**](eosinput.md) |             |       |

#### Return type

[**AccountAPIResponse**](accountapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **getEosAccount**

> AccountAPIResponse getEosAccount(authorization, accountName)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = EosApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val accountName : kotlin.String = accountName_example // kotlin.String | 
try {
    val result : AccountAPIResponse = apiInstance.getEosAccount(authorization, accountName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EosApi#getEosAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EosApi#getEosAccount")
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

## **listEosAccounts**

> AccountAPIResponse listEosAccounts(authorization)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = EosApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
try {
    val result : AccountAPIResponse = apiInstance.listEosAccounts(authorization)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EosApi#listEosAccounts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EosApi#listEosAccounts")
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

## **signEosTransaction**

> EosAPIResponse signEosTransaction(authorization, accountName, eosTransactionInput)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = EosApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val accountName : kotlin.String = accountName_example // kotlin.String | 
val eosTransactionInput : EosTransactionInput =  // EosTransactionInput | 
try {
    val result : EosAPIResponse = apiInstance.signEosTransaction(authorization, accountName, eosTransactionInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EosApi#signEosTransaction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EosApi#signEosTransaction")
    e.printStackTrace()
}
```

#### Parameters

| Name                    | Type                                              | Description | Notes |
| ----------------------- | ------------------------------------------------- | ----------- | ----- |
| **authorization**       | **kotlin.String**                                 |             |       |
| **accountName**         | **kotlin.String**                                 |             |       |
| **eosTransactionInput** | [**EosTransactionInput**](eostransactioninput.md) |             |       |

#### Return type

[**EosAPIResponse**](eosapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json
