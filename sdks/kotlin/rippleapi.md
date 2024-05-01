# RippleApi

## RippleApi

All URIs are relative to _https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app_

| Method                                                          | HTTP request                           | Description |
| --------------------------------------------------------------- | -------------------------------------- | ----------- |
| [**createRippleAccount**](rippleapi.md#createRippleAccount)     | **POST** /ripple                       |             |
| [**getRippleAccount**](rippleapi.md#getRippleAccount)           | **GET** /ripple/{accountName}          |             |
| [**listRippleAccounts**](rippleapi.md#listRippleAccounts)       | **GET** /ripple                        |             |
| [**signRippleTransaction**](rippleapi.md#signRippleTransaction) | **POST** /ripple/{accountName}/sign-tx |             |

## **createRippleAccount**

> AccountAPIResponse createRippleAccount(authorization, rippleInput)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = RippleApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val rippleInput : RippleInput =  // RippleInput | 
try {
    val result : AccountAPIResponse = apiInstance.createRippleAccount(authorization, rippleInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RippleApi#createRippleAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RippleApi#createRippleAccount")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                              | Description | Notes |
| ----------------- | --------------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**                 |             |       |
| **rippleInput**   | [**RippleInput**](rippleinput.md) |             |       |

#### Return type

[**AccountAPIResponse**](accountapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **getRippleAccount**

> AccountAPIResponse getRippleAccount(authorization, accountName)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = RippleApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val accountName : kotlin.String = accountName_example // kotlin.String | 
try {
    val result : AccountAPIResponse = apiInstance.getRippleAccount(authorization, accountName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RippleApi#getRippleAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RippleApi#getRippleAccount")
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

## **listRippleAccounts**

> AccountAPIResponse listRippleAccounts(authorization)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = RippleApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
try {
    val result : AccountAPIResponse = apiInstance.listRippleAccounts(authorization)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RippleApi#listRippleAccounts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RippleApi#listRippleAccounts")
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

## **signRippleTransaction**

> RippleAPIResponse signRippleTransaction(authorization, accountName, rippleTransactionInput)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = RippleApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val accountName : kotlin.String = accountName_example // kotlin.String | 
val rippleTransactionInput : RippleTransactionInput =  // RippleTransactionInput | 
try {
    val result : RippleAPIResponse = apiInstance.signRippleTransaction(authorization, accountName, rippleTransactionInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RippleApi#signRippleTransaction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RippleApi#signRippleTransaction")
    e.printStackTrace()
}
```

#### Parameters

| Name                       | Type                                                    | Description | Notes |
| -------------------------- | ------------------------------------------------------- | ----------- | ----- |
| **authorization**          | **kotlin.String**                                       |             |       |
| **accountName**            | **kotlin.String**                                       |             |       |
| **rippleTransactionInput** | [**RippleTransactionInput**](rippletransactioninput.md) |             |       |

#### Return type

[**RippleAPIResponse**](rippleapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json
