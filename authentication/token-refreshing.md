# Token Refreshing

## `Token Refreshing`

The `/auth/refresh` endpoint is a POST request that is used to refresh a user's session. This is particularly useful when the user's session has expired and needs to be renewed.

The Moon SDK will automatically refresh the user's session when it expires. This means that you don't have to manually refresh the session in most cases. However, this endpoint is still useful in scenarios where you need to manually control the session refresh.

### Request

The request should include a `refresh_token` in the body. This token is used to authenticate the user and generate a new session.

```json
{
  "refresh_token": "your_refresh_token_here"
}
```

### Response

The response will return the new session data if the request is successful. If there is an error, it will return a 500 status code along with the error message.

### Code Example

Here is an example of how to use this endpoint:

```typescript
import axios from 'axios';

const refreshToken = 'your_refresh_token_here';

axios.post('https://beta.usemoon.ai/auth/refresh', { refresh_token: refreshToken })
  .then(response => {
    console.log(response.data);
  })
  .catch(error => {
    console.error(error);
  });
```

