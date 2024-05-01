# BitcoinAPI

## BitcoinAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method                     | HTTP request                            | Description |
| -------------------------- | --------------------------------------- | ----------- |
| **createBitcoinAccount**   | **POST** /bitcoin                       |             |
| **getBitcoinAccount**      | **GET** /bitcoin/{accountName}          |             |
| **listBitcoinAccounts**    | **GET** /bitcoin                        |             |
| **signBitcoinTransaction** | **POST** /bitcoin/{accountName}/sign-tx |             |

## **createBitcoinAccount**

```swift
    open class func createBitcoinAccount(authorization: String, bitcoinInput: BitcoinInput, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let bitcoinInput = BitcoinInput(network: "network_example", privateKey: "privateKey_example") // BitcoinInput | 

BitcoinAPI.createBitcoinAccount(authorization: authorization, bitcoinInput: bitcoinInput) { (response, error) in
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
| **bitcoinInput**  | **BitcoinInput** |             |       |

#### Return type

**AccountAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **getBitcoinAccount**

```swift
    open class func getBitcoinAccount(authorization: String, accountName: String, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let accountName = "accountName_example" // String | 

BitcoinAPI.getBitcoinAccount(authorization: authorization, accountName: accountName) { (response, error) in
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

## **listBitcoinAccounts**

```swift
    open class func listBitcoinAccounts(authorization: String, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 

BitcoinAPI.listBitcoinAccounts(authorization: authorization) { (response, error) in
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

## **signBitcoinTransaction**

```swift
    open class func signBitcoinTransaction(authorization: String, accountName: String, bitcoinTransactionInput: BitcoinTransactionInput, completion: @escaping (_ data: BitcoinAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let accountName = "accountName_example" // String | 
let bitcoinTransactionInput = BitcoinTransactionInput(to: "to_example", value: 123, network: "network_example", compress: false) // BitcoinTransactionInput | 

BitcoinAPI.signBitcoinTransaction(authorization: authorization, accountName: accountName, bitcoinTransactionInput: bitcoinTransactionInput) { (response, error) in
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

| Name                        | Type                        | Description | Notes |
| --------------------------- | --------------------------- | ----------- | ----- |
| **authorization**           | **String**                  |             |       |
| **accountName**             | **String**                  |             |       |
| **bitcoinTransactionInput** | **BitcoinTransactionInput** |             |       |

#### Return type

**BitcoinAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
