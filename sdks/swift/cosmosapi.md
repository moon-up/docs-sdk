# CosmosAPI

## CosmosAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method                    | HTTP request                           | Description |
| ------------------------- | -------------------------------------- | ----------- |
| **createCosmosAccount**   | **POST** /cosmos                       |             |
| **getCosmosAccount**      | **GET** /cosmos/{accountName}          |             |
| **listCosmosAccounts**    | **GET** /cosmos                        |             |
| **signCosmosTransaction** | **POST** /cosmos/{accountName}/sign-tx |             |

## **createCosmosAccount**

```swift
    open class func createCosmosAccount(authorization: String, cosmosInput: CosmosInput, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let cosmosInput = CosmosInput(network: "network_example", privateKey: "privateKey_example") // CosmosInput | 

CosmosAPI.createCosmosAccount(authorization: authorization, cosmosInput: cosmosInput) { (response, error) in
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
| **cosmosInput**   | **CosmosInput** |             |       |

#### Return type

**AccountAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **getCosmosAccount**

```swift
    open class func getCosmosAccount(authorization: String, accountName: String, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let accountName = "accountName_example" // String | 

CosmosAPI.getCosmosAccount(authorization: authorization, accountName: accountName) { (response, error) in
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

## **listCosmosAccounts**

```swift
    open class func listCosmosAccounts(authorization: String, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 

CosmosAPI.listCosmosAccounts(authorization: authorization) { (response, error) in
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

## **signCosmosTransaction**

```swift
    open class func signCosmosTransaction(authorization: String, accountName: String, cosmosTransactionInput: CosmosTransactionInput, completion: @escaping (_ data: CosmosAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let accountName = "accountName_example" // String | 
let cosmosTransactionInput = CosmosTransactionInput(to: "to_example", value: 123, network: "network_example", compress: false) // CosmosTransactionInput | 

CosmosAPI.signCosmosTransaction(authorization: authorization, accountName: accountName, cosmosTransactionInput: cosmosTransactionInput) { (response, error) in
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
| **cosmosTransactionInput** | **CosmosTransactionInput** |             |       |

#### Return type

**CosmosAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
