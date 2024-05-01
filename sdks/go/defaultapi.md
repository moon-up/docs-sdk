# \DefaultAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method                                     | HTTP request  | Description |
| ------------------------------------------ | ------------- | ----------- |
| [**GetMessage**](defaultapi.md#GetMessage) | **Get** /ping |             |

## GetMessage

> PingResponse GetMessage(ctx).Execute()

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DefaultAPI.GetMessage(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DefaultAPI.GetMessage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetMessage`: PingResponse
	fmt.Fprintf(os.Stdout, "Response from `DefaultAPI.GetMessage`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetMessageRequest struct via the builder pattern

### Return type

[**PingResponse**](pingresponse.md)

### Authorization

No authorization required

### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](defaultapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
