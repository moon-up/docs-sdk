# \AaveApi

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                    | HTTP request                            | Description |
| --------------------------------------------------------- | --------------------------------------- | ----------- |
| [**borrow**](aaveapi.md#borrow)                           | **POST** /aave/{name}/borrow            |             |
| [**lend**](aaveapi.md#lend)                               | **POST** /aave/{name}/lend              |             |
| [**repay**](aaveapi.md#repay)                             | **POST** /aave/{name}/repay             |             |
| [**user\_reserve\_data**](aaveapi.md#user\_reserve\_data) | **POST** /aave/{name}/user-reserve-data |             |

## borrow

> crate::models::TransactionApiResponse borrow(authorization, name, aave\_input)

### Parameters

| Name              | Type                          | Description | Required    | Notes |
| ----------------- | ----------------------------- | ----------- | ----------- | ----- |
| **authorization** | **String**                    |             | \[required] |       |
| **name**          | **String**                    |             | \[required] |       |
| **aave\_input**   | [**AaveInput**](aaveinput.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](../../rust/docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](aaveapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## lend

> crate::models::TransactionApiResponse lend(authorization, name, aave\_input)

### Parameters

| Name              | Type                          | Description | Required    | Notes |
| ----------------- | ----------------------------- | ----------- | ----------- | ----- |
| **authorization** | **String**                    |             | \[required] |       |
| **name**          | **String**                    |             | \[required] |       |
| **aave\_input**   | [**AaveInput**](aaveinput.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](../../rust/docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](aaveapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## repay

> crate::models::TransactionApiResponse repay(authorization, name, aave\_input)

### Parameters

| Name              | Type                          | Description | Required    | Notes |
| ----------------- | ----------------------------- | ----------- | ----------- | ----- |
| **authorization** | **String**                    |             | \[required] |       |
| **name**          | **String**                    |             | \[required] |       |
| **aave\_input**   | [**AaveInput**](aaveinput.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](../../rust/docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](aaveapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## user\_reserve\_data

> crate::models::AaveReservesApiResponse user\_reserve\_data(authorization, name, aave\_input)

### Parameters

| Name              | Type                          | Description | Required    | Notes |
| ----------------- | ----------------------------- | ----------- | ----------- | ----- |
| **authorization** | **String**                    |             | \[required] |       |
| **name**          | **String**                    |             | \[required] |       |
| **aave\_input**   | [**AaveInput**](aaveinput.md) |             | \[required] |       |

### Return type

[**crate::models::AaveReservesApiResponse**](../../rust/docs/AaveReservesAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](aaveapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
