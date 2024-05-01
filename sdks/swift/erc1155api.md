# ERC1155API

## ERC1155API

All URIs are relative to _https://beta.usemoon.ai_

| Method                    | HTTP request                                      | Description |
| ------------------------- | ------------------------------------------------- | ----------- |
| **balanceOf**             | **POST** /erc1155/{name}/balance-of               |             |
| **balanceOfBatch**        | **POST** /erc1155/{name}/balance-of-batch         |             |
| **isApprovedForAll**      | **POST** /erc1155/{name}/is-approved-for-all      |             |
| **safeBatchTransferFrom** | **POST** /erc1155/{name}/safe-batch-transfer-from |             |
| **safeTransferFrom**      | **POST** /erc1155/{name}/safe-transfer-from       |             |
| **setApprovalForAll**     | **POST** /erc1155/{name}/set-approval-for-all     |             |

## **balanceOf**

```swift
    open class func balanceOf(name: String, authorization: String, erc1155Request: Erc1155Request, completion: @escaping (_ data: TransactionAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let name = "name_example" // String | 
let authorization = "authorization_example" // String | 
let erc1155Request = Erc1155Request(to: "to_example", data: "data_example", input: "input_example", value: "value_example", nonce: "nonce_example", gas: "gas_example", gasPrice: "gasPrice_example", chainId: "chainId_example", encoding: "encoding_example", EOA: false, contractAddress: "contractAddress_example", tokenId: "tokenId_example", tokenIds: "tokenIds_example", approved: false, broadcast: false) // Erc1155Request | 

ERC1155API.balanceOf(name: name, authorization: authorization, erc1155Request: erc1155Request) { (response, error) in
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

| Name               | Type               | Description | Notes |
| ------------------ | ------------------ | ----------- | ----- |
| **name**           | **String**         |             |       |
| **authorization**  | **String**         |             |       |
| **erc1155Request** | **Erc1155Request** |             |       |

#### Return type

**TransactionAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **balanceOfBatch**

```swift
    open class func balanceOfBatch(name: String, authorization: String, erc1155Request: Erc1155Request, completion: @escaping (_ data: TransactionAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let name = "name_example" // String | 
let authorization = "authorization_example" // String | 
let erc1155Request = Erc1155Request(to: "to_example", data: "data_example", input: "input_example", value: "value_example", nonce: "nonce_example", gas: "gas_example", gasPrice: "gasPrice_example", chainId: "chainId_example", encoding: "encoding_example", EOA: false, contractAddress: "contractAddress_example", tokenId: "tokenId_example", tokenIds: "tokenIds_example", approved: false, broadcast: false) // Erc1155Request | 

ERC1155API.balanceOfBatch(name: name, authorization: authorization, erc1155Request: erc1155Request) { (response, error) in
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

| Name               | Type               | Description | Notes |
| ------------------ | ------------------ | ----------- | ----- |
| **name**           | **String**         |             |       |
| **authorization**  | **String**         |             |       |
| **erc1155Request** | **Erc1155Request** |             |       |

#### Return type

**TransactionAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **isApprovedForAll**

```swift
    open class func isApprovedForAll(name: String, authorization: String, erc1155Request: Erc1155Request, completion: @escaping (_ data: TransactionAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let name = "name_example" // String | 
let authorization = "authorization_example" // String | 
let erc1155Request = Erc1155Request(to: "to_example", data: "data_example", input: "input_example", value: "value_example", nonce: "nonce_example", gas: "gas_example", gasPrice: "gasPrice_example", chainId: "chainId_example", encoding: "encoding_example", EOA: false, contractAddress: "contractAddress_example", tokenId: "tokenId_example", tokenIds: "tokenIds_example", approved: false, broadcast: false) // Erc1155Request | 

ERC1155API.isApprovedForAll(name: name, authorization: authorization, erc1155Request: erc1155Request) { (response, error) in
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

| Name               | Type               | Description | Notes |
| ------------------ | ------------------ | ----------- | ----- |
| **name**           | **String**         |             |       |
| **authorization**  | **String**         |             |       |
| **erc1155Request** | **Erc1155Request** |             |       |

#### Return type

**TransactionAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **safeBatchTransferFrom**

```swift
    open class func safeBatchTransferFrom(name: String, authorization: String, erc1155Request: Erc1155Request, completion: @escaping (_ data: TransactionAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let name = "name_example" // String | 
let authorization = "authorization_example" // String | 
let erc1155Request = Erc1155Request(to: "to_example", data: "data_example", input: "input_example", value: "value_example", nonce: "nonce_example", gas: "gas_example", gasPrice: "gasPrice_example", chainId: "chainId_example", encoding: "encoding_example", EOA: false, contractAddress: "contractAddress_example", tokenId: "tokenId_example", tokenIds: "tokenIds_example", approved: false, broadcast: false) // Erc1155Request | 

ERC1155API.safeBatchTransferFrom(name: name, authorization: authorization, erc1155Request: erc1155Request) { (response, error) in
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

| Name               | Type               | Description | Notes |
| ------------------ | ------------------ | ----------- | ----- |
| **name**           | **String**         |             |       |
| **authorization**  | **String**         |             |       |
| **erc1155Request** | **Erc1155Request** |             |       |

#### Return type

**TransactionAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **safeTransferFrom**

```swift
    open class func safeTransferFrom(name: String, authorization: String, erc1155Request: Erc1155Request, completion: @escaping (_ data: TransactionAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let name = "name_example" // String | 
let authorization = "authorization_example" // String | 
let erc1155Request = Erc1155Request(to: "to_example", data: "data_example", input: "input_example", value: "value_example", nonce: "nonce_example", gas: "gas_example", gasPrice: "gasPrice_example", chainId: "chainId_example", encoding: "encoding_example", EOA: false, contractAddress: "contractAddress_example", tokenId: "tokenId_example", tokenIds: "tokenIds_example", approved: false, broadcast: false) // Erc1155Request | 

ERC1155API.safeTransferFrom(name: name, authorization: authorization, erc1155Request: erc1155Request) { (response, error) in
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

| Name               | Type               | Description | Notes |
| ------------------ | ------------------ | ----------- | ----- |
| **name**           | **String**         |             |       |
| **authorization**  | **String**         |             |       |
| **erc1155Request** | **Erc1155Request** |             |       |

#### Return type

**TransactionAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **setApprovalForAll**

```swift
    open class func setApprovalForAll(name: String, authorization: String, erc1155Request: Erc1155Request, completion: @escaping (_ data: TransactionAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let name = "name_example" // String | 
let authorization = "authorization_example" // String | 
let erc1155Request = Erc1155Request(to: "to_example", data: "data_example", input: "input_example", value: "value_example", nonce: "nonce_example", gas: "gas_example", gasPrice: "gasPrice_example", chainId: "chainId_example", encoding: "encoding_example", EOA: false, contractAddress: "contractAddress_example", tokenId: "tokenId_example", tokenIds: "tokenIds_example", approved: false, broadcast: false) // Erc1155Request | 

ERC1155API.setApprovalForAll(name: name, authorization: authorization, erc1155Request: erc1155Request) { (response, error) in
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

| Name               | Type               | Description | Notes |
| ------------------ | ------------------ | ----------- | ----- |
| **name**           | **String**         |             |       |
| **authorization**  | **String**         |             |       |
| **erc1155Request** | **Erc1155Request** |             |       |

#### Return type

**TransactionAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
