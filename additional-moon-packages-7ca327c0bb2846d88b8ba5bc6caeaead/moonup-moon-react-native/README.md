# @moonup/moon-react-native

## @moonup/moon-react-native Package Documentation

## Getting Started with Moon React Native Package

This guide will help you get started with the `@moonup/moon-react-native` package, which provides a set of tools for interacting with various blockchain networks in a React Native application.

### Table of Contents

* Installation
* Initialization
* Setting up the Context Provider Globally
* Using Expo and TypeScript

### Installation

To install the `@moonup/moon-react-native` package, run the following command in your project directory:

{% tabs %}
{% tab title="npm" %}
```bash
npm install @moonup/moon-react-native
```
{% endtab %}

{% tab title="yarn" %}
```bash
yarn add @moonup/moon-react-native
```
{% endtab %}

{% tab title="pnpm" %}
```bash
pnpm add @moonup/moon-react-native
```
{% endtab %}
{% endtabs %}

### Initialization

Before you can use the package, you need to initialize it in your application. This can be done by creating a new instance of the `MoonSDK` class and passing it to the `MoonContextProvider` component.

Here's an example of how to initialize the package in your `App.tsx` file:

```javascript
import React from 'react';
import { MoonSDK } from '@moonup/moon-sdk';
import { MoonContextProvider } from '@moonup/moon-react-native';

const moon = new MoonSDK({
  apiKey: 'your-api-key',
});

export default function App() {
  return (
    <MoonContextProvider moon={moon}>
      {/* Your app components go here */}
    </MoonContextProvider>
  );
}
```

Replace `'your-api-key'` with your actual API key.

### Setting up the Context Provider Globally

To make the `MoonSDK` instance and other context values available to all components in your application, you can set up the `MoonContextProvider` component at the root level of your application.

Here's an example of how to do this in your `App.tsx` file:

```javascript
import React from 'react';
import { MoonSDK } from '@moonup/moon-sdk';
import { MoonContextProvider } from '@moonup/moon-react-native';
import { NavigationContainer } from '@react-navigation/native';

import MainStackNavigator from './navigators/MainStackNavigator';

const moon = new MoonSDK({
  apiKey: 'your-api-key',
});

export default function App() {
  return (
    <MoonContextProvider moon={moon}>
      <NavigationContainer>
        <MainStackNavigator />
      </NavigationContainer>
    </MoonContextProvider>
  );
}
```

In this example, we've wrapped the `NavigationContainer` and `MainStackNavigator` components with the `MoonContextProvider` component, which makes the `MoonSDK` instance and other context values available to all components in the navigation hierarchy.

Sure, here's an example of how to use the Moon hooks in a subcomponent:

```javascript
import React from 'react';
import { Button, Text } from 'react-native';
import { useSolanaSDK } from '@moonup/moon-react-native';

export default function BalanceDisplay() {
  const solanaSDK = useSolanaSDK();
  const [balance, setBalance] = React.useState(null);

  const handleGetBalance = async () => {
    try {
      const response = await solanaSDK.getBalance('your-solana-address');
      setBalance(response.data.balance);
    } catch (error) {
      console.error(error);
    }
  };

  return (
    <>
      <Button title="Get Balance" onPress={handleGetBalance} />
      {balance && <Text>Balance: {balance}</Text>}
    </>
  );
}
```

In this example, we've created a new `BalanceDisplay` component that uses the `useSolanaSDK` hook to get the balance of a Solana address. The component renders a button that, when pressed, calls the `handleGetBalance` function to retrieve the balance and update the component's state. The component then displays the balance in a `Text` component.

You can use this component in your main component like this:

```javascript
import React from 'react';
import { View } from 'react-native';
import BalanceDisplay from './BalanceDisplay';

export default function App() {
  return (
    <View>
      <BalanceDisplay />
    </View>
  );
}
```

In this example, we've imported the `BalanceDisplay` component and used it in the `App` component's render method. The `BalanceDisplay` component is rendered inside a `View` component, which is a container component provided by React Native.
