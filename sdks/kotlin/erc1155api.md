# ERC1155Api

## ERC1155Api

All URIs are relative to _https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app_

| Method                                                           | HTTP request                                      | Description |
| ---------------------------------------------------------------- | ------------------------------------------------- | ----------- |
| [**balanceOf**](erc1155api.md#balanceOf)                         | **POST** /erc1155/{name}/balance-of               |             |
| [**balanceOfBatch**](erc1155api.md#balanceOfBatch)               | **POST** /erc1155/{name}/balance-of-batch         |             |
| [**isApprovedForAll**](erc1155api.md#isApprovedForAll)           | **POST** /erc1155/{name}/is-approved-for-all      |             |
| [**safeBatchTransferFrom**](erc1155api.md#safeBatchTransferFrom) | **POST** /erc1155/{name}/safe-batch-transfer-from |             |
| [**safeTransferFrom**](erc1155api.md#safeTransferFrom)           | **POST** /erc1155/{name}/safe-transfer-from       |             |
| [**setApprovalForAll**](erc1155api.md#setApprovalForAll)         | **POST** /erc1155/{name}/set-approval-for-all     |             |

## **balanceOf**

> TransactionAPIResponse balanceOf(name, authorization, erc1155Request)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = ERC1155Api()
val name : kotlin.String = name_example // kotlin.String | 
val authorization : kotlin.String = authorization_example // kotlin.String | 
val erc1155Request : Erc1155Request =  // Erc1155Request | 
try {
    val result : TransactionAPIResponse = apiInstance.balanceOf(name, authorization, erc1155Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ERC1155Api#balanceOf")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ERC1155Api#balanceOf")
    e.printStackTrace()
}
```

#### Parameters

| Name               | Type                                    | Description | Notes |
| ------------------ | --------------------------------------- | ----------- | ----- |
| **name**           | **kotlin.String**                       |             |       |
| **authorization**  | **kotlin.String**                       |             |       |
| **erc1155Request** | [**Erc1155Request**](erc1155request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **balanceOfBatch**

> TransactionAPIResponse balanceOfBatch(name, authorization, erc1155Request)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = ERC1155Api()
val name : kotlin.String = name_example // kotlin.String | 
val authorization : kotlin.String = authorization_example // kotlin.String | 
val erc1155Request : Erc1155Request =  // Erc1155Request | 
try {
    val result : TransactionAPIResponse = apiInstance.balanceOfBatch(name, authorization, erc1155Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ERC1155Api#balanceOfBatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ERC1155Api#balanceOfBatch")
    e.printStackTrace()
}
```

#### Parameters

| Name               | Type                                    | Description | Notes |
| ------------------ | --------------------------------------- | ----------- | ----- |
| **name**           | **kotlin.String**                       |             |       |
| **authorization**  | **kotlin.String**                       |             |       |
| **erc1155Request** | [**Erc1155Request**](erc1155request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **isApprovedForAll**

> TransactionAPIResponse isApprovedForAll(name, authorization, erc1155Request)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = ERC1155Api()
val name : kotlin.String = name_example // kotlin.String | 
val authorization : kotlin.String = authorization_example // kotlin.String | 
val erc1155Request : Erc1155Request =  // Erc1155Request | 
try {
    val result : TransactionAPIResponse = apiInstance.isApprovedForAll(name, authorization, erc1155Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ERC1155Api#isApprovedForAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ERC1155Api#isApprovedForAll")
    e.printStackTrace()
}
```

#### Parameters

| Name               | Type                                    | Description | Notes |
| ------------------ | --------------------------------------- | ----------- | ----- |
| **name**           | **kotlin.String**                       |             |       |
| **authorization**  | **kotlin.String**                       |             |       |
| **erc1155Request** | [**Erc1155Request**](erc1155request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **safeBatchTransferFrom**

> TransactionAPIResponse safeBatchTransferFrom(name, authorization, erc1155Request)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = ERC1155Api()
val name : kotlin.String = name_example // kotlin.String | 
val authorization : kotlin.String = authorization_example // kotlin.String | 
val erc1155Request : Erc1155Request =  // Erc1155Request | 
try {
    val result : TransactionAPIResponse = apiInstance.safeBatchTransferFrom(name, authorization, erc1155Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ERC1155Api#safeBatchTransferFrom")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ERC1155Api#safeBatchTransferFrom")
    e.printStackTrace()
}
```

#### Parameters

| Name               | Type                                    | Description | Notes |
| ------------------ | --------------------------------------- | ----------- | ----- |
| **name**           | **kotlin.String**                       |             |       |
| **authorization**  | **kotlin.String**                       |             |       |
| **erc1155Request** | [**Erc1155Request**](erc1155request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **safeTransferFrom**

> TransactionAPIResponse safeTransferFrom(name, authorization, erc1155Request)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = ERC1155Api()
val name : kotlin.String = name_example // kotlin.String | 
val authorization : kotlin.String = authorization_example // kotlin.String | 
val erc1155Request : Erc1155Request =  // Erc1155Request | 
try {
    val result : TransactionAPIResponse = apiInstance.safeTransferFrom(name, authorization, erc1155Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ERC1155Api#safeTransferFrom")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ERC1155Api#safeTransferFrom")
    e.printStackTrace()
}
```

#### Parameters

| Name               | Type                                    | Description | Notes |
| ------------------ | --------------------------------------- | ----------- | ----- |
| **name**           | **kotlin.String**                       |             |       |
| **authorization**  | **kotlin.String**                       |             |       |
| **erc1155Request** | [**Erc1155Request**](erc1155request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

## **setApprovalForAll**

> TransactionAPIResponse setApprovalForAll(name, authorization, erc1155Request)

#### Example

```kotlin
// Import classes:
//import org.usemoonai.moonsdk.infrastructure.*
//import org.usemoonai.moonsdk.models.*

val apiInstance = ERC1155Api()
val name : kotlin.String = name_example // kotlin.String | 
val authorization : kotlin.String = authorization_example // kotlin.String | 
val erc1155Request : Erc1155Request =  // Erc1155Request | 
try {
    val result : TransactionAPIResponse = apiInstance.setApprovalForAll(name, authorization, erc1155Request)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ERC1155Api#setApprovalForAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ERC1155Api#setApprovalForAll")
    e.printStackTrace()
}
```

#### Parameters

| Name               | Type                                    | Description | Notes |
| ------------------ | --------------------------------------- | ----------- | ----- |
| **name**           | **kotlin.String**                       |             |       |
| **authorization**  | **kotlin.String**                       |             |       |
| **erc1155Request** | [**Erc1155Request**](erc1155request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

Configure ApiKeyAuth: ApiClient.apiKey\["x-api-key"] = "" ApiClient.apiKeyPrefix\["x-api-key"] = "" Configure BearerAuth: ApiClient.apiKey\["Authorization"] = "" ApiClient.apiKeyPrefix\["Authorization"] = ""

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json
