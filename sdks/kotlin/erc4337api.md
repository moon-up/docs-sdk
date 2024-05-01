# Erc4337Api

## Erc4337Api

All URIs are relative to _https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app_

| Method                                                           | HTTP request                                             | Description |
| ---------------------------------------------------------------- | -------------------------------------------------------- | ----------- |
| [**getAddress**](erc4337api.md#getAddress)                       | **POST** /erc4337/{accountName}/address                  |             |
| [**signBroadcastUserOpTx**](erc4337api.md#signBroadcastUserOpTx) | **POST** /erc4337/{accountName}/sign-broadcast-userop-tx |             |

## **getAddress**

> AccountAPIResponse getAddress(authorization, accountName, inputBody)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = Erc4337Api()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val accountName : kotlin.String = accountName_example // kotlin.String | 
val inputBody : InputBody =  // InputBody | 
try {
    val result : AccountAPIResponse = apiInstance.getAddress(authorization, accountName, inputBody)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling Erc4337Api#getAddress")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling Erc4337Api#getAddress")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                          | Description | Notes |
| ----------------- | ----------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**             |             |       |
| **accountName**   | **kotlin.String**             |             |       |
| **inputBody**     | [**InputBody**](inputbody.md) |             |       |

#### Return type

[**AccountAPIResponse**](accountapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **signBroadcastUserOpTx**

> TransactionAPIResponse signBroadcastUserOpTx(authorization, accountName, inputBody)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = Erc4337Api()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val accountName : kotlin.String = accountName_example // kotlin.String | 
val inputBody : InputBody =  // InputBody | 
try {
    val result : TransactionAPIResponse = apiInstance.signBroadcastUserOpTx(authorization, accountName, inputBody)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling Erc4337Api#signBroadcastUserOpTx")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling Erc4337Api#signBroadcastUserOpTx")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                          | Description | Notes |
| ----------------- | ----------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**             |             |       |
| **accountName**   | **kotlin.String**             |             |       |
| **inputBody**     | [**InputBody**](inputbody.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json
