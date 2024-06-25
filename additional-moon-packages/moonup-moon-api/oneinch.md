# OneInch

The `OneInch` class from `@moonup/moon-api` provides a convenient way to interact with the 1inch API. This API allows you to perform various operations related to cryptocurrency swaps, approvals, and data retrieval.

Here's a detailed documentation for the `OneInch` class:

### Initialization

To use the `OneInch` class, you need to create an instance of it with a configured `HttpClient`. The `HttpClient` is responsible for making HTTP requests to the 1inch API.

Here's an example of how to create an instance of the `OneInch` class:

```javascript
import { HttpClient } from '@moonup/moon-api';
import { OneInch } from '@moonup/moon-api';

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

const oneinch = new OneInch(http);
```

### Class: OneInch

#### Methods

**`approveCallData(data: ApproveCallDataPayload, params?: RequestParams)`**

This method is used to get the call data for approving a token transfer.

* **Parameters:**
  * `data`: An object containing the token address and the amount to approve.
  * `params`: Optional request parameters.
* **Returns:** A promise that resolves to the call data for approving the token transfer.
*   **Example:**

    ```javascript
    const data = {
      tokenAddress: '0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984',
      amount: '1000000000000000000', // 1 UNI
    };

    try {
      const response = await oneinch.approveCallData(data);
      console.log(response);
    } catch (error) {
      console.error(error);
    }
    ```

**`approveSpender(data: ApproveSpenderPayload, params?: RequestParams)`**

This method is used to approve a spender to transfer tokens on your behalf.

* **Parameters:**
  * `data`: An object containing the token address and the spender address.
  * `params`: Optional request parameters.
* **Returns:** A promise that resolves to the transaction hash of the approval.
*   **Example:**

    ```javascript
    const data = {
      tokenAddress: '0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984',
      spenderAddress: '0x88757f2f99175387ab4c6a4b3067c77a695b0349',
    };

    try {
      const response = await oneinch.approveSpender(data);
      console.log(response);
    } catch (error) {
      console.error(error);
    }
    ```

**`protocols(data: ProtocolsPayload, params?: RequestParams)`**

This method is used to get the list of supported protocols.

* **Parameters:**
  * `data`: An object containing the chain ID.
  * `params`: Optional request parameters.
* **Returns:** A promise that resolves to the list of supported protocols.
*   **Example:**

    ```javascript
    const data = {
      chainId: 1, // Ethereum Mainnet
    };

    try {
      const response = await oneinch.protocols(data);
      console.log(response);
    } catch (error) {
      console.error(error);
    }
    ```

**`quote(data: QuotePayload, params?: RequestParams)`**

This method is used to get a quote for a swap.

* **Parameters:**
  * `data`: An object containing the source token address, the destination token address, and the amount to swap.
  * `params`: Optional request parameters.
* **Returns:** A promise that resolves to the quote for the swap.
*   **Example:**

    ```javascript
    const data = {
      fromTokenAddress: '0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984',
      toTokenAddress: '0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2',
      amount: '1000000000000000000', // 1 UNI
    };

    try {
      const response = await oneinch.quote(data);
      console.log(response);
    } catch (error) {
      console.error(error);
    }
    ```

**`swap(accountName: string, data: GetSwapDto, params?: RequestParams)`**

This method is used to perform a swap.

* **Parameters:**
  * `accountName`: The name of the account to use for the swap.
  * `data`: An object containing the swap details, such as the source token address, the destination token address, the amount to swap, and the slippage tolerance.
  * `params`: Optional request parameters.
* **Returns:** A promise that resolves to the transaction hash of the swap.
*   **Example:**

    ```javascript
    const accountName = 'myAccount';
    const data = {
      fromTokenAddress: '0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984',
      toTokenAddress: '0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2',
      amount: '1000000000000000000', // 1 UNI
      slippage: 0.5, // 0.5% slippage tolerance
    };

    try {
      const response = await oneinch.swap(accountName, data);
      console.log(response);
    } catch (error) {
      console.error(error);
    }
    ```

**`tokens(data: TokensPayload, params?: RequestParams)`**

This method is used to get the list of supported tokens.

* **Parameters:**
  * `data`: An object containing the chain ID.
  * `params`: Optional request parameters.
* **Returns:** A promise that resolves to the list of supported tokens.
*   **Example:**

    ```javascript
    const data = {
      chainId: 1, // Ethereum Mainnet
    };

    try {
      const response = await oneinch.tokens(data);
      console.log(response);
    } catch (error) {
      console.error(error);
    }
    ```

#### Usage

To use the `OneInch` class, you need to create an instance of it with a configured `HttpClient`. The `HttpClient` is responsible for making HTTP requests to the 1inch API.

You can then use the `oneinch` instance to call the various methods of the `OneInch` class. Make sure to handle any potential errors that may occur during the API calls using `try-catch` blocks.
