# OneinchApi

## OneinchApi

All URIs are relative to _https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app_

| Method                                               | HTTP request                         | Description |
| ---------------------------------------------------- | ------------------------------------ | ----------- |
| [**approveCallData**](oneinchapi.md#approveCallData) | **POST** /oneinch/approve-call-data  |             |
| [**approveSpender**](oneinchapi.md#approveSpender)   | **POST** /oneinch/approve-spender    |             |
| [**protocols**](oneinchapi.md#protocols)             | **POST** /oneinch/protocols          |             |
| [**quote**](oneinchapi.md#quote)                     | **POST** /oneinch/quote              |             |
| [**swap**](oneinchapi.md#swap)                       | **POST** /oneinch/{accountName}/swap |             |
| [**tokens**](oneinchapi.md#tokens)                   | **POST** /oneinch/tokens             |             |

## **approveCallData**

> kotlin.Any approveCallData(body)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = OneinchApi()
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.approveCallData(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OneinchApi#approveCallData")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OneinchApi#approveCallData")
    e.printStackTrace()
}
```

#### Parameters

| Name     | Type           | Description | Notes |
| -------- | -------------- | ----------- | ----- |
| **body** | **kotlin.Any** |             |       |

#### Return type

[**kotlin.Any**](../../kotlin/docs/kotlin.Any.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **approveSpender**

> kotlin.Any approveSpender(body)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = OneinchApi()
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.approveSpender(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OneinchApi#approveSpender")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OneinchApi#approveSpender")
    e.printStackTrace()
}
```

#### Parameters

| Name     | Type           | Description | Notes |
| -------- | -------------- | ----------- | ----- |
| **body** | **kotlin.Any** |             |       |

#### Return type

[**kotlin.Any**](../../kotlin/docs/kotlin.Any.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **protocols**

> kotlin.Any protocols(body)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = OneinchApi()
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.protocols(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OneinchApi#protocols")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OneinchApi#protocols")
    e.printStackTrace()
}
```

#### Parameters

| Name     | Type           | Description | Notes |
| -------- | -------------- | ----------- | ----- |
| **body** | **kotlin.Any** |             |       |

#### Return type

[**kotlin.Any**](../../kotlin/docs/kotlin.Any.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **quote**

> kotlin.Any quote(body)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = OneinchApi()
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.quote(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OneinchApi#quote")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OneinchApi#quote")
    e.printStackTrace()
}
```

#### Parameters

| Name     | Type           | Description | Notes |
| -------- | -------------- | ----------- | ----- |
| **body** | **kotlin.Any** |             |       |

#### Return type

[**kotlin.Any**](../../kotlin/docs/kotlin.Any.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **swap**

> kotlin.Any swap(accountName, authorization, getSwapDto)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = OneinchApi()
val accountName : kotlin.String = accountName_example // kotlin.String | 
val authorization : kotlin.String = authorization_example // kotlin.String | 
val getSwapDto : GetSwapDto =  // GetSwapDto | 
try {
    val result : kotlin.Any = apiInstance.swap(accountName, authorization, getSwapDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OneinchApi#swap")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OneinchApi#swap")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                            | Description | Notes |
| ----------------- | ------------------------------- | ----------- | ----- |
| **accountName**   | **kotlin.String**               |             |       |
| **authorization** | **kotlin.String**               |             |       |
| **getSwapDto**    | [**GetSwapDto**](getswapdto.md) |             |       |

#### Return type

[**kotlin.Any**](../../kotlin/docs/kotlin.Any.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **tokens**

> kotlin.Any tokens(body)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = OneinchApi()
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.tokens(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OneinchApi#tokens")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OneinchApi#tokens")
    e.printStackTrace()
}
```

#### Parameters

| Name     | Type           | Description | Notes |
| -------- | -------------- | ----------- | ----- |
| **body** | **kotlin.Any** |             |       |

#### Return type

[**kotlin.Any**](../../kotlin/docs/kotlin.Any.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json
