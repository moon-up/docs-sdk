# \Erc1155Api

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                                       | HTTP request                                      | Description |
| ---------------------------------------------------------------------------- | ------------------------------------------------- | ----------- |
| [**balance\_of**](erc1155api.md#balance\_of)                                 | **POST** /erc1155/{name}/balance-of               |             |
| [**balance\_of\_batch**](erc1155api.md#balance\_of\_batch)                   | **POST** /erc1155/{name}/balance-of-batch         |             |
| [**is\_approved\_for\_all**](erc1155api.md#is\_approved\_for\_all)           | **POST** /erc1155/{name}/is-approved-for-all      |             |
| [**safe\_batch\_transfer\_from**](erc1155api.md#safe\_batch\_transfer\_from) | **POST** /erc1155/{name}/safe-batch-transfer-from |             |
| [**safe\_transfer\_from**](erc1155api.md#safe\_transfer\_from)               | **POST** /erc1155/{name}/safe-transfer-from       |             |
| [**set\_approval\_for\_all**](erc1155api.md#set\_approval\_for\_all)         | **POST** /erc1155/{name}/set-approval-for-all     |             |

## balance\_of

> crate::models::TransactionApiResponse balance\_of(name, authorization, erc1155\_request)

### Parameters

| Name                 | Type                                    | Description | Required    | Notes |
| -------------------- | --------------------------------------- | ----------- | ----------- | ----- |
| **name**             | **String**                              |             | \[required] |       |
| **authorization**    | **String**                              |             | \[required] |       |
| **erc1155\_request** | [**Erc1155Request**](erc1155request.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](../../rust/docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc1155api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## balance\_of\_batch

> crate::models::TransactionApiResponse balance\_of\_batch(name, authorization, erc1155\_request)

### Parameters

| Name                 | Type                                    | Description | Required    | Notes |
| -------------------- | --------------------------------------- | ----------- | ----------- | ----- |
| **name**             | **String**                              |             | \[required] |       |
| **authorization**    | **String**                              |             | \[required] |       |
| **erc1155\_request** | [**Erc1155Request**](erc1155request.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](../../rust/docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc1155api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## is\_approved\_for\_all

> crate::models::TransactionApiResponse is\_approved\_for\_all(name, authorization, erc1155\_request)

### Parameters

| Name                 | Type                                    | Description | Required    | Notes |
| -------------------- | --------------------------------------- | ----------- | ----------- | ----- |
| **name**             | **String**                              |             | \[required] |       |
| **authorization**    | **String**                              |             | \[required] |       |
| **erc1155\_request** | [**Erc1155Request**](erc1155request.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](../../rust/docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc1155api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## safe\_batch\_transfer\_from

> crate::models::TransactionApiResponse safe\_batch\_transfer\_from(name, authorization, erc1155\_request)

### Parameters

| Name                 | Type                                    | Description | Required    | Notes |
| -------------------- | --------------------------------------- | ----------- | ----------- | ----- |
| **name**             | **String**                              |             | \[required] |       |
| **authorization**    | **String**                              |             | \[required] |       |
| **erc1155\_request** | [**Erc1155Request**](erc1155request.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](../../rust/docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc1155api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## safe\_transfer\_from

> crate::models::TransactionApiResponse safe\_transfer\_from(name, authorization, erc1155\_request)

### Parameters

| Name                 | Type                                    | Description | Required    | Notes |
| -------------------- | --------------------------------------- | ----------- | ----------- | ----- |
| **name**             | **String**                              |             | \[required] |       |
| **authorization**    | **String**                              |             | \[required] |       |
| **erc1155\_request** | [**Erc1155Request**](erc1155request.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](../../rust/docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc1155api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## set\_approval\_for\_all

> crate::models::TransactionApiResponse set\_approval\_for\_all(name, authorization, erc1155\_request)

### Parameters

| Name                 | Type                                    | Description | Required    | Notes |
| -------------------- | --------------------------------------- | ----------- | ----------- | ----- |
| **name**             | **String**                              |             | \[required] |       |
| **authorization**    | **String**                              |             | \[required] |       |
| **erc1155\_request** | [**Erc1155Request**](erc1155request.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](../../rust/docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc1155api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
