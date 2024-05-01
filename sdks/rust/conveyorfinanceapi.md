# \ConveyorFinanceApi

All URIs are relative to _https://beta.usemoon.ai_

| Method                                 | HTTP request                          | Description |
| -------------------------------------- | ------------------------------------- | ----------- |
| [**swap**](conveyorfinanceapi.md#swap) | **POST** /conveyorfinance/{name}/swap |             |

## swap

> crate::models::ConveyorFinanceControllerResponse swap(authorization, name, token\_swap\_params)

### Parameters

| Name                    | Type                                      | Description | Required    | Notes |
| ----------------------- | ----------------------------------------- | ----------- | ----------- | ----- |
| **authorization**       | **String**                                |             | \[required] |       |
| **name**                | **String**                                |             | \[required] |       |
| **token\_swap\_params** | [**TokenSwapParams**](tokenswapparams.md) |             | \[required] |       |

### Return type

[**crate::models::ConveyorFinanceControllerResponse**](conveyorfinancecontrollerresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](conveyorfinanceapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
