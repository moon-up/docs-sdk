# \YearnApi

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                             | HTTP request                                 | Description |
| ------------------------------------------------------------------ | -------------------------------------------- | ----------- |
| [**add\_liquidity**](YearnApi.md#add\_liquidity)                   | **POST** /yearn/{name}/add-liquidity         |             |
| [**add\_liquidity\_weth**](YearnApi.md#add\_liquidity\_weth)       | **POST** /yearn/{name}/add-liquidity-weth    |             |
| [**remove\_liquidity**](YearnApi.md#remove\_liquidity)             | **POST** /yearn/{name}/remove-liquidity      |             |
| [**remove\_liquidity\_weth**](YearnApi.md#remove\_liquidity\_weth) | **POST** /yearn/{name}/remove-liquidity-weth |             |

## add\_liquidity

> crate::models::TransactionApiResponse add\_liquidity(authorization, name, input\_body)

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

[\[Back to top\]](YearnApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## add\_liquidity\_weth

> crate::models::TransactionApiResponse add\_liquidity\_weth(authorization, name, input\_body)

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

[\[Back to top\]](YearnApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## remove\_liquidity

> crate::models::TransactionApiResponse remove\_liquidity(authorization, name, input\_body)

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

[\[Back to top\]](YearnApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## remove\_liquidity\_weth

> crate::models::TransactionApiResponse remove\_liquidity\_weth(authorization, name, input\_body)

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

[\[Back to top\]](YearnApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
