# PaymentApi

## PaymentApi

All URIs are relative to _https://vault-api.usemoon.ai_

| Method                                                                       | HTTP request                         | Description |
| ---------------------------------------------------------------------------- | ------------------------------------ | ----------- |
| [**createPaymentIntentConfig**](paymentapi.md#createPaymentIntentConfig)     | **POST** /payment/config             |             |
| [**deletePaymentIntentConfig**](paymentapi.md#deletePaymentIntentConfig)     | **DELETE** /payment/config/{id}      |             |
| [**getAllPaymentIntentConfigs**](paymentapi.md#getAllPaymentIntentConfigs)   | **GET** /payment/config              |             |
| [**getOnePaymentIntentConfigs**](paymentapi.md#getOnePaymentIntentConfigs)   | **GET** /payment/config/{id}         |             |
| [**moralisWebhook**](paymentapi.md#moralisWebhook)                           | **POST** /payment/webhook/{id}       |             |
| [**paymentCreatePaymentIntent**](paymentapi.md#paymentCreatePaymentIntent)   | **POST** /payment                    |             |
| [**paymentDeletePaymentIntent**](paymentapi.md#paymentDeletePaymentIntent)   | **DELETE** /payment/{id}             |             |
| [**paymentGetAllPaymentIntents**](paymentapi.md#paymentGetAllPaymentIntents) | **GET** /payment                     |             |
| [**paymentGetAvailableChains**](paymentapi.md#paymentGetAvailableChains)     | **GET** /payment/chains              |             |
| [**paymentGetPaymentIntent**](paymentapi.md#paymentGetPaymentIntent)         | **GET** /payment/{id}                |             |
| [**paymentUpdatePaymentIntent**](paymentapi.md#paymentUpdatePaymentIntent)   | **PUT** /payment/{id}                |             |
| [**tatumWebhook**](paymentapi.md#tatumWebhook)                               | **POST** /payment/webhook/tatum/{id} |             |
| [**updatePaymentIntentConfig**](paymentapi.md#updatePaymentIntentConfig)     | **PUT** /payment/config/{id}         |             |

## **createPaymentIntentConfig**

> kotlin.Any createPaymentIntentConfig(authorization, body)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = PaymentApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.createPaymentIntentConfig(authorization, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentApi#createPaymentIntentConfig")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentApi#createPaymentIntentConfig")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type              | Description | Notes |
| ----------------- | ----------------- | ----------- | ----- |
| **authorization** | **kotlin.String** |             |       |
| **body**          | **kotlin.Any**    |             |       |

#### Return type

[**kotlin.Any**](../../kotlin/docs/kotlin.Any.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **deletePaymentIntentConfig**

> PaymentIntentResponse deletePaymentIntentConfig(authorization, id)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = PaymentApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : PaymentIntentResponse = apiInstance.deletePaymentIntentConfig(authorization, id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentApi#deletePaymentIntentConfig")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentApi#deletePaymentIntentConfig")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type              | Description | Notes |
| ----------------- | ----------------- | ----------- | ----- |
| **authorization** | **kotlin.String** |             |       |
| **id**            | **kotlin.String** |             |       |

#### Return type

[**PaymentIntentResponse**](paymentintentresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

## **getAllPaymentIntentConfigs**

> kotlin.collections.List\<PaymentIntentResponse> getAllPaymentIntentConfigs(authorization)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = PaymentApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
try {
    val result : kotlin.collections.List<PaymentIntentResponse> = apiInstance.getAllPaymentIntentConfigs(authorization)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentApi#getAllPaymentIntentConfigs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentApi#getAllPaymentIntentConfigs")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type              | Description | Notes |
| ----------------- | ----------------- | ----------- | ----- |
| **authorization** | **kotlin.String** |             |       |

#### Return type

[**kotlin.collections.List\<PaymentIntentResponse>**](paymentintentresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

## **getOnePaymentIntentConfigs**

> PaymentIntentResponse getOnePaymentIntentConfigs(authorization, id)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = PaymentApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : PaymentIntentResponse = apiInstance.getOnePaymentIntentConfigs(authorization, id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentApi#getOnePaymentIntentConfigs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentApi#getOnePaymentIntentConfigs")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type              | Description | Notes |
| ----------------- | ----------------- | ----------- | ----- |
| **authorization** | **kotlin.String** |             |       |
| **id**            | **kotlin.String** |             |       |

#### Return type

[**PaymentIntentResponse**](paymentintentresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

## **moralisWebhook**

> kotlin.Any moralisWebhook(id, iwebhook)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = PaymentApi()
val id : kotlin.String = id_example // kotlin.String | 
val iwebhook : IWebhook =  // IWebhook | 
try {
    val result : kotlin.Any = apiInstance.moralisWebhook(id, iwebhook)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentApi#moralisWebhook")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentApi#moralisWebhook")
    e.printStackTrace()
}
```

#### Parameters

| Name         | Type                        | Description | Notes |
| ------------ | --------------------------- | ----------- | ----- |
| **id**       | **kotlin.String**           |             |       |
| **iwebhook** | [**IWebhook**](iwebhook.md) |             |       |

#### Return type

[**kotlin.Any**](../../kotlin/docs/kotlin.Any.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **paymentCreatePaymentIntent**

> PaymentIntentResponse paymentCreatePaymentIntent(authorization, createPaymentIntentInput)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = PaymentApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val createPaymentIntentInput : CreatePaymentIntentInput =  // CreatePaymentIntentInput | 
try {
    val result : PaymentIntentResponse = apiInstance.paymentCreatePaymentIntent(authorization, createPaymentIntentInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentApi#paymentCreatePaymentIntent")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentApi#paymentCreatePaymentIntent")
    e.printStackTrace()
}
```

#### Parameters

| Name                         | Type                                                        | Description | Notes |
| ---------------------------- | ----------------------------------------------------------- | ----------- | ----- |
| **authorization**            | **kotlin.String**                                           |             |       |
| **createPaymentIntentInput** | [**CreatePaymentIntentInput**](createpaymentintentinput.md) |             |       |

#### Return type

[**PaymentIntentResponse**](paymentintentresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **paymentDeletePaymentIntent**

> PaymentIntentResponse paymentDeletePaymentIntent(authorization, id)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = PaymentApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : PaymentIntentResponse = apiInstance.paymentDeletePaymentIntent(authorization, id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentApi#paymentDeletePaymentIntent")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentApi#paymentDeletePaymentIntent")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type              | Description | Notes |
| ----------------- | ----------------- | ----------- | ----- |
| **authorization** | **kotlin.String** |             |       |
| **id**            | **kotlin.String** |             |       |

#### Return type

[**PaymentIntentResponse**](paymentintentresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

## **paymentGetAllPaymentIntents**

> kotlin.collections.List\<PaymentIntentResponse> paymentGetAllPaymentIntents(authorization)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = PaymentApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
try {
    val result : kotlin.collections.List<PaymentIntentResponse> = apiInstance.paymentGetAllPaymentIntents(authorization)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentApi#paymentGetAllPaymentIntents")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentApi#paymentGetAllPaymentIntents")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type              | Description | Notes |
| ----------------- | ----------------- | ----------- | ----- |
| **authorization** | **kotlin.String** |             |       |

#### Return type

[**kotlin.collections.List\<PaymentIntentResponse>**](paymentintentresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

## **paymentGetAvailableChains**

> kotlin.collections.List\<kotlin.String> paymentGetAvailableChains()

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = PaymentApi()
try {
    val result : kotlin.collections.List<kotlin.String> = apiInstance.paymentGetAvailableChains()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentApi#paymentGetAvailableChains")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentApi#paymentGetAvailableChains")
    e.printStackTrace()
}
```

#### Parameters

This endpoint does not need any parameter.

#### Return type

**kotlin.collections.List\<kotlin.String>**

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

## **paymentGetPaymentIntent**

> PaymentIntentResponse paymentGetPaymentIntent(authorization, id)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = PaymentApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : PaymentIntentResponse = apiInstance.paymentGetPaymentIntent(authorization, id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentApi#paymentGetPaymentIntent")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentApi#paymentGetPaymentIntent")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type              | Description | Notes |
| ----------------- | ----------------- | ----------- | ----- |
| **authorization** | **kotlin.String** |             |       |
| **id**            | **kotlin.String** |             |       |

#### Return type

[**PaymentIntentResponse**](paymentintentresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

## **paymentUpdatePaymentIntent**

> PaymentIntentResponse paymentUpdatePaymentIntent(authorization, id, createPaymentIntentInput)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = PaymentApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val id : kotlin.String = id_example // kotlin.String | 
val createPaymentIntentInput : CreatePaymentIntentInput =  // CreatePaymentIntentInput | 
try {
    val result : PaymentIntentResponse = apiInstance.paymentUpdatePaymentIntent(authorization, id, createPaymentIntentInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentApi#paymentUpdatePaymentIntent")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentApi#paymentUpdatePaymentIntent")
    e.printStackTrace()
}
```

#### Parameters

| Name                         | Type                                                        | Description | Notes |
| ---------------------------- | ----------------------------------------------------------- | ----------- | ----- |
| **authorization**            | **kotlin.String**                                           |             |       |
| **id**                       | **kotlin.String**                                           |             |       |
| **createPaymentIntentInput** | [**CreatePaymentIntentInput**](createpaymentintentinput.md) |             |       |

#### Return type

[**PaymentIntentResponse**](paymentintentresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **tatumWebhook**

> kotlin.Any tatumWebhook(id, tatumTransactionEvent)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = PaymentApi()
val id : kotlin.String = id_example // kotlin.String | 
val tatumTransactionEvent : TatumTransactionEvent =  // TatumTransactionEvent | 
try {
    val result : kotlin.Any = apiInstance.tatumWebhook(id, tatumTransactionEvent)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentApi#tatumWebhook")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentApi#tatumWebhook")
    e.printStackTrace()
}
```

#### Parameters

| Name                      | Type                                                  | Description | Notes |
| ------------------------- | ----------------------------------------------------- | ----------- | ----- |
| **id**                    | **kotlin.String**                                     |             |       |
| **tatumTransactionEvent** | [**TatumTransactionEvent**](tatumtransactionevent.md) |             |       |

#### Return type

[**kotlin.Any**](../../kotlin/docs/kotlin.Any.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **updatePaymentIntentConfig**

> PaymentIntentResponse updatePaymentIntentConfig(authorization, id, body)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = PaymentApi()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val id : kotlin.String = id_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : PaymentIntentResponse = apiInstance.updatePaymentIntentConfig(authorization, id, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentApi#updatePaymentIntentConfig")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentApi#updatePaymentIntentConfig")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type              | Description | Notes |
| ----------------- | ----------------- | ----------- | ----- |
| **authorization** | **kotlin.String** |             |       |
| **id**            | **kotlin.String** |             |       |
| **body**          | **kotlin.Any**    |             |       |

#### Return type

[**PaymentIntentResponse**](paymentintentresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json
