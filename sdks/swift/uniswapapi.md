# UniSwapAPI

## UniSwapAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method                       | HTTP request                                          | Description |
| ---------------------------- | ----------------------------------------------------- | ----------- |
| **addLiquidity**             | **POST** /uniswap/{name}/add-liquidity                |             |
| **removeLiquidity**          | **POST** /uniswap/{name}/remove-liquidity             |             |
| **swapExactETHForTokens**    | **POST** /uniswap/{name}/swap-exact-eth-for-tokens    |             |
| **swapExactTokensForTokens** | **POST** /uniswap/{name}/swap-exact-tokens-for-tokens |             |

## **addLiquidity**

```swift
    open class func addLiquidity(authorization: String, name: String, uniswapInput: UniswapInput, completion: @escaping (_ data: TransactionAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let name = "name_example" // String | 
let uniswapInput = UniswapInput(to: "to_example", data: "data_example", input: "input_example", value: "value_example", nonce: "nonce_example", gas: "gas_example", gasPrice: "gasPrice_example", chainId: "chainId_example", encoding: "encoding_example", EOA: false, contractAddress: "contractAddress_example", tokenId: "tokenId_example", tokenIds: "tokenIds_example", approved: false, broadcast: false, tokenA: "tokenA_example", tokenB: "tokenB_example", amountA: "amountA_example", amountB: "amountB_example") // UniswapInput | 

UniSwapAPI.addLiquidity(authorization: authorization, name: name, uniswapInput: uniswapInput) { (response, error) in
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

| Name              | Type             | Description | Notes |
| ----------------- | ---------------- | ----------- | ----- |
| **authorization** | **String**       |             |       |
| **name**          | **String**       |             |       |
| **uniswapInput**  | **UniswapInput** |             |       |

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
    open class func removeLiquidity(authorization: String, name: String, uniswapInput: UniswapInput, completion: @escaping (_ data: TransactionAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let name = "name_example" // String | 
let uniswapInput = UniswapInput(to: "to_example", data: "data_example", input: "input_example", value: "value_example", nonce: "nonce_example", gas: "gas_example", gasPrice: "gasPrice_example", chainId: "chainId_example", encoding: "encoding_example", EOA: false, contractAddress: "contractAddress_example", tokenId: "tokenId_example", tokenIds: "tokenIds_example", approved: false, broadcast: false, tokenA: "tokenA_example", tokenB: "tokenB_example", amountA: "amountA_example", amountB: "amountB_example") // UniswapInput | 

UniSwapAPI.removeLiquidity(authorization: authorization, name: name, uniswapInput: uniswapInput) { (response, error) in
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

| Name              | Type             | Description | Notes |
| ----------------- | ---------------- | ----------- | ----- |
| **authorization** | **String**       |             |       |
| **name**          | **String**       |             |       |
| **uniswapInput**  | **UniswapInput** |             |       |

#### Return type

**TransactionAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **swapExactETHForTokens**

```swift
    open class func swapExactETHForTokens(authorization: String, name: String, uniswapInput: UniswapInput, completion: @escaping (_ data: TransactionAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let name = "name_example" // String | 
let uniswapInput = UniswapInput(to: "to_example", data: "data_example", input: "input_example", value: "value_example", nonce: "nonce_example", gas: "gas_example", gasPrice: "gasPrice_example", chainId: "chainId_example", encoding: "encoding_example", EOA: false, contractAddress: "contractAddress_example", tokenId: "tokenId_example", tokenIds: "tokenIds_example", approved: false, broadcast: false, tokenA: "tokenA_example", tokenB: "tokenB_example", amountA: "amountA_example", amountB: "amountB_example") // UniswapInput | 

UniSwapAPI.swapExactETHForTokens(authorization: authorization, name: name, uniswapInput: uniswapInput) { (response, error) in
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

| Name              | Type             | Description | Notes |
| ----------------- | ---------------- | ----------- | ----- |
| **authorization** | **String**       |             |       |
| **name**          | **String**       |             |       |
| **uniswapInput**  | **UniswapInput** |             |       |

#### Return type

**TransactionAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **swapExactTokensForTokens**

```swift
    open class func swapExactTokensForTokens(authorization: String, name: String, uniswapInput: UniswapInput, completion: @escaping (_ data: TransactionAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let name = "name_example" // String | 
let uniswapInput = UniswapInput(to: "to_example", data: "data_example", input: "input_example", value: "value_example", nonce: "nonce_example", gas: "gas_example", gasPrice: "gasPrice_example", chainId: "chainId_example", encoding: "encoding_example", EOA: false, contractAddress: "contractAddress_example", tokenId: "tokenId_example", tokenIds: "tokenIds_example", approved: false, broadcast: false, tokenA: "tokenA_example", tokenB: "tokenB_example", amountA: "amountA_example", amountB: "amountB_example") // UniswapInput | 

UniSwapAPI.swapExactTokensForTokens(authorization: authorization, name: name, uniswapInput: uniswapInput) { (response, error) in
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

| Name              | Type             | Description | Notes |
| ----------------- | ---------------- | ----------- | ----- |
| **authorization** | **String**       |             |       |
| **name**          | **String**       |             |       |
| **uniswapInput**  | **UniswapInput** |             |       |

#### Return type

**TransactionAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
