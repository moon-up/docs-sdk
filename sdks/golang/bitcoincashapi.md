# \BitcoincashAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method                         | HTTP request                                | Description |
| ------------------------------ | ------------------------------------------- | ----------- |
| **CreateBitcoinCashAccount**   | **Post** /bitcoincash                       |             |
| **GetBitcoinCashAccount**      | **Get** /bitcoincash/{accountName}          |             |
| **ListBitcoinCashAccounts**    | **Get** /bitcoincash                        |             |
| **SignBitcoinCashTransaction** | **Post** /bitcoincash/{accountName}/sign-tx |             |

## CreateBitcoinCashAccount

> AccountAPIResponse CreateBitcoinCashAccount(ctx).Authorization(authorization).BitcoinCashInput(bitcoinCashInput).Execute()

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
	bitcoinCashInput := *openapiclient.NewBitcoinCashInput() // BitcoinCashInput | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BitcoincashAPI.CreateBitcoinCashAccount(context.Background()).Authorization(authorization).BitcoinCashInput(bitcoinCashInput).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BitcoincashAPI.CreateBitcoinCashAccount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateBitcoinCashAccount`: AccountAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `BitcoincashAPI.CreateBitcoinCashAccount`: %v\n", resp)
}
```

### Path Parameters

### Other Parameters

Other parameters are passed through a pointer to a apiCreateBitcoinCashAccountRequest struct via the builder pattern

| Name                 | Type                 | Description | Notes |
| -------------------- | -------------------- | ----------- | ----- |
| **authorization**    | **string**           |             |       |
| **bitcoinCashInput** | **BitcoinCashInput** |             |       |

### Return type

**AccountAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## GetBitcoinCashAccount

> AccountAPIResponse GetBitcoinCashAccount(ctx, accountName).Authorization(authorization).Execute()

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
	resp, r, err := apiClient.BitcoincashAPI.GetBitcoinCashAccount(context.Background(), accountName).Authorization(authorization).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BitcoincashAPI.GetBitcoinCashAccount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetBitcoinCashAccount`: AccountAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `BitcoincashAPI.GetBitcoinCashAccount`: %v\n", resp)
}
```

### Path Parameters

| Name            | Type                | Description                                                                 | Notes |
| --------------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**         | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **accountName** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiGetBitcoinCashAccountRequest struct via the builder pattern

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

## ListBitcoinCashAccounts

> AccountAPIResponse ListBitcoinCashAccounts(ctx).Authorization(authorization).Execute()

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
	resp, r, err := apiClient.BitcoincashAPI.ListBitcoinCashAccounts(context.Background()).Authorization(authorization).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BitcoincashAPI.ListBitcoinCashAccounts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListBitcoinCashAccounts`: AccountAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `BitcoincashAPI.ListBitcoinCashAccounts`: %v\n", resp)
}
```

### Path Parameters

### Other Parameters

Other parameters are passed through a pointer to a apiListBitcoinCashAccountsRequest struct via the builder pattern

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

## SignBitcoinCashTransaction

> BitcoinCashAPIResponse SignBitcoinCashTransaction(ctx, accountName).Authorization(authorization).BitcoinCashTransactionInput(bitcoinCashTransactionInput).Execute()

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
	bitcoinCashTransactionInput := *openapiclient.NewBitcoinCashTransactionInput() // BitcoinCashTransactionInput | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BitcoincashAPI.SignBitcoinCashTransaction(context.Background(), accountName).Authorization(authorization).BitcoinCashTransactionInput(bitcoinCashTransactionInput).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BitcoincashAPI.SignBitcoinCashTransaction``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SignBitcoinCashTransaction`: BitcoinCashAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `BitcoincashAPI.SignBitcoinCashTransaction`: %v\n", resp)
}
```

### Path Parameters

| Name            | Type                | Description                                                                 | Notes |
| --------------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**         | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **accountName** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiSignBitcoinCashTransactionRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**bitcoinCashTransactionInput** | **BitcoinCashTransactionInput** | |

### Return type

**BitcoinCashAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
