# Erc721Api

## Erc721Api

All URIs are relative to _https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app_

| Method                                                  | HTTP request                                 | Description |
| ------------------------------------------------------- | -------------------------------------------- | ----------- |
| [**approve**](erc721api.md#approve)                     | **POST** /erc721/{name}/approve              |             |
| [**balanceOf**](erc721api.md#balanceOf)                 | **POST** /erc721/{name}/balance-of           |             |
| [**getApproved**](erc721api.md#getApproved)             | **POST** /erc721/{name}/get-approved         |             |
| [**isApprovedForAll**](erc721api.md#isApprovedForAll)   | **POST** /erc721/{name}/is-approved-for-all  |             |
| [**name**](erc721api.md#name)                           | **POST** /erc721/{name}/name                 |             |
| [**ownerOf**](erc721api.md#ownerOf)                     | **POST** /erc721/{name}/owner-of             |             |
| [**safeTransferFrom**](erc721api.md#safeTransferFrom)   | **POST** /erc721/{name}/safe-transfer-from   |             |
| [**setApprovalForAll**](erc721api.md#setApprovalForAll) | **POST** /erc721/{name}/set-approval-for-all |             |
| [**symbol**](erc721api.md#symbol)                       | **POST** /erc721/{name}/symbol               |             |
| [**tokenUri**](erc721api.md#tokenUri)                   | **POST** /erc721/{name}/token-uri            |             |
| [**transfer**](erc721api.md#transfer)                   | **POST** /erc721/{name}/transfer             |             |
| [**transferFrom**](erc721api.md#transferFrom)           | **POST** /erc721/{name}/transfer-from        |             |

## **approve**

> TransactionAPIResponse approve(authorization, name, erc721Request)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = Erc721Api()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val erc721Request : Erc721Request =  // Erc721Request | 
try {
    val result : TransactionAPIResponse = apiInstance.approve(authorization, name, erc721Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling Erc721Api#approve")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling Erc721Api#approve")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**                     |             |       |
| **name**          | **kotlin.String**                     |             |       |
| **erc721Request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **balanceOf**

> TransactionAPIResponse balanceOf(authorization, name, erc721Request)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = Erc721Api()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val erc721Request : Erc721Request =  // Erc721Request | 
try {
    val result : TransactionAPIResponse = apiInstance.balanceOf(authorization, name, erc721Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling Erc721Api#balanceOf")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling Erc721Api#balanceOf")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**                     |             |       |
| **name**          | **kotlin.String**                     |             |       |
| **erc721Request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **getApproved**

> TransactionAPIResponse getApproved(authorization, name, erc721Request)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = Erc721Api()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val erc721Request : Erc721Request =  // Erc721Request | 
try {
    val result : TransactionAPIResponse = apiInstance.getApproved(authorization, name, erc721Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling Erc721Api#getApproved")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling Erc721Api#getApproved")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**                     |             |       |
| **name**          | **kotlin.String**                     |             |       |
| **erc721Request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **isApprovedForAll**

> TransactionAPIResponse isApprovedForAll(authorization, name, erc721Request)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = Erc721Api()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val erc721Request : Erc721Request =  // Erc721Request | 
try {
    val result : TransactionAPIResponse = apiInstance.isApprovedForAll(authorization, name, erc721Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling Erc721Api#isApprovedForAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling Erc721Api#isApprovedForAll")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**                     |             |       |
| **name**          | **kotlin.String**                     |             |       |
| **erc721Request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **name**

> TransactionAPIResponse name(authorization, name, erc721Request)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = Erc721Api()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val erc721Request : Erc721Request =  // Erc721Request | 
try {
    val result : TransactionAPIResponse = apiInstance.name(authorization, name, erc721Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling Erc721Api#name")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling Erc721Api#name")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**                     |             |       |
| **name**          | **kotlin.String**                     |             |       |
| **erc721Request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **ownerOf**

> TransactionAPIResponse ownerOf(authorization, name, erc721Request)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = Erc721Api()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val erc721Request : Erc721Request =  // Erc721Request | 
try {
    val result : TransactionAPIResponse = apiInstance.ownerOf(authorization, name, erc721Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling Erc721Api#ownerOf")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling Erc721Api#ownerOf")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**                     |             |       |
| **name**          | **kotlin.String**                     |             |       |
| **erc721Request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **safeTransferFrom**

> TransactionAPIResponse safeTransferFrom(authorization, name, erc721Request)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = Erc721Api()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val erc721Request : Erc721Request =  // Erc721Request | 
try {
    val result : TransactionAPIResponse = apiInstance.safeTransferFrom(authorization, name, erc721Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling Erc721Api#safeTransferFrom")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling Erc721Api#safeTransferFrom")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**                     |             |       |
| **name**          | **kotlin.String**                     |             |       |
| **erc721Request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **setApprovalForAll**

> TransactionAPIResponse setApprovalForAll(authorization, name, erc721Request)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = Erc721Api()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val erc721Request : Erc721Request =  // Erc721Request | 
try {
    val result : TransactionAPIResponse = apiInstance.setApprovalForAll(authorization, name, erc721Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling Erc721Api#setApprovalForAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling Erc721Api#setApprovalForAll")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**                     |             |       |
| **name**          | **kotlin.String**                     |             |       |
| **erc721Request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **symbol**

> TransactionAPIResponse symbol(authorization, name, erc721Request)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = Erc721Api()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val erc721Request : Erc721Request =  // Erc721Request | 
try {
    val result : TransactionAPIResponse = apiInstance.symbol(authorization, name, erc721Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling Erc721Api#symbol")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling Erc721Api#symbol")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**                     |             |       |
| **name**          | **kotlin.String**                     |             |       |
| **erc721Request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **tokenUri**

> TransactionAPIResponse tokenUri(authorization, name, erc721Request)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = Erc721Api()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val erc721Request : Erc721Request =  // Erc721Request | 
try {
    val result : TransactionAPIResponse = apiInstance.tokenUri(authorization, name, erc721Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling Erc721Api#tokenUri")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling Erc721Api#tokenUri")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**                     |             |       |
| **name**          | **kotlin.String**                     |             |       |
| **erc721Request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **transfer**

> TransactionAPIResponse transfer(authorization, name, erc721Request)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = Erc721Api()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val erc721Request : Erc721Request =  // Erc721Request | 
try {
    val result : TransactionAPIResponse = apiInstance.transfer(authorization, name, erc721Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling Erc721Api#transfer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling Erc721Api#transfer")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**                     |             |       |
| **name**          | **kotlin.String**                     |             |       |
| **erc721Request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **transferFrom**

> TransactionAPIResponse transferFrom(authorization, name, erc721Request)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = Erc721Api()
val authorization : kotlin.String = authorization_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val erc721Request : Erc721Request =  // Erc721Request | 
try {
    val result : TransactionAPIResponse = apiInstance.transferFrom(authorization, name, erc721Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling Erc721Api#transferFrom")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling Erc721Api#transferFrom")
    e.printStackTrace()
}
```

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **kotlin.String**                     |             |       |
| **name**          | **kotlin.String**                     |             |       |
| **erc721Request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json
