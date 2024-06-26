# Unity

No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)

This C# SDK is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:

* API version: 1.0.0
* SDK version: 1.0.0
* Build package: org.openapitools.codegen.languages.CSharpClientCodegen

## Version support

This generator should support all current LTS versions of Unity

* Unity 2020.3 (LTS) and up
* .NET Standard 2.1 / .NET Framework

## Dependencies

* [Newtonsoft.Json](https://docs.unity3d.com/Packages/com.unity.nuget.newtonsoft-json@3.0/manual/index.html) - 3.0.2 or later
* [Unity Test Framework](https://docs.unity3d.com/Packages/com.unity.test-framework@1.1/manual/index.html) - 1.1.33 or later

## Installation

Add the dependencies to `Packages/manifest.json`

```
{
  "dependencies": {
    ...
    "com.unity.nuget.newtonsoft-json": "3.0.2",
    "com.unity.test-framework": "1.1.33",
  }
}
```

Then use the namespaces:

```csharp
using com.usemoon.MoonSDK.Api;
using com.usemoon.MoonSDK.Client;
using com.usemoon.MoonSDK.Model;
```

## Getting Started

```csharp
using System;
using System.Collections.Generic;
using UnityEngine;
using com.usemoon.MoonSDK.Api;
using com.usemoon.MoonSDK.Client;
using com.usemoon.MoonSDK.Model;

namespace com.usemoon.MoonSDKExample
{

    public class BorrowExample : MonoBehaviour
    {
        async void Start()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://beta.usemoon.ai";
            // Configure API key authorization: ApiKeyAuth
            config.ApiKey.Add("x-api-key", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.ApiKeyPrefix.Add("x-api-key", "Bearer");
            // Configure API key authorization: BearerAuth
            config.ApiKey.Add("Authorization", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.ApiKeyPrefix.Add("Authorization", "Bearer");

            var apiInstance = new AaveApi(config);
            var authorization = "authorization_example";  // string | 
            var name = "name_example";  // string | 
            var aaveInput = new AaveInput(); // AaveInput | 

            try
            {
                TransactionAPIResponse result = await apiInstance.BorrowAsync(authorization, name, aaveInput);
                Debug.Log(result);
                Debug.Log("Done!");
            }
            catch (ApiException e)
            {
                Debug.LogError("Exception when calling AaveApi.Borrow: " + e.Message );
                Debug.LogError("Status Code: "+ e.ErrorCode);
                Debug.LogError(e.StackTrace);
            }

        }
    }
}
```

## Documentation for API Endpoints

All URIs are relative to _https://beta.usemoon.ai_

| Class                | Method                                   | HTTP request                                          | Description |
| -------------------- | ---------------------------------------- | ----------------------------------------------------- | ----------- |
| _AaveApi_            | **Borrow**                               | **POST** /aave/{name}/borrow                          |             |
| _AaveApi_            | **Lend**                                 | **POST** /aave/{name}/lend                            |             |
| _AaveApi_            | **Repay**                                | **POST** /aave/{name}/repay                           |             |
| _AaveApi_            | **UserReserveData**                      | **POST** /aave/{name}/user-reserve-data               |             |
| _AccountsApi_        | **BroadcastTx**                          | **POST** /accounts/{accountName}/broadcast-tx         |             |
| _AccountsApi_        | **CreateAccount**                        | **POST** /accounts                                    |             |
| _AccountsApi_        | **DeleteAccount**                        | **DELETE** /accounts/{accountName}                    |             |
| _AccountsApi_        | **DeployContract**                       | **POST** /accounts/{accountName}/deploy               |             |
| _AccountsApi_        | **GetAccount**                           | **GET** /accounts/{accountName}                       |             |
| _AccountsApi_        | **GetBalance**                           | **GET** /accounts/{accountName}/balance               |             |
| _AccountsApi_        | **GetNonce**                             | **GET** /accounts/{accountName}/nonce                 |             |
| _AccountsApi_        | **ListAccounts**                         | **GET** /accounts                                     |             |
| _AccountsApi_        | **SignMessage**                          | **POST** /accounts/{accountName}/sign-message         |             |
| _AccountsApi_        | **SignTransaction**                      | **POST** /accounts/{accountName}/sign-transaction     |             |
| _AccountsApi_        | **SignTypedData**                        | **POST** /accounts/{accountName}/sign-typed-data      |             |
| _AccountsApi_        | **TransferEth**                          | **POST** /accounts/{accountName}/transfer-eth         |             |
| _BitcoinApi_         | **CreateBitcoinAccount**                 | **POST** /bitcoin                                     |             |
| _BitcoinApi_         | **GetBitcoinAccount**                    | **GET** /bitcoin/{accountName}                        |             |
| _BitcoinApi_         | **ListBitcoinAccounts**                  | **GET** /bitcoin                                      |             |
| _BitcoinApi_         | **SignBitcoinTransaction**               | **POST** /bitcoin/{accountName}/sign-tx               |             |
| _BitcoincashApi_     | **CreateBitcoinCashAccount**             | **POST** /bitcoincash                                 |             |
| _BitcoincashApi_     | **GetBitcoinCashAccount**                | **GET** /bitcoincash/{accountName}                    |             |
| _BitcoincashApi_     | **ListBitcoinCashAccounts**              | **GET** /bitcoincash                                  |             |
| _BitcoincashApi_     | **SignBitcoinCashTransaction**           | **POST** /bitcoincash/{accountName}/sign-tx           |             |
| _ConveyorFinanceApi_ | **Swap**                                 | **POST** /conveyorfinance/{name}/swap                 |             |
| _CosmosApi_          | **CreateCosmosAccount**                  | **POST** /cosmos                                      |             |
| _CosmosApi_          | **GetCosmosAccount**                     | **GET** /cosmos/{accountName}                         |             |
| _CosmosApi_          | **ListCosmosAccounts**                   | **GET** /cosmos                                       |             |
| _CosmosApi_          | **SignCosmosTransaction**                | **POST** /cosmos/{accountName}/sign-tx                |             |
| _DefaultApi_         | **GetMessage**                           | **GET** /ping                                         |             |
| _DogeCoinApi_        | **CreateDogeCoinAccount**                | **POST** /dogecoin                                    |             |
| _DogeCoinApi_        | **GetDogeCoinAccount**                   | **GET** /dogecoin/{accountName}                       |             |
| _DogeCoinApi_        | **ListDogeCoinAccounts**                 | **GET** /dogecoin                                     |             |
| _DogeCoinApi_        | **SignDogeCoinTransaction**              | **POST** /dogecoin/{accountName}/sign-tx              |             |
| _ENSApi_             | **Resolve**                              | **POST** /ens/resolve                                 |             |
| _ERC1155Api_         | **BalanceOf**                            | **POST** /erc1155/{name}/balance-of                   |             |
| _ERC1155Api_         | **BalanceOfBatch**                       | **POST** /erc1155/{name}/balance-of-batch             |             |
| _ERC1155Api_         | **IsApprovedForAll**                     | **POST** /erc1155/{name}/is-approved-for-all          |             |
| _ERC1155Api_         | **SafeBatchTransferFrom**                | **POST** /erc1155/{name}/safe-batch-transfer-from     |             |
| _ERC1155Api_         | **SafeTransferFrom**                     | **POST** /erc1155/{name}/safe-transfer-from           |             |
| _ERC1155Api_         | **SetApprovalForAll**                    | **POST** /erc1155/{name}/set-approval-for-all         |             |
| _EosApi_             | **CreateEosAccount**                     | **POST** /eos                                         |             |
| _EosApi_             | **GetEosAccount**                        | **GET** /eos/{accountName}                            |             |
| _EosApi_             | **ListEosAccounts**                      | **GET** /eos                                          |             |
| _EosApi_             | **SignEosTransaction**                   | **POST** /eos/{accountName}/sign-tx                   |             |
| _Erc20Api_           | **AllowanceErc20**                       | **POST** /erc20/{name}/allowance                      |             |
| _Erc20Api_           | **ApproveErc20**                         | **POST** /erc20/{name}/approve                        |             |
| _Erc20Api_           | **BalanceOfErc20**                       | **POST** /erc20/{name}/balance-of                     |             |
| _Erc20Api_           | **DecimalsErc20**                        | **POST** /erc20/{name}/decimals                       |             |
| _Erc20Api_           | **NameErc20**                            | **POST** /erc20/{name}/name                           |             |
| _Erc20Api_           | **SymbolErc20**                          | **POST** /erc20/{name}/symbol                         |             |
| _Erc20Api_           | **TotalSupplyErc20**                     | **POST** /erc20/{name}/total-supply                   |             |
| _Erc20Api_           | **TransferErc20**                        | **POST** /erc20/{name}/transfer                       |             |
| _Erc20Api_           | **TransferFromErc20**                    | **POST** /erc20/{name}/transfer-from                  |             |
| _Erc721Api_          | **Approve**                              | **POST** /erc721/{name}/approve                       |             |
| _Erc721Api_          | **BalanceOf**                            | **POST** /erc721/{name}/balance-of                    |             |
| _Erc721Api_          | **GetApproved**                          | **POST** /erc721/{name}/get-approved                  |             |
| _Erc721Api_          | **IsApprovedForAll**                     | **POST** /erc721/{name}/is-approved-for-all           |             |
| _Erc721Api_          | **Name**                                 | **POST** /erc721/{name}/name                          |             |
| _Erc721Api_          | **OwnerOf**                              | **POST** /erc721/{name}/owner-of                      |             |
| _Erc721Api_          | **SafeTransferFrom**                     | **POST** /erc721/{name}/safe-transfer-from            |             |
| _Erc721Api_          | **SetApprovalForAll**                    | **POST** /erc721/{name}/set-approval-for-all          |             |
| _Erc721Api_          | **Symbol**                               | **POST** /erc721/{name}/symbol                        |             |
| _Erc721Api_          | **TokenUri**                             | **POST** /erc721/{name}/token-uri                     |             |
| _Erc721Api_          | **Transfer**                             | **POST** /erc721/{name}/transfer                      |             |
| _Erc721Api_          | **TransferFrom**                         | **POST** /erc721/{name}/transfer-from                 |             |
| _LitecoinApi_        | **CreateLitecoinAccount**                | **POST** /litecoin                                    |             |
| _LitecoinApi_        | **GetLitecoinAccount**                   | **GET** /litecoin/{accountName}                       |             |
| _LitecoinApi_        | **ListLitecoinAccounts**                 | **GET** /litecoin                                     |             |
| _LitecoinApi_        | **SignLitecoinTransaction**              | **POST** /litecoin/{accountName}/sign-tx              |             |
| _OneinchApi_         | **ApproveCallData**                      | **POST** /oneinch/approve-call-data                   |             |
| _OneinchApi_         | **ApproveSpender**                       | **POST** /oneinch/approve-spender                     |             |
| _OneinchApi_         | **Protocols**                            | **POST** /oneinch/protocols                           |             |
| _OneinchApi_         | **Quote**                                | **POST** /oneinch/quote                               |             |
| _OneinchApi_         | **Swap**                                 | **POST** /oneinch/{accountName}/swap                  |             |
| _OneinchApi_         | **Tokens**                               | **POST** /oneinch/tokens                              |             |
| _OnramperApi_        | **OnRamperCheckout**                     | **POST** /onramper/fund/${accountName}                |             |
| _OnramperApi_        | **OnRamperGetQuotesBuy**                 | **GET** /onramper/quotes/buy                          |             |
| _OnramperApi_        | **OnRamperGetQuotesSell**                | **GET** /onramper/quotes/sell                         |             |
| _OnramperApi_        | **OnRamperGetSupportedAssets**           | **GET** /onramper/assets                              |             |
| _OnramperApi_        | **OnRamperGetSupportedCurrencies**       | **GET** /onramper/currencies                          |             |
| _OnramperApi_        | **OnRamperGetSupportedDefaultsAll**      | **GET** /onramper/defaults                            |             |
| _OnramperApi_        | **OnRamperGetSupportedOnRampsAll**       | **GET** /onramper/onramps                             |             |
| _OnramperApi_        | **OnRamperGetSupportedPaymentTypes**     | **GET** /onramper/payment-types                       |             |
| _OnramperApi_        | **OnRamperGetSupportedPaymentTypesFiat** | **GET** /onramper/payment-types/fiat                  |             |
| _RippleApi_          | **CreateRippleAccount**                  | **POST** /ripple                                      |             |
| _RippleApi_          | **GetRippleAccount**                     | **GET** /ripple/{accountName}                         |             |
| _RippleApi_          | **ListRippleAccounts**                   | **GET** /ripple                                       |             |
| _RippleApi_          | **SignRippleTransaction**                | **POST** /ripple/{accountName}/sign-tx                |             |
| _SolanaApi_          | **CreateSolanaAccount**                  | **POST** /solana                                      |             |
| _SolanaApi_          | **GetSolanaAccount**                     | **GET** /solana/{accountName}                         |             |
| _SolanaApi_          | **ListSolanaAccounts**                   | **GET** /solana                                       |             |
| _SolanaApi_          | **SignSolanaTransaction**                | **POST** /solana/{accountName}/sign-tx                |             |
| _TronApi_            | **CreateTronAccount**                    | **POST** /tron                                        |             |
| _TronApi_            | **GetTronAccount**                       | **GET** /tron/{accountName}                           |             |
| _TronApi_            | **ListTronAccounts**                     | **GET** /tron                                         |             |
| _TronApi_            | **SignTronTransaction**                  | **POST** /tron/{accountName}/sign-tx                  |             |
| _UniSwapApi_         | **AddLiquidity**                         | **POST** /uniswap/{name}/add-liquidity                |             |
| _UniSwapApi_         | **RemoveLiquidity**                      | **POST** /uniswap/{name}/remove-liquidity             |             |
| _UniSwapApi_         | **SwapExactETHForTokens**                | **POST** /uniswap/{name}/swap-exact-eth-for-tokens    |             |
| _UniSwapApi_         | **SwapExactTokensForTokens**             | **POST** /uniswap/{name}/swap-exact-tokens-for-tokens |             |
| _YearnApi_           | **AddLiquidity**                         | **POST** /yearn/{name}/add-liquidity                  |             |
| _YearnApi_           | **AddLiquidityWeth**                     | **POST** /yearn/{name}/add-liquidity-weth             |             |
| _YearnApi_           | **RemoveLiquidity**                      | **POST** /yearn/{name}/remove-liquidity               |             |
| _YearnApi_           | **RemoveLiquidityWeth**                  | **POST** /yearn/{name}/remove-liquidity-weth          |             |

## Documentation for Models

* Model.AaveInput
* Model.AaveReservesAPIResponse
* Model.AaveReservesData
* Model.AccountAPIResponse
* Model.AccountData
* Model.AccountResponse
* Model.AvailablePaymentMethod
* Model.BalanceAPIResponse
* Model.BalanceResponse
* Model.BitcoinAPIResponse
* Model.BitcoinCashAPIResponse
* Model.BitcoinCashInput
* Model.BitcoinCashTransactionInput
* Model.BitcoinCashTransactionOutput
* Model.BitcoinInput
* Model.BitcoinTransactionInput
* Model.BitcoinTransactionOutput
* Model.BroadCastRawTransactionAPIResponse
* Model.BroadCastRawTransactionResponse
* Model.BroadcastInput
* Model.ConveyorFinanceControllerResponse
* Model.CosmosAPIResponse
* Model.CosmosInput
* Model.CosmosTransactionInput
* Model.CosmosTransactionOutput
* Model.CreateAccountInput
* Model.CryptoCurrency
* Model.DeployInput
* Model.DogeCoinAPIResponse
* Model.DogeCoinInput
* Model.DogeCoinTransactionInput
* Model.DogeCoinTransactionOutput
* Model.EnsResolveAPIResponse
* Model.EnsResolveInput
* Model.EnsResolveResponse
* Model.EosAPIResponse
* Model.EosInput
* Model.EosTransactionInput
* Model.EosTransactionOutput
* Model.Erc1155Request
* Model.Erc721Request
* Model.FiatCurrency
* Model.GetSupportedOnRampsResponse
* Model.GetSupportedOnRampsResponseMessageInner
* Model.GetSupportedOnRampsResponseMessageInnerIcons
* Model.GetSupportedOnRampsResponseMessageInnerIconsPng
* Model.GetSwapDto
* Model.InputBody
* Model.LitecoinAPIResponse
* Model.LitecoinInput
* Model.LitecoinTransactionInput
* Model.LitecoinTransactionOutput
* Model.Message
* Model.NonceAPIResponse
* Model.NonceResponse
* Model.PaymentType
* Model.PingResponse
* Model.Quote
* Model.RippleAPIResponse
* Model.RippleInput
* Model.RippleTransactionInput
* Model.RippleTransactionOutput
* Model.SellQuote
* Model.SignMessage
* Model.SignMessageAPIResponse
* Model.SignTypedData
* Model.SolanaAPIResponse
* Model.SolanaInput
* Model.SolanaTransactionInput
* Model.SolanaTransactionOutput
* Model.SupportedAssetResponse
* Model.SupportedAssetResponseAssetsInner
* Model.SupportedCurrenciesResponse
* Model.SupportedDefaultResponse
* Model.SupportedDefaultResponseDefaults
* Model.SupportedDefaultResponseDefaultsId
* Model.SupportedPaymentTypesCurrencyResponse
* Model.SupportedPaymentTypesMessage
* Model.TokenSwapParams
* Model.Transaction
* Model.TransactionAPIResponse
* Model.TransactionData
* Model.TransactionInput
* Model.TransactionInputMetaData
* Model.TransactionInputSupportedParams
* Model.TransactionInputSupportedParamsPartnerData
* Model.TransactionInputSupportedParamsPartnerDataRedirectUrl
* Model.TransactionInputSupportedParamsTheme
* Model.TransactionInputWallet
* Model.TransactionRequest
* Model.TransactionResponse
* Model.TransactionResponseInfo
* Model.TransactionResponseTx
* Model.TronAPIResponse
* Model.TronInput
* Model.TronTransactionInput
* Model.TronTransactionOutput
* Model.Tx
* Model.UniswapInput

## Documentation for Authorization

Authentication schemes defined for the API:

### BearerAuth

* **Type**: API key
* **API key parameter name**: Authorization
* **Location**: HTTP header

### OAuth2

* **Type**: OAuth
* **Flow**: password
* **Authorization URL**:
* **Scopes**:
  * authorization\_code: grants authorization\_code

### ApiKeyAuth

* **Type**: API key
* **API key parameter name**: x-api-key
* **Location**: HTTP header
