# \Erc721Api

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                              | HTTP request                                 | Description |
| ------------------------------------------------------------------- | -------------------------------------------- | ----------- |
| [**approve**](erc721api.md#approve)                                 | **POST** /erc721/{name}/approve              |             |
| [**balance\_of**](erc721api.md#balance\_of)                         | **POST** /erc721/{name}/balance-of           |             |
| [**get\_approved**](erc721api.md#get\_approved)                     | **POST** /erc721/{name}/get-approved         |             |
| [**is\_approved\_for\_all**](erc721api.md#is\_approved\_for\_all)   | **POST** /erc721/{name}/is-approved-for-all  |             |
| [**name**](erc721api.md#name)                                       | **POST** /erc721/{name}/name                 |             |
| [**owner\_of**](erc721api.md#owner\_of)                             | **POST** /erc721/{name}/owner-of             |             |
| [**safe\_transfer\_from**](erc721api.md#safe\_transfer\_from)       | **POST** /erc721/{name}/safe-transfer-from   |             |
| [**set\_approval\_for\_all**](erc721api.md#set\_approval\_for\_all) | **POST** /erc721/{name}/set-approval-for-all |             |
| [**symbol**](erc721api.md#symbol)                                   | **POST** /erc721/{name}/symbol               |             |
| [**token\_uri**](erc721api.md#token\_uri)                           | **POST** /erc721/{name}/token-uri            |             |
| [**transfer**](erc721api.md#transfer)                               | **POST** /erc721/{name}/transfer             |             |
| [**transfer\_from**](erc721api.md#transfer\_from)                   | **POST** /erc721/{name}/transfer-from        |             |

## approve

> crate::models::TransactionApiResponse approve(authorization, name, erc721\_request)

### Parameters

| Name                | Type                                  | Description | Required    | Notes |
| ------------------- | ------------------------------------- | ----------- | ----------- | ----- |
| **authorization**   | **String**                            |             | \[required] |       |
| **name**            | **String**                            |             | \[required] |       |
| **erc721\_request** | [**Erc721Request**](erc721request.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](../../rust/docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## balance\_of

> crate::models::TransactionApiResponse balance\_of(authorization, name, erc721\_request)

### Parameters

| Name                | Type                                  | Description | Required    | Notes |
| ------------------- | ------------------------------------- | ----------- | ----------- | ----- |
| **authorization**   | **String**                            |             | \[required] |       |
| **name**            | **String**                            |             | \[required] |       |
| **erc721\_request** | [**Erc721Request**](erc721request.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](../../rust/docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## get\_approved

> crate::models::TransactionApiResponse get\_approved(authorization, name, erc721\_request)

### Parameters

| Name                | Type                                  | Description | Required    | Notes |
| ------------------- | ------------------------------------- | ----------- | ----------- | ----- |
| **authorization**   | **String**                            |             | \[required] |       |
| **name**            | **String**                            |             | \[required] |       |
| **erc721\_request** | [**Erc721Request**](erc721request.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](../../rust/docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## is\_approved\_for\_all

> crate::models::TransactionApiResponse is\_approved\_for\_all(authorization, name, erc721\_request)

### Parameters

| Name                | Type                                  | Description | Required    | Notes |
| ------------------- | ------------------------------------- | ----------- | ----------- | ----- |
| **authorization**   | **String**                            |             | \[required] |       |
| **name**            | **String**                            |             | \[required] |       |
| **erc721\_request** | [**Erc721Request**](erc721request.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](../../rust/docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## name

> crate::models::TransactionApiResponse name(authorization, name, erc721\_request)

### Parameters

| Name                | Type                                  | Description | Required    | Notes |
| ------------------- | ------------------------------------- | ----------- | ----------- | ----- |
| **authorization**   | **String**                            |             | \[required] |       |
| **name**            | **String**                            |             | \[required] |       |
| **erc721\_request** | [**Erc721Request**](erc721request.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](../../rust/docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## owner\_of

> crate::models::TransactionApiResponse owner\_of(authorization, name, erc721\_request)

### Parameters

| Name                | Type                                  | Description | Required    | Notes |
| ------------------- | ------------------------------------- | ----------- | ----------- | ----- |
| **authorization**   | **String**                            |             | \[required] |       |
| **name**            | **String**                            |             | \[required] |       |
| **erc721\_request** | [**Erc721Request**](erc721request.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](../../rust/docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## safe\_transfer\_from

> crate::models::TransactionApiResponse safe\_transfer\_from(authorization, name, erc721\_request)

### Parameters

| Name                | Type                                  | Description | Required    | Notes |
| ------------------- | ------------------------------------- | ----------- | ----------- | ----- |
| **authorization**   | **String**                            |             | \[required] |       |
| **name**            | **String**                            |             | \[required] |       |
| **erc721\_request** | [**Erc721Request**](erc721request.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](../../rust/docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## set\_approval\_for\_all

> crate::models::TransactionApiResponse set\_approval\_for\_all(authorization, name, erc721\_request)

### Parameters

| Name                | Type                                  | Description | Required    | Notes |
| ------------------- | ------------------------------------- | ----------- | ----------- | ----- |
| **authorization**   | **String**                            |             | \[required] |       |
| **name**            | **String**                            |             | \[required] |       |
| **erc721\_request** | [**Erc721Request**](erc721request.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](../../rust/docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## symbol

> crate::models::TransactionApiResponse symbol(authorization, name, erc721\_request)

### Parameters

| Name                | Type                                  | Description | Required    | Notes |
| ------------------- | ------------------------------------- | ----------- | ----------- | ----- |
| **authorization**   | **String**                            |             | \[required] |       |
| **name**            | **String**                            |             | \[required] |       |
| **erc721\_request** | [**Erc721Request**](erc721request.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](../../rust/docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## token\_uri

> crate::models::TransactionApiResponse token\_uri(authorization, name, erc721\_request)

### Parameters

| Name                | Type                                  | Description | Required    | Notes |
| ------------------- | ------------------------------------- | ----------- | ----------- | ----- |
| **authorization**   | **String**                            |             | \[required] |       |
| **name**            | **String**                            |             | \[required] |       |
| **erc721\_request** | [**Erc721Request**](erc721request.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](../../rust/docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## transfer

> crate::models::TransactionApiResponse transfer(authorization, name, erc721\_request)

### Parameters

| Name                | Type                                  | Description | Required    | Notes |
| ------------------- | ------------------------------------- | ----------- | ----------- | ----- |
| **authorization**   | **String**                            |             | \[required] |       |
| **name**            | **String**                            |             | \[required] |       |
| **erc721\_request** | [**Erc721Request**](erc721request.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](../../rust/docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## transfer\_from

> crate::models::TransactionApiResponse transfer\_from(authorization, name, erc721\_request)

### Parameters

| Name                | Type                                  | Description | Required    | Notes |
| ------------------- | ------------------------------------- | ----------- | ----------- | ----- |
| **authorization**   | **String**                            |             | \[required] |       |
| **name**            | **String**                            |             | \[required] |       |
| **erc721\_request** | [**Erc721Request**](erc721request.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](../../rust/docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
