# EosAPI

## EosAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method                 | HTTP request                        | Description |
| ---------------------- | ----------------------------------- | ----------- |
| **createEosAccount**   | **POST** /eos                       |             |
| **getEosAccount**      | **GET** /eos/{accountName}          |             |
| **listEosAccounts**    | **GET** /eos                        |             |
| **signEosTransaction** | **POST** /eos/{accountName}/sign-tx |             |

## **createEosAccount**

```swift
    open class func createEosAccount(authorization: String, eosInput: EosInput, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let eosInput = EosInput(network: "network_example", privateKey: "privateKey_example") // EosInput | 

EosAPI.createEosAccount(authorization: authorization, eosInput: eosInput) { (response, error) in
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

| Name              | Type         | Description | Notes |
| ----------------- | ------------ | ----------- | ----- |
| **authorization** | **String**   |             |       |
| **eosInput**      | **EosInput** |             |       |

#### Return type

**AccountAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **getEosAccount**

```swift
    open class func getEosAccount(authorization: String, accountName: String, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let accountName = "accountName_example" // String | 

EosAPI.getEosAccount(authorization: authorization, accountName: accountName) { (response, error) in
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

## **listEosAccounts**

```swift
    open class func listEosAccounts(authorization: String, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 

EosAPI.listEosAccounts(authorization: authorization) { (response, error) in
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

## **signEosTransaction**

```swift
    open class func signEosTransaction(authorization: String, accountName: String, eosTransactionInput: EosTransactionInput, completion: @escaping (_ data: EosAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let accountName = "accountName_example" // String | 
let eosTransactionInput = EosTransactionInput(to: "to_example", value: 123, network: "network_example", compress: false) // EosTransactionInput | 

EosAPI.signEosTransaction(authorization: authorization, accountName: accountName, eosTransactionInput: eosTransactionInput) { (response, error) in
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

| Name                    | Type                    | Description | Notes |
| ----------------------- | ----------------------- | ----------- | ----- |
| **authorization**       | **String**              |             |       |
| **accountName**         | **String**              |             |       |
| **eosTransactionInput** | **EosTransactionInput** |             |       |

#### Return type

**EosAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
