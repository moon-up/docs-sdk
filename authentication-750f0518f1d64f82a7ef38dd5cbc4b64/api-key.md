# API Key

Sure, here's a revised version of the documentation page that uses the term "API tokens" instead of "X-API-Key/API tokens":

## API Token Authentication

Moon supports the use of API tokens for authentication in API requests. This allows developers to secure their requests to the Moon API using a token, rather than using OAuth2 authentication.

### Using API Tokens

To use API tokens for authentication, follow these steps:

1. Obtain an API token from the Moon dashboard.
2. Include the `X-API-Key` header in your API requests, with the value set to your API token.

Here's an example of how to include the `X-API-Key` header in an API request using the `fetch` API:

```javascript
const apiToken = 'YOUR_API_TOKEN';

async function getAccounts() {
  try {
    const response = await fetch('https://beta.usemoon.ai/api/v1/accounts', {
      headers: {
        'X-API-Key': apiToken,
      },
    });
    const data = await response.json();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

getAccounts();
```

In this example, the `fetch` method is used to send a GET request to the Moon API's `/api/v1/accounts` endpoint. The `headers` option is used to include the `X-API-Key` header in the request, with the value set to the API token obtained from the Moon dashboard.

### Using API Tokens with the `@moonup/moon-api` Package

The `@moonup/moon-api` package also supports the use of API tokens for authentication. To use API tokens with the `@moonup/moon-api` package, configure the `securityWorker` function in the `ApiConfig` object to include the `X-API-Key` header in the request.

Here's an example of how to configure the `securityWorker` function to include the `X-API-Key` header in an API request using the `@moonup/moon-api` package:

```javascript
import { Accounts, ApiConfig, ContentType, HttpClient } from '@moonup/moon-api';

const baseApiParams: ApiConfig = {
  baseUrl: 'https://beta.usemoon.ai',
  baseApiParams: {
    secure: true,
    type: ContentType.Json,
    format: 'json',
  },
  securityWorker: async (securityData) => {
    return Promise.resolve({
      headers: {
        'X-API-Key': securityData.token,
      },
    });
  },
};

const http = new HttpClient(baseApiParams);
const accountsSDK = new Accounts(http);

async function listAccounts() {
  const response = await accountsSDK.listAccounts();
  console.log(response.data);
}

listAccounts();
```

In this example, the `securityWorker` function is configured to include the `X-API-Key` header in the request, with the value set to the API token obtained from the Moon dashboard. The `Accounts` SDK is then used to send a request to the Moon API's `/api/v1/accounts` endpoint, which is authenticated using the `X-API-Key` header.

### Security Considerations

When using API tokens for authentication, it's important to ensure that your API token is kept secure. Never expose your API token in client-side code or include it in version control systems. Instead, store your API token in a secure environment variable or configuration file.

### Conclusion

The use of API tokens for authentication is a convenient way to secure API requests to the Moon API. By including the `X-API-Key` header in your requests, you can easily authenticate your requests using a token. Whether you're using the `@moonup/moon-api` package or making requests using a library like `fetch`, the process is similar. Just remember to keep your API token secure and be aware of the rate limits imposed by Moon.
