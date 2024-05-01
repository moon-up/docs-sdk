# AaveApi

## AaveApi

All URIs are relative to _https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app_

| Method                                            | HTTP request                            | Description |
| ------------------------------------------------- | --------------------------------------- | ----------- |
| [**borrow**](aaveapi.md#borrow)                   | **POST** /aave/{name}/borrow            |             |
| [**lend**](aaveapi.md#lend)                       | **POST** /aave/{name}/lend              |             |
| [**repay**](aaveapi.md#repay)                     | **POST** /aave/{name}/repay             |             |
| [**userReserveData**](aaveapi.md#userReserveData) | **POST** /aave/{name}/user-reserve-data |             |

## **borrow**

> TransactionAPIResponse borrow(authorization, name, aaveInput)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = AaveApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val aaveInput : AaveInput =  // AaveInput | 
try {
    val result : TransactionAPIResponse = apiInstance.borrow(authorization, name, aaveInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AaveApi#borrow")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AaveApi#borrow")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                          | Description | Notes |
| ----------------- | ----------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**             |             |       |
| **name**          | **kotlin.String**             |             |       |
| **aaveInput**     | [**AaveInput**](aaveinput.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **lend**

> TransactionAPIResponse lend(authorization, name, aaveInput)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = AaveApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val aaveInput : AaveInput =  // AaveInput | 
try {
    val result : TransactionAPIResponse = apiInstance.lend(authorization, name, aaveInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AaveApi#lend")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AaveApi#lend")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                          | Description | Notes |
| ----------------- | ----------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**             |             |       |
| **name**          | **kotlin.String**             |             |       |
| **aaveInput**     | [**AaveInput**](aaveinput.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **repay**

> TransactionAPIResponse repay(authorization, name, aaveInput)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = AaveApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val aaveInput : AaveInput =  // AaveInput | 
try {
    val result : TransactionAPIResponse = apiInstance.repay(authorization, name, aaveInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AaveApi#repay")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AaveApi#repay")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                          | Description | Notes |
| ----------------- | ----------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**             |             |       |
| **name**          | **kotlin.String**             |             |       |
| **aaveInput**     | [**AaveInput**](aaveinput.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **userReserveData**

> AaveReservesAPIResponse userReserveData(authorization, name, aaveInput)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = AaveApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val aaveInput : AaveInput =  // AaveInput | 
try {
    val result : AaveReservesAPIResponse = apiInstance.userReserveData(authorization, name, aaveInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AaveApi#userReserveData")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AaveApi#userReserveData")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                          | Description | Notes |
| ----------------- | ----------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**             |             |       |
| **name**          | **kotlin.String**             |             |       |
| **aaveInput**     | [**AaveInput**](aaveinput.md) |             |       |

#### Return type

[**AaveReservesAPIResponse**](aavereservesapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json
