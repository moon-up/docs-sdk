# YearnApi

## moonsdk.api.YearnApi

### Load the API package

```dart
import 'package:moonsdk/api.dart';
```

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                     | HTTP request                                 | Description |
| ---------------------------------------------------------- | -------------------------------------------- | ----------- |
| [**addLiquidity**](yearnapi.md#addliquidity)               | **POST** /yearn/{name}/add-liquidity         |             |
| [**addLiquidityWeth**](yearnapi.md#addliquidityweth)       | **POST** /yearn/{name}/add-liquidity-weth    |             |
| [**removeLiquidity**](yearnapi.md#removeliquidity)         | **POST** /yearn/{name}/remove-liquidity      |             |
| [**removeLiquidityWeth**](yearnapi.md#removeliquidityweth) | **POST** /yearn/{name}/remove-liquidity-weth |             |

## **addLiquidity**

> TransactionAPIResponse addLiquidity(authorization, name, inputBody)

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

final api = Moonsdk().getYearnApi();
final String authorization = authorization_example; // String | 
final String name = name_example; // String | 
final InputBody inputBody = ; // InputBody | 

try {
    final response = api.addLiquidity(authorization, name, inputBody);
    print(response);
} catch on DioException (e) {
    print('Exception when calling YearnApi->addLiquidity: $e\n');
}
```

#### Parameters

| Name              | Type                          | Description | Notes |
| ----------------- | ----------------------------- | ----------- | ----- |
| **authorization** | **String**                    |             |       |
| **name**          | **String**                    |             |       |
| **inputBody**     | [**InputBody**](inputbody.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](yearnapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **addLiquidityWeth**

> TransactionAPIResponse addLiquidityWeth(authorization, name, inputBody)

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

final api = Moonsdk().getYearnApi();
final String authorization = authorization_example; // String | 
final String name = name_example; // String | 
final InputBody inputBody = ; // InputBody | 

try {
    final response = api.addLiquidityWeth(authorization, name, inputBody);
    print(response);
} catch on DioException (e) {
    print('Exception when calling YearnApi->addLiquidityWeth: $e\n');
}
```

#### Parameters

| Name              | Type                          | Description | Notes |
| ----------------- | ----------------------------- | ----------- | ----- |
| **authorization** | **String**                    |             |       |
| **name**          | **String**                    |             |       |
| **inputBody**     | [**InputBody**](inputbody.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](yearnapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **removeLiquidity**

> TransactionAPIResponse removeLiquidity(authorization, name, inputBody)

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

final api = Moonsdk().getYearnApi();
final String authorization = authorization_example; // String | 
final String name = name_example; // String | 
final InputBody inputBody = ; // InputBody | 

try {
    final response = api.removeLiquidity(authorization, name, inputBody);
    print(response);
} catch on DioException (e) {
    print('Exception when calling YearnApi->removeLiquidity: $e\n');
}
```

#### Parameters

| Name              | Type                          | Description | Notes |
| ----------------- | ----------------------------- | ----------- | ----- |
| **authorization** | **String**                    |             |       |
| **name**          | **String**                    |             |       |
| **inputBody**     | [**InputBody**](inputbody.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](yearnapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **removeLiquidityWeth**

> TransactionAPIResponse removeLiquidityWeth(authorization, name, inputBody)

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

final api = Moonsdk().getYearnApi();
final String authorization = authorization_example; // String | 
final String name = name_example; // String | 
final InputBody inputBody = ; // InputBody | 

try {
    final response = api.removeLiquidityWeth(authorization, name, inputBody);
    print(response);
} catch on DioException (e) {
    print('Exception when calling YearnApi->removeLiquidityWeth: $e\n');
}
```

#### Parameters

| Name              | Type                          | Description | Notes |
| ----------------- | ----------------------------- | ----------- | ----- |
| **authorization** | **String**                    |             |       |
| **name**          | **String**                    |             |       |
| **inputBody**     | [**InputBody**](inputbody.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](yearnapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
