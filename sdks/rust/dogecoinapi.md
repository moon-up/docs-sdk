# \DogeCoinApi

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                                            | HTTP request                             | Description |
| --------------------------------------------------------------------------------- | ---------------------------------------- | ----------- |
| [**create\_doge\_coin\_account**](dogecoinapi.md#create\_doge\_coin\_account)     | **POST** /dogecoin                       |             |
| [**get\_doge\_coin\_account**](dogecoinapi.md#get\_doge\_coin\_account)           | **GET** /dogecoin/{accountName}          |             |
| [**list\_doge\_coin\_accounts**](dogecoinapi.md#list\_doge\_coin\_accounts)       | **GET** /dogecoin                        |             |
| [**sign\_doge\_coin\_transaction**](dogecoinapi.md#sign\_doge\_coin\_transaction) | **POST** /dogecoin/{accountName}/sign-tx |             |

## create\_doge\_coin\_account

> crate::models::AccountApiResponse create\_doge\_coin\_account(authorization, doge\_coin\_input)

### Parameters

| Name                  | Type                                  | Description | Required    | Notes |
| --------------------- | ------------------------------------- | ----------- | ----------- | ----- |
| **authorization**     | **String**                            |             | \[required] |       |
| **doge\_coin\_input** | [**DogeCoinInput**](dogecoininput.md) |             | \[required] |       |

### Return type

[**crate::models::AccountApiResponse**](../../rust/docs/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](dogecoinapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## get\_doge\_coin\_account

> crate::models::AccountApiResponse get\_doge\_coin\_account(authorization, account\_name)

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

[\[Back to top\]](dogecoinapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## list\_doge\_coin\_accounts

> crate::models::AccountApiResponse list\_doge\_coin\_accounts(authorization)

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

[\[Back to top\]](dogecoinapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## sign\_doge\_coin\_transaction

> crate::models::DogeCoinApiResponse sign\_doge\_coin\_transaction(authorization, account\_name, doge\_coin\_transaction\_input)

### Parameters

| Name                               | Type                                                        | Description | Required    | Notes |
| ---------------------------------- | ----------------------------------------------------------- | ----------- | ----------- | ----- |
| **authorization**                  | **String**                                                  |             | \[required] |       |
| **account\_name**                  | **String**                                                  |             | \[required] |       |
| **doge\_coin\_transaction\_input** | [**DogeCoinTransactionInput**](dogecointransactioninput.md) |             | \[required] |       |

### Return type

[**crate::models::DogeCoinApiResponse**](../../rust/docs/DogeCoinAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](dogecoinapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
