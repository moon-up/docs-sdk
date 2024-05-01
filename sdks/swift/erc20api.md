# Erc20API

## Erc20API

All URIs are relative to _https://beta.usemoon.ai_

| Method                | HTTP request                         | Description |
| --------------------- | ------------------------------------ | ----------- |
| **allowanceErc20**    | **POST** /erc20/{name}/allowance     |             |
| **approveErc20**      | **POST** /erc20/{name}/approve       |             |
| **balanceOfErc20**    | **POST** /erc20/{name}/balance-of    |             |
| **decimalsErc20**     | **POST** /erc20/{name}/decimals      |             |
| **nameErc20**         | **POST** /erc20/{name}/name          |             |
| **symbolErc20**       | **POST** /erc20/{name}/symbol        |             |
| **totalSupplyErc20**  | **POST** /erc20/{name}/total-supply  |             |
| **transferErc20**     | **POST** /erc20/{name}/transfer      |             |
| **transferFromErc20** | **POST** /erc20/{name}/transfer-from |             |

## **allowanceErc20**

```swift
    open class func allowanceErc20(authorization: String, name: String, inputBody: InputBody, completion: @escaping (_ data: TransactionAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let name = "name_example" // String | 
let inputBody = InputBody(to: "to_example", data: "data_example", input: "input_example", value: "value_example", nonce: "nonce_example", gas: "gas_example", gasPrice: "gasPrice_example", chainId: "chainId_example", encoding: "encoding_example", EOA: false, contractAddress: "contractAddress_example", tokenId: "tokenId_example", tokenIds: "tokenIds_example", approved: false, broadcast: false) // InputBody | 

Erc20API.allowanceErc20(authorization: authorization, name: name, inputBody: inputBody) { (response, error) in
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
| **name**          | **String**    |             |       |
| **inputBody**     | **InputBody** |             |       |

#### Return type

**TransactionAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **approveErc20**

```swift
    open class func approveErc20(authorization: String, name: String, inputBody: InputBody, completion: @escaping (_ data: TransactionAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let name = "name_example" // String | 
let inputBody = InputBody(to: "to_example", data: "data_example", input: "input_example", value: "value_example", nonce: "nonce_example", gas: "gas_example", gasPrice: "gasPrice_example", chainId: "chainId_example", encoding: "encoding_example", EOA: false, contractAddress: "contractAddress_example", tokenId: "tokenId_example", tokenIds: "tokenIds_example", approved: false, broadcast: false) // InputBody | 

Erc20API.approveErc20(authorization: authorization, name: name, inputBody: inputBody) { (response, error) in
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
| **name**          | **String**    |             |       |
| **inputBody**     | **InputBody** |             |       |

#### Return type

**TransactionAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **balanceOfErc20**

```swift
    open class func balanceOfErc20(authorization: String, name: String, inputBody: InputBody, completion: @escaping (_ data: TransactionAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let name = "name_example" // String | 
let inputBody = InputBody(to: "to_example", data: "data_example", input: "input_example", value: "value_example", nonce: "nonce_example", gas: "gas_example", gasPrice: "gasPrice_example", chainId: "chainId_example", encoding: "encoding_example", EOA: false, contractAddress: "contractAddress_example", tokenId: "tokenId_example", tokenIds: "tokenIds_example", approved: false, broadcast: false) // InputBody | 

Erc20API.balanceOfErc20(authorization: authorization, name: name, inputBody: inputBody) { (response, error) in
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
| **name**          | **String**    |             |       |
| **inputBody**     | **InputBody** |             |       |

#### Return type

**TransactionAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **decimalsErc20**

```swift
    open class func decimalsErc20(authorization: String, name: String, inputBody: InputBody, completion: @escaping (_ data: TransactionAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let name = "name_example" // String | 
let inputBody = InputBody(to: "to_example", data: "data_example", input: "input_example", value: "value_example", nonce: "nonce_example", gas: "gas_example", gasPrice: "gasPrice_example", chainId: "chainId_example", encoding: "encoding_example", EOA: false, contractAddress: "contractAddress_example", tokenId: "tokenId_example", tokenIds: "tokenIds_example", approved: false, broadcast: false) // InputBody | 

Erc20API.decimalsErc20(authorization: authorization, name: name, inputBody: inputBody) { (response, error) in
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
| **name**          | **String**    |             |       |
| **inputBody**     | **InputBody** |             |       |

#### Return type

**TransactionAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **nameErc20**

```swift
    open class func nameErc20(authorization: String, name: String, inputBody: InputBody, completion: @escaping (_ data: TransactionAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let name = "name_example" // String | 
let inputBody = InputBody(to: "to_example", data: "data_example", input: "input_example", value: "value_example", nonce: "nonce_example", gas: "gas_example", gasPrice: "gasPrice_example", chainId: "chainId_example", encoding: "encoding_example", EOA: false, contractAddress: "contractAddress_example", tokenId: "tokenId_example", tokenIds: "tokenIds_example", approved: false, broadcast: false) // InputBody | 

Erc20API.nameErc20(authorization: authorization, name: name, inputBody: inputBody) { (response, error) in
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
| **name**          | **String**    |             |       |
| **inputBody**     | **InputBody** |             |       |

#### Return type

**TransactionAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **symbolErc20**

```swift
    open class func symbolErc20(authorization: String, name: String, inputBody: InputBody, completion: @escaping (_ data: TransactionAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let name = "name_example" // String | 
let inputBody = InputBody(to: "to_example", data: "data_example", input: "input_example", value: "value_example", nonce: "nonce_example", gas: "gas_example", gasPrice: "gasPrice_example", chainId: "chainId_example", encoding: "encoding_example", EOA: false, contractAddress: "contractAddress_example", tokenId: "tokenId_example", tokenIds: "tokenIds_example", approved: false, broadcast: false) // InputBody | 

Erc20API.symbolErc20(authorization: authorization, name: name, inputBody: inputBody) { (response, error) in
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
| **name**          | **String**    |             |       |
| **inputBody**     | **InputBody** |             |       |

#### Return type

**TransactionAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **totalSupplyErc20**

```swift
    open class func totalSupplyErc20(authorization: String, name: String, inputBody: InputBody, completion: @escaping (_ data: TransactionAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let name = "name_example" // String | 
let inputBody = InputBody(to: "to_example", data: "data_example", input: "input_example", value: "value_example", nonce: "nonce_example", gas: "gas_example", gasPrice: "gasPrice_example", chainId: "chainId_example", encoding: "encoding_example", EOA: false, contractAddress: "contractAddress_example", tokenId: "tokenId_example", tokenIds: "tokenIds_example", approved: false, broadcast: false) // InputBody | 

Erc20API.totalSupplyErc20(authorization: authorization, name: name, inputBody: inputBody) { (response, error) in
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
| **name**          | **String**    |             |       |
| **inputBody**     | **InputBody** |             |       |

#### Return type

**TransactionAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **transferErc20**

```swift
    open class func transferErc20(authorization: String, name: String, inputBody: InputBody, completion: @escaping (_ data: TransactionAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let name = "name_example" // String | 
let inputBody = InputBody(to: "to_example", data: "data_example", input: "input_example", value: "value_example", nonce: "nonce_example", gas: "gas_example", gasPrice: "gasPrice_example", chainId: "chainId_example", encoding: "encoding_example", EOA: false, contractAddress: "contractAddress_example", tokenId: "tokenId_example", tokenIds: "tokenIds_example", approved: false, broadcast: false) // InputBody | 

Erc20API.transferErc20(authorization: authorization, name: name, inputBody: inputBody) { (response, error) in
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
| **name**          | **String**    |             |       |
| **inputBody**     | **InputBody** |             |       |

#### Return type

**TransactionAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **transferFromErc20**

```swift
    open class func transferFromErc20(authorization: String, name: String, inputBody: InputBody, completion: @escaping (_ data: TransactionAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let name = "name_example" // String | 
let inputBody = InputBody(to: "to_example", data: "data_example", input: "input_example", value: "value_example", nonce: "nonce_example", gas: "gas_example", gasPrice: "gasPrice_example", chainId: "chainId_example", encoding: "encoding_example", EOA: false, contractAddress: "contractAddress_example", tokenId: "tokenId_example", tokenIds: "tokenIds_example", approved: false, broadcast: false) // InputBody | 

Erc20API.transferFromErc20(authorization: authorization, name: name, inputBody: inputBody) { (response, error) in
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
| **name**          | **String**    |             |       |
| **inputBody**     | **InputBody** |             |       |

#### Return type

**TransactionAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
