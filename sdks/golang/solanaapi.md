# \SolanaAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method                    | HTTP request                           | Description |
| ------------------------- | -------------------------------------- | ----------- |
| **CreateSolanaAccount**   | **Post** /solana                       |             |
| **GetSolanaAccount**      | **Get** /solana/{accountName}          |             |
| **ListSolanaAccounts**    | **Get** /solana                        |             |
| **SignSolanaTransaction** | **Post** /solana/{accountName}/sign-tx |             |

## CreateSolanaAccount

> AccountAPIResponse CreateSolanaAccount(ctx).Authorization(authorization).SolanaInput(solanaInput).Execute()

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/moon-up/moon-sdk-go"
)

func main() {
	authorization := "authorization_example" // string | 
	solanaInput := *openapiclient.NewSolanaInput() // SolanaInput | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SolanaAPI.CreateSolanaAccount(context.Background()).Authorization(authorization).SolanaInput(solanaInput).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SolanaAPI.CreateSolanaAccount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateSolanaAccount`: AccountAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `SolanaAPI.CreateSolanaAccount`: %v\n", resp)
}
```

### Path Parameters

### Other Parameters

Other parameters are passed through a pointer to a apiCreateSolanaAccountRequest struct via the builder pattern

| Name              | Type            | Description | Notes |
| ----------------- | --------------- | ----------- | ----- |
| **authorization** | **string**      |             |       |
| **solanaInput**   | **SolanaInput** |             |       |

### Return type

**AccountAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## GetSolanaAccount

> AccountAPIResponse GetSolanaAccount(ctx, accountName).Authorization(authorization).Execute()

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/moon-up/moon-sdk-go"
)

func main() {
	authorization := "authorization_example" // string | 
	accountName := "accountName_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SolanaAPI.GetSolanaAccount(context.Background(), accountName).Authorization(authorization).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SolanaAPI.GetSolanaAccount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetSolanaAccount`: AccountAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `SolanaAPI.GetSolanaAccount`: %v\n", resp)
}
```

### Path Parameters

| Name            | Type                | Description                                                                 | Notes |
| --------------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**         | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **accountName** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiGetSolanaAccountRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

### Return type

**AccountAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## ListSolanaAccounts

> AccountAPIResponse ListSolanaAccounts(ctx).Authorization(authorization).Execute()

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/moon-up/moon-sdk-go"
)

func main() {
	authorization := "authorization_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SolanaAPI.ListSolanaAccounts(context.Background()).Authorization(authorization).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SolanaAPI.ListSolanaAccounts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListSolanaAccounts`: AccountAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `SolanaAPI.ListSolanaAccounts`: %v\n", resp)
}
```

### Path Parameters

### Other Parameters

Other parameters are passed through a pointer to a apiListSolanaAccountsRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

### Return type

**AccountAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## SignSolanaTransaction

> SolanaAPIResponse SignSolanaTransaction(ctx, accountName).Authorization(authorization).SolanaTransactionInput(solanaTransactionInput).Execute()

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/moon-up/moon-sdk-go"
)

func main() {
	authorization := "authorization_example" // string | 
	accountName := "accountName_example" // string | 
	solanaTransactionInput := *openapiclient.NewSolanaTransactionInput() // SolanaTransactionInput | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SolanaAPI.SignSolanaTransaction(context.Background(), accountName).Authorization(authorization).SolanaTransactionInput(solanaTransactionInput).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SolanaAPI.SignSolanaTransaction``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SignSolanaTransaction`: SolanaAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `SolanaAPI.SignSolanaTransaction`: %v\n", resp)
}
```

### Path Parameters

| Name            | Type                | Description                                                                 | Notes |
| --------------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**         | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **accountName** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiSignSolanaTransactionRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**solanaTransactionInput** | **SolanaTransactionInput** | |

### Return type

**SolanaAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
