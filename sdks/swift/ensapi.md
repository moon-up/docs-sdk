# ENSAPI

## ENSAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method      | HTTP request          | Description |
| ----------- | --------------------- | ----------- |
| **resolve** | **POST** /ens/resolve |             |

## **resolve**

```swift
    open class func resolve(authorization: String, ensResolveInput: EnsResolveInput, completion: @escaping (_ data: EnsResolveAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let ensResolveInput = EnsResolveInput(domain: "domain_example", chainId: "chainId_example") // EnsResolveInput | 

ENSAPI.resolve(authorization: authorization, ensResolveInput: ensResolveInput) { (response, error) in
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

| Name                | Type                | Description | Notes |
| ------------------- | ------------------- | ----------- | ----- |
| **authorization**   | **String**          |             |       |
| **ensResolveInput** | **EnsResolveInput** |             |       |

#### Return type

**EnsResolveAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
