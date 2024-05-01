# LitecoinAPI

## LitecoinAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method                      | HTTP request                             | Description |
| --------------------------- | ---------------------------------------- | ----------- |
| **createLitecoinAccount**   | **POST** /litecoin                       |             |
| **getLitecoinAccount**      | **GET** /litecoin/{accountName}          |             |
| **listLitecoinAccounts**    | **GET** /litecoin                        |             |
| **signLitecoinTransaction** | **POST** /litecoin/{accountName}/sign-tx |             |

## **createLitecoinAccount**

```swift
    open class func createLitecoinAccount(authorization: String, litecoinInput: LitecoinInput, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let litecoinInput = LitecoinInput(network: "network_example", privateKey: "privateKey_example") // LitecoinInput | 

LitecoinAPI.createLitecoinAccount(authorization: authorization, litecoinInput: litecoinInput) { (response, error) in
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

| Name              | Type              | Description | Notes |
| ----------------- | ----------------- | ----------- | ----- |
| **authorization** | **String**        |             |       |
| **litecoinInput** | **LitecoinInput** |             |       |

#### Return type

**AccountAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **getLitecoinAccount**

```swift
    open class func getLitecoinAccount(authorization: String, accountName: String, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let accountName = "accountName_example" // String | 

LitecoinAPI.getLitecoinAccount(authorization: authorization, accountName: accountName) { (response, error) in
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

## **listLitecoinAccounts**

```swift
    open class func listLitecoinAccounts(authorization: String, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 

LitecoinAPI.listLitecoinAccounts(authorization: authorization) { (response, error) in
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

## **signLitecoinTransaction**

```swift
    open class func signLitecoinTransaction(authorization: String, accountName: String, litecoinTransactionInput: LitecoinTransactionInput, completion: @escaping (_ data: LitecoinAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let accountName = "accountName_example" // String | 
let litecoinTransactionInput = LitecoinTransactionInput(to: "to_example", value: 123, network: "network_example", compress: false) // LitecoinTransactionInput | 

LitecoinAPI.signLitecoinTransaction(authorization: authorization, accountName: accountName, litecoinTransactionInput: litecoinTransactionInput) { (response, error) in
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

| Name                         | Type                         | Description | Notes |
| ---------------------------- | ---------------------------- | ----------- | ----- |
| **authorization**            | **String**                   |             |       |
| **accountName**              | **String**                   |             |       |
| **litecoinTransactionInput** | **LitecoinTransactionInput** |             |       |

#### Return type

**LitecoinAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
