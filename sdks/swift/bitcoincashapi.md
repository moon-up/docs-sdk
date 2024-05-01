# BitcoincashAPI

## BitcoincashAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method                         | HTTP request                                | Description |
| ------------------------------ | ------------------------------------------- | ----------- |
| **createBitcoinCashAccount**   | **POST** /bitcoincash                       |             |
| **getBitcoinCashAccount**      | **GET** /bitcoincash/{accountName}          |             |
| **listBitcoinCashAccounts**    | **GET** /bitcoincash                        |             |
| **signBitcoinCashTransaction** | **POST** /bitcoincash/{accountName}/sign-tx |             |

## **createBitcoinCashAccount**

```swift
    open class func createBitcoinCashAccount(authorization: String, bitcoinCashInput: BitcoinCashInput, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let bitcoinCashInput = BitcoinCashInput(network: "network_example", privateKey: "privateKey_example") // BitcoinCashInput | 

BitcoincashAPI.createBitcoinCashAccount(authorization: authorization, bitcoinCashInput: bitcoinCashInput) { (response, error) in
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

| Name                 | Type                 | Description | Notes |
| -------------------- | -------------------- | ----------- | ----- |
| **authorization**    | **String**           |             |       |
| **bitcoinCashInput** | **BitcoinCashInput** |             |       |

#### Return type

**AccountAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **getBitcoinCashAccount**

```swift
    open class func getBitcoinCashAccount(authorization: String, accountName: String, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let accountName = "accountName_example" // String | 

BitcoincashAPI.getBitcoinCashAccount(authorization: authorization, accountName: accountName) { (response, error) in
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

## **listBitcoinCashAccounts**

```swift
    open class func listBitcoinCashAccounts(authorization: String, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 

BitcoincashAPI.listBitcoinCashAccounts(authorization: authorization) { (response, error) in
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

## **signBitcoinCashTransaction**

```swift
    open class func signBitcoinCashTransaction(authorization: String, accountName: String, bitcoinCashTransactionInput: BitcoinCashTransactionInput, completion: @escaping (_ data: BitcoinCashAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let accountName = "accountName_example" // String | 
let bitcoinCashTransactionInput = BitcoinCashTransactionInput(to: "to_example", value: 123, network: "network_example", compress: false) // BitcoinCashTransactionInput | 

BitcoincashAPI.signBitcoinCashTransaction(authorization: authorization, accountName: accountName, bitcoinCashTransactionInput: bitcoinCashTransactionInput) { (response, error) in
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

| Name                            | Type                            | Description | Notes |
| ------------------------------- | ------------------------------- | ----------- | ----- |
| **authorization**               | **String**                      |             |       |
| **accountName**                 | **String**                      |             |       |
| **bitcoinCashTransactionInput** | **BitcoinCashTransactionInput** |             |       |

#### Return type

**BitcoinCashAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
