# OnramperAPI

## OnramperAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method                                   | HTTP request                           | Description |
| ---------------------------------------- | -------------------------------------- | ----------- |
| **onRamperCheckout**                     | **POST** /onramper/fund/${accountName} |             |
| **onRamperGetQuotesBuy**                 | **GET** /onramper/quotes/buy           |             |
| **onRamperGetQuotesSell**                | **GET** /onramper/quotes/sell          |             |
| **onRamperGetSupportedAssets**           | **GET** /onramper/assets               |             |
| **onRamperGetSupportedCurrencies**       | **GET** /onramper/currencies           |             |
| **onRamperGetSupportedDefaultsAll**      | **GET** /onramper/defaults             |             |
| **onRamperGetSupportedOnRampsAll**       | **GET** /onramper/onramps              |             |
| **onRamperGetSupportedPaymentTypes**     | **GET** /onramper/payment-types        |             |
| **onRamperGetSupportedPaymentTypesFiat** | **GET** /onramper/payment-types/fiat   |             |

## **onRamperCheckout**

```swift
    open class func onRamperCheckout(authorization: String, accountName: String, transactionInput: TransactionInput, completion: @escaping (_ data: AnyCodable?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let accountName = "accountName_example" // String | 
let transactionInput = TransactionInput(supportedParams: TransactionInput_supportedParams(partnerData: TransactionInput_supportedParams_partnerData(redirectUrl: TransactionInput_supportedParams_partnerData_redirectUrl(success: "success_example")), theme: TransactionInput_supportedParams_theme(borderRadius: 123, cardColor: "cardColor_example", secondaryTextColor: "secondaryTextColor_example", primaryTextColor: "primaryTextColor_example", secondaryColor: "secondaryColor_example", primaryColor: "primaryColor_example", themeName: "themeName_example", isDark: false)), wallet: TransactionInput_wallet(address: "address_example"), metaData: TransactionInput_metaData(quoteId: "quoteId_example"), originatingHost: "originatingHost_example", partnerContext: "partnerContext_example", uuid: "uuid_example", network: "network_example", paymentMethod: "paymentMethod_example", type: "type_example", amount: 123, destination: "destination_example", source: "source_example", onramp: "onramp_example") // TransactionInput | 

OnramperAPI.onRamperCheckout(authorization: authorization, accountName: accountName, transactionInput: transactionInput) { (response, error) in
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
| **accountName**      | **String**           |             |       |
| **transactionInput** | **TransactionInput** |             |       |

#### Return type

**AnyCodable**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **onRamperGetQuotesBuy**

```swift
    open class func onRamperGetQuotesBuy(authorization: String, fiat: String, crypto: String, amount: Double, paymentMethod: String? = nil, uuid: String? = nil, clientName: String? = nil, country: String? = nil, completion: @escaping (_ data: [Quote]?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let fiat = "fiat_example" // String | 
let crypto = "crypto_example" // String | 
let amount = 987 // Double | 
let paymentMethod = "paymentMethod_example" // String |  (optional) (default to "creditcard")
let uuid = "uuid_example" // String |  (optional) (default to "")
let clientName = "clientName_example" // String |  (optional) (default to "")
let country = "country_example" // String |  (optional) (default to "")

OnramperAPI.onRamperGetQuotesBuy(authorization: authorization, fiat: fiat, crypto: crypto, amount: amount, paymentMethod: paymentMethod, uuid: uuid, clientName: clientName, country: country) { (response, error) in
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

| Name              | Type       | Description | Notes                                  |
| ----------------- | ---------- | ----------- | -------------------------------------- |
| **authorization** | **String** |             |                                        |
| **fiat**          | **String** |             |                                        |
| **crypto**        | **String** |             |                                        |
| **amount**        | **Double** |             |                                        |
| **paymentMethod** | **String** |             | \[optional] \[default to "creditcard"] |
| **uuid**          | **String** |             | \[optional] \[default to ""]           |
| **clientName**    | **String** |             | \[optional] \[default to ""]           |
| **country**       | **String** |             | \[optional] \[default to ""]           |

#### Return type

**\[Quote]**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **onRamperGetQuotesSell**

```swift
    open class func onRamperGetQuotesSell(authorization: String, fiat: String, crypto: String, amount: Double, paymentMethod: String? = nil, uuid: String? = nil, clientName: String? = nil, country: String? = nil, completion: @escaping (_ data: [SellQuote]?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let fiat = "fiat_example" // String | 
let crypto = "crypto_example" // String | 
let amount = 987 // Double | 
let paymentMethod = "paymentMethod_example" // String |  (optional) (default to "creditcard")
let uuid = "uuid_example" // String |  (optional) (default to "")
let clientName = "clientName_example" // String |  (optional) (default to "")
let country = "country_example" // String |  (optional) (default to "")

OnramperAPI.onRamperGetQuotesSell(authorization: authorization, fiat: fiat, crypto: crypto, amount: amount, paymentMethod: paymentMethod, uuid: uuid, clientName: clientName, country: country) { (response, error) in
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

| Name              | Type       | Description | Notes                                  |
| ----------------- | ---------- | ----------- | -------------------------------------- |
| **authorization** | **String** |             |                                        |
| **fiat**          | **String** |             |                                        |
| **crypto**        | **String** |             |                                        |
| **amount**        | **Double** |             |                                        |
| **paymentMethod** | **String** |             | \[optional] \[default to "creditcard"] |
| **uuid**          | **String** |             | \[optional] \[default to ""]           |
| **clientName**    | **String** |             | \[optional] \[default to ""]           |
| **country**       | **String** |             | \[optional] \[default to ""]           |

#### Return type

**\[SellQuote]**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **onRamperGetSupportedAssets**

```swift
    open class func onRamperGetSupportedAssets(authorization: String, source: String, country: String, completion: @escaping (_ data: SupportedAssetResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let source = "source_example" // String | 
let country = "country_example" // String | 

OnramperAPI.onRamperGetSupportedAssets(authorization: authorization, source: source, country: country) { (response, error) in
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
| **source**        | **String** |             |       |
| **country**       | **String** |             |       |

#### Return type

**SupportedAssetResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **onRamperGetSupportedCurrencies**

```swift
    open class func onRamperGetSupportedCurrencies(authorization: String, type: String, completion: @escaping (_ data: SupportedCurrenciesResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let type = "type_example" // String | 

OnramperAPI.onRamperGetSupportedCurrencies(authorization: authorization, type: type) { (response, error) in
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
| **type**          | **String** |             |       |

#### Return type

**SupportedCurrenciesResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **onRamperGetSupportedDefaultsAll**

```swift
    open class func onRamperGetSupportedDefaultsAll(authorization: String, country: String, type: String, completion: @escaping (_ data: SupportedDefaultResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let country = "country_example" // String | 
let type = "type_example" // String | 

OnramperAPI.onRamperGetSupportedDefaultsAll(authorization: authorization, country: country, type: type) { (response, error) in
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
| **country**       | **String** |             |       |
| **type**          | **String** |             |       |

#### Return type

**SupportedDefaultResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **onRamperGetSupportedOnRampsAll**

```swift
    open class func onRamperGetSupportedOnRampsAll(authorization: String, completion: @escaping (_ data: GetSupportedOnRampsResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 

OnramperAPI.onRamperGetSupportedOnRampsAll(authorization: authorization) { (response, error) in
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

**GetSupportedOnRampsResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **onRamperGetSupportedPaymentTypes**

```swift
    open class func onRamperGetSupportedPaymentTypes(authorization: String, fiat: String, country: String, type: String, completion: @escaping (_ data: SupportedPaymentTypesCurrencyResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let fiat = "fiat_example" // String | 
let country = "country_example" // String | 
let type = "type_example" // String | 

OnramperAPI.onRamperGetSupportedPaymentTypes(authorization: authorization, fiat: fiat, country: country, type: type) { (response, error) in
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
| **fiat**          | **String** |             |       |
| **country**       | **String** |             |       |
| **type**          | **String** |             |       |

#### Return type

**SupportedPaymentTypesCurrencyResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## **onRamperGetSupportedPaymentTypesFiat**

```swift
    open class func onRamperGetSupportedPaymentTypesFiat(authorization: String, fiat: String, country: String, completion: @escaping (_ data: SupportedPaymentTypesCurrencyResponse?, _ error: Error?) -> Void)
```

#### Example

```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let authorization = "authorization_example" // String | 
let fiat = "fiat_example" // String | 
let country = "country_example" // String | 

OnramperAPI.onRamperGetSupportedPaymentTypesFiat(authorization: authorization, fiat: fiat, country: country) { (response, error) in
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
| **fiat**          | **String** |             |       |
| **country**       | **String** |             |       |

#### Return type

**SupportedPaymentTypesCurrencyResponse**

#### Authorization

ApiKeyAuth, BearerAuth

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
