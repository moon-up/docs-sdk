# DefaultAPI

## DefaultAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method         | HTTP request  | Description |
| -------------- | ------------- | ----------- |
| **getMessage** | **GET** /ping |             |

## **getMessage**

```swift
    open class func getMessage(completion: @escaping (_ data: PingResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient


DefaultAPI.getMessage() { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

#### Parameters

This endpoint does not need any parameter.

#### Return type

**PingResponse**

#### Authorization

No authorization required

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
