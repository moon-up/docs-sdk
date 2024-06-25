# Embedded accounts

Moon Supports Embedded Account Endpoint for Seamless Integration with Existing Authentication Solutions

Moon supports an embedded account endpoint that allows users to create sub-accounts and associate wallets with those accounts. This endpoint enables seamless integration with existing authentication solutions, allowing developers to create sub-accounts for their users and associate wallets with those accounts.

Using the Embedded Account Endpoint

To use the embedded account endpoint, send a POST request to the `/client` endpoint of the Moon API. The request should include the following headers and payload:

* Headers:
  * Authorization: A valid API token or OAuth2 access token.
  * Content-Type: application/json
* Payload:
  * name: A unique name for the sub-account.
  * metadata: Optional metadata for the sub-account.

Here's an example of how to use the embedded account endpoint using the `fetch` API:

```javascript
async function createEmbeddedAccount(email, domain, userId) {
  const url = 'https://beta.usemoon.ai/client';
  const headers = {
    'X-API-KEY': 'YOUR_API_TOKEN',
    'Content-Type': 'application/json',
  };
  const body = JSON.stringify({
    name: email,
    metadata: {
      from: domain,
      user: userId,
    },
  });
  const requestOptions = {
    method: 'POST',
    headers: headers,
    body: body,
    redirect: 'follow',
  };

  try {
    const response = await fetch(url, requestOptions);
    const result = await response.text();
    console.log(result);
  } catch (error) {
    console.error(error);
  }
}
createEmbeddedAccount('user@example.com', 'mydomain.com', '1234567890');
```

In this example, the `fetch` API is used to send a POST request to the `/client` endpoint of the Moon API. The request includes the `Authorization` header, which is set to a valid API token or OAuth2 access token. The request also includes the `Content-Type` header, which is set to `application/json`. The payload of the request is a JSON object that includes the `name` and `metadata` properties for the sub-account.

The response from the API will include the details of the newly created sub-account, including its unique ID and the associated wallets.

Benefits of Using the Embedded Account Endpoint

Using the embedded account endpoint provides the following benefits:

* Seamless integration with existing authentication solutions: The embedded account endpoint enables seamless integration with existing authentication solutions, allowing developers to create sub-accounts for their users and associate wallets with those accounts.
* Fine-grained access control: The embedded account endpoint allows for fine-grained access control, enabling developers to restrict access to specific resources or actions for individual sub-accounts.
* Scalability: The embedded account endpoint enables scalability, allowing developers to create and manage multiple sub-accounts for their users as their application grows.

Conclusion

The embedded account endpoint is a powerful feature that enables seamless integration with existing authentication solutions. By using the embedded account endpoint, developers can create sub-accounts for their users and associate wallets with those accounts, providing fine-grained access control and scalability. Whether you're building a new application or integrating Moon into an existing one, the embedded account endpoint is a valuable tool that can help you meet your users' needs.
