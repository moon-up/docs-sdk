# OAuth 2.0

## OAuth2 Authentication in MoonSDK

MoonSDK supports OAuth2 authentication with various providers, allowing users to log in using their existing accounts on these platforms. This documentation page explains how to use the MoonSDK class functions for OAuth2 authentication and provides examples of the process of redirection to code exchange for a session token.

### Available Providers

MoonSDK supports the following OAuth2 providers:

* Discord
* GitHub
* Google
* Twitter

### OAuth2 Authentication Process

The OAuth2 authentication process involves the following steps:

1. Redirect the user to the OAuth2 login page of the provider.
2. The user logs in to their account on the provider's website.
3. The provider redirects the user back to your application with a code.
4. Exchange the code for a session token.

### Example: Discord OAuth2 Authentication

Here's an example of how to use the `performDiscordOAuth` and `performDiscordOauthCodeExchange` functions to authenticate a user with Discord:

1. Redirect the user to the Discord OAuth2 login page:

```javascript
import { MoonSDK } from '@moonup/moon-sdk';

const sdk = new MoonSDK({
  clientId: 'YOUR_CLIENT_ID',
});

sdk.performDiscordOAuth();
```

2. The user logs in to their Discord account and is redirected back to your application with a code in the URL query string.
3. Exchange the code for a session token:

```javascript
const code = new URLSearchParams(window.location.search).get('code');
const token = await sdk.performDiscordOauthCodeExchange(code);
```

The `performDiscordOauthCodeExchange` function sends a request to the Discord API to exchange the code for a session token and returns the token.

### Example: GitHub OAuth2 Authentication

Here's an example of how to use the `performGithubOAuth` and `performGithubOauthCodeExchange` functions to authenticate a user with GitHub:

1. Redirect the user to the GitHub OAuth2 login page:

```javascript
import { MoonSDK } from '@moonup/moon-sdk';

const sdk = new MoonSDK({
  clientId: 'YOUR_CLIENT_ID',
});

sdk.performGithubOAuth();
```

2. The user logs in to their GitHub account and is redirected back to your application with a code in the URL query string.
3. Exchange the code for a session token:

```javascript
const code = new URLSearchParams(window.location.search).get('code');
const token = await sdk.performGithubOauthCodeExchange(code);
```

The `performGithubOauthCodeExchange` function sends a request to the GitHub API to exchange the code for a session token and returns the token.

### Example: Google OAuth2 Authentication

Here's an example of how to use the `performGoogleOAuth` and `performGoogleOauthCodeExchange` functions to authenticate a user with Google:

1. Redirect the user to the Google OAuth2 login page:

```javascript
import { MoonSDK } from '@moonup/moon-sdk';

const sdk = new MoonSDK({
  clientId: 'YOUR_CLIENT_ID',
});

sdk.performGoogleOAuth();
```

2. The user logs in to their Google account and is redirected back to your application with a code in the URL query string.
3. Exchange the code for a session token:

```javascript
const code = new URLSearchParams(window.location.search).get('code');
const token = await sdk.performGoogleOauthCodeExchange(code);
```

The `performGoogleOauthCodeExchange` function sends a request to the Google API to exchange the code for a session token and returns the token.

### Example: Twitter OAuth2 Authentication

Here's an example of how to use the `performTwitterOauth` and `performTwitterOauthCodeExchange` functions to authenticate a user with Twitter:

1. Redirect the user to the Twitter OAuth2 login page:

```javascript
import { MoonSDK } from '@moonup/moon-sdk';

const sdk = new MoonSDK({
  clientId: 'YOUR_CLIENT_ID',
});

sdk.performTwitterOauth();
```

2. The user logs in to their Twitter account and is redirected back to your application with a code in the URL query string.
3. Exchange the code for a session token:

```javascript
const code = new URLSearchParams(window.location.search).get('code');
const token = await sdk.performTwitterOauthCodeExchange(code);
```

The `performTwitterOauthCodeExchange` function sends a request to the Twitter API to exchange the code for a session token and returns the token.

### Conclusion

MoonSDK supports OAuth2 authentication with various providers, allowing users to log in using their existing accounts on these platforms. This documentation page explains how to use the MoonSDK class functions for OAuth2 authentication and provides examples of the process of redirection to code exchange for a session token. Whether you're building a new application or looking to improve the authentication flow of an existing one, MoonSDK's OAuth2 support is a great choice.
