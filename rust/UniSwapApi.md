# \UniSwapApi

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                                                 | HTTP request                                          | Description |
| -------------------------------------------------------------------------------------- | ----------------------------------------------------- | ----------- |
| [**add\_liquidity**](UniSwapApi.md#add\_liquidity)                                     | **POST** /uniswap/{name}/add-liquidity                |             |
| [**remove\_liquidity**](UniSwapApi.md#remove\_liquidity)                               | **POST** /uniswap/{name}/remove-liquidity             |             |
| [**swap\_exact\_eth\_for\_tokens**](UniSwapApi.md#swap\_exact\_eth\_for\_tokens)       | **POST** /uniswap/{name}/swap-exact-eth-for-tokens    |             |
| [**swap\_exact\_tokens\_for\_tokens**](UniSwapApi.md#swap\_exact\_tokens\_for\_tokens) | **POST** /uniswap/{name}/swap-exact-tokens-for-tokens |             |

## add\_liquidity

> crate::models::TransactionApiResponse add\_liquidity(authorization, name, uniswap\_input)

### Parameters

| Name               | Type                                | Description | Required    | Notes |
| ------------------ | ----------------------------------- | ----------- | ----------- | ----- |
| **authorization**  | **String**                          |             | \[required] |       |
| **name**           | **String**                          |             | \[required] |       |
| **uniswap\_input** | [**UniswapInput**](UniswapInput.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](UniSwapApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## remove\_liquidity

> crate::models::TransactionApiResponse remove\_liquidity(authorization, name, uniswap\_input)

### Parameters

| Name               | Type                                | Description | Required    | Notes |
| ------------------ | ----------------------------------- | ----------- | ----------- | ----- |
| **authorization**  | **String**                          |             | \[required] |       |
| **name**           | **String**                          |             | \[required] |       |
| **uniswap\_input** | [**UniswapInput**](UniswapInput.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](UniSwapApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## swap\_exact\_eth\_for\_tokens

> crate::models::TransactionApiResponse swap\_exact\_eth\_for\_tokens(authorization, name, uniswap\_input)

### Parameters

| Name               | Type                                | Description | Required    | Notes |
| ------------------ | ----------------------------------- | ----------- | ----------- | ----- |
| **authorization**  | **String**                          |             | \[required] |       |
| **name**           | **String**                          |             | \[required] |       |
| **uniswap\_input** | [**UniswapInput**](UniswapInput.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](UniSwapApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## swap\_exact\_tokens\_for\_tokens

> crate::models::TransactionApiResponse swap\_exact\_tokens\_for\_tokens(authorization, name, uniswap\_input)

### Parameters

| Name               | Type                                | Description | Required    | Notes |
| ------------------ | ----------------------------------- | ----------- | ----------- | ----- |
| **authorization**  | **String**                          |             | \[required] |       |
| **name**           | **String**                          |             | \[required] |       |
| **uniswap\_input** | [**UniswapInput**](UniswapInput.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](UniSwapApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
