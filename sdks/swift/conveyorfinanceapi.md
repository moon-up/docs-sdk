# ConveyorFinanceAPI

## ConveyorFinanceAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method   | HTTP request                          | Description |
| -------- | ------------------------------------- | ----------- |
| **swap** | **POST** /conveyorfinance/{name}/swap |             |

## **swap**

```swift
    open class func swap(authorization: String, name: String, tokenSwapParams: TokenSwapParams, completion: @escaping (_ data: ConveyorFinanceControllerResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let name = "name_example" // String | 
let tokenSwapParams = TokenSwapParams(to: "to_example", data: "data_example", input: "input_example", value: "value_example", nonce: "nonce_example", gas: "gas_example", gasPrice: "gasPrice_example", chainId: "chainId_example", encoding: "encoding_example", EOA: false, contractAddress: "contractAddress_example", tokenId: "tokenId_example", tokenIds: "tokenIds_example", approved: false, broadcast: false, tokenIn: "tokenIn_example", tokenOut: "tokenOut_example", tokenInDecimals: 123, tokenOutDecimals: 123, amountIn: "amountIn_example", slippage: "slippage_example", recipient: "recipient_example", referrer: "referrer_example") // TokenSwapParams | 

ConveyorFinanceAPI.swap(authorization: authorization, name: name, tokenSwapParams: tokenSwapParams) { (response, error) in
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
| **name**            | **String**          |             |       |
| **tokenSwapParams** | **TokenSwapParams** |             |       |

#### Return type

**ConveyorFinanceControllerResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
