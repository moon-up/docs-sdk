# \BitcoinAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method                     | HTTP request                            | Description |
| -------------------------- | --------------------------------------- | ----------- |
| **CreateBitcoinAccount**   | **Post** /bitcoin                       |             |
| **GetBitcoinAccount**      | **Get** /bitcoin/{accountName}          |             |
| **ListBitcoinAccounts**    | **Get** /bitcoin                        |             |
| **SignBitcoinTransaction** | **Post** /bitcoin/{accountName}/sign-tx |             |

## CreateBitcoinAccount

> AccountAPIResponse CreateBitcoinAccount(ctx).Authorization(authorization).BitcoinInput(bitcoinInput).Execute()

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
	bitcoinInput := *openapiclient.NewBitcoinInput() // BitcoinInput | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BitcoinAPI.CreateBitcoinAccount(context.Background()).Authorization(authorization).BitcoinInput(bitcoinInput).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BitcoinAPI.CreateBitcoinAccount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateBitcoinAccount`: AccountAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `BitcoinAPI.CreateBitcoinAccount`: %v\n", resp)
}
```

### Path Parameters

### Other Parameters

Other parameters are passed through a pointer to a apiCreateBitcoinAccountRequest struct via the builder pattern

| Name              | Type             | Description | Notes |
| ----------------- | ---------------- | ----------- | ----- |
| **authorization** | **string**       |             |       |
| **bitcoinInput**  | **BitcoinInput** |             |       |

### Return type

**AccountAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## GetBitcoinAccount

> AccountAPIResponse GetBitcoinAccount(ctx, accountName).Authorization(authorization).Execute()

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
	resp, r, err := apiClient.BitcoinAPI.GetBitcoinAccount(context.Background(), accountName).Authorization(authorization).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BitcoinAPI.GetBitcoinAccount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetBitcoinAccount`: AccountAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `BitcoinAPI.GetBitcoinAccount`: %v\n", resp)
}
```

### Path Parameters

| Name            | Type                | Description                                                                 | Notes |
| --------------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**         | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **accountName** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiGetBitcoinAccountRequest struct via the builder pattern

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

## ListBitcoinAccounts

> AccountAPIResponse ListBitcoinAccounts(ctx).Authorization(authorization).Execute()

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
	resp, r, err := apiClient.BitcoinAPI.ListBitcoinAccounts(context.Background()).Authorization(authorization).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BitcoinAPI.ListBitcoinAccounts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListBitcoinAccounts`: AccountAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `BitcoinAPI.ListBitcoinAccounts`: %v\n", resp)
}
```

### Path Parameters

### Other Parameters

Other parameters are passed through a pointer to a apiListBitcoinAccountsRequest struct via the builder pattern

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

## SignBitcoinTransaction

> BitcoinAPIResponse SignBitcoinTransaction(ctx, accountName).Authorization(authorization).BitcoinTransactionInput(bitcoinTransactionInput).Execute()

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
	bitcoinTransactionInput := *openapiclient.NewBitcoinTransactionInput() // BitcoinTransactionInput | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BitcoinAPI.SignBitcoinTransaction(context.Background(), accountName).Authorization(authorization).BitcoinTransactionInput(bitcoinTransactionInput).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BitcoinAPI.SignBitcoinTransaction``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SignBitcoinTransaction`: BitcoinAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `BitcoinAPI.SignBitcoinTransaction`: %v\n", resp)
}
```

### Path Parameters

| Name            | Type                | Description                                                                 | Notes |
| --------------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**         | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **accountName** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiSignBitcoinTransactionRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**bitcoinTransactionInput** | **BitcoinTransactionInput** | |

### Return type

**BitcoinAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
