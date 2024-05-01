# \EnsApi

All URIs are relative to _https://beta.usemoon.ai_

| Method                           | HTTP request          | Description |
| -------------------------------- | --------------------- | ----------- |
| [**resolve**](EnsApi.md#resolve) | **POST** /ens/resolve |             |

## resolve

> crate::models::EnsResolveApiResponse resolve(authorization, ens\_resolve\_input)

### Parameters

| Name                    | Type                                      | Description | Required    | Notes |
| ----------------------- | ----------------------------------------- | ----------- | ----------- | ----- |
| **authorization**       | **String**                                |             | \[required] |       |
| **ens\_resolve\_input** | [**EnsResolveInput**](EnsResolveInput.md) |             | \[required] |       |

### Return type

[**crate::models::EnsResolveApiResponse**](docs/EnsResolveAPIResponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](EnsApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
