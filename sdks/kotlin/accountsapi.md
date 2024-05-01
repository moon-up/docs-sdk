# AccountsApi

## AccountsApi

All URIs are relative to _https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app_

| Method                                                | HTTP request                                      | Description |
| ----------------------------------------------------- | ------------------------------------------------- | ----------- |
| [**broadcastTx**](accountsapi.md#broadcastTx)         | **POST** /accounts/{accountName}/broadcast-tx     |             |
| [**createAccount**](accountsapi.md#createAccount)     | **POST** /accounts                                |             |
| [**deleteAccount**](accountsapi.md#deleteAccount)     | **DELETE** /accounts/{accountName}                |             |
| [**deployContract**](accountsapi.md#deployContract)   | **POST** /accounts/{accountName}/deploy           |             |
| [**getAccount**](accountsapi.md#getAccount)           | **GET** /accounts/{accountName}                   |             |
| [**getBalance**](accountsapi.md#getBalance)           | **GET** /accounts/{accountName}/balance           |             |
| [**getNonce**](accountsapi.md#getNonce)               | **GET** /accounts/{accountName}/nonce             |             |
| [**listAccounts**](accountsapi.md#listAccounts)       | **GET** /accounts                                 |             |
| [**signMessage**](accountsapi.md#signMessage)         | **POST** /accounts/{accountName}/sign-message     |             |
| [**signTransaction**](accountsapi.md#signTransaction) | **POST** /accounts/{accountName}/sign-transaction |             |
| [**signTypedData**](accountsapi.md#signTypedData)     | **POST** /accounts/{accountName}/sign-typed-data  |             |
| [**transferEth**](accountsapi.md#transferEth)         | **POST** /accounts/{accountName}/transfer-eth     |             |

## **broadcastTx**

> BroadCastRawTransactionAPIResponse broadcastTx(authorization, accountName, broadcastInput)

#### Example

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

#### Parameters

| Name               | Type                                    | Description | Notes |
| ------------------ | --------------------------------------- | ----------- | ----- |
| **authorization**  | **kotlin.String**                       |             |       |
| **accountName**    | **kotlin.String**                       |             |       |
| **broadcastInput** | [**BroadcastInput**](broadcastinput.md) |             |       |

#### Return type

[**BroadCastRawTransactionAPIResponse**](broadcastrawtransactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **createAccount**

> AccountAPIResponse createAccount(authorization, createAccountInput)

#### Example

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

#### Parameters

| Name                   | Type                                            | Description | Notes |
| ---------------------- | ----------------------------------------------- | ----------- | ----- |
| **authorization**      | **kotlin.String**                               |             |       |
| **createAccountInput** | [**CreateAccountInput**](createaccountinput.md) |             |       |

#### Return type

[**AccountAPIResponse**](accountapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **deleteAccount**

> AccountAPIResponse deleteAccount(authorization, accountName)

#### Example

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

## **deployContract**

> TransactionAPIResponse deployContract(authorization, accountName, deployInput)

#### Example

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

#### Parameters

| Name              | Type                              | Description | Notes |
| ----------------- | --------------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**                 |             |       |
| **accountName**   | **kotlin.String**                 |             |       |
| **deployInput**   | [**DeployInput**](deployinput.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **getAccount**

> AccountAPIResponse getAccount(authorization, accountName)

#### Example

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

## **getBalance**

> BalanceAPIResponse getBalance(accountName, authorization, chainId)

#### Example

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

#### Parameters

| Name              | Type              | Description | Notes |
| ----------------- | ----------------- | ----------- | ----- |
| **accountName**   | **kotlin.String** |             |       |
| **authorization** | **kotlin.String** |             |       |
| **chainId**       | **kotlin.String** |             |       |

#### Return type

[**BalanceAPIResponse**](balanceapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

## **getNonce**

> NonceAPIResponse getNonce(accountName, authorization)

#### Example

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

#### Parameters

| Name              | Type              | Description | Notes |
| ----------------- | ----------------- | ----------- | ----- |
| **accountName**   | **kotlin.String** |             |       |
| **authorization** | **kotlin.String** |             |       |

#### Return type

[**NonceAPIResponse**](nonceapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

## **listAccounts**

> AccountAPIResponse listAccounts(authorization)

#### Example

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

## **signMessage**

> SignMessageAPIResponse signMessage(accountName, authorization, signMessage)

#### Example

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

#### Parameters

| Name              | Type                              | Description | Notes |
| ----------------- | --------------------------------- | ----------- | ----- |
| **accountName**   | **kotlin.String**                 |             |       |
| **authorization** | **kotlin.String**                 |             |       |
| **signMessage**   | [**SignMessage**](signmessage.md) |             |       |

#### Return type

[**SignMessageAPIResponse**](signmessageapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **signTransaction**

> TransactionAPIResponse signTransaction(accountName, authorization, inputBody)

#### Example

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

#### Parameters

| Name              | Type                          | Description | Notes |
| ----------------- | ----------------------------- | ----------- | ----- |
| **accountName**   | **kotlin.String**             |             |       |
| **authorization** | **kotlin.String**             |             |       |
| **inputBody**     | [**InputBody**](inputbody.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **signTypedData**

> SignMessageAPIResponse signTypedData(accountName, authorization, signTypedData)

#### Example

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

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **accountName**   | **kotlin.String**                     |             |       |
| **authorization** | **kotlin.String**                     |             |       |
| **signTypedData** | [**SignTypedData**](signtypeddata.md) |             |       |

#### Return type

[**SignMessageAPIResponse**](signmessageapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **transferEth**

> TransactionAPIResponse transferEth(accountName, authorization, inputBody)

#### Example

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

#### Parameters

| Name              | Type                          | Description | Notes |
| ----------------- | ----------------------------- | ----------- | ----- |
| **accountName**   | **kotlin.String**             |             |       |
| **authorization** | **kotlin.String**             |             |       |
| **inputBody**     | [**InputBody**](inputbody.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json
