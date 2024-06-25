# Yearn

The `Yearn` class from `@moonup/moon-api` provides a convenient way to interact with the Yearn Finance protocol. This API allows you to perform various operations related to adding liquidity, removing liquidity, and managing your Yearn vaults.

Here's a detailed documentation for the `Yearn` class:

### Initialization

To use the `Yearn` class, you need to create an instance of it with a configured `HttpClient`. The `HttpClient` is responsible for making HTTP requests to the Yearn API.

Here's an example of how to create an instance of the `Yearn` class:

```javascript
import { HttpClient } from '@moonup/moon-api';
import { Yearn } from '@moonup/moon-api';

const http = new HttpClient({
  baseUrl: 'https://beta.usemoon.ai',
  securityWorker: async (securityData) => {
    return {
      headers: {
        Authorization: `Bearer ${securityData.token}`,
      },
    };
  },
});

const yearn = new Yearn(http);
```

### Class: Yearn

#### Methods

**`addLiquidity(name: string, data: InputBody, params?: RequestParams)`**

This method is used to add liquidity to a Yearn vault.

* **Parameters:**
  * `name`: The name of the Yearn vault.
  * `data`: An object containing the input data for adding liquidity.
  * `params`: Optional request parameters.
* **Returns:** A promise that resolves to the result of the liquidity addition.
*   **Example:**

    ```javascript
    const name = 'myYearnVault';
    const data = {
      value: '1000000000000000000', // 1 ETH
      // Other input data
    };

    try {
      const response = await yearn.addLiquidity(name, data);
      console.log(response);
    } catch (error) {
      console.error(error);
    }
    ```

**`addLiquidityWeth(name: string, data: InputBody, params?: RequestParams)`**

This method is used to add WETH liquidity to a Yearn vault.

* **Parameters:**
  * `name`: The name of the Yearn vault.
  * `data`: An object containing the input data for adding WETH liquidity.
  * `params`: Optional request parameters.
* **Returns:** A promise that resolves to the data of the WETH liquidity addition.
*   **Example:**

    ```javascript
    const name = 'myYearnVault';
    const data = {
      value: '1000000000000000000', // 1 WETH
      // Other input data
    };

    try {
      const response = await yearn.addLiquidityWeth(name, data);
      console.log(response);
    } catch (error) {
      console.error(error);
    }
    ```

**`removeLiquidity(name: string, data: InputBody, params?: RequestParams)`**

This method is used to remove liquidity from a Yearn vault.

* **Parameters:**
  * `name`: The name of the Yearn vault.
  * `data`: An object containing the input data for removing liquidity.
  * `params`: Optional request parameters.
* **Returns:** A promise that resolves to the result of the liquidity removal.
*   **Example:**

    ```javascript
    const name = 'myYearnVault';
    const data = {
      amount: '1000000000000000000', // 1 LP token
      // Other input data
    };

    try {
      const response = await yearn.removeLiquidity(name, data);
      console.log(response);
    } catch (error) {
      console.error(error);
    }
    ```

**`removeLiquidityWeth(name: string, data: InputBody, params?: RequestParams)`**

This method is used to remove WETH liquidity from a Yearn vault.

* **Parameters:**
  * `name`: The name of the Yearn vault.
  * `data`: An object containing the input data for removing WETH liquidity.
  * `params`: Optional request parameters.
* **Returns:** A promise that resolves to the data of the WETH liquidity removal.
*   **Example:**

    ```javascript
    const name = 'myYearnVault';
    const data = {
      amount: '1000000000000000000', // 1 WETH
      // Other input data
    };

    try {
      const response = await yearn.removeLiquidityWeth(name, data);
      console.log(response);
    } catch (error) {
      console.error(error);
    }
    ```

#### Usage

To use the `Yearn` class, you need to create an instance of it with a configured `HttpClient`. The `HttpClient` is responsible for making HTTP requests to the Yearn API.

You can then use the `yearn` instance to call the various methods of the `Yearn` class. Make sure to handle any potential errors that may occur during the API calls using `try-catch` blocks.
