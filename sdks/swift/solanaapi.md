# SolanaAPI

## SolanaAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method                    | HTTP request                           | Description |
| ------------------------- | -------------------------------------- | ----------- |
| **createSolanaAccount**   | **POST** /solana                       |             |
| **getSolanaAccount**      | **GET** /solana/{accountName}          |             |
| **listSolanaAccounts**    | **GET** /solana                        |             |
| **signSolanaTransaction** | **POST** /solana/{accountName}/sign-tx |             |

## **createSolanaAccount**

```swift
    open class func createSolanaAccount(authorization: String, solanaInput: SolanaInput, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let solanaInput = SolanaInput(network: "network_example", privateKey: "privateKey_example") // SolanaInput | 

SolanaAPI.createSolanaAccount(authorization: authorization, solanaInput: solanaInput) { (response, error) in
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
| **solanaInput**   | **SolanaInput** |             |       |

#### Return type

**AccountAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **getSolanaAccount**

```swift
    open class func getSolanaAccount(authorization: String, accountName: String, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let accountName = "accountName_example" // String | 

SolanaAPI.getSolanaAccount(authorization: authorization, accountName: accountName) { (response, error) in
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

## **listSolanaAccounts**

```swift
    open class func listSolanaAccounts(authorization: String, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 

SolanaAPI.listSolanaAccounts(authorization: authorization) { (response, error) in
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

## **signSolanaTransaction**

```swift
    open class func signSolanaTransaction(authorization: String, accountName: String, solanaTransactionInput: SolanaTransactionInput, completion: @escaping (_ data: SolanaAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let accountName = "accountName_example" // String | 
let solanaTransactionInput = SolanaTransactionInput(to: "to_example", value: 123, network: "network_example", compress: false) // SolanaTransactionInput | 

SolanaAPI.signSolanaTransaction(authorization: authorization, accountName: accountName, solanaTransactionInput: solanaTransactionInput) { (response, error) in
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
| **solanaTransactionInput** | **SolanaTransactionInput** |             |       |

#### Return type

**SolanaAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
