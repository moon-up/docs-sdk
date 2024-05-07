# ENSApi

## moonsdk.api.ENSApi

### Load the API package

```dart
import 'package:moonsdk/api.dart';
```

All URIs are relative to _https://beta.usemoon.ai_

| Method                           | HTTP request          | Description |
| -------------------------------- | --------------------- | ----------- |
| [**resolve**](ensapi.md#resolve) | **POST** /ens/resolve |             |

## **resolve**

> EnsResolveAPIResponse resolve(authorization, ensResolveInput)

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

final api = Moonsdk().getENSApi();
final String authorization = authorization_example; // String | 
final EnsResolveInput ensResolveInput = ; // EnsResolveInput | 

try {
    final response = api.resolve(authorization, ensResolveInput);
    print(response);
} catch on DioException (e) {
    print('Exception when calling ENSApi->resolve: $e\n');
}
```

#### Parameters

| Name                | Type                                      | Description | Notes |
| ------------------- | ----------------------------------------- | ----------- | ----- |
| **authorization**   | **String**                                |             |       |
| **ensResolveInput** | [**EnsResolveInput**](ensresolveinput.md) |             |       |

#### Return type

[**EnsResolveAPIResponse**](ensresolveapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](ensapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
