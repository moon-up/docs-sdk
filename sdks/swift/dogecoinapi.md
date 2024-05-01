# DogeCoinAPI

## DogeCoinAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method                      | HTTP request                             | Description |
| --------------------------- | ---------------------------------------- | ----------- |
| **createDogeCoinAccount**   | **POST** /dogecoin                       |             |
| **getDogeCoinAccount**      | **GET** /dogecoin/{accountName}          |             |
| **listDogeCoinAccounts**    | **GET** /dogecoin                        |             |
| **signDogeCoinTransaction** | **POST** /dogecoin/{accountName}/sign-tx |             |

## **createDogeCoinAccount**

```swift
    open class func createDogeCoinAccount(authorization: String, dogeCoinInput: DogeCoinInput, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let dogeCoinInput = DogeCoinInput(network: "network_example", privateKey: "privateKey_example") // DogeCoinInput | 

DogeCoinAPI.createDogeCoinAccount(authorization: authorization, dogeCoinInput: dogeCoinInput) { (response, error) in
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
| **dogeCoinInput** | **DogeCoinInput** |             |       |

#### Return type

**AccountAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **getDogeCoinAccount**

```swift
    open class func getDogeCoinAccount(authorization: String, accountName: String, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let accountName = "accountName_example" // String | 

DogeCoinAPI.getDogeCoinAccount(authorization: authorization, accountName: accountName) { (response, error) in
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

## **listDogeCoinAccounts**

```swift
    open class func listDogeCoinAccounts(authorization: String, completion: @escaping (_ data: AccountAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 

DogeCoinAPI.listDogeCoinAccounts(authorization: authorization) { (response, error) in
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

## **signDogeCoinTransaction**

```swift
    open class func signDogeCoinTransaction(authorization: String, accountName: String, dogeCoinTransactionInput: DogeCoinTransactionInput, completion: @escaping (_ data: DogeCoinAPIResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let accountName = "accountName_example" // String | 
let dogeCoinTransactionInput = DogeCoinTransactionInput(to: "to_example", value: 123, network: "network_example", compress: false) // DogeCoinTransactionInput | 

DogeCoinAPI.signDogeCoinTransaction(authorization: authorization, accountName: accountName, dogeCoinTransactionInput: dogeCoinTransactionInput) { (response, error) in
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
| **dogeCoinTransactionInput** | **DogeCoinTransactionInput** |             |       |

#### Return type

**DogeCoinAPIResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
