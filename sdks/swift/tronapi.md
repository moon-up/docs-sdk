# TronAPI

## TronAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method                  | HTTP request                         | Description |
| ----------------------- | ------------------------------------ | ----------- |
| **createTronAccount**   | **POST** /tron                       |             |
| **getTronAccount**      | **GET** /tron/{accountName}          |             |
| **listTronAccounts**    | **GET** /tron                        |             |
| **signTronTransaction** | **POST** /tron/{accountName}/sign-tx |             |

## **createTronAccount**

```swift
    open class func createTronAccount(authorization: String, tronInput: TronInput, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let tronInput = TronInput(network: "network_example", privateKey: "privateKey_example") // TronInput | 

TronAPI.createTronAccount(authorization: authorization, tronInput: tronInput) { (response, error) in
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

| Name              | Type          | Description | Notes |
| ----------------- | ------------- | ----------- | ----- |
| **authorization** | **String**    |             |       |
| **tronInput**     | **TronInput** |             |       |

#### Return type

**AccountAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **getTronAccount**

```swift
    open class func getTronAccount(authorization: String, accountName: String, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let accountName = "accountName_example" // String | 

TronAPI.getTronAccount(authorization: authorization, accountName: accountName) { (response, error) in
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

## **listTronAccounts**

```swift
    open class func listTronAccounts(authorization: String, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 

TronAPI.listTronAccounts(authorization: authorization) { (response, error) in
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

## **signTronTransaction**

```swift
    open class func signTronTransaction(authorization: String, accountName: String, tronTransactionInput: TronTransactionInput, completion: @escaping (_ data: TronAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let accountName = "accountName_example" // String | 
let tronTransactionInput = TronTransactionInput(to: "to_example", value: 123, network: "network_example", compress: false) // TronTransactionInput | 

TronAPI.signTronTransaction(authorization: authorization, accountName: accountName, tronTransactionInput: tronTransactionInput) { (response, error) in
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

| Name                     | Type                     | Description | Notes |
| ------------------------ | ------------------------ | ----------- | ----- |
| **authorization**        | **String**               |             |       |
| **accountName**          | **String**               |             |       |
| **tronTransactionInput** | **TronTransactionInput** |             |       |

#### Return type

**TronAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
