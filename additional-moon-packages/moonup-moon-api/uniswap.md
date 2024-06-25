# Uniswap

The `Uniswap` class from `@moonup/moon-api` provides a convenient way to interact with the Uniswap protocol. This API allows you to perform various operations related to adding liquidity, removing liquidity, and swapping tokens on Uniswap.

Here's a detailed documentation for the `Uniswap` class:

### Initialization

To use the `Uniswap` class, you need to create an instance of it with a configured `HttpClient`. The `HttpClient` is responsible for making HTTP requests to the Uniswap API.

Here's an example of how to create an instance of the `Uniswap` class:

```javascript
import { HttpClient } from '@moonup/moon-api';
import { Uniswap } from '@moonup/moon-api';

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

const uniswap = new Uniswap(http);
```

### Class: Uniswap

#### Methods

**`addLiquidity(name: string, data: UniswapInput, params?: RequestParams)`**

This method is used to add liquidity to a Uniswap pool.

* **Parameters:**
  * `name`: The name of the Uniswap pool.
  * `data`: An object containing the input data for adding liquidity.
  * `params`: Optional request parameters.
* **Returns:** A promise that resolves to the data of the liquidity addition.
*   **Example:**

    ```javascript
    const name = 'myUniswapPool';
    const data = {
      token_a: '0x6B175474E89094C44Da98b954EedeAC495271d0F', // DAI
      token_b: '0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2', // WETH
      amount_a: '1000000000000000000', // 1 DAI
      amount_b: '1000000000000000000', // 1 WETH
      // Other input data
    };

    try {
      const response = await uniswap.addLiquidity(name, data);
      console.log(response);
    } catch (error) {
      console.error(error);
    }
    ```

**`removeLiquidity(name: string, data: UniswapInput, params?: RequestParams)`**

This method is used to remove liquidity from a Uniswap pool.

* **Parameters:**
  * `name`: The name of the Uniswap pool.
  * `data`: An object containing the input data for removing liquidity.
  * `params`: Optional request parameters.
* **Returns:** A promise that resolves to the data of the liquidity removal.
*   **Example:**

    ```javascript
    const name = 'myUniswapPool';
    const data = {
      token_a: '0x6B175474E89094C44Da98b954EedeAC495271d0F', // DAI
      token_b: '0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2', // WETH
      liquidity: '1000000000000000000', // 1 LP token
      // Other input data
    };

    try {
      const response = await uniswap.removeLiquidity(name, data);
      console.log(response);
    } catch (error) {
      console.error(error);
    }
    ```

**`swapExactEthForTokens(name: string, data: UniswapInput, params?: RequestParams)`**

This method is used to swap ETH for tokens on Uniswap.

* **Parameters:**
  * `name`: The name of the Uniswap pool.
  * `data`: An object containing the input data for the swap.
  * `params`: Optional request parameters.
* **Returns:** A promise that resolves to the data of the swap.
*   **Example:**

    ```javascript
    const name = 'myUniswapPool';
    const data = {
      token_a: '0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2', // WETH
      token_b: '0x6B175474E89094C44Da98b954EedeAC495271d0F', // DAI
      amount_a: '1000000000000000000', // 1 ETH
      // Other input data
    };

    try {
      const response = await uniswap.swapExactEthForTokens(name, data);
      console.log(response);
    } catch (error) {
      console.error(error);
    }
    ```

**`swapExactTokensForTokens(name: string, data: UniswapInput, params?: RequestParams)`**

This method is used to swap tokens for tokens on Uniswap.

* **Parameters:**
  * `name`: The name of the Uniswap pool.
  * `data`: An object containing the input data for the swap.
  * `params`: Optional request parameters.
* **Returns:** A promise that resolves to the data of the swap.
*   **Example:**

    ```javascript
    const name = 'myUniswapPool';
    const data = {
      token_a: '0x6B175474E89094C44Da98b954EedeAC495271d0F', // DAI
      token_b: '0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2', // WETH
      amount_a: '1000000000000000000', // 1 DAI
      // Other input data
    };

    try {
      const response = await uniswap.swapExactTokensForTokens(name, data);
      console.log(response);
    } catch (error) {
      console.error(error);
    }
    ```

#### Usage

To use the `Uniswap` class, you need to create an instance of it with a configured `HttpClient`. The `HttpClient` is responsible for making HTTP requests to the Uniswap API.

You can then use the `uniswap` instance to call the various methods of the `Uniswap` class. Make sure to handle any potential errors that may occur during the API calls using `try-catch` blocks.
