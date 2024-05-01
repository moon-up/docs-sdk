# \EosAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method                 | HTTP request                        | Description |
| ---------------------- | ----------------------------------- | ----------- |
| **CreateEosAccount**   | **Post** /eos                       |             |
| **GetEosAccount**      | **Get** /eos/{accountName}          |             |
| **ListEosAccounts**    | **Get** /eos                        |             |
| **SignEosTransaction** | **Post** /eos/{accountName}/sign-tx |             |

## CreateEosAccount

> AccountAPIResponse CreateEosAccount(ctx).Authorization(authorization).EosInput(eosInput).Execute()

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
	eosInput := *openapiclient.NewEosInput() // EosInput | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EosAPI.CreateEosAccount(context.Background()).Authorization(authorization).EosInput(eosInput).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EosAPI.CreateEosAccount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateEosAccount`: AccountAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `EosAPI.CreateEosAccount`: %v\n", resp)
}
```

### Path Parameters

### Other Parameters

Other parameters are passed through a pointer to a apiCreateEosAccountRequest struct via the builder pattern

| Name              | Type         | Description | Notes |
| ----------------- | ------------ | ----------- | ----- |
| **authorization** | **string**   |             |       |
| **eosInput**      | **EosInput** |             |       |

### Return type

**AccountAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## GetEosAccount

> AccountAPIResponse GetEosAccount(ctx, accountName).Authorization(authorization).Execute()

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
	resp, r, err := apiClient.EosAPI.GetEosAccount(context.Background(), accountName).Authorization(authorization).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EosAPI.GetEosAccount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetEosAccount`: AccountAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `EosAPI.GetEosAccount`: %v\n", resp)
}
```

### Path Parameters

| Name            | Type                | Description                                                                 | Notes |
| --------------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**         | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **accountName** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiGetEosAccountRequest struct via the builder pattern

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

## ListEosAccounts

> AccountAPIResponse ListEosAccounts(ctx).Authorization(authorization).Execute()

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
	resp, r, err := apiClient.EosAPI.ListEosAccounts(context.Background()).Authorization(authorization).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EosAPI.ListEosAccounts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListEosAccounts`: AccountAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `EosAPI.ListEosAccounts`: %v\n", resp)
}
```

### Path Parameters

### Other Parameters

Other parameters are passed through a pointer to a apiListEosAccountsRequest struct via the builder pattern

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

## SignEosTransaction

> EosAPIResponse SignEosTransaction(ctx, accountName).Authorization(authorization).EosTransactionInput(eosTransactionInput).Execute()

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
	eosTransactionInput := *openapiclient.NewEosTransactionInput() // EosTransactionInput | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EosAPI.SignEosTransaction(context.Background(), accountName).Authorization(authorization).EosTransactionInput(eosTransactionInput).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EosAPI.SignEosTransaction``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SignEosTransaction`: EosAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `EosAPI.SignEosTransaction`: %v\n", resp)
}
```

### Path Parameters

| Name            | Type                | Description                                                                 | Notes |
| --------------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**         | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **accountName** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiSignEosTransactionRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**eosTransactionInput** | **EosTransactionInput** | |

### Return type

**EosAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
