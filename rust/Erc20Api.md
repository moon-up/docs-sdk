# \Erc20Api

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                         | HTTP request                         | Description |
| -------------------------------------------------------------- | ------------------------------------ | ----------- |
| [**allowance\_erc20**](Erc20Api.md#allowance\_erc20)           | **POST** /erc20/{name}/allowance     |             |
| [**approve\_erc20**](Erc20Api.md#approve\_erc20)               | **POST** /erc20/{name}/approve       |             |
| [**balance\_of\_erc20**](Erc20Api.md#balance\_of\_erc20)       | **POST** /erc20/{name}/balance-of    |             |
| [**decimals\_erc20**](Erc20Api.md#decimals\_erc20)             | **POST** /erc20/{name}/decimals      |             |
| [**name\_erc20**](Erc20Api.md#name\_erc20)                     | **POST** /erc20/{name}/name          |             |
| [**symbol\_erc20**](Erc20Api.md#symbol\_erc20)                 | **POST** /erc20/{name}/symbol        |             |
| [**total\_supply\_erc20**](Erc20Api.md#total\_supply\_erc20)   | **POST** /erc20/{name}/total-supply  |             |
| [**transfer\_erc20**](Erc20Api.md#transfer\_erc20)             | **POST** /erc20/{name}/transfer      |             |
| [**transfer\_from\_erc20**](Erc20Api.md#transfer\_from\_erc20) | **POST** /erc20/{name}/transfer-from |             |

## allowance\_erc20

> crate::models::TransactionApiResponse allowance\_erc20(authorization, name, input\_body)

### Parameters

| Name              | Type                          | Description | Required    | Notes |
| ----------------- | ----------------------------- | ----------- | ----------- | ----- |
| **authorization** | **String**                    |             | \[required] |       |
| **name**          | **String**                    |             | \[required] |       |
| **input\_body**   | [**InputBody**](InputBody.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](Erc20Api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## approve\_erc20

> crate::models::TransactionApiResponse approve\_erc20(authorization, name, input\_body)

### Parameters

| Name              | Type                          | Description | Required    | Notes |
| ----------------- | ----------------------------- | ----------- | ----------- | ----- |
| **authorization** | **String**                    |             | \[required] |       |
| **name**          | **String**                    |             | \[required] |       |
| **input\_body**   | [**InputBody**](InputBody.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](Erc20Api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## balance\_of\_erc20

> crate::models::TransactionApiResponse balance\_of\_erc20(authorization, name, input\_body)

### Parameters

| Name              | Type                          | Description | Required    | Notes |
| ----------------- | ----------------------------- | ----------- | ----------- | ----- |
| **authorization** | **String**                    |             | \[required] |       |
| **name**          | **String**                    |             | \[required] |       |
| **input\_body**   | [**InputBody**](InputBody.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](Erc20Api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## decimals\_erc20

> crate::models::TransactionApiResponse decimals\_erc20(authorization, name, input\_body)

### Parameters

| Name              | Type                          | Description | Required    | Notes |
| ----------------- | ----------------------------- | ----------- | ----------- | ----- |
| **authorization** | **String**                    |             | \[required] |       |
| **name**          | **String**                    |             | \[required] |       |
| **input\_body**   | [**InputBody**](InputBody.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](Erc20Api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## name\_erc20

> crate::models::TransactionApiResponse name\_erc20(authorization, name, input\_body)

### Parameters

| Name              | Type                          | Description | Required    | Notes |
| ----------------- | ----------------------------- | ----------- | ----------- | ----- |
| **authorization** | **String**                    |             | \[required] |       |
| **name**          | **String**                    |             | \[required] |       |
| **input\_body**   | [**InputBody**](InputBody.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](Erc20Api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## symbol\_erc20

> crate::models::TransactionApiResponse symbol\_erc20(authorization, name, input\_body)

### Parameters

| Name              | Type                          | Description | Required    | Notes |
| ----------------- | ----------------------------- | ----------- | ----------- | ----- |
| **authorization** | **String**                    |             | \[required] |       |
| **name**          | **String**                    |             | \[required] |       |
| **input\_body**   | [**InputBody**](InputBody.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](Erc20Api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## total\_supply\_erc20

> crate::models::TransactionApiResponse total\_supply\_erc20(authorization, name, input\_body)

### Parameters

| Name              | Type                          | Description | Required    | Notes |
| ----------------- | ----------------------------- | ----------- | ----------- | ----- |
| **authorization** | **String**                    |             | \[required] |       |
| **name**          | **String**                    |             | \[required] |       |
| **input\_body**   | [**InputBody**](InputBody.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](Erc20Api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## transfer\_erc20

> crate::models::TransactionApiResponse transfer\_erc20(authorization, name, input\_body)

### Parameters

| Name              | Type                          | Description | Required    | Notes |
| ----------------- | ----------------------------- | ----------- | ----------- | ----- |
| **authorization** | **String**                    |             | \[required] |       |
| **name**          | **String**                    |             | \[required] |       |
| **input\_body**   | [**InputBody**](InputBody.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](Erc20Api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## transfer\_from\_erc20

> crate::models::TransactionApiResponse transfer\_from\_erc20(authorization, name, input\_body)

### Parameters

| Name              | Type                          | Description | Required    | Notes |
| ----------------- | ----------------------------- | ----------- | ----------- | ----- |
| **authorization** | **String**                    |             | \[required] |       |
| **name**          | **String**                    |             | \[required] |       |
| **input\_body**   | [**InputBody**](InputBody.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](Erc20Api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
