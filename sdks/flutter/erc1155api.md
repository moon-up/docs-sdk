# ERC1155Api

## moonsdk.api.ERC1155Api

### Load the API package

```dart
import 'package:moonsdk/api.dart';
```

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                           | HTTP request                                      | Description |
| ---------------------------------------------------------------- | ------------------------------------------------- | ----------- |
| [**balanceOf**](erc1155api.md#balanceof)                         | **POST** /erc1155/{name}/balance-of               |             |
| [**balanceOfBatch**](erc1155api.md#balanceofbatch)               | **POST** /erc1155/{name}/balance-of-batch         |             |
| [**isApprovedForAll**](erc1155api.md#isapprovedforall)           | **POST** /erc1155/{name}/is-approved-for-all      |             |
| [**safeBatchTransferFrom**](erc1155api.md#safebatchtransferfrom) | **POST** /erc1155/{name}/safe-batch-transfer-from |             |
| [**safeTransferFrom**](erc1155api.md#safetransferfrom)           | **POST** /erc1155/{name}/safe-transfer-from       |             |
| [**setApprovalForAll**](erc1155api.md#setapprovalforall)         | **POST** /erc1155/{name}/set-approval-for-all     |             |

## **balanceOf**

> TransactionAPIResponse balanceOf(name, authorization, erc1155Request)

#### Example

```dart
import 'package:moonsdk/api.dart';
// TODO Configure API key authorization: ApiKeyAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKeyPrefix = 'Bearer';
// TODO Configure API key authorization: BearerAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKeyPrefix = 'Bearer';

final api = Moonsdk().getERC1155Api();
final String name = name_example; // String | 
final String authorization = authorization_example; // String | 
final Erc1155Request erc1155Request = ; // Erc1155Request | 

try {
    final response = api.balanceOf(name, authorization, erc1155Request);
    print(response);
} catch on DioException (e) {
    print('Exception when calling ERC1155Api->balanceOf: $e\n');
}
```

#### Parameters

| Name               | Type                                    | Description | Notes |
| ------------------ | --------------------------------------- | ----------- | ----- |
| **name**           | **String**                              |             |       |
| **authorization**  | **String**                              |             |       |
| **erc1155Request** | [**Erc1155Request**](erc1155request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc1155api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **balanceOfBatch**

> TransactionAPIResponse balanceOfBatch(name, authorization, erc1155Request)

#### Example

```dart
import 'package:moonsdk/api.dart';
// TODO Configure API key authorization: ApiKeyAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKeyPrefix = 'Bearer';
// TODO Configure API key authorization: BearerAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKeyPrefix = 'Bearer';

final api = Moonsdk().getERC1155Api();
final String name = name_example; // String | 
final String authorization = authorization_example; // String | 
final Erc1155Request erc1155Request = ; // Erc1155Request | 

try {
    final response = api.balanceOfBatch(name, authorization, erc1155Request);
    print(response);
} catch on DioException (e) {
    print('Exception when calling ERC1155Api->balanceOfBatch: $e\n');
}
```

#### Parameters

| Name               | Type                                    | Description | Notes |
| ------------------ | --------------------------------------- | ----------- | ----- |
| **name**           | **String**                              |             |       |
| **authorization**  | **String**                              |             |       |
| **erc1155Request** | [**Erc1155Request**](erc1155request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc1155api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **isApprovedForAll**

> TransactionAPIResponse isApprovedForAll(name, authorization, erc1155Request)

#### Example

```dart
import 'package:moonsdk/api.dart';
// TODO Configure API key authorization: ApiKeyAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKeyPrefix = 'Bearer';
// TODO Configure API key authorization: BearerAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKeyPrefix = 'Bearer';

final api = Moonsdk().getERC1155Api();
final String name = name_example; // String | 
final String authorization = authorization_example; // String | 
final Erc1155Request erc1155Request = ; // Erc1155Request | 

try {
    final response = api.isApprovedForAll(name, authorization, erc1155Request);
    print(response);
} catch on DioException (e) {
    print('Exception when calling ERC1155Api->isApprovedForAll: $e\n');
}
```

#### Parameters

| Name               | Type                                    | Description | Notes |
| ------------------ | --------------------------------------- | ----------- | ----- |
| **name**           | **String**                              |             |       |
| **authorization**  | **String**                              |             |       |
| **erc1155Request** | [**Erc1155Request**](erc1155request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc1155api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **safeBatchTransferFrom**

> TransactionAPIResponse safeBatchTransferFrom(name, authorization, erc1155Request)

#### Example

```dart
import 'package:moonsdk/api.dart';
// TODO Configure API key authorization: ApiKeyAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKeyPrefix = 'Bearer';
// TODO Configure API key authorization: BearerAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKeyPrefix = 'Bearer';

final api = Moonsdk().getERC1155Api();
final String name = name_example; // String | 
final String authorization = authorization_example; // String | 
final Erc1155Request erc1155Request = ; // Erc1155Request | 

try {
    final response = api.safeBatchTransferFrom(name, authorization, erc1155Request);
    print(response);
} catch on DioException (e) {
    print('Exception when calling ERC1155Api->safeBatchTransferFrom: $e\n');
}
```

#### Parameters

| Name               | Type                                    | Description | Notes |
| ------------------ | --------------------------------------- | ----------- | ----- |
| **name**           | **String**                              |             |       |
| **authorization**  | **String**                              |             |       |
| **erc1155Request** | [**Erc1155Request**](erc1155request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc1155api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **safeTransferFrom**

> TransactionAPIResponse safeTransferFrom(name, authorization, erc1155Request)

#### Example

```dart
import 'package:moonsdk/api.dart';
// TODO Configure API key authorization: ApiKeyAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKeyPrefix = 'Bearer';
// TODO Configure API key authorization: BearerAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKeyPrefix = 'Bearer';

final api = Moonsdk().getERC1155Api();
final String name = name_example; // String | 
final String authorization = authorization_example; // String | 
final Erc1155Request erc1155Request = ; // Erc1155Request | 

try {
    final response = api.safeTransferFrom(name, authorization, erc1155Request);
    print(response);
} catch on DioException (e) {
    print('Exception when calling ERC1155Api->safeTransferFrom: $e\n');
}
```

#### Parameters

| Name               | Type                                    | Description | Notes |
| ------------------ | --------------------------------------- | ----------- | ----- |
| **name**           | **String**                              |             |       |
| **authorization**  | **String**                              |             |       |
| **erc1155Request** | [**Erc1155Request**](erc1155request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc1155api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **setApprovalForAll**

> TransactionAPIResponse setApprovalForAll(name, authorization, erc1155Request)

#### Example

```dart
import 'package:moonsdk/api.dart';
// TODO Configure API key authorization: ApiKeyAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKeyPrefix = 'Bearer';
// TODO Configure API key authorization: BearerAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKeyPrefix = 'Bearer';

final api = Moonsdk().getERC1155Api();
final String name = name_example; // String | 
final String authorization = authorization_example; // String | 
final Erc1155Request erc1155Request = ; // Erc1155Request | 

try {
    final response = api.setApprovalForAll(name, authorization, erc1155Request);
    print(response);
} catch on DioException (e) {
    print('Exception when calling ERC1155Api->setApprovalForAll: $e\n');
}
```

#### Parameters

| Name               | Type                                    | Description | Notes |
| ------------------ | --------------------------------------- | ----------- | ----- |
| **name**           | **String**                              |             |       |
| **authorization**  | **String**                              |             |       |
| **erc1155Request** | [**Erc1155Request**](erc1155request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc1155api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
