# \OneinchApi

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                       | HTTP request                         | Description |
| ------------------------------------------------------------ | ------------------------------------ | ----------- |
| [**approve\_call\_data**](oneinchapi.md#approve\_call\_data) | **POST** /oneinch/approve-call-data  |             |
| [**approve\_spender**](oneinchapi.md#approve\_spender)       | **POST** /oneinch/approve-spender    |             |
| [**protocols**](oneinchapi.md#protocols)                     | **POST** /oneinch/protocols          |             |
| [**quote**](oneinchapi.md#quote)                             | **POST** /oneinch/quote              |             |
| [**swap**](oneinchapi.md#swap)                               | **POST** /oneinch/{accountName}/swap |             |
| [**tokens**](oneinchapi.md#tokens)                           | **POST** /oneinch/tokens             |             |

## approve\_call\_data

> serde\_json::Value approve\_call\_data(body)

### Parameters

| Name     | Type                           | Description | Required    | Notes |
| -------- | ------------------------------ | ----------- | ----------- | ----- |
| **body** | Option<**serde\_json::Value**> |             | \[required] |       |

### Return type

[**serde\_json::Value**](../../rust/docs/serde\_json::Value.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](oneinchapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## approve\_spender

> serde\_json::Value approve\_spender(body)

### Parameters

| Name     | Type                           | Description | Required    | Notes |
| -------- | ------------------------------ | ----------- | ----------- | ----- |
| **body** | Option<**serde\_json::Value**> |             | \[required] |       |

### Return type

[**serde\_json::Value**](../../rust/docs/serde\_json::Value.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](oneinchapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## protocols

> serde\_json::Value protocols(body)

### Parameters

| Name     | Type                           | Description | Required    | Notes |
| -------- | ------------------------------ | ----------- | ----------- | ----- |
| **body** | Option<**serde\_json::Value**> |             | \[required] |       |

### Return type

[**serde\_json::Value**](../../rust/docs/serde\_json::Value.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](oneinchapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## quote

> serde\_json::Value quote(body)

### Parameters

| Name     | Type                           | Description | Required    | Notes |
| -------- | ------------------------------ | ----------- | ----------- | ----- |
| **body** | Option<**serde\_json::Value**> |             | \[required] |       |

### Return type

[**serde\_json::Value**](../../rust/docs/serde\_json::Value.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](oneinchapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## swap

> serde\_json::Value swap(account\_name, authorization, get\_swap\_dto)

### Parameters

| Name               | Type                            | Description | Required    | Notes |
| ------------------ | ------------------------------- | ----------- | ----------- | ----- |
| **account\_name**  | **String**                      |             | \[required] |       |
| **authorization**  | **String**                      |             | \[required] |       |
| **get\_swap\_dto** | [**GetSwapDto**](getswapdto.md) |             | \[required] |       |

### Return type

[**serde\_json::Value**](../../rust/docs/serde\_json::Value.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](oneinchapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## tokens

> serde\_json::Value tokens(body)

### Parameters

| Name     | Type                           | Description | Required    | Notes |
| -------- | ------------------------------ | ----------- | ----------- | ----- |
| **body** | Option<**serde\_json::Value**> |             | \[required] |       |

### Return type

[**serde\_json::Value**](../../rust/docs/serde\_json::Value.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](oneinchapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
