# Aave



Sure, here's the documentation for the `Aave` class from the `@moonup/moon-api` library, including an initialization section and usage examples for all of the functions:

### Initialization

To use the `Aave` class, you first need to initialize an `HttpClient` object with your API base URL and security worker. The security worker is a function that returns the headers to be included in the API requests. In this case, it returns an authorization header with a bearer token.

```javascript
import { HttpClient, Aave } from '@moonup/moon-api';

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

const aave = new Aave(http);
```

### Methods

#### `borrow(name: string, data: AaveInput, params: RequestParams = {})`

Borrows an asset from the Aave protocol.

* **Parameters:**
  * `name`: The name of the account.
  * `data`: An object containing the `asset` and `amount` properties.
  * `params`: Optional request parameters.
* **Returns:** A promise that resolves to a `BorrowData` object.
*   **Example:**

    ```javascript
    const borrowData = await aave.borrow('accountName', {
      asset: 'asset_address',
      amount: 'amount_to_borrow',
    });
    console.log('Borrow successful:', borrowData.transactionHash);
    ```

#### `lend(name: string, data: AaveInput, params: RequestParams = {})`

Lends an asset to the Aave protocol.

* **Parameters:**
  * `name`: The name of the account.
  * `data`: An object containing the `asset` and `amount` properties.
  * `params`: Optional request parameters.
* **Returns:** A promise that resolves to a `LendData` object.
*   **Example:**

    ```javascript
    const lendData = await aave.lend('accountName', {
      asset: 'asset_address',
      amount: 'amount_to_lend',
    });
    console.log('Lend successful:', lendData.transactionHash);
    ```

#### `repay(name: string, data: AaveInput, params: RequestParams = {})`

Repays a borrowed asset to the Aave protocol.

* **Parameters:**
  * `name`: The name of the account.
  * `data`: An object containing the `asset` and `amount` properties.
  * `params`: Optional request parameters.
* **Returns:** A promise that resolves to a `RepayData` object.
*   **Example:**

    ```javascript
    const repayData = await aave.repay('accountName', {
      asset: 'asset_address',
      amount: 'amount_to_repay',
    });
    console.log('Repay successful:', repayData.transactionHash);
    ```

#### `userReserveData(name: string, data: AaveInput, params: RequestParams = {})`

Retrieves data about a user's reserve in the Aave protocol.

* **Parameters:**
  * `name`: The name of the account.
  * `data`: An object containing the `asset` property.
  * `params`: Optional request parameters.
* **Returns:** A promise that resolves to a `UserReserveDataData` object.
*   **Example:**

    ```javascript
    const userReserveDataData = await aave.userReserveData('accountName', {
      asset: 'asset_address',
    });
    console.log('User reserve data:', userReserveDataData);
    ```

These examples assume that you have already initialized the `HttpClient` and `Aave` objects as shown in the initialization section. Make sure to replace the placeholders with actual values.
