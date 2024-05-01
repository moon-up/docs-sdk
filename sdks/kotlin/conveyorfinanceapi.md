# ConveyorFinanceApi

## ConveyorFinanceApi

All URIs are relative to _https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app_

| Method                                 | HTTP request                          | Description |
| -------------------------------------- | ------------------------------------- | ----------- |
| [**swap**](conveyorfinanceapi.md#swap) | **POST** /conveyorfinance/{name}/swap |             |

## **swap**

> ConveyorFinanceControllerResponse swap(authorization, name, tokenSwapParams)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = ConveyorFinanceApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val tokenSwapParams : TokenSwapParams =  // TokenSwapParams | 
try {
    val result : ConveyorFinanceControllerResponse = apiInstance.swap(authorization, name, tokenSwapParams)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConveyorFinanceApi#swap")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConveyorFinanceApi#swap")
    e.printStackTrace()
}
```

#### Parameters

| Name                | Type                                      | Description | Notes |
| ------------------- | ----------------------------------------- | ----------- | ----- |
| **authorization**   | **kotlin.String**                         |             |       |
| **name**            | **kotlin.String**                         |             |       |
| **tokenSwapParams** | [**TokenSwapParams**](tokenswapparams.md) |             |       |

#### Return type

[**ConveyorFinanceControllerResponse**](conveyorfinancecontrollerresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json
