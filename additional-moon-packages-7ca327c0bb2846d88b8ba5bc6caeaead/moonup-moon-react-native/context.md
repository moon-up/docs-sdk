# Context

## MoonContextProvider Documentation

The `MoonContextProvider` is a React context provider that provides access to the Moon SDK and Ethers.js provider instances, as well as various authentication and session management functions. This documentation page will guide you through the basics of using the `MoonContextProvider` in your React Native project.

### Table of Contents

* Installation
* Usage
* Context Values
* Example

### Installation

To use the `MoonContextProvider` in your project, you'll need to install the `@moonup/moon-react-native` package. You can install it using npm:

```bash
npm install @moonup/moon-react-native
```

### Usage

To use the `MoonContextProvider`, you'll need to wrap your application with it. Here's an example of how to do this:

```javascript
import React from 'react';
import { MoonContextProvider } from '@moonup/moon-react-native';
import App from './App';

export default function Main() {
  return (
    <MoonContextProvider>
      <App />
    </MoonContextProvider>
  );
}
```



### API Reference

#### Context Provider Functions

**`connect(accessToken?: string, refreshToken?: string)`**

Connects to the Moon API using the provided access and refresh tokens.

Example:

```javascript
const handleConnect = async () => {
  try {
    await connect();
  } catch (error) {
    console.error(error);
  }
};
```

**`disconnect()`**

Disconnects from the Moon API.

Example:

```javascript
const handleDisconnect = async () => {
  try {
    await disconnect();
  } catch (error) {
    console.error(error);
  }
};
```

**`getUserSession()`**

Retrieves the current user session.

Example:

```javascript
const handleGetUserSession = async () => {
  try {
    const session = await getUserSession();
    console.log(session);
  } catch (error) {
    console.error(error);
  }
};
```

**`connectEthers()`**

Connects to the Ethers.js provider.

Example:

```javascript
const handleConnectEthers = async () => {
  try {
    await connectEthers();
  } catch (error) {
    console.error(error);
  }
};
```

**`disconnectEthers()`**

Disconnects from the Ethers.js provider.

Example:

```javascript
const handleDisconnectEthers = async () => {
  try {
    await disconnectEthers();
  } catch (error) {
    console.error(error);
  }
};
```

**`request(args: RequestArguments)`**

Sends a request to the Ethers.js provider.

Example:

```javascript
const handleRequest = async () => {
  try {
    const result = await request({ method: 'eth_accounts' });
    console.log(result);
  } catch (error) {
    console.error(error);
  }
};
```

**`signUp(email: string, password: string)`**

Signs up a new user with the provided email and password.

Example:

```javascript
const handleSignUp = async () => {
  try {
    await signUp('test@example.com', 'password');
  } catch (error) {
    console.error(error);
  }
};
```

**`signInWithPassword(email: string, password: string)`**

Signs in a user with the provided email and password.

Example:

```javascript
const handleSignInWithPassword = async () => {
  try {
    await signInWithPassword('test@example.com', 'password');
  } catch (error) {
    console.error(error);
  }
};
```

**`signOut()`**

Signs out the current user.

Example:

```javascript
const handleSignOut = async () => {
  try {
    await signOut();
  } catch (error) {
    console.error(error);
  }
};
```

**`signInWithDiscord()`**

Signs in a user using Discord OAuth.

Example:

```javascript
const handleSignInWithDiscord = async () => {
  try {
    await signInWithDiscord();
  } catch (error) {
    console.error(error);
  }
};
```

**`signInWithGithub()`**

Signs in a user using GitHub OAuth.

Example:

```javascript
const handleSignInWithGithub = async () => {
  try {
    await signInWithGithub();
  } catch (error) {
    console.error(error);
  }
};
```

**`signInWithTwitter()`**

Signs in a user using Twitter OAuth.

Example:

```javascript
const handleSignInWithTwitter = async () => {
  try {
    await signInWithTwitter();
  } catch (error) {
    console.error(error);
  }
};
```

**`signInWithGoogle()`**

Signs in a user using Google OAuth.

Example:

```javascript
const handleSignInWithGoogle = async () => {
  try {
    await signInWithGoogle();
  } catch (error) {
    console.error(error);
  }
};
```

**`sendMagicLink(email: string)`**

Sends a magic link to the provided email address.

Example:

```javascript
const handleSendMagicLink = async () => {
  try {
    await sendMagicLink('test@example.com');
  } catch (error) {
    console.error(error);
  }
};
```

#### Context Provider Variables

**`user`**

The current user object, or `null` if the user is not authenticated.

Example:

```javascript
console.log(user);
```

**`session`**

The current session object, or `null` if the user is not authenticated.

Example:

```javascript
console.log(session);
```

**`initialized`**

A boolean value indicating whether the authentication state has been initialized.

Example:

```javascript
console.log(initialized);
```

**`moon`**

An instance of the Moon SDK.

Example:

```javascript
console.log(moon);
```

**`ethers`**

An instance of the Ethers.js provider.

Example:

```javascript
console.log(ethers);
```

### Example

Here's an example of how to use the `MoonContextProvider` to sign in a user with Discord OAuth:

```javascript
import React from 'react';
import { Button, Text } from 'react-native';
import { useMoon } from '@moonup/moon-react-native';

export default function App() {
  const {
    user,
    session,
    initialized,
    moon,
    ethers,
    connect,
    disconnect,
    getUserSession,
    connectEthers,
    disconnectEthers,
    request,
    signUp,
    signInWithPassword,
    signOut,
    signInWithDiscord,
    signInWithGithub,
    signInWithTwitter,
    signInWithGoogle,
    sendMagicLink,
  } = useMoon();

  const handleSignUp = async () => {
    try {
      await signUp('test@example.com', 'password');
    } catch (error) {
      console.error(error);
    }
  };

  const handleSignInWithPassword = async () => {
    try {
      await signInWithPassword('test@example.com', 'password');
    } catch (error) {
      console.error(error);
    }
  };

  const handleSignOut = async () => {
    try {
      await signOut();
    } catch (error) {
      console.error(error);
    }
  };

  const handleConnect = async () => {
    try {
      await connect();
    } catch (error) {
      console.error(error);
    }
  };

  const handleDisconnect = async () => {
    try {
      await disconnect();
    } catch (error) {
      console.error(error);
    }
  };

  const handleGetUserSession = async () => {
    try {
      const session = await getUserSession();
      console.log(session);
    } catch (error) {
      console.error(error);
    }
  };

  const handleConnectEthers = async () => {
    try {
      await connectEthers();
    } catch (error) {
      console.error(error);
    }
  };

  const handleDisconnectEthers = async () => {
    try {
      await disconnectEthers();
    } catch (error) {
      console.error(error);
    }
  };

  const handleRequest = async () => {
    try {
      const result = await request({ method: 'eth_accounts' });
      console.log(result);
    } catch (error) {
      console.error(error);
    }
  };

  const handleSendMagicLink = async () => {
    try {
      await sendMagicLink('test@example.com');
    } catch (error) {
      console.error(error);
    }
  };

  return (
    <>
      {initialized && (
        <>
          {user ? (
            <>
              <Text>User: {user.email}</Text>
              <Button title="Sign out" onPress={handleSignOut} />
              <Button title="Connect" onPress={handleConnect} />
              <Button title="Disconnect" onPress={handleDisconnect} />
              <Button title="Get user session" onPress={handleGetUserSession} />
              <Button title="Connect Ethers" onPress={handleConnectEthers} />
              <Button title="Disconnect Ethers" onPress={handleDisconnectEthers} />
              <Button title="Request" onPress={handleRequest} />
            </>
          ) : (
            <>
              <Button title="Sign up" onPress={handleSignUp} />
              <Button title="Sign in with password" onPress={handleSignInWithPassword} />
              <Button title="Sign in with Discord" onPress={signInWithDiscord} />
              <Button title="Sign in with GitHub" onPress={signInWithGithub} />
              <Button title="Sign in with Twitter" onPress={signInWithTwitter} />
              <Button title="Sign in with Google" onPress={signInWithGoogle} />
              <Button title="Send magic link" onPress={handleSendMagicLink} />
            </>
          )}
        </>
      )}
    </>
  );
}
```

In this example, we import the `useMoon` hook from the `@moonup/moon-react-native` package and use it to access all of the context provider functions and variables. We then use these functions and variables to handle various authentication and session management tasks, such as signing up a new user, signing in a user with a password, signing out a user, connecting to the Moon API, disconnecting from the Moon API, getting the current user session, connecting to the Ethers.js provider, disconnecting from the Ethers.js provider, sending a request to the Ethers.js provider, and sending a magic link to a user's email address.

In this example, we import the `useMoon` hook from the `@moonup/moon-react-native` package and use it to access the `signInWithDiscord` function. We then use this function to sign in a user with Discord OAuth when the button is pressed.
