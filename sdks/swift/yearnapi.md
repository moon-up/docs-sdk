# YearnAPI

## YearnAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method                  | HTTP request                                 | Description |
| ----------------------- | -------------------------------------------- | ----------- |
| **addLiquidity**        | **POST** /yearn/{name}/add-liquidity         |             |
| **addLiquidityWeth**    | **POST** /yearn/{name}/add-liquidity-weth    |             |
| **removeLiquidity**     | **POST** /yearn/{name}/remove-liquidity      |             |
| **removeLiquidityWeth** | **POST** /yearn/{name}/remove-liquidity-weth |             |

## **addLiquidity**

```swift
    open class func addLiquidity(authorization: String, name: String, inputBody: InputBody, completion: @escaping (_ data: TransactionAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let name = "name_example" // String | 
let inputBody = InputBody(to: "to_example", data: "data_example", input: "input_example", value: "value_example", nonce: "nonce_example", gas: "gas_example", gasPrice: "gasPrice_example", chainId: "chainId_example", encoding: "encoding_example", EOA: false, contractAddress: "contractAddress_example", tokenId: "tokenId_example", tokenIds: "tokenIds_example", approved: false, broadcast: false) // InputBody | 

YearnAPI.addLiquidity(authorization: authorization, name: name, inputBody: inputBody) { (response, error) in
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

## **addLiquidityWeth**

```swift
    open class func addLiquidityWeth(authorization: String, name: String, inputBody: InputBody, completion: @escaping (_ data: TransactionAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let name = "name_example" // String | 
let inputBody = InputBody(to: "to_example", data: "data_example", input: "input_example", value: "value_example", nonce: "nonce_example", gas: "gas_example", gasPrice: "gasPrice_example", chainId: "chainId_example", encoding: "encoding_example", EOA: false, contractAddress: "contractAddress_example", tokenId: "tokenId_example", tokenIds: "tokenIds_example", approved: false, broadcast: false) // InputBody | 

YearnAPI.addLiquidityWeth(authorization: authorization, name: name, inputBody: inputBody) { (response, error) in
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

## **removeLiquidity**

```swift
    open class func removeLiquidity(authorization: String, name: String, inputBody: InputBody, completion: @escaping (_ data: TransactionAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let name = "name_example" // String | 
let inputBody = InputBody(to: "to_example", data: "data_example", input: "input_example", value: "value_example", nonce: "nonce_example", gas: "gas_example", gasPrice: "gasPrice_example", chainId: "chainId_example", encoding: "encoding_example", EOA: false, contractAddress: "contractAddress_example", tokenId: "tokenId_example", tokenIds: "tokenIds_example", approved: false, broadcast: false) // InputBody | 

YearnAPI.removeLiquidity(authorization: authorization, name: name, inputBody: inputBody) { (response, error) in
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

## **removeLiquidityWeth**

```swift
    open class func removeLiquidityWeth(authorization: String, name: String, inputBody: InputBody, completion: @escaping (_ data: TransactionAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let name = "name_example" // String | 
let inputBody = InputBody(to: "to_example", data: "data_example", input: "input_example", value: "value_example", nonce: "nonce_example", gas: "gas_example", gasPrice: "gasPrice_example", chainId: "chainId_example", encoding: "encoding_example", EOA: false, contractAddress: "contractAddress_example", tokenId: "tokenId_example", tokenIds: "tokenIds_example", approved: false, broadcast: false) // InputBody | 

YearnAPI.removeLiquidityWeth(authorization: authorization, name: name, inputBody: inputBody) { (response, error) in
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
