# \Erc721API

All URIs are relative to _https://beta.usemoon.ai_

| Method                | HTTP request                                 | Description |
| --------------------- | -------------------------------------------- | ----------- |
| **Approve**           | **Post** /erc721/{name}/approve              |             |
| **BalanceOf**         | **Post** /erc721/{name}/balance-of           |             |
| **GetApproved**       | **Post** /erc721/{name}/get-approved         |             |
| **IsApprovedForAll**  | **Post** /erc721/{name}/is-approved-for-all  |             |
| **Name**              | **Post** /erc721/{name}/name                 |             |
| **OwnerOf**           | **Post** /erc721/{name}/owner-of             |             |
| **SafeTransferFrom**  | **Post** /erc721/{name}/safe-transfer-from   |             |
| **SetApprovalForAll** | **Post** /erc721/{name}/set-approval-for-all |             |
| **Symbol**            | **Post** /erc721/{name}/symbol               |             |
| **TokenUri**          | **Post** /erc721/{name}/token-uri            |             |
| **Transfer**          | **Post** /erc721/{name}/transfer             |             |
| **TransferFrom**      | **Post** /erc721/{name}/transfer-from        |             |

## Approve

> TransactionAPIResponse Approve(ctx, name).Authorization(authorization).Erc721Request(erc721Request).Execute()

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
	name := "name_example" // string | 
	erc721Request := *openapiclient.NewErc721Request() // Erc721Request | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.Erc721API.Approve(context.Background(), name).Authorization(authorization).Erc721Request(erc721Request).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `Erc721API.Approve``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `Approve`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `Erc721API.Approve`: %v\n", resp)
}
```

### Path Parameters

| Name     | Type                | Description                                                                 | Notes |
| -------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**  | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **name** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiApproveRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**erc721Request** | **Erc721Request** | |

### Return type

**TransactionAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## BalanceOf

> TransactionAPIResponse BalanceOf(ctx, name).Authorization(authorization).Erc721Request(erc721Request).Execute()

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
	name := "name_example" // string | 
	erc721Request := *openapiclient.NewErc721Request() // Erc721Request | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.Erc721API.BalanceOf(context.Background(), name).Authorization(authorization).Erc721Request(erc721Request).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `Erc721API.BalanceOf``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BalanceOf`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `Erc721API.BalanceOf`: %v\n", resp)
}
```

### Path Parameters

| Name     | Type                | Description                                                                 | Notes |
| -------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**  | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **name** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiBalanceOfRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**erc721Request** | **Erc721Request** | |

### Return type

**TransactionAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## GetApproved

> TransactionAPIResponse GetApproved(ctx, name).Authorization(authorization).Erc721Request(erc721Request).Execute()

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
	name := "name_example" // string | 
	erc721Request := *openapiclient.NewErc721Request() // Erc721Request | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.Erc721API.GetApproved(context.Background(), name).Authorization(authorization).Erc721Request(erc721Request).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `Erc721API.GetApproved``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetApproved`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `Erc721API.GetApproved`: %v\n", resp)
}
```

### Path Parameters

| Name     | Type                | Description                                                                 | Notes |
| -------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**  | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **name** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiGetApprovedRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**erc721Request** | **Erc721Request** | |

### Return type

**TransactionAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## IsApprovedForAll

> TransactionAPIResponse IsApprovedForAll(ctx, name).Authorization(authorization).Erc721Request(erc721Request).Execute()

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
	name := "name_example" // string | 
	erc721Request := *openapiclient.NewErc721Request() // Erc721Request | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.Erc721API.IsApprovedForAll(context.Background(), name).Authorization(authorization).Erc721Request(erc721Request).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `Erc721API.IsApprovedForAll``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `IsApprovedForAll`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `Erc721API.IsApprovedForAll`: %v\n", resp)
}
```

### Path Parameters

| Name     | Type                | Description                                                                 | Notes |
| -------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**  | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **name** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiIsApprovedForAllRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**erc721Request** | **Erc721Request** | |

### Return type

**TransactionAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## Name

> TransactionAPIResponse Name(ctx, name).Authorization(authorization).Erc721Request(erc721Request).Execute()

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
	name := "name_example" // string | 
	erc721Request := *openapiclient.NewErc721Request() // Erc721Request | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.Erc721API.Name(context.Background(), name).Authorization(authorization).Erc721Request(erc721Request).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `Erc721API.Name``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `Name`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `Erc721API.Name`: %v\n", resp)
}
```

### Path Parameters

| Name     | Type                | Description                                                                 | Notes |
| -------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**  | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **name** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiNameRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**erc721Request** | **Erc721Request** | |

### Return type

**TransactionAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## OwnerOf

> TransactionAPIResponse OwnerOf(ctx, name).Authorization(authorization).Erc721Request(erc721Request).Execute()

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
	name := "name_example" // string | 
	erc721Request := *openapiclient.NewErc721Request() // Erc721Request | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.Erc721API.OwnerOf(context.Background(), name).Authorization(authorization).Erc721Request(erc721Request).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `Erc721API.OwnerOf``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `OwnerOf`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `Erc721API.OwnerOf`: %v\n", resp)
}
```

### Path Parameters

| Name     | Type                | Description                                                                 | Notes |
| -------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**  | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **name** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiOwnerOfRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**erc721Request** | **Erc721Request** | |

### Return type

**TransactionAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## SafeTransferFrom

> TransactionAPIResponse SafeTransferFrom(ctx, name).Authorization(authorization).Erc721Request(erc721Request).Execute()

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
	name := "name_example" // string | 
	erc721Request := *openapiclient.NewErc721Request() // Erc721Request | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.Erc721API.SafeTransferFrom(context.Background(), name).Authorization(authorization).Erc721Request(erc721Request).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `Erc721API.SafeTransferFrom``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SafeTransferFrom`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `Erc721API.SafeTransferFrom`: %v\n", resp)
}
```

### Path Parameters

| Name     | Type                | Description                                                                 | Notes |
| -------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**  | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **name** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiSafeTransferFromRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**erc721Request** | **Erc721Request** | |

### Return type

**TransactionAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## SetApprovalForAll

> TransactionAPIResponse SetApprovalForAll(ctx, name).Authorization(authorization).Erc721Request(erc721Request).Execute()

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
	name := "name_example" // string | 
	erc721Request := *openapiclient.NewErc721Request() // Erc721Request | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.Erc721API.SetApprovalForAll(context.Background(), name).Authorization(authorization).Erc721Request(erc721Request).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `Erc721API.SetApprovalForAll``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SetApprovalForAll`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `Erc721API.SetApprovalForAll`: %v\n", resp)
}
```

### Path Parameters

| Name     | Type                | Description                                                                 | Notes |
| -------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**  | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **name** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiSetApprovalForAllRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**erc721Request** | **Erc721Request** | |

### Return type

**TransactionAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## Symbol

> TransactionAPIResponse Symbol(ctx, name).Authorization(authorization).Erc721Request(erc721Request).Execute()

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
	name := "name_example" // string | 
	erc721Request := *openapiclient.NewErc721Request() // Erc721Request | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.Erc721API.Symbol(context.Background(), name).Authorization(authorization).Erc721Request(erc721Request).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `Erc721API.Symbol``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `Symbol`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `Erc721API.Symbol`: %v\n", resp)
}
```

### Path Parameters

| Name     | Type                | Description                                                                 | Notes |
| -------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**  | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **name** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiSymbolRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**erc721Request** | **Erc721Request** | |

### Return type

**TransactionAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## TokenUri

> TransactionAPIResponse TokenUri(ctx, name).Authorization(authorization).Erc721Request(erc721Request).Execute()

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
	name := "name_example" // string | 
	erc721Request := *openapiclient.NewErc721Request() // Erc721Request | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.Erc721API.TokenUri(context.Background(), name).Authorization(authorization).Erc721Request(erc721Request).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `Erc721API.TokenUri``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TokenUri`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `Erc721API.TokenUri`: %v\n", resp)
}
```

### Path Parameters

| Name     | Type                | Description                                                                 | Notes |
| -------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**  | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **name** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiTokenUriRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**erc721Request** | **Erc721Request** | |

### Return type

**TransactionAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## Transfer

> TransactionAPIResponse Transfer(ctx, name).Authorization(authorization).Erc721Request(erc721Request).Execute()

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
	name := "name_example" // string | 
	erc721Request := *openapiclient.NewErc721Request() // Erc721Request | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.Erc721API.Transfer(context.Background(), name).Authorization(authorization).Erc721Request(erc721Request).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `Erc721API.Transfer``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `Transfer`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `Erc721API.Transfer`: %v\n", resp)
}
```

### Path Parameters

| Name     | Type                | Description                                                                 | Notes |
| -------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**  | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **name** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiTransferRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**erc721Request** | **Erc721Request** | |

### Return type

**TransactionAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]

## TransferFrom

> TransactionAPIResponse TransferFrom(ctx, name).Authorization(authorization).Erc721Request(erc721Request).Execute()

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
	name := "name_example" // string | 
	erc721Request := *openapiclient.NewErc721Request() // Erc721Request | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.Erc721API.TransferFrom(context.Background(), name).Authorization(authorization).Erc721Request(erc721Request).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `Erc721API.TransferFrom``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TransferFrom`: TransactionAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `Erc721API.TransferFrom`: %v\n", resp)
}
```

### Path Parameters

| Name     | Type                | Description                                                                 | Notes |
| -------- | ------------------- | --------------------------------------------------------------------------- | ----- |
| **ctx**  | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc. |       |
| **name** | **string**          |                                                                             |       |

### Other Parameters

Other parameters are passed through a pointer to a apiTransferFromRequest struct via the builder pattern

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **string** |             |       |

**erc721Request** | **Erc721Request** | |

### Return type

**TransactionAPIResponse**

### Authorization

ApiKeyAuth, BearerAuth

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](broken-reference) \[Back to API list] \[Back to Model list] \[Back to README]
