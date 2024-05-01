# RippleAPI

## RippleAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method                    | HTTP request                           | Description |
| ------------------------- | -------------------------------------- | ----------- |
| **createRippleAccount**   | **POST** /ripple                       |             |
| **getRippleAccount**      | **GET** /ripple/{accountName}          |             |
| **listRippleAccounts**    | **GET** /ripple                        |             |
| **signRippleTransaction** | **POST** /ripple/{accountName}/sign-tx |             |

## **createRippleAccount**

```swift
    open class func createRippleAccount(authorization: String, rippleInput: RippleInput, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let rippleInput = RippleInput(network: "network_example", privateKey: "privateKey_example") // RippleInput | 

RippleAPI.createRippleAccount(authorization: authorization, rippleInput: rippleInput) { (response, error) in
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

| Name              | Type            | Description | Notes |
| ----------------- | --------------- | ----------- | ----- |
| **authorization** | **String**      |             |       |
| **rippleInput**   | **RippleInput** |             |       |

#### Return type

**AccountAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **getRippleAccount**

```swift
    open class func getRippleAccount(authorization: String, accountName: String, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let accountName = "accountName_example" // String | 

RippleAPI.getRippleAccount(authorization: authorization, accountName: accountName) { (response, error) in
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

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **String** |             |       |
| **accountName**   | **String** |             |       |

#### Return type

**AccountAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **listRippleAccounts**

```swift
    open class func listRippleAccounts(authorization: String, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 

RippleAPI.listRippleAccounts(authorization: authorization) { (response, error) in
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

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **String** |             |       |

#### Return type

**AccountAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **signRippleTransaction**

```swift
    open class func signRippleTransaction(authorization: String, accountName: String, rippleTransactionInput: RippleTransactionInput, completion: @escaping (_ data: RippleAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let accountName = "accountName_example" // String | 
let rippleTransactionInput = RippleTransactionInput(to: "to_example", value: 123, network: "network_example", compress: false) // RippleTransactionInput | 

RippleAPI.signRippleTransaction(authorization: authorization, accountName: accountName, rippleTransactionInput: rippleTransactionInput) { (response, error) in
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

| Name                       | Type                       | Description | Notes |
| -------------------------- | -------------------------- | ----------- | ----- |
| **authorization**          | **String**                 |             |       |
| **accountName**            | **String**                 |             |       |
| **rippleTransactionInput** | **RippleTransactionInput** |             |       |

#### Return type

**RippleAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
