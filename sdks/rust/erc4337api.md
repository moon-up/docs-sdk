# \Erc4337Api

All URIs are relative to _https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app_

| Method                                                                           | HTTP request                                             | Description |
| -------------------------------------------------------------------------------- | -------------------------------------------------------- | ----------- |
| [**get\_address**](erc4337api.md#get\_address)                                   | **POST** /erc4337/{accountName}/address                  |             |
| [**sign\_broadcast\_user\_op\_tx**](erc4337api.md#sign\_broadcast\_user\_op\_tx) | **POST** /erc4337/{accountName}/sign-broadcast-userop-tx |             |

## get\_address

> crate::models::AccountApiResponse get\_address(authorization, account\_name, input\_body)

### Parameters

| Name              | Type                          | Description | Required    | Notes |
| ----------------- | ----------------------------- | ----------- | ----------- | ----- |
| **authorization** | **String**                    |             | \[required] |       |
| **account\_name** | **String**                    |             | \[required] |       |
| **input\_body**   | [**InputBody**](inputbody.md) |             | \[required] |       |

### Return type

[**crate::models::AccountApiResponse**](../../rust/docs/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc4337api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## sign\_broadcast\_user\_op\_tx

> crate::models::TransactionApiResponse sign\_broadcast\_user\_op\_tx(authorization, account\_name, input\_body)

### Parameters

| Name              | Type                          | Description | Required    | Notes |
| ----------------- | ----------------------------- | ----------- | ----------- | ----- |
| **authorization** | **String**                    |             | \[required] |       |
| **account\_name** | **String**                    |             | \[required] |       |
| **input\_body**   | [**InputBody**](inputbody.md) |             | \[required] |       |

### Return type

[**crate::models::TransactionApiResponse**](../../rust/docs/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc4337api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
