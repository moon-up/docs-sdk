# Flutter

No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)

This Dart package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:

* API version: 1.0.0
* Generator version: 7.4.0
* Build package: org.openapitools.codegen.languages.DartDioClientCodegen

## Requirements

* Dart 2.15.0+ or Flutter 2.8.0+
* Dio 5.0.0+ (https://pub.dev/packages/dio)

## Installation & Usage

### pub.dev

To use the package from [pub.dev](https://pub.dev), please include the following in pubspec.yaml

```yaml
dependencies:
  moonsdk: 1.0.0
```

### Github

If this Dart package is published to Github, please include the following in pubspec.yaml

```yaml
dependencies:
  moonsdk:
    git:
      url: https://github.com/GIT_USER_ID/GIT_REPO_ID.git
      #ref: main
```

### Local development

To use the package from your local drive, please include the following in pubspec.yaml

```yaml
dependencies:
  moonsdk:
    path: /path/to/moonsdk
```

## Getting Started

Please follow the [installation procedure](./#installation--usage) and then run the following:

```dart
import 'package:moonsdk/moonsdk.dart';


final api = Moonsdk().getAaveApi();
final String authorization = authorization_example; // String | 
final String name = name_example; // String | 
final AaveInput aaveInput = ; // AaveInput | 

try {
    final response = await api.borrow(authorization, name, aaveInput);
    print(response);
} catch on DioException (e) {
    print("Exception when calling AaveApi->borrow: $e\n");
}

```

## Documentation for API Endpoints

All URIs are relative to _https://beta.usemoon.ai_

| Class                                              | Method                                                                                               | HTTP request                                          | Description |
| -------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ----------------------------------------------------- | ----------- |
| [_AaveApi_](dart/AaveApi.md)                       | [**borrow**](dart/AaveApi.md#borrow)                                                                 | **POST** /aave/{name}/borrow                          |             |
| [_AaveApi_](dart/AaveApi.md)                       | [**lend**](dart/AaveApi.md#lend)                                                                     | **POST** /aave/{name}/lend                            |             |
| [_AaveApi_](dart/AaveApi.md)                       | [**repay**](dart/AaveApi.md#repay)                                                                   | **POST** /aave/{name}/repay                           |             |
| [_AaveApi_](dart/AaveApi.md)                       | [**userReserveData**](dart/AaveApi.md#userreservedata)                                               | **POST** /aave/{name}/user-reserve-data               |             |
| [_AccountsApi_](dart/AccountsApi.md)               | [**broadcastTx**](dart/AccountsApi.md#broadcasttx)                                                   | **POST** /accounts/{accountName}/broadcast-tx         |             |
| [_AccountsApi_](dart/AccountsApi.md)               | [**createAccount**](dart/AccountsApi.md#createaccount)                                               | **POST** /accounts                                    |             |
| [_AccountsApi_](dart/AccountsApi.md)               | [**deleteAccount**](dart/AccountsApi.md#deleteaccount)                                               | **DELETE** /accounts/{accountName}                    |             |
| [_AccountsApi_](dart/AccountsApi.md)               | [**deployContract**](dart/AccountsApi.md#deploycontract)                                             | **POST** /accounts/{accountName}/deploy               |             |
| [_AccountsApi_](dart/AccountsApi.md)               | [**getAccount**](dart/AccountsApi.md#getaccount)                                                     | **GET** /accounts/{accountName}                       |             |
| [_AccountsApi_](dart/AccountsApi.md)               | [**getBalance**](dart/AccountsApi.md#getbalance)                                                     | **GET** /accounts/{accountName}/balance               |             |
| [_AccountsApi_](dart/AccountsApi.md)               | [**getNonce**](dart/AccountsApi.md#getnonce)                                                         | **GET** /accounts/{accountName}/nonce                 |             |
| [_AccountsApi_](dart/AccountsApi.md)               | [**listAccounts**](dart/AccountsApi.md#listaccounts)                                                 | **GET** /accounts                                     |             |
| [_AccountsApi_](dart/AccountsApi.md)               | [**signMessage**](dart/AccountsApi.md#signmessage)                                                   | **POST** /accounts/{accountName}/sign-message         |             |
| [_AccountsApi_](dart/AccountsApi.md)               | [**signTransaction**](dart/AccountsApi.md#signtransaction)                                           | **POST** /accounts/{accountName}/sign-transaction     |             |
| [_AccountsApi_](dart/AccountsApi.md)               | [**signTypedData**](dart/AccountsApi.md#signtypeddata)                                               | **POST** /accounts/{accountName}/sign-typed-data      |             |
| [_AccountsApi_](dart/AccountsApi.md)               | [**transferEth**](dart/AccountsApi.md#transfereth)                                                   | **POST** /accounts/{accountName}/transfer-eth         |             |
| [_BitcoinApi_](dart/BitcoinApi.md)                 | [**createBitcoinAccount**](dart/BitcoinApi.md#createbitcoinaccount)                                  | **POST** /bitcoin                                     |             |
| [_BitcoinApi_](dart/BitcoinApi.md)                 | [**getBitcoinAccount**](dart/BitcoinApi.md#getbitcoinaccount)                                        | **GET** /bitcoin/{accountName}                        |             |
| [_BitcoinApi_](dart/BitcoinApi.md)                 | [**listBitcoinAccounts**](dart/BitcoinApi.md#listbitcoinaccounts)                                    | **GET** /bitcoin                                      |             |
| [_BitcoinApi_](dart/BitcoinApi.md)                 | [**signBitcoinTransaction**](dart/BitcoinApi.md#signbitcointransaction)                              | **POST** /bitcoin/{accountName}/sign-tx               |             |
| [_BitcoincashApi_](dart/BitcoincashApi.md)         | [**createBitcoinCashAccount**](dart/BitcoincashApi.md#createbitcoincashaccount)                      | **POST** /bitcoincash                                 |             |
| [_BitcoincashApi_](dart/BitcoincashApi.md)         | [**getBitcoinCashAccount**](dart/BitcoincashApi.md#getbitcoincashaccount)                            | **GET** /bitcoincash/{accountName}                    |             |
| [_BitcoincashApi_](dart/BitcoincashApi.md)         | [**listBitcoinCashAccounts**](dart/BitcoincashApi.md#listbitcoincashaccounts)                        | **GET** /bitcoincash                                  |             |
| [_BitcoincashApi_](dart/BitcoincashApi.md)         | [**signBitcoinCashTransaction**](dart/BitcoincashApi.md#signbitcoincashtransaction)                  | **POST** /bitcoincash/{accountName}/sign-tx           |             |
| [_ConveyorFinanceApi_](dart/ConveyorFinanceApi.md) | [**swap**](dart/ConveyorFinanceApi.md#swap)                                                          | **POST** /conveyorfinance/{name}/swap                 |             |
| [_CosmosApi_](dart/CosmosApi.md)                   | [**createCosmosAccount**](dart/CosmosApi.md#createcosmosaccount)                                     | **POST** /cosmos                                      |             |
| [_CosmosApi_](dart/CosmosApi.md)                   | [**getCosmosAccount**](dart/CosmosApi.md#getcosmosaccount)                                           | **GET** /cosmos/{accountName}                         |             |
| [_CosmosApi_](dart/CosmosApi.md)                   | [**listCosmosAccounts**](dart/CosmosApi.md#listcosmosaccounts)                                       | **GET** /cosmos                                       |             |
| [_CosmosApi_](dart/CosmosApi.md)                   | [**signCosmosTransaction**](dart/CosmosApi.md#signcosmostransaction)                                 | **POST** /cosmos/{accountName}/sign-tx                |             |
| [_DefaultApi_](dart/DefaultApi.md)                 | [**getMessage**](dart/DefaultApi.md#getmessage)                                                      | **GET** /ping                                         |             |
| [_DogeCoinApi_](dart/DogeCoinApi.md)               | [**createDogeCoinAccount**](dart/DogeCoinApi.md#createdogecoinaccount)                               | **POST** /dogecoin                                    |             |
| [_DogeCoinApi_](dart/DogeCoinApi.md)               | [**getDogeCoinAccount**](dart/DogeCoinApi.md#getdogecoinaccount)                                     | **GET** /dogecoin/{accountName}                       |             |
| [_DogeCoinApi_](dart/DogeCoinApi.md)               | [**listDogeCoinAccounts**](dart/DogeCoinApi.md#listdogecoinaccounts)                                 | **GET** /dogecoin                                     |             |
| [_DogeCoinApi_](dart/DogeCoinApi.md)               | [**signDogeCoinTransaction**](dart/DogeCoinApi.md#signdogecointransaction)                           | **POST** /dogecoin/{accountName}/sign-tx              |             |
| [_ENSApi_](dart/ENSApi.md)                         | [**resolve**](dart/ENSApi.md#resolve)                                                                | **POST** /ens/resolve                                 |             |
| [_ERC1155Api_](dart/ERC1155Api.md)                 | [**balanceOf**](dart/ERC1155Api.md#balanceof)                                                        | **POST** /erc1155/{name}/balance-of                   |             |
| [_ERC1155Api_](dart/ERC1155Api.md)                 | [**balanceOfBatch**](dart/ERC1155Api.md#balanceofbatch)                                              | **POST** /erc1155/{name}/balance-of-batch             |             |
| [_ERC1155Api_](dart/ERC1155Api.md)                 | [**isApprovedForAll**](dart/ERC1155Api.md#isapprovedforall)                                          | **POST** /erc1155/{name}/is-approved-for-all          |             |
| [_ERC1155Api_](dart/ERC1155Api.md)                 | [**safeBatchTransferFrom**](dart/ERC1155Api.md#safebatchtransferfrom)                                | **POST** /erc1155/{name}/safe-batch-transfer-from     |             |
| [_ERC1155Api_](dart/ERC1155Api.md)                 | [**safeTransferFrom**](dart/ERC1155Api.md#safetransferfrom)                                          | **POST** /erc1155/{name}/safe-transfer-from           |             |
| [_ERC1155Api_](dart/ERC1155Api.md)                 | [**setApprovalForAll**](dart/ERC1155Api.md#setapprovalforall)                                        | **POST** /erc1155/{name}/set-approval-for-all         |             |
| [_EosApi_](dart/EosApi.md)                         | [**createEosAccount**](dart/EosApi.md#createeosaccount)                                              | **POST** /eos                                         |             |
| [_EosApi_](dart/EosApi.md)                         | [**getEosAccount**](dart/EosApi.md#geteosaccount)                                                    | **GET** /eos/{accountName}                            |             |
| [_EosApi_](dart/EosApi.md)                         | [**listEosAccounts**](dart/EosApi.md#listeosaccounts)                                                | **GET** /eos                                          |             |
| [_EosApi_](dart/EosApi.md)                         | [**signEosTransaction**](dart/EosApi.md#signeostransaction)                                          | **POST** /eos/{accountName}/sign-tx                   |             |
| [_Erc20Api_](dart/Erc20Api.md)                     | [**allowanceErc20**](dart/Erc20Api.md#allowanceerc20)                                                | **POST** /erc20/{name}/allowance                      |             |
| [_Erc20Api_](dart/Erc20Api.md)                     | [**approveErc20**](dart/Erc20Api.md#approveerc20)                                                    | **POST** /erc20/{name}/approve                        |             |
| [_Erc20Api_](dart/Erc20Api.md)                     | [**balanceOfErc20**](dart/Erc20Api.md#balanceoferc20)                                                | **POST** /erc20/{name}/balance-of                     |             |
| [_Erc20Api_](dart/Erc20Api.md)                     | [**decimalsErc20**](dart/Erc20Api.md#decimalserc20)                                                  | **POST** /erc20/{name}/decimals                       |             |
| [_Erc20Api_](dart/Erc20Api.md)                     | [**nameErc20**](dart/Erc20Api.md#nameerc20)                                                          | **POST** /erc20/{name}/name                           |             |
| [_Erc20Api_](dart/Erc20Api.md)                     | [**symbolErc20**](dart/Erc20Api.md#symbolerc20)                                                      | **POST** /erc20/{name}/symbol                         |             |
| [_Erc20Api_](dart/Erc20Api.md)                     | [**totalSupplyErc20**](dart/Erc20Api.md#totalsupplyerc20)                                            | **POST** /erc20/{name}/total-supply                   |             |
| [_Erc20Api_](dart/Erc20Api.md)                     | [**transferErc20**](dart/Erc20Api.md#transfererc20)                                                  | **POST** /erc20/{name}/transfer                       |             |
| [_Erc20Api_](dart/Erc20Api.md)                     | [**transferFromErc20**](dart/Erc20Api.md#transferfromerc20)                                          | **POST** /erc20/{name}/transfer-from                  |             |
| [_Erc721Api_](dart/Erc721Api.md)                   | [**approve**](dart/Erc721Api.md#approve)                                                             | **POST** /erc721/{name}/approve                       |             |
| [_Erc721Api_](dart/Erc721Api.md)                   | [**balanceOf**](dart/Erc721Api.md#balanceof)                                                         | **POST** /erc721/{name}/balance-of                    |             |
| [_Erc721Api_](dart/Erc721Api.md)                   | [**getApproved**](dart/Erc721Api.md#getapproved)                                                     | **POST** /erc721/{name}/get-approved                  |             |
| [_Erc721Api_](dart/Erc721Api.md)                   | [**isApprovedForAll**](dart/Erc721Api.md#isapprovedforall)                                           | **POST** /erc721/{name}/is-approved-for-all           |             |
| [_Erc721Api_](dart/Erc721Api.md)                   | [**name**](dart/Erc721Api.md#name)                                                                   | **POST** /erc721/{name}/name                          |             |
| [_Erc721Api_](dart/Erc721Api.md)                   | [**ownerOf**](dart/Erc721Api.md#ownerof)                                                             | **POST** /erc721/{name}/owner-of                      |             |
| [_Erc721Api_](dart/Erc721Api.md)                   | [**safeTransferFrom**](dart/Erc721Api.md#safetransferfrom)                                           | **POST** /erc721/{name}/safe-transfer-from            |             |
| [_Erc721Api_](dart/Erc721Api.md)                   | [**setApprovalForAll**](dart/Erc721Api.md#setapprovalforall)                                         | **POST** /erc721/{name}/set-approval-for-all          |             |
| [_Erc721Api_](dart/Erc721Api.md)                   | [**symbol**](dart/Erc721Api.md#symbol)                                                               | **POST** /erc721/{name}/symbol                        |             |
| [_Erc721Api_](dart/Erc721Api.md)                   | [**tokenUri**](dart/Erc721Api.md#tokenuri)                                                           | **POST** /erc721/{name}/token-uri                     |             |
| [_Erc721Api_](dart/Erc721Api.md)                   | [**transfer**](dart/Erc721Api.md#transfer)                                                           | **POST** /erc721/{name}/transfer                      |             |
| [_Erc721Api_](dart/Erc721Api.md)                   | [**transferFrom**](dart/Erc721Api.md#transferfrom)                                                   | **POST** /erc721/{name}/transfer-from                 |             |
| [_LitecoinApi_](dart/LitecoinApi.md)               | [**createLitecoinAccount**](dart/LitecoinApi.md#createlitecoinaccount)                               | **POST** /litecoin                                    |             |
| [_LitecoinApi_](dart/LitecoinApi.md)               | [**getLitecoinAccount**](dart/LitecoinApi.md#getlitecoinaccount)                                     | **GET** /litecoin/{accountName}                       |             |
| [_LitecoinApi_](dart/LitecoinApi.md)               | [**listLitecoinAccounts**](dart/LitecoinApi.md#listlitecoinaccounts)                                 | **GET** /litecoin                                     |             |
| [_LitecoinApi_](dart/LitecoinApi.md)               | [**signLitecoinTransaction**](dart/LitecoinApi.md#signlitecointransaction)                           | **POST** /litecoin/{accountName}/sign-tx              |             |
| [_OneinchApi_](dart/OneinchApi.md)                 | [**approveCallData**](dart/OneinchApi.md#approvecalldata)                                            | **POST** /oneinch/approve-call-data                   |             |
| [_OneinchApi_](dart/OneinchApi.md)                 | [**approveSpender**](dart/OneinchApi.md#approvespender)                                              | **POST** /oneinch/approve-spender                     |             |
| [_OneinchApi_](dart/OneinchApi.md)                 | [**protocols**](dart/OneinchApi.md#protocols)                                                        | **POST** /oneinch/protocols                           |             |
| [_OneinchApi_](dart/OneinchApi.md)                 | [**quote**](dart/OneinchApi.md#quote)                                                                | **POST** /oneinch/quote                               |             |
| [_OneinchApi_](dart/OneinchApi.md)                 | [**swap**](dart/OneinchApi.md#swap)                                                                  | **POST** /oneinch/{accountName}/swap                  |             |
| [_OneinchApi_](dart/OneinchApi.md)                 | [**tokens**](dart/OneinchApi.md#tokens)                                                              | **POST** /oneinch/tokens                              |             |
| [_OnramperApi_](dart/OnramperApi.md)               | [**onRamperCheckout**](dart/OnramperApi.md#onrampercheckout)                                         | **POST** /onramper/fund/${accountName}                |             |
| [_OnramperApi_](dart/OnramperApi.md)               | [**onRamperGetQuotesBuy**](dart/OnramperApi.md#onrampergetquotesbuy)                                 | **GET** /onramper/quotes/buy                          |             |
| [_OnramperApi_](dart/OnramperApi.md)               | [**onRamperGetQuotesSell**](dart/OnramperApi.md#onrampergetquotessell)                               | **GET** /onramper/quotes/sell                         |             |
| [_OnramperApi_](dart/OnramperApi.md)               | [**onRamperGetSupportedAssets**](dart/OnramperApi.md#onrampergetsupportedassets)                     | **GET** /onramper/assets                              |             |
| [_OnramperApi_](dart/OnramperApi.md)               | [**onRamperGetSupportedCurrencies**](dart/OnramperApi.md#onrampergetsupportedcurrencies)             | **GET** /onramper/currencies                          |             |
| [_OnramperApi_](dart/OnramperApi.md)               | [**onRamperGetSupportedDefaultsAll**](dart/OnramperApi.md#onrampergetsupporteddefaultsall)           | **GET** /onramper/defaults                            |             |
| [_OnramperApi_](dart/OnramperApi.md)               | [**onRamperGetSupportedOnRampsAll**](dart/OnramperApi.md#onrampergetsupportedonrampsall)             | **GET** /onramper/onramps                             |             |
| [_OnramperApi_](dart/OnramperApi.md)               | [**onRamperGetSupportedPaymentTypes**](dart/OnramperApi.md#onrampergetsupportedpaymenttypes)         | **GET** /onramper/payment-types                       |             |
| [_OnramperApi_](dart/OnramperApi.md)               | [**onRamperGetSupportedPaymentTypesFiat**](dart/OnramperApi.md#onrampergetsupportedpaymenttypesfiat) | **GET** /onramper/payment-types/fiat                  |             |
| [_RippleApi_](dart/RippleApi.md)                   | [**createRippleAccount**](dart/RippleApi.md#createrippleaccount)                                     | **POST** /ripple                                      |             |
| [_RippleApi_](dart/RippleApi.md)                   | [**getRippleAccount**](dart/RippleApi.md#getrippleaccount)                                           | **GET** /ripple/{accountName}                         |             |
| [_RippleApi_](dart/RippleApi.md)                   | [**listRippleAccounts**](dart/RippleApi.md#listrippleaccounts)                                       | **GET** /ripple                                       |             |
| [_RippleApi_](dart/RippleApi.md)                   | [**signRippleTransaction**](dart/RippleApi.md#signrippletransaction)                                 | **POST** /ripple/{accountName}/sign-tx                |             |
| [_SolanaApi_](dart/SolanaApi.md)                   | [**createSolanaAccount**](dart/SolanaApi.md#createsolanaaccount)                                     | **POST** /solana                                      |             |
| [_SolanaApi_](dart/SolanaApi.md)                   | [**getSolanaAccount**](dart/SolanaApi.md#getsolanaaccount)                                           | **GET** /solana/{accountName}                         |             |
| [_SolanaApi_](dart/SolanaApi.md)                   | [**listSolanaAccounts**](dart/SolanaApi.md#listsolanaaccounts)                                       | **GET** /solana                                       |             |
| [_SolanaApi_](dart/SolanaApi.md)                   | [**signSolanaTransaction**](dart/SolanaApi.md#signsolanatransaction)                                 | **POST** /solana/{accountName}/sign-tx                |             |
| [_TronApi_](dart/TronApi.md)                       | [**createTronAccount**](dart/TronApi.md#createtronaccount)                                           | **POST** /tron                                        |             |
| [_TronApi_](dart/TronApi.md)                       | [**getTronAccount**](dart/TronApi.md#gettronaccount)                                                 | **GET** /tron/{accountName}                           |             |
| [_TronApi_](dart/TronApi.md)                       | [**listTronAccounts**](dart/TronApi.md#listtronaccounts)                                             | **GET** /tron                                         |             |
| [_TronApi_](dart/TronApi.md)                       | [**signTronTransaction**](dart/TronApi.md#signtrontransaction)                                       | **POST** /tron/{accountName}/sign-tx                  |             |
| [_UniSwapApi_](dart/UniSwapApi.md)                 | [**addLiquidity**](dart/UniSwapApi.md#addliquidity)                                                  | **POST** /uniswap/{name}/add-liquidity                |             |
| [_UniSwapApi_](dart/UniSwapApi.md)                 | [**removeLiquidity**](dart/UniSwapApi.md#removeliquidity)                                            | **POST** /uniswap/{name}/remove-liquidity             |             |
| [_UniSwapApi_](dart/UniSwapApi.md)                 | [**swapExactETHForTokens**](dart/UniSwapApi.md#swapexactethfortokens)                                | **POST** /uniswap/{name}/swap-exact-eth-for-tokens    |             |
| [_UniSwapApi_](dart/UniSwapApi.md)                 | [**swapExactTokensForTokens**](dart/UniSwapApi.md#swapexacttokensfortokens)                          | **POST** /uniswap/{name}/swap-exact-tokens-for-tokens |             |
| [_YearnApi_](dart/YearnApi.md)                     | [**addLiquidity**](dart/YearnApi.md#addliquidity)                                                    | **POST** /yearn/{name}/add-liquidity                  |             |
| [_YearnApi_](dart/YearnApi.md)                     | [**addLiquidityWeth**](dart/YearnApi.md#addliquidityweth)                                            | **POST** /yearn/{name}/add-liquidity-weth             |             |
| [_YearnApi_](dart/YearnApi.md)                     | [**removeLiquidity**](dart/YearnApi.md#removeliquidity)                                              | **POST** /yearn/{name}/remove-liquidity               |             |
| [_YearnApi_](dart/YearnApi.md)                     | [**removeLiquidityWeth**](dart/YearnApi.md#removeliquidityweth)                                      | **POST** /yearn/{name}/remove-liquidity-weth          |             |

## Documentation For Models

* [AaveInput](dart/AaveInput.md)
* [AaveReservesAPIResponse](dart/AaveReservesAPIResponse.md)
* [AaveReservesData](dart/AaveReservesData.md)
* [AccountAPIResponse](dart/AccountAPIResponse.md)
* [AccountData](dart/AccountData.md)
* [AccountResponse](dart/AccountResponse.md)
* [AvailablePaymentMethod](dart/AvailablePaymentMethod.md)
* [BalanceAPIResponse](dart/BalanceAPIResponse.md)
* [BalanceResponse](dart/BalanceResponse.md)
* [BitcoinAPIResponse](dart/BitcoinAPIResponse.md)
* [BitcoinCashAPIResponse](dart/BitcoinCashAPIResponse.md)
* [BitcoinCashInput](dart/BitcoinCashInput.md)
* [BitcoinCashTransactionInput](dart/BitcoinCashTransactionInput.md)
* [BitcoinCashTransactionOutput](dart/BitcoinCashTransactionOutput.md)
* [BitcoinInput](dart/BitcoinInput.md)
* [BitcoinTransactionInput](dart/BitcoinTransactionInput.md)
* [BitcoinTransactionOutput](dart/BitcoinTransactionOutput.md)
* [BroadCastRawTransactionAPIResponse](dart/BroadCastRawTransactionAPIResponse.md)
* [BroadCastRawTransactionResponse](dart/BroadCastRawTransactionResponse.md)
* [BroadcastInput](dart/BroadcastInput.md)
* [ConveyorFinanceControllerResponse](dart/ConveyorFinanceControllerResponse.md)
* [CosmosAPIResponse](dart/CosmosAPIResponse.md)
* [CosmosInput](dart/CosmosInput.md)
* [CosmosTransactionInput](dart/CosmosTransactionInput.md)
* [CosmosTransactionOutput](dart/CosmosTransactionOutput.md)
* [CreateAccountInput](dart/CreateAccountInput.md)
* [CryptoCurrency](dart/CryptoCurrency.md)
* [DeployInput](dart/DeployInput.md)
* [DogeCoinAPIResponse](dart/DogeCoinAPIResponse.md)
* [DogeCoinInput](dart/DogeCoinInput.md)
* [DogeCoinTransactionInput](dart/DogeCoinTransactionInput.md)
* [DogeCoinTransactionOutput](dart/DogeCoinTransactionOutput.md)
* [EnsResolveAPIResponse](dart/EnsResolveAPIResponse.md)
* [EnsResolveInput](dart/EnsResolveInput.md)
* [EnsResolveResponse](dart/EnsResolveResponse.md)
* [EosAPIResponse](dart/EosAPIResponse.md)
* [EosInput](dart/EosInput.md)
* [EosTransactionInput](dart/EosTransactionInput.md)
* [EosTransactionOutput](dart/EosTransactionOutput.md)
* [Erc1155Request](dart/Erc1155Request.md)
* [Erc721Request](dart/Erc721Request.md)
* [FiatCurrency](dart/FiatCurrency.md)
* [GetSupportedOnRampsResponse](dart/GetSupportedOnRampsResponse.md)
* [GetSupportedOnRampsResponseMessageInner](dart/GetSupportedOnRampsResponseMessageInner.md)
* [GetSupportedOnRampsResponseMessageInnerIcons](dart/GetSupportedOnRampsResponseMessageInnerIcons.md)
* [GetSupportedOnRampsResponseMessageInnerIconsPng](dart/GetSupportedOnRampsResponseMessageInnerIconsPng.md)
* [GetSwapDto](dart/GetSwapDto.md)
* [InputBody](dart/InputBody.md)
* [LitecoinAPIResponse](dart/LitecoinAPIResponse.md)
* [LitecoinInput](dart/LitecoinInput.md)
* [LitecoinTransactionInput](dart/LitecoinTransactionInput.md)
* [LitecoinTransactionOutput](dart/LitecoinTransactionOutput.md)
* [Message](dart/Message.md)
* [NonceAPIResponse](dart/NonceAPIResponse.md)
* [NonceResponse](dart/NonceResponse.md)
* [PaymentType](dart/PaymentType.md)
* [PingResponse](dart/PingResponse.md)
* [Quote](dart/Quote.md)
* [RippleAPIResponse](dart/RippleAPIResponse.md)
* [RippleInput](dart/RippleInput.md)
* [RippleTransactionInput](dart/RippleTransactionInput.md)
* [RippleTransactionOutput](dart/RippleTransactionOutput.md)
* [SellQuote](dart/SellQuote.md)
* [SignMessage](dart/SignMessage.md)
* [SignMessageAPIResponse](dart/SignMessageAPIResponse.md)
* [SignTypedData](dart/SignTypedData.md)
* [SolanaAPIResponse](dart/SolanaAPIResponse.md)
* [SolanaInput](dart/SolanaInput.md)
* [SolanaTransactionInput](dart/SolanaTransactionInput.md)
* [SolanaTransactionOutput](dart/SolanaTransactionOutput.md)
* [SupportedAssetResponse](dart/SupportedAssetResponse.md)
* [SupportedAssetResponseAssetsInner](dart/SupportedAssetResponseAssetsInner.md)
* [SupportedCurrenciesResponse](dart/SupportedCurrenciesResponse.md)
* [SupportedDefaultResponse](dart/SupportedDefaultResponse.md)
* [SupportedDefaultResponseDefaults](dart/SupportedDefaultResponseDefaults.md)
* [SupportedDefaultResponseDefaultsId](dart/SupportedDefaultResponseDefaultsId.md)
* [SupportedPaymentTypesCurrencyResponse](dart/SupportedPaymentTypesCurrencyResponse.md)
* [SupportedPaymentTypesMessage](dart/SupportedPaymentTypesMessage.md)
* [TokenSwapParams](dart/TokenSwapParams.md)
* [Transaction](dart/Transaction.md)
* [TransactionAPIResponse](dart/TransactionAPIResponse.md)
* [TransactionData](dart/TransactionData.md)
* [TransactionInput](dart/TransactionInput.md)
* [TransactionInputMetaData](dart/TransactionInputMetaData.md)
* [TransactionInputSupportedParams](dart/TransactionInputSupportedParams.md)
* [TransactionInputSupportedParamsPartnerData](dart/TransactionInputSupportedParamsPartnerData.md)
* [TransactionInputSupportedParamsPartnerDataRedirectUrl](dart/TransactionInputSupportedParamsPartnerDataRedirectUrl.md)
* [TransactionInputSupportedParamsTheme](dart/TransactionInputSupportedParamsTheme.md)
* [TransactionInputWallet](dart/TransactionInputWallet.md)
* [TransactionRequest](dart/TransactionRequest.md)
* [TransactionResponse](dart/TransactionResponse.md)
* [TransactionResponseInfo](dart/TransactionResponseInfo.md)
* [TransactionResponseTx](dart/TransactionResponseTx.md)
* [TronAPIResponse](dart/TronAPIResponse.md)
* [TronInput](dart/TronInput.md)
* [TronTransactionInput](dart/TronTransactionInput.md)
* [TronTransactionOutput](dart/TronTransactionOutput.md)
* [Tx](dart/Tx.md)
* [UniswapInput](dart/UniswapInput.md)

## Documentation For Authorization

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
* **authorization\_code**: grants authorization\_code

### ApiKeyAuth

* **Type**: API key
* **API key parameter name**: x-api-key
* **Location**: HTTP header

## Author
