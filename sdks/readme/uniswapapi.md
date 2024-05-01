# UniSwapApi

## moonsdk.api.UniSwapApi

### Load the API package

```dart
import 'package:moonsdk/api.dart';
```

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                                 | HTTP request                                          | Description |
| ---------------------------------------------------------------------- | ----------------------------------------------------- | ----------- |
| [**addLiquidity**](uniswapapi.md#addliquidity)                         | **POST** /uniswap/{name}/add-liquidity                |             |
| [**removeLiquidity**](uniswapapi.md#removeliquidity)                   | **POST** /uniswap/{name}/remove-liquidity             |             |
| [**swapExactETHForTokens**](uniswapapi.md#swapexactethfortokens)       | **POST** /uniswap/{name}/swap-exact-eth-for-tokens    |             |
| [**swapExactTokensForTokens**](uniswapapi.md#swapexacttokensfortokens) | **POST** /uniswap/{name}/swap-exact-tokens-for-tokens |             |

## **addLiquidity**

> TransactionAPIResponse addLiquidity(authorization, name, uniswapInput)

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

final api = Moonsdk().getUniSwapApi();
final String authorization = authorization_example; // String | 
final String name = name_example; // String | 
final UniswapInput uniswapInput = ; // UniswapInput | 

try {
    final response = api.addLiquidity(authorization, name, uniswapInput);
    print(response);
} catch on DioException (e) {
    print('Exception when calling UniSwapApi->addLiquidity: $e\n');
}
```

#### Parameters

| Name              | Type                                | Description | Notes |
| ----------------- | ----------------------------------- | ----------- | ----- |
| **authorization** | **String**                          |             |       |
| **name**          | **String**                          |             |       |
| **uniswapInput**  | [**UniswapInput**](uniswapinput.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](uniswapapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **removeLiquidity**

> TransactionAPIResponse removeLiquidity(authorization, name, uniswapInput)

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

final api = Moonsdk().getUniSwapApi();
final String authorization = authorization_example; // String | 
final String name = name_example; // String | 
final UniswapInput uniswapInput = ; // UniswapInput | 

try {
    final response = api.removeLiquidity(authorization, name, uniswapInput);
    print(response);
} catch on DioException (e) {
    print('Exception when calling UniSwapApi->removeLiquidity: $e\n');
}
```

#### Parameters

| Name              | Type                                | Description | Notes |
| ----------------- | ----------------------------------- | ----------- | ----- |
| **authorization** | **String**                          |             |       |
| **name**          | **String**                          |             |       |
| **uniswapInput**  | [**UniswapInput**](uniswapinput.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](uniswapapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **swapExactETHForTokens**

> TransactionAPIResponse swapExactETHForTokens(authorization, name, uniswapInput)

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

final api = Moonsdk().getUniSwapApi();
final String authorization = authorization_example; // String | 
final String name = name_example; // String | 
final UniswapInput uniswapInput = ; // UniswapInput | 

try {
    final response = api.swapExactETHForTokens(authorization, name, uniswapInput);
    print(response);
} catch on DioException (e) {
    print('Exception when calling UniSwapApi->swapExactETHForTokens: $e\n');
}
```

#### Parameters

| Name              | Type                                | Description | Notes |
| ----------------- | ----------------------------------- | ----------- | ----- |
| **authorization** | **String**                          |             |       |
| **name**          | **String**                          |             |       |
| **uniswapInput**  | [**UniswapInput**](uniswapinput.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](uniswapapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **swapExactTokensForTokens**

> TransactionAPIResponse swapExactTokensForTokens(authorization, name, uniswapInput)

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

final api = Moonsdk().getUniSwapApi();
final String authorization = authorization_example; // String | 
final String name = name_example; // String | 
final UniswapInput uniswapInput = ; // UniswapInput | 

try {
    final response = api.swapExactTokensForTokens(authorization, name, uniswapInput);
    print(response);
} catch on DioException (e) {
    print('Exception when calling UniSwapApi->swapExactTokensForTokens: $e\n');
}
```

#### Parameters

| Name              | Type                                | Description | Notes |
| ----------------- | ----------------------------------- | ----------- | ----- |
| **authorization** | **String**                          |             |       |
| **name**          | **String**                          |             |       |
| **uniswapInput**  | [**UniswapInput**](uniswapinput.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](uniswapapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
