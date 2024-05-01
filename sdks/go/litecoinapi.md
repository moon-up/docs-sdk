# \LitecoinAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                                | HTTP request                             | Description |
| --------------------------------------------------------------------- | ---------------------------------------- | ----------- |
| [**CreateLitecoinAccount**](litecoinapi.md#CreateLitecoinAccount)     | **Post** /litecoin                       |             |
| [**GetLitecoinAccount**](litecoinapi.md#GetLitecoinAccount)           | **Get** /litecoin/{accountName}          |             |
| [**ListLitecoinAccounts**](litecoinapi.md#ListLitecoinAccounts)       | **Get** /litecoin                        |             |
| [**SignLitecoinTransaction**](litecoinapi.md#SignLitecoinTransaction) | **Post** /litecoin/{accountName}/sign-tx |             |

## CreateLitecoinAccount

> AccountAPIResponse CreateLitecoinAccount(ctx).Authorization(authorization).LitecoinInput(litecoinInput).Execute()

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
	litecoinInput := *openapiclient.NewLitecoinInput() // LitecoinInput | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LitecoinAPI.CreateLitecoinAccount(context.Background()).Authorization(authorization).LitecoinInput(litecoinInput).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LitecoinAPI.CreateLitecoinAccount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateLitecoinAccount`: AccountAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `LitecoinAPI.CreateLitecoinAccount`: %v\n", resp)
}
```

### Path Parameters

### Other Parameters

Other parameters are passed through a pointer to a apiCreateLitecoinAccountRequest struct via the builder pattern

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **string**                            |             |       |
| **litecoinInput** | [**LitecoinInput**](litecoininput.md) |             |       |

### Return type

[**AccountAPIResponse**](accountapiresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](litecoinapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## GetLitecoinAccount

> AccountAPIResponse GetLitecoinAccount(ctx, accountName).Authorization(authorization).Execute()

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
	resp, r, err := apiClient.LitecoinAPI.GetLitecoinAccount(context.Background(), accountName).Authorization(authorization).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LitecoinAPI.GetLitecoinAccount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetLitecoinAccount`: AccountAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `LitecoinAPI.GetLitecoinAccount`: %v\n", resp)
}
```

### Path Parameters

| Name            | Type                | Description                                                                 | Notes |
| --------------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**         | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **accountName** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiGetLitecoinAccountRequest struct via the builder pattern

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

[\[Back to top\]](litecoinapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## ListLitecoinAccounts

> AccountAPIResponse ListLitecoinAccounts(ctx).Authorization(authorization).Execute()

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
	resp, r, err := apiClient.LitecoinAPI.ListLitecoinAccounts(context.Background()).Authorization(authorization).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LitecoinAPI.ListLitecoinAccounts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListLitecoinAccounts`: AccountAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `LitecoinAPI.ListLitecoinAccounts`: %v\n", resp)
}
```

### Path Parameters

### Other Parameters

Other parameters are passed through a pointer to a apiListLitecoinAccountsRequest struct via the builder pattern

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

[\[Back to top\]](litecoinapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## SignLitecoinTransaction

> LitecoinAPIResponse SignLitecoinTransaction(ctx, accountName).Authorization(authorization).LitecoinTransactionInput(litecoinTransactionInput).Execute()

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
	litecoinTransactionInput := *openapiclient.NewLitecoinTransactionInput() // LitecoinTransactionInput | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LitecoinAPI.SignLitecoinTransaction(context.Background(), accountName).Authorization(authorization).LitecoinTransactionInput(litecoinTransactionInput).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LitecoinAPI.SignLitecoinTransaction``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SignLitecoinTransaction`: LitecoinAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `LitecoinAPI.SignLitecoinTransaction`: %v\n", resp)
}
```

### Path Parameters

| Name            | Type                | Description                                                                 | Notes |
| --------------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**         | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **accountName** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiSignLitecoinTransactionRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**litecoinTransactionInput** | [**LitecoinTransactionInput**](litecointransactioninput.md) | |

### Return type

[**LitecoinAPIResponse**](litecoinapiresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](litecoinapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)