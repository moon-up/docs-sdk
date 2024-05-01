# \AccountsAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                | HTTP request                                      | Description |
| ----------------------------------------------------- | ------------------------------------------------- | ----------- |
| [**BroadcastTx**](accountsapi.md#BroadcastTx)         | **Post** /accounts/{accountName}/broadcast-tx     |             |
| [**CreateAccount**](accountsapi.md#CreateAccount)     | **Post** /accounts                                |             |
| [**DeleteAccount**](accountsapi.md#DeleteAccount)     | **Delete** /accounts/{accountName}                |             |
| [**DeployContract**](accountsapi.md#DeployContract)   | **Post** /accounts/{accountName}/deploy           |             |
| [**GetAccount**](accountsapi.md#GetAccount)           | **Get** /accounts/{accountName}                   |             |
| [**GetBalance**](accountsapi.md#GetBalance)           | **Get** /accounts/{accountName}/balance           |             |
| [**GetNonce**](accountsapi.md#GetNonce)               | **Get** /accounts/{accountName}/nonce             |             |
| [**ListAccounts**](accountsapi.md#ListAccounts)       | **Get** /accounts                                 |             |
| [**SignMessage**](accountsapi.md#SignMessage)         | **Post** /accounts/{accountName}/sign-message     |             |
| [**SignTransaction**](accountsapi.md#SignTransaction) | **Post** /accounts/{accountName}/sign-transaction |             |
| [**SignTypedData**](accountsapi.md#SignTypedData)     | **Post** /accounts/{accountName}/sign-typed-data  |             |
| [**TransferEth**](accountsapi.md#TransferEth)         | **Post** /accounts/{accountName}/transfer-eth     |             |

## BroadcastTx

> BroadCastRawTransactionAPIResponse BroadcastTx(ctx, accountName).Authorization(authorization).BroadcastInput(broadcastInput).Execute()

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
	broadcastInput := *openapiclient.NewBroadcastInput("ChainId_example", "RawTransaction_example") // BroadcastInput | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AccountsAPI.BroadcastTx(context.Background(), accountName).Authorization(authorization).BroadcastInput(broadcastInput).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AccountsAPI.BroadcastTx``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BroadcastTx`: BroadCastRawTransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `AccountsAPI.BroadcastTx`: %v\n", resp)
}
```

### Path Parameters

| Name            | Type                | Description                                                                 | Notes |
| --------------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**         | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **accountName** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiBroadcastTxRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**broadcastInput** | [**BroadcastInput**](broadcastinput.md) | |

### Return type

[**BroadCastRawTransactionAPIResponse**](broadcastrawtransactionapiresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## CreateAccount

> AccountAPIResponse CreateAccount(ctx).Authorization(authorization).CreateAccountInput(createAccountInput).Execute()

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
	createAccountInput := *openapiclient.NewCreateAccountInput() // CreateAccountInput | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AccountsAPI.CreateAccount(context.Background()).Authorization(authorization).CreateAccountInput(createAccountInput).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AccountsAPI.CreateAccount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateAccount`: AccountAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `AccountsAPI.CreateAccount`: %v\n", resp)
}
```

### Path Parameters

### Other Parameters

Other parameters are passed through a pointer to a apiCreateAccountRequest struct via the builder pattern

| Name                   | Type                                            | Description | Notes |
| ---------------------- | ----------------------------------------------- | ----------- | ----- |
| **authorization**      | **string**                                      |             |       |
| **createAccountInput** | [**CreateAccountInput**](createaccountinput.md) |             |       |

### Return type

[**AccountAPIResponse**](accountapiresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## DeleteAccount

> AccountAPIResponse DeleteAccount(ctx, accountName).Authorization(authorization).Execute()

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
	resp, r, err := apiClient.AccountsAPI.DeleteAccount(context.Background(), accountName).Authorization(authorization).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AccountsAPI.DeleteAccount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteAccount`: AccountAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `AccountsAPI.DeleteAccount`: %v\n", resp)
}
```

### Path Parameters

| Name            | Type                | Description                                                                 | Notes |
| --------------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**         | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **accountName** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteAccountRequest struct via the builder pattern

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

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## DeployContract

> TransactionAPIResponse DeployContract(ctx, accountName).Authorization(authorization).DeployInput(deployInput).Execute()

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
	deployInput := *openapiclient.NewDeployInput("Abi_example", "Bytecode_example") // DeployInput | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AccountsAPI.DeployContract(context.Background(), accountName).Authorization(authorization).DeployInput(deployInput).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AccountsAPI.DeployContract``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeployContract`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `AccountsAPI.DeployContract`: %v\n", resp)
}
```

### Path Parameters

| Name            | Type                | Description                                                                 | Notes |
| --------------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**         | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **accountName** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiDeployContractRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**deployInput** | [**DeployInput**](deployinput.md) | |

### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## GetAccount

> AccountAPIResponse GetAccount(ctx, accountName).Authorization(authorization).Execute()

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
	resp, r, err := apiClient.AccountsAPI.GetAccount(context.Background(), accountName).Authorization(authorization).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AccountsAPI.GetAccount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetAccount`: AccountAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `AccountsAPI.GetAccount`: %v\n", resp)
}
```

### Path Parameters

| Name            | Type                | Description                                                                 | Notes |
| --------------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**         | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **accountName** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiGetAccountRequest struct via the builder pattern

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

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## GetBalance

> BalanceAPIResponse GetBalance(ctx, accountName).Authorization(authorization).ChainId(chainId).Execute()

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
	accountName := "accountName_example" // string | 
	authorization := "authorization_example" // string | 
	chainId := "chainId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AccountsAPI.GetBalance(context.Background(), accountName).Authorization(authorization).ChainId(chainId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AccountsAPI.GetBalance``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetBalance`: BalanceAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `AccountsAPI.GetBalance`: %v\n", resp)
}
```

### Path Parameters

| Name            | Type                | Description                                                                 | Notes |
| --------------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**         | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **accountName** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiGetBalanceRequest struct via the builder pattern

**authorization** | **string** | | **chainId** | **string** | |

### Return type

[**BalanceAPIResponse**](balanceapiresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## GetNonce

> NonceAPIResponse GetNonce(ctx, accountName).Authorization(authorization).Execute()

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
	accountName := "accountName_example" // string | 
	authorization := "authorization_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AccountsAPI.GetNonce(context.Background(), accountName).Authorization(authorization).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AccountsAPI.GetNonce``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetNonce`: NonceAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `AccountsAPI.GetNonce`: %v\n", resp)
}
```

### Path Parameters

| Name            | Type                | Description                                                                 | Notes |
| --------------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**         | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **accountName** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiGetNonceRequest struct via the builder pattern

**authorization** | **string** | |

### Return type

[**NonceAPIResponse**](nonceapiresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## ListAccounts

> AccountAPIResponse ListAccounts(ctx).Authorization(authorization).Execute()

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
	resp, r, err := apiClient.AccountsAPI.ListAccounts(context.Background()).Authorization(authorization).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AccountsAPI.ListAccounts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListAccounts`: AccountAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `AccountsAPI.ListAccounts`: %v\n", resp)
}
```

### Path Parameters

### Other Parameters

Other parameters are passed through a pointer to a apiListAccountsRequest struct via the builder pattern

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

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## SignMessage

> SignMessageAPIResponse SignMessage(ctx, accountName).Authorization(authorization).SignMessage(signMessage).Execute()

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
	accountName := "accountName_example" // string | 
	authorization := "authorization_example" // string | 
	signMessage := *openapiclient.NewSignMessage("Data_example") // SignMessage | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AccountsAPI.SignMessage(context.Background(), accountName).Authorization(authorization).SignMessage(signMessage).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AccountsAPI.SignMessage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SignMessage`: SignMessageAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `AccountsAPI.SignMessage`: %v\n", resp)
}
```

### Path Parameters

| Name            | Type                | Description                                                                 | Notes |
| --------------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**         | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **accountName** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiSignMessageRequest struct via the builder pattern

**authorization** | **string** | | **signMessage** | [**SignMessage**](signmessage.md) | |

### Return type

[**SignMessageAPIResponse**](signmessageapiresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## SignTransaction

> TransactionAPIResponse SignTransaction(ctx, accountName).Authorization(authorization).InputBody(inputBody).Execute()

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
	accountName := "accountName_example" // string | 
	authorization := "authorization_example" // string | 
	inputBody := *openapiclient.NewInputBody() // InputBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AccountsAPI.SignTransaction(context.Background(), accountName).Authorization(authorization).InputBody(inputBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AccountsAPI.SignTransaction``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SignTransaction`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `AccountsAPI.SignTransaction`: %v\n", resp)
}
```

### Path Parameters

| Name            | Type                | Description                                                                 | Notes |
| --------------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**         | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **accountName** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiSignTransactionRequest struct via the builder pattern

**authorization** | **string** | | **inputBody** | [**InputBody**](inputbody.md) | |

### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## SignTypedData

> SignMessageAPIResponse SignTypedData(ctx, accountName).Authorization(authorization).SignTypedData(signTypedData).Execute()

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
	accountName := "accountName_example" // string | 
	authorization := "authorization_example" // string | 
	signTypedData := *openapiclient.NewSignTypedData("Data_example") // SignTypedData | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AccountsAPI.SignTypedData(context.Background(), accountName).Authorization(authorization).SignTypedData(signTypedData).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AccountsAPI.SignTypedData``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SignTypedData`: SignMessageAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `AccountsAPI.SignTypedData`: %v\n", resp)
}
```

### Path Parameters

| Name            | Type                | Description                                                                 | Notes |
| --------------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**         | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **accountName** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiSignTypedDataRequest struct via the builder pattern

**authorization** | **string** | | **signTypedData** | [**SignTypedData**](signtypeddata.md) | |

### Return type

[**SignMessageAPIResponse**](signmessageapiresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## TransferEth

> TransactionAPIResponse TransferEth(ctx, accountName).Authorization(authorization).InputBody(inputBody).Execute()

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
	accountName := "accountName_example" // string | 
	authorization := "authorization_example" // string | 
	inputBody := *openapiclient.NewInputBody() // InputBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AccountsAPI.TransferEth(context.Background(), accountName).Authorization(authorization).InputBody(inputBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AccountsAPI.TransferEth``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TransferEth`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `AccountsAPI.TransferEth`: %v\n", resp)
}
```

### Path Parameters

| Name            | Type                | Description                                                                 | Notes |
| --------------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**         | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **accountName** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiTransferEthRequest struct via the builder pattern

**authorization** | **string** | | **inputBody** | [**InputBody**](inputbody.md) | |

### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
