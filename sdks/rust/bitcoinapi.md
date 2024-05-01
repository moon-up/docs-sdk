# \BitcoinApi

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                                     | HTTP request                            | Description |
| -------------------------------------------------------------------------- | --------------------------------------- | ----------- |
| [**create\_bitcoin\_account**](bitcoinapi.md#create\_bitcoin\_account)     | **POST** /bitcoin                       |             |
| [**get\_bitcoin\_account**](bitcoinapi.md#get\_bitcoin\_account)           | **GET** /bitcoin/{accountName}          |             |
| [**list\_bitcoin\_accounts**](bitcoinapi.md#list\_bitcoin\_accounts)       | **GET** /bitcoin                        |             |
| [**sign\_bitcoin\_transaction**](bitcoinapi.md#sign\_bitcoin\_transaction) | **POST** /bitcoin/{accountName}/sign-tx |             |

## create\_bitcoin\_account

> crate::models::AccountApiResponse create\_bitcoin\_account(authorization, bitcoin\_input)

### Parameters

| Name               | Type                                | Description | Required    | Notes |
| ------------------ | ----------------------------------- | ----------- | ----------- | ----- |
| **authorization**  | **String**                          |             | \[required] |       |
| **bitcoin\_input** | [**BitcoinInput**](bitcoininput.md) |             | \[required] |       |

### Return type

[**crate::models::AccountApiResponse**](../../rust/docs/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](bitcoinapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## get\_bitcoin\_account

> crate::models::AccountApiResponse get\_bitcoin\_account(authorization, account\_name)

### Parameters

| Name              | Type       | Description | Required    | Notes |
| ----------------- | ---------- | ----------- | ----------- | ----- |
| **authorization** | **String** |             | \[required] |       |
| **account\_name** | **String** |             | \[required] |       |

### Return type

[**crate::models::AccountApiResponse**](../../rust/docs/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](bitcoinapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## list\_bitcoin\_accounts

> crate::models::AccountApiResponse list\_bitcoin\_accounts(authorization)

### Parameters

| Name              | Type       | Description | Required    | Notes |
| ----------------- | ---------- | ----------- | ----------- | ----- |
| **authorization** | **String** |             | \[required] |       |

### Return type

[**crate::models::AccountApiResponse**](../../rust/docs/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](bitcoinapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## sign\_bitcoin\_transaction

> crate::models::BitcoinApiResponse sign\_bitcoin\_transaction(authorization, account\_name, bitcoin\_transaction\_input)

### Parameters

| Name                            | Type                                                      | Description | Required    | Notes |
| ------------------------------- | --------------------------------------------------------- | ----------- | ----------- | ----- |
| **authorization**               | **String**                                                |             | \[required] |       |
| **account\_name**               | **String**                                                |             | \[required] |       |
| **bitcoin\_transaction\_input** | [**BitcoinTransactionInput**](bitcointransactioninput.md) |             | \[required] |       |

### Return type

[**crate::models::BitcoinApiResponse**](../../rust/docs/BitcoinAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](bitcoinapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
