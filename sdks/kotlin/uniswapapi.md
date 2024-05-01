# UniSwapApi

## UniSwapApi

All URIs are relative to _https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app_

| Method                                                                 | HTTP request                                          | Description |
| ---------------------------------------------------------------------- | ----------------------------------------------------- | ----------- |
| [**addLiquidity**](uniswapapi.md#addLiquidity)                         | **POST** /uniswap/{name}/add-liquidity                |             |
| [**removeLiquidity**](uniswapapi.md#removeLiquidity)                   | **POST** /uniswap/{name}/remove-liquidity             |             |
| [**swapExactETHForTokens**](uniswapapi.md#swapExactETHForTokens)       | **POST** /uniswap/{name}/swap-exact-eth-for-tokens    |             |
| [**swapExactTokensForTokens**](uniswapapi.md#swapExactTokensForTokens) | **POST** /uniswap/{name}/swap-exact-tokens-for-tokens |             |

## **addLiquidity**

> TransactionAPIResponse addLiquidity(authorization, name, uniswapInput)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = UniSwapApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val uniswapInput : UniswapInput =  // UniswapInput | 
try {
    val result : TransactionAPIResponse = apiInstance.addLiquidity(authorization, name, uniswapInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UniSwapApi#addLiquidity")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UniSwapApi#addLiquidity")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                                | Description | Notes |
| ----------------- | ----------------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**                   |             |       |
| **name**          | **kotlin.String**                   |             |       |
| **uniswapInput**  | [**UniswapInput**](uniswapinput.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **removeLiquidity**

> TransactionAPIResponse removeLiquidity(authorization, name, uniswapInput)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = UniSwapApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val uniswapInput : UniswapInput =  // UniswapInput | 
try {
    val result : TransactionAPIResponse = apiInstance.removeLiquidity(authorization, name, uniswapInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UniSwapApi#removeLiquidity")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UniSwapApi#removeLiquidity")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                                | Description | Notes |
| ----------------- | ----------------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**                   |             |       |
| **name**          | **kotlin.String**                   |             |       |
| **uniswapInput**  | [**UniswapInput**](uniswapinput.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **swapExactETHForTokens**

> TransactionAPIResponse swapExactETHForTokens(authorization, name, uniswapInput)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = UniSwapApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val uniswapInput : UniswapInput =  // UniswapInput | 
try {
    val result : TransactionAPIResponse = apiInstance.swapExactETHForTokens(authorization, name, uniswapInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UniSwapApi#swapExactETHForTokens")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UniSwapApi#swapExactETHForTokens")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                                | Description | Notes |
| ----------------- | ----------------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**                   |             |       |
| **name**          | **kotlin.String**                   |             |       |
| **uniswapInput**  | [**UniswapInput**](uniswapinput.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **swapExactTokensForTokens**

> TransactionAPIResponse swapExactTokensForTokens(authorization, name, uniswapInput)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = UniSwapApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val uniswapInput : UniswapInput =  // UniswapInput | 
try {
    val result : TransactionAPIResponse = apiInstance.swapExactTokensForTokens(authorization, name, uniswapInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UniSwapApi#swapExactTokensForTokens")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UniSwapApi#swapExactTokensForTokens")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                                | Description | Notes |
| ----------------- | ----------------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**                   |             |       |
| **name**          | **kotlin.String**                   |             |       |
| **uniswapInput**  | [**UniswapInput**](uniswapinput.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json
