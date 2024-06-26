# \RippleAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method                    | HTTP request                           | Description |
| ------------------------- | -------------------------------------- | ----------- |
| **CreateRippleAccount**   | **Post** /ripple                       |             |
| **GetRippleAccount**      | **Get** /ripple/{accountName}          |             |
| **ListRippleAccounts**    | **Get** /ripple                        |             |
| **SignRippleTransaction** | **Post** /ripple/{accountName}/sign-tx |             |

## CreateRippleAccount

> AccountAPIResponse CreateRippleAccount(ctx).Authorization(authorization).RippleInput(rippleInput).Execute()

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
	rippleInput := *openapiclient.NewRippleInput() // RippleInput | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RippleAPI.CreateRippleAccount(context.Background()).Authorization(authorization).RippleInput(rippleInput).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RippleAPI.CreateRippleAccount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateRippleAccount`: AccountAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `RippleAPI.CreateRippleAccount`: %v\n", resp)
}
```

### Path Parameters

### Other Parameters

Other parameters are passed through a pointer to a apiCreateRippleAccountRequest struct via the builder pattern

| Name              | Type            | Description | Notes |
| ----------------- | --------------- | ----------- | ----- |
| **authorization** | **string**      |             |       |
| **rippleInput**   | **RippleInput** |             |       |

### Return type

**AccountAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## GetRippleAccount

> AccountAPIResponse GetRippleAccount(ctx, accountName).Authorization(authorization).Execute()

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
	resp, r, err := apiClient.RippleAPI.GetRippleAccount(context.Background(), accountName).Authorization(authorization).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RippleAPI.GetRippleAccount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetRippleAccount`: AccountAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `RippleAPI.GetRippleAccount`: %v\n", resp)
}
```

### Path Parameters

| Name            | Type                | Description                                                                 | Notes |
| --------------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**         | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **accountName** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiGetRippleAccountRequest struct via the builder pattern

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

## ListRippleAccounts

> AccountAPIResponse ListRippleAccounts(ctx).Authorization(authorization).Execute()

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
	resp, r, err := apiClient.RippleAPI.ListRippleAccounts(context.Background()).Authorization(authorization).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RippleAPI.ListRippleAccounts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListRippleAccounts`: AccountAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `RippleAPI.ListRippleAccounts`: %v\n", resp)
}
```

### Path Parameters

### Other Parameters

Other parameters are passed through a pointer to a apiListRippleAccountsRequest struct via the builder pattern

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

## SignRippleTransaction

> RippleAPIResponse SignRippleTransaction(ctx, accountName).Authorization(authorization).RippleTransactionInput(rippleTransactionInput).Execute()

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
	rippleTransactionInput := *openapiclient.NewRippleTransactionInput() // RippleTransactionInput | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RippleAPI.SignRippleTransaction(context.Background(), accountName).Authorization(authorization).RippleTransactionInput(rippleTransactionInput).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RippleAPI.SignRippleTransaction``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SignRippleTransaction`: RippleAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `RippleAPI.SignRippleTransaction`: %v\n", resp)
}
```

### Path Parameters

| Name            | Type                | Description                                                                 | Notes |
| --------------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**         | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **accountName** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiSignRippleTransactionRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**rippleTransactionInput** | **RippleTransactionInput** | |

### Return type

**RippleAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
