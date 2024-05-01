# \ENSAPI

All URIs are relative to _https://beta.usemoon.ai_

| Method                           | HTTP request          | Description |
| -------------------------------- | --------------------- | ----------- |
| [**Resolve**](ensapi.md#Resolve) | **Post** /ens/resolve |             |

## Resolve

> EnsResolveAPIResponse Resolve(ctx).Authorization(authorization).EnsResolveInput(ensResolveInput).Execute()

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
	ensResolveInput := *openapiclient.NewEnsResolveInput("Domain_example", "ChainId_example") // EnsResolveInput | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ENSAPI.Resolve(context.Background()).Authorization(authorization).EnsResolveInput(ensResolveInput).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ENSAPI.Resolve``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `Resolve`: EnsResolveAPIResponse
	fmt.Fprintf(os.Stdout, "Response from `ENSAPI.Resolve`: %v\n", resp)
}
```

### Path Parameters

### Other Parameters

Other parameters are passed through a pointer to a apiResolveRequest struct via the builder pattern

| Name                | Type                                      | Description | Notes |
| ------------------- | ----------------------------------------- | ----------- | ----- |
| **authorization**   | **string**                                |             |       |
| **ensResolveInput** | [**EnsResolveInput**](ensresolveinput.md) |             |       |

### Return type

[**EnsResolveAPIResponse**](ensresolveapiresponse.md)

### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](ensapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)