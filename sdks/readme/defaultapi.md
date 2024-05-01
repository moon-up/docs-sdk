# DefaultApi

## moonsdk.api.DefaultApi

### Load the API package

```dart
import 'package:moonsdk/api.dart';
```

All URIs are relative to _https://beta.usemoon.ai_

| Method                                     | HTTP request  | Description |
| ------------------------------------------ | ------------- | ----------- |
| [**getMessage**](defaultapi.md#getmessage) | **GET** /ping |             |

## **getMessage**

> PingResponse getMessage()

#### Example

```dart
import 'package:moonsdk/api.dart';

final api = Moonsdk().getDefaultApi();

try {
    final response = api.getMessage();
    print(response);
} catch on DioException (e) {
    print('Exception when calling DefaultApi->getMessage: $e\n');
}
```

#### Parameters

This endpoint does not need any parameter.

#### Return type

[**PingResponse**](pingresponse.md)

#### Authorization

No authorization required

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](defaultapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
