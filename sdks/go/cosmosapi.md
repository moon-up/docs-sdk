# \CosmosAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                          | HTTP request                           | Description |
| --------------------------------------------------------------- | -------------------------------------- | ----------- |
| [**CreateCosmosAccount**](cosmosapi.md#CreateCosmosAccount)     | **Post** /cosmos                       |             |
| [**GetCosmosAccount**](cosmosapi.md#GetCosmosAccount)           | **Get** /cosmos/{accountName}          |             |
| [**ListCosmosAccounts**](cosmosapi.md#ListCosmosAccounts)       | **Get** /cosmos                        |             |
| [**SignCosmosTransaction**](cosmosapi.md#SignCosmosTransaction) | **Post** /cosmos/{accountName}/sign-tx |             |

## CreateCosmosAccount

> AccountAPIResponse CreateCosmosAccount(ctx).Authorization(authorization).CosmosInput(cosmosInput).Execute()

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	authorization := "authorization_example" // string | 
	cosmosInput := *openapiclient.NewCosmosInput() // CosmosInput | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CosmosAPI.CreateCosmosAccount(context.Background()).Authorization(authorization).CosmosInput(cosmosInput).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CosmosAPI.CreateCosmosAccount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateCosmosAccount`: AccountAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `CosmosAPI.CreateCosmosAccount`: %v\n", resp)
}
```

### Path Parameters

### Other Parameters

Other parameters are passed through a pointer to a apiCreateCosmosAccountRequest struct via the builder pattern

| Name              | Type                              | Description | Notes |
| ----------------- | --------------------------------- | ----------- | ----- |
| **authorization** | **string**                        |             |       |
| **cosmosInput**   | [**CosmosInput**](cosmosinput.md) |             |       |

### Return type

[**AccountAPIResponse**](accountapiresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](cosmosapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## GetCosmosAccount

> AccountAPIResponse GetCosmosAccount(ctx, accountName).Authorization(authorization).Execute()

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	authorization := "authorization_example" // string | 
	accountName := "accountName_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CosmosAPI.GetCosmosAccount(context.Background(), accountName).Authorization(authorization).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CosmosAPI.GetCosmosAccount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetCosmosAccount`: AccountAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `CosmosAPI.GetCosmosAccount`: %v\n", resp)
}
```

### Path Parameters

| Name            | Type                | Description                                                                 | Notes |
| --------------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**         | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **accountName** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiGetCosmosAccountRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

### Return type

[**AccountAPIResponse**](accountapiresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](cosmosapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## ListCosmosAccounts

> AccountAPIResponse ListCosmosAccounts(ctx).Authorization(authorization).Execute()

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	authorization := "authorization_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CosmosAPI.ListCosmosAccounts(context.Background()).Authorization(authorization).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CosmosAPI.ListCosmosAccounts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCosmosAccounts`: AccountAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `CosmosAPI.ListCosmosAccounts`: %v\n", resp)
}
```

### Path Parameters

### Other Parameters

Other parameters are passed through a pointer to a apiListCosmosAccountsRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

### Return type

[**AccountAPIResponse**](accountapiresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](cosmosapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## SignCosmosTransaction

> CosmosAPIResponse SignCosmosTransaction(ctx, accountName).Authorization(authorization).CosmosTransactionInput(cosmosTransactionInput).Execute()

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	authorization := "authorization_example" // string | 
	accountName := "accountName_example" // string | 
	cosmosTransactionInput := *openapiclient.NewCosmosTransactionInput() // CosmosTransactionInput | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CosmosAPI.SignCosmosTransaction(context.Background(), accountName).Authorization(authorization).CosmosTransactionInput(cosmosTransactionInput).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CosmosAPI.SignCosmosTransaction``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SignCosmosTransaction`: CosmosAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `CosmosAPI.SignCosmosTransaction`: %v\n", resp)
}
```

### Path Parameters

| Name            | Type                | Description                                                                 | Notes |
| --------------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**         | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **accountName** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiSignCosmosTransactionRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**cosmosTransactionInput** | [**CosmosTransactionInput**](cosmostransactioninput.md) | |

### Return type

[**CosmosAPIResponse**](cosmosapiresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](cosmosapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
