# OneinchAPI

## OneinchAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method              | HTTP request                         | Description |
| ------------------- | ------------------------------------ | ----------- |
| **approveCallData** | **POST** /oneinch/approve-call-data  |             |
| **approveSpender**  | **POST** /oneinch/approve-spender    |             |
| **protocols**       | **POST** /oneinch/protocols          |             |
| **quote**           | **POST** /oneinch/quote              |             |
| **swap**            | **POST** /oneinch/{accountName}/swap |             |
| **tokens**          | **POST** /oneinch/tokens             |             |

## **approveCallData**

```swift
    open class func approveCallData(body: AnyCodable, completion: @escaping (_ data: AnyCodable?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let body =  // AnyCodable | 

OneinchAPI.approveCallData(body: body) { (response, error) in
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

| Name     | Type           | Description | Notes |
| -------- | -------------- | ----------- | ----- |
| **body** | **AnyCodable** |             |       |

#### Return type

**AnyCodable**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **approveSpender**

```swift
    open class func approveSpender(body: AnyCodable, completion: @escaping (_ data: AnyCodable?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let body =  // AnyCodable | 

OneinchAPI.approveSpender(body: body) { (response, error) in
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

| Name     | Type           | Description | Notes |
| -------- | -------------- | ----------- | ----- |
| **body** | **AnyCodable** |             |       |

#### Return type

**AnyCodable**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **protocols**

```swift
    open class func protocols(body: AnyCodable, completion: @escaping (_ data: AnyCodable?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let body =  // AnyCodable | 

OneinchAPI.protocols(body: body) { (response, error) in
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

| Name     | Type           | Description | Notes |
| -------- | -------------- | ----------- | ----- |
| **body** | **AnyCodable** |             |       |

#### Return type

**AnyCodable**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **quote**

```swift
    open class func quote(body: AnyCodable, completion: @escaping (_ data: AnyCodable?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let body =  // AnyCodable | 

OneinchAPI.quote(body: body) { (response, error) in
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

| Name     | Type           | Description | Notes |
| -------- | -------------- | ----------- | ----- |
| **body** | **AnyCodable** |             |       |

#### Return type

**AnyCodable**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **swap**

```swift
    open class func swap(accountName: String, authorization: String, getSwapDto: GetSwapDto, completion: @escaping (_ data: AnyCodable?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let accountName = "accountName_example" // String | 
let authorization = "authorization_example" // String | 
let getSwapDto = GetSwapDto(src: "src_example", dst: "dst_example", amount: "amount_example", from: "from_example", slippage: 123, protocols: "protocols_example", fee: "fee_example", disableEstimate: false, permit: "permit_example", includeTokensInfo: false, includeProtocols: false, compatibility: false, allowPartialFill: false, parts: "parts_example", mainRouteParts: "mainRouteParts_example", connectorTokens: "connectorTokens_example", complexityLevel: "complexityLevel_example", gasLimit: "gasLimit_example", gasPrice: "gasPrice_example", referrer: "referrer_example", receiver: "receiver_example", chainId: 123) // GetSwapDto | 

OneinchAPI.swap(accountName: accountName, authorization: authorization, getSwapDto: getSwapDto) { (response, error) in
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

| Name              | Type           | Description | Notes |
| ----------------- | -------------- | ----------- | ----- |
| **accountName**   | **String**     |             |       |
| **authorization** | **String**     |             |       |
| **getSwapDto**    | **GetSwapDto** |             |       |

#### Return type

**AnyCodable**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **tokens**

```swift
    open class func tokens(body: AnyCodable, completion: @escaping (_ data: AnyCodable?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let body =  // AnyCodable | 

OneinchAPI.tokens(body: body) { (response, error) in
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

| Name     | Type           | Description | Notes |
| -------- | -------------- | ----------- | ----- |
| **body** | **AnyCodable** |             |       |

#### Return type

**AnyCodable**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
