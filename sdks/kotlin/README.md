# Kotlin

No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)

## Overview

This API client was generated by the [OpenAPI Generator](https://openapi-generator.tech) project. By using the [openapi-spec](https://github.com/OAI/OpenAPI-Specification) from a remote server, you can easily generate an API client.

* API version: 1.0.0
* Package version:
* Build package: org.openapitools.codegen.languages.KotlinClientCodegen

## Requires

* Kotlin 1.7.21
* Gradle 7.5

## Build

First, create the gradle wrapper script:

```
gradle wrapper
```

Then, run:

```
./gradlew check assemble
```

This runs all tests and packages the library.

## Features/Implementation Notes

* Supports JSON inputs/outputs, File inputs, and Form inputs.
* Supports collection formats for query parameters: csv, tsv, ssv, pipes.
* Some Kotlin and Java types are fully qualified to avoid conflicts with types defined in OpenAPI definitions.
* Implementation of ApiClient is intended to reduce method counts, specifically to benefit Android targets.

## Documentation for API Endpoints

All URIs are relative to _https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app_

| Class                | Method                                                                                          | HTTP request                                             | Description |
| -------------------- | ----------------------------------------------------------------------------------------------- | -------------------------------------------------------- | ----------- |
| _AaveApi_            | [**borrow**](aaveapi.md#borrow)                                                                 | **POST** /aave/{name}/borrow                             |             |
| _AaveApi_            | [**lend**](aaveapi.md#lend)                                                                     | **POST** /aave/{name}/lend                               |             |
| _AaveApi_            | [**repay**](aaveapi.md#repay)                                                                   | **POST** /aave/{name}/repay                              |             |
| _AaveApi_            | [**userReserveData**](aaveapi.md#userreservedata)                                               | **POST** /aave/{name}/user-reserve-data                  |             |
| _AccountsApi_        | [**broadcastTx**](accountsapi.md#broadcasttx)                                                   | **POST** /accounts/{accountName}/broadcast-tx            |             |
| _AccountsApi_        | [**createAccount**](accountsapi.md#createaccount)                                               | **POST** /accounts                                       |             |
| _AccountsApi_        | [**deleteAccount**](accountsapi.md#deleteaccount)                                               | **DELETE** /accounts/{accountName}                       |             |
| _AccountsApi_        | [**deployContract**](accountsapi.md#deploycontract)                                             | **POST** /accounts/{accountName}/deploy                  |             |
| _AccountsApi_        | [**getAccount**](accountsapi.md#getaccount)                                                     | **GET** /accounts/{accountName}                          |             |
| _AccountsApi_        | [**getBalance**](accountsapi.md#getbalance)                                                     | **GET** /accounts/{accountName}/balance                  |             |
| _AccountsApi_        | [**getNonce**](accountsapi.md#getnonce)                                                         | **GET** /accounts/{accountName}/nonce                    |             |
| _AccountsApi_        | [**listAccounts**](accountsapi.md#listaccounts)                                                 | **GET** /accounts                                        |             |
| _AccountsApi_        | [**signMessage**](accountsapi.md#signmessage)                                                   | **POST** /accounts/{accountName}/sign-message            |             |
| _AccountsApi_        | [**signTransaction**](accountsapi.md#signtransaction)                                           | **POST** /accounts/{accountName}/sign-transaction        |             |
| _AccountsApi_        | [**signTypedData**](accountsapi.md#signtypeddata)                                               | **POST** /accounts/{accountName}/sign-typed-data         |             |
| _AccountsApi_        | [**transferEth**](accountsapi.md#transfereth)                                                   | **POST** /accounts/{accountName}/transfer-eth            |             |
| _BitcoinApi_         | [**createBitcoinAccount**](bitcoinapi.md#createbitcoinaccount)                                  | **POST** /bitcoin                                        |             |
| _BitcoinApi_         | [**getBitcoinAccount**](bitcoinapi.md#getbitcoinaccount)                                        | **GET** /bitcoin/{accountName}                           |             |
| _BitcoinApi_         | [**listBitcoinAccounts**](bitcoinapi.md#listbitcoinaccounts)                                    | **GET** /bitcoin                                         |             |
| _BitcoinApi_         | [**signBitcoinTransaction**](bitcoinapi.md#signbitcointransaction)                              | **POST** /bitcoin/{accountName}/sign-tx                  |             |
| _BitcoincashApi_     | [**createBitcoinCashAccount**](bitcoincashapi.md#createbitcoincashaccount)                      | **POST** /bitcoincash                                    |             |
| _BitcoincashApi_     | [**getBitcoinCashAccount**](bitcoincashapi.md#getbitcoincashaccount)                            | **GET** /bitcoincash/{accountName}                       |             |
| _BitcoincashApi_     | [**listBitcoinCashAccounts**](bitcoincashapi.md#listbitcoincashaccounts)                        | **GET** /bitcoincash                                     |             |
| _BitcoincashApi_     | [**signBitcoinCashTransaction**](bitcoincashapi.md#signbitcoincashtransaction)                  | **POST** /bitcoincash/{accountName}/sign-tx              |             |
| _ConveyorFinanceApi_ | [**swap**](conveyorfinanceapi.md#swap)                                                          | **POST** /conveyorfinance/{name}/swap                    |             |
| _CosmosApi_          | [**createCosmosAccount**](cosmosapi.md#createcosmosaccount)                                     | **POST** /cosmos                                         |             |
| _CosmosApi_          | [**getCosmosAccount**](cosmosapi.md#getcosmosaccount)                                           | **GET** /cosmos/{accountName}                            |             |
| _CosmosApi_          | [**listCosmosAccounts**](cosmosapi.md#listcosmosaccounts)                                       | **GET** /cosmos                                          |             |
| _CosmosApi_          | [**signCosmosTransaction**](cosmosapi.md#signcosmostransaction)                                 | **POST** /cosmos/{accountName}/sign-tx                   |             |
| _DefaultApi_         | [**getMessage**](defaultapi.md#getmessage)                                                      | **GET** /ping                                            |             |
| _DogeCoinApi_        | [**createDogeCoinAccount**](dogecoinapi.md#createdogecoinaccount)                               | **POST** /dogecoin                                       |             |
| _DogeCoinApi_        | [**getDogeCoinAccount**](dogecoinapi.md#getdogecoinaccount)                                     | **GET** /dogecoin/{accountName}                          |             |
| _DogeCoinApi_        | [**listDogeCoinAccounts**](dogecoinapi.md#listdogecoinaccounts)                                 | **GET** /dogecoin                                        |             |
| _DogeCoinApi_        | [**signDogeCoinTransaction**](dogecoinapi.md#signdogecointransaction)                           | **POST** /dogecoin/{accountName}/sign-tx                 |             |
| _ENSApi_             | [**resolve**](ensapi.md#resolve)                                                                | **POST** /ens/resolve                                    |             |
| _ERC1155Api_         | [**balanceOf**](erc1155api.md#balanceof)                                                        | **POST** /erc1155/{name}/balance-of                      |             |
| _ERC1155Api_         | [**balanceOfBatch**](erc1155api.md#balanceofbatch)                                              | **POST** /erc1155/{name}/balance-of-batch                |             |
| _ERC1155Api_         | [**isApprovedForAll**](erc1155api.md#isapprovedforall)                                          | **POST** /erc1155/{name}/is-approved-for-all             |             |
| _ERC1155Api_         | [**safeBatchTransferFrom**](erc1155api.md#safebatchtransferfrom)                                | **POST** /erc1155/{name}/safe-batch-transfer-from        |             |
| _ERC1155Api_         | [**safeTransferFrom**](erc1155api.md#safetransferfrom)                                          | **POST** /erc1155/{name}/safe-transfer-from              |             |
| _ERC1155Api_         | [**setApprovalForAll**](erc1155api.md#setapprovalforall)                                        | **POST** /erc1155/{name}/set-approval-for-all            |             |
| _EosApi_             | [**createEosAccount**](eosapi.md#createeosaccount)                                              | **POST** /eos                                            |             |
| _EosApi_             | [**getEosAccount**](eosapi.md#geteosaccount)                                                    | **GET** /eos/{accountName}                               |             |
| _EosApi_             | [**listEosAccounts**](eosapi.md#listeosaccounts)                                                | **GET** /eos                                             |             |
| _EosApi_             | [**signEosTransaction**](eosapi.md#signeostransaction)                                          | **POST** /eos/{accountName}/sign-tx                      |             |
| _Erc20Api_           | [**allowanceErc20**](erc20api.md#allowanceerc20)                                                | **POST** /erc20/{name}/allowance                         |             |
| _Erc20Api_           | [**approveErc20**](erc20api.md#approveerc20)                                                    | **POST** /erc20/{name}/approve                           |             |
| _Erc20Api_           | [**balanceOfErc20**](erc20api.md#balanceoferc20)                                                | **POST** /erc20/{name}/balance-of                        |             |
| _Erc20Api_           | [**decimalsErc20**](erc20api.md#decimalserc20)                                                  | **POST** /erc20/{name}/decimals                          |             |
| _Erc20Api_           | [**nameErc20**](erc20api.md#nameerc20)                                                          | **POST** /erc20/{name}/name                              |             |
| _Erc20Api_           | [**symbolErc20**](erc20api.md#symbolerc20)                                                      | **POST** /erc20/{name}/symbol                            |             |
| _Erc20Api_           | [**totalSupplyErc20**](erc20api.md#totalsupplyerc20)                                            | **POST** /erc20/{name}/total-supply                      |             |
| _Erc20Api_           | [**transferErc20**](erc20api.md#transfererc20)                                                  | **POST** /erc20/{name}/transfer                          |             |
| _Erc20Api_           | [**transferFromErc20**](erc20api.md#transferfromerc20)                                          | **POST** /erc20/{name}/transfer-from                     |             |
| _Erc4337Api_         | [**getAddress**](erc4337api.md#getaddress)                                                      | **POST** /erc4337/{accountName}/address                  |             |
| _Erc4337Api_         | [**signBroadcastUserOpTx**](erc4337api.md#signbroadcastuseroptx)                                | **POST** /erc4337/{accountName}/sign-broadcast-userop-tx |             |
| _Erc721Api_          | [**approve**](erc721api.md#approve)                                                             | **POST** /erc721/{name}/approve                          |             |
| _Erc721Api_          | [**balanceOf**](erc721api.md#balanceof)                                                         | **POST** /erc721/{name}/balance-of                       |             |
| _Erc721Api_          | [**getApproved**](erc721api.md#getapproved)                                                     | **POST** /erc721/{name}/get-approved                     |             |
| _Erc721Api_          | [**isApprovedForAll**](erc721api.md#isapprovedforall)                                           | **POST** /erc721/{name}/is-approved-for-all              |             |
| _Erc721Api_          | [**name**](erc721api.md#name)                                                                   | **POST** /erc721/{name}/name                             |             |
| _Erc721Api_          | [**ownerOf**](erc721api.md#ownerof)                                                             | **POST** /erc721/{name}/owner-of                         |             |
| _Erc721Api_          | [**safeTransferFrom**](erc721api.md#safetransferfrom)                                           | **POST** /erc721/{name}/safe-transfer-from               |             |
| _Erc721Api_          | [**setApprovalForAll**](erc721api.md#setapprovalforall)                                         | **POST** /erc721/{name}/set-approval-for-all             |             |
| _Erc721Api_          | [**symbol**](erc721api.md#symbol)                                                               | **POST** /erc721/{name}/symbol                           |             |
| _Erc721Api_          | [**tokenUri**](erc721api.md#tokenuri)                                                           | **POST** /erc721/{name}/token-uri                        |             |
| _Erc721Api_          | [**transfer**](erc721api.md#transfer)                                                           | **POST** /erc721/{name}/transfer                         |             |
| _Erc721Api_          | [**transferFrom**](erc721api.md#transferfrom)                                                   | **POST** /erc721/{name}/transfer-from                    |             |
| _LitecoinApi_        | [**createLitecoinAccount**](litecoinapi.md#createlitecoinaccount)                               | **POST** /litecoin                                       |             |
| _LitecoinApi_        | [**getLitecoinAccount**](litecoinapi.md#getlitecoinaccount)                                     | **GET** /litecoin/{accountName}                          |             |
| _LitecoinApi_        | [**listLitecoinAccounts**](litecoinapi.md#listlitecoinaccounts)                                 | **GET** /litecoin                                        |             |
| _LitecoinApi_        | [**signLitecoinTransaction**](litecoinapi.md#signlitecointransaction)                           | **POST** /litecoin/{accountName}/sign-tx                 |             |
| _OneinchApi_         | [**approveCallData**](oneinchapi.md#approvecalldata)                                            | **POST** /oneinch/approve-call-data                      |             |
| _OneinchApi_         | [**approveSpender**](oneinchapi.md#approvespender)                                              | **POST** /oneinch/approve-spender                        |             |
| _OneinchApi_         | [**protocols**](oneinchapi.md#protocols)                                                        | **POST** /oneinch/protocols                              |             |
| _OneinchApi_         | [**quote**](oneinchapi.md#quote)                                                                | **POST** /oneinch/quote                                  |             |
| _OneinchApi_         | [**swap**](oneinchapi.md#swap)                                                                  | **POST** /oneinch/{accountName}/swap                     |             |
| _OneinchApi_         | [**tokens**](oneinchapi.md#tokens)                                                              | **POST** /oneinch/tokens                                 |             |
| _OnramperApi_        | [**onRamperCheckout**](onramperapi.md#onrampercheckout)                                         | **POST** /onramper/fund/${accountName}                   |             |
| _OnramperApi_        | [**onRamperGetQuotesBuy**](onramperapi.md#onrampergetquotesbuy)                                 | **GET** /onramper/quotes/buy                             |             |
| _OnramperApi_        | [**onRamperGetQuotesSell**](onramperapi.md#onrampergetquotessell)                               | **GET** /onramper/quotes/sell                            |             |
| _OnramperApi_        | [**onRamperGetSupportedAssets**](onramperapi.md#onrampergetsupportedassets)                     | **GET** /onramper/assets                                 |             |
| _OnramperApi_        | [**onRamperGetSupportedCurrencies**](onramperapi.md#onrampergetsupportedcurrencies)             | **GET** /onramper/currencies                             |             |
| _OnramperApi_        | [**onRamperGetSupportedDefaultsAll**](onramperapi.md#onrampergetsupporteddefaultsall)           | **GET** /onramper/defaults                               |             |
| _OnramperApi_        | [**onRamperGetSupportedOnRampsAll**](onramperapi.md#onrampergetsupportedonrampsall)             | **GET** /onramper/onramps                                |             |
| _OnramperApi_        | [**onRamperGetSupportedPaymentTypes**](onramperapi.md#onrampergetsupportedpaymenttypes)         | **GET** /onramper/payment-types                          |             |
| _OnramperApi_        | [**onRamperGetSupportedPaymentTypesFiat**](onramperapi.md#onrampergetsupportedpaymenttypesfiat) | **GET** /onramper/payment-types/fiat                     |             |
| _RippleApi_          | [**createRippleAccount**](rippleapi.md#createrippleaccount)                                     | **POST** /ripple                                         |             |
| _RippleApi_          | [**getRippleAccount**](rippleapi.md#getrippleaccount)                                           | **GET** /ripple/{accountName}                            |             |
| _RippleApi_          | [**listRippleAccounts**](rippleapi.md#listrippleaccounts)                                       | **GET** /ripple                                          |             |
| _RippleApi_          | [**signRippleTransaction**](rippleapi.md#signrippletransaction)                                 | **POST** /ripple/{accountName}/sign-tx                   |             |
| _SolanaApi_          | [**createSolanaAccount**](solanaapi.md#createsolanaaccount)                                     | **POST** /solana                                         |             |
| _SolanaApi_          | [**getSolanaAccount**](solanaapi.md#getsolanaaccount)                                           | **GET** /solana/{accountName}                            |             |
| _SolanaApi_          | [**listSolanaAccounts**](solanaapi.md#listsolanaaccounts)                                       | **GET** /solana                                          |             |
| _SolanaApi_          | [**signSolanaTransaction**](solanaapi.md#signsolanatransaction)                                 | **POST** /solana/{accountName}/sign-tx                   |             |
| _TronApi_            | [**createTronAccount**](tronapi.md#createtronaccount)                                           | **POST** /tron                                           |             |
| _TronApi_            | [**getTronAccount**](tronapi.md#gettronaccount)                                                 | **GET** /tron/{accountName}                              |             |
| _TronApi_            | [**listTronAccounts**](tronapi.md#listtronaccounts)                                             | **GET** /tron                                            |             |
| _TronApi_            | [**signTronTransaction**](tronapi.md#signtrontransaction)                                       | **POST** /tron/{accountName}/sign-tx                     |             |
| _UniSwapApi_         | [**addLiquidity**](uniswapapi.md#addliquidity)                                                  | **POST** /uniswap/{name}/add-liquidity                   |             |
| _UniSwapApi_         | [**removeLiquidity**](uniswapapi.md#removeliquidity)                                            | **POST** /uniswap/{name}/remove-liquidity                |             |
| _UniSwapApi_         | [**swapExactETHForTokens**](uniswapapi.md#swapexactethfortokens)                                | **POST** /uniswap/{name}/swap-exact-eth-for-tokens       |             |
| _UniSwapApi_         | [**swapExactTokensForTokens**](uniswapapi.md#swapexacttokensfortokens)                          | **POST** /uniswap/{name}/swap-exact-tokens-for-tokens    |             |
| _YearnApi_           | [**addLiquidity**](yearnapi.md#addliquidity)                                                    | **POST** /yearn/{name}/add-liquidity                     |             |
| _YearnApi_           | [**addLiquidityWeth**](yearnapi.md#addliquidityweth)                                            | **POST** /yearn/{name}/add-liquidity-weth                |             |
| _YearnApi_           | [**removeLiquidity**](yearnapi.md#removeliquidity)                                              | **POST** /yearn/{name}/remove-liquidity                  |             |
| _YearnApi_           | [**removeLiquidityWeth**](yearnapi.md#removeliquidityweth)                                      | **POST** /yearn/{name}/remove-liquidity-weth             |             |

## Documentation for Models

* [org.usemoonai.moonsdk.models.AaveInput](aaveinput.md)
* [org.usemoonai.moonsdk.models.AaveReservesAPIResponse](aavereservesapiresponse.md)
* [org.usemoonai.moonsdk.models.AaveReservesData](aavereservesdata.md)
* [org.usemoonai.moonsdk.models.AccountAPIResponse](accountapiresponse.md)
* [org.usemoonai.moonsdk.models.AccountData](accountdata.md)
* [org.usemoonai.moonsdk.models.AccountResponse](accountresponse.md)
* [org.usemoonai.moonsdk.models.AvailablePaymentMethod](availablepaymentmethod.md)
* [org.usemoonai.moonsdk.models.BalanceAPIResponse](balanceapiresponse.md)
* [org.usemoonai.moonsdk.models.BalanceResponse](balanceresponse.md)
* [org.usemoonai.moonsdk.models.BitcoinAPIResponse](bitcoinapiresponse.md)
* [org.usemoonai.moonsdk.models.BitcoinCashAPIResponse](bitcoincashapiresponse.md)
* [org.usemoonai.moonsdk.models.BitcoinCashInput](bitcoincashinput.md)
* [org.usemoonai.moonsdk.models.BitcoinCashTransactionInput](bitcoincashtransactioninput.md)
* [org.usemoonai.moonsdk.models.BitcoinCashTransactionOutput](bitcoincashtransactionoutput.md)
* [org.usemoonai.moonsdk.models.BitcoinInput](bitcoininput.md)
* [org.usemoonai.moonsdk.models.BitcoinTransactionInput](bitcointransactioninput.md)
* [org.usemoonai.moonsdk.models.BitcoinTransactionOutput](bitcointransactionoutput.md)
* [org.usemoonai.moonsdk.models.BroadCastRawTransactionAPIResponse](broadcastrawtransactionapiresponse.md)
* [org.usemoonai.moonsdk.models.BroadCastRawTransactionResponse](broadcastrawtransactionresponse.md)
* [org.usemoonai.moonsdk.models.BroadcastInput](broadcastinput.md)
* [org.usemoonai.moonsdk.models.ConveyorFinanceControllerResponse](conveyorfinancecontrollerresponse.md)
* [org.usemoonai.moonsdk.models.CosmosAPIResponse](cosmosapiresponse.md)
* [org.usemoonai.moonsdk.models.CosmosInput](cosmosinput.md)
* [org.usemoonai.moonsdk.models.CosmosTransactionInput](cosmostransactioninput.md)
* [org.usemoonai.moonsdk.models.CosmosTransactionOutput](cosmostransactionoutput.md)
* [org.usemoonai.moonsdk.models.CreateAccountInput](createaccountinput.md)
* [org.usemoonai.moonsdk.models.CryptoCurrency](cryptocurrency.md)
* [org.usemoonai.moonsdk.models.DeployInput](deployinput.md)
* [org.usemoonai.moonsdk.models.DogeCoinAPIResponse](dogecoinapiresponse.md)
* [org.usemoonai.moonsdk.models.DogeCoinInput](dogecoininput.md)
* [org.usemoonai.moonsdk.models.DogeCoinTransactionInput](dogecointransactioninput.md)
* [org.usemoonai.moonsdk.models.DogeCoinTransactionOutput](dogecointransactionoutput.md)
* [org.usemoonai.moonsdk.models.EnsResolveAPIResponse](ensresolveapiresponse.md)
* [org.usemoonai.moonsdk.models.EnsResolveInput](ensresolveinput.md)
* [org.usemoonai.moonsdk.models.EnsResolveResponse](ensresolveresponse.md)
* [org.usemoonai.moonsdk.models.EosAPIResponse](eosapiresponse.md)
* [org.usemoonai.moonsdk.models.EosInput](eosinput.md)
* [org.usemoonai.moonsdk.models.EosTransactionInput](eostransactioninput.md)
* [org.usemoonai.moonsdk.models.EosTransactionOutput](eostransactionoutput.md)
* [org.usemoonai.moonsdk.models.Erc1155Request](erc1155request.md)
* [org.usemoonai.moonsdk.models.Erc721Request](erc721request.md)
* [org.usemoonai.moonsdk.models.FiatCurrency](fiatcurrency.md)
* [org.usemoonai.moonsdk.models.GetSupportedOnRampsResponse](getsupportedonrampsresponse.md)
* [org.usemoonai.moonsdk.models.GetSupportedOnRampsResponseMessageInner](getsupportedonrampsresponsemessageinner.md)
* [org.usemoonai.moonsdk.models.GetSupportedOnRampsResponseMessageInnerIcons](getsupportedonrampsresponsemessageinnericons.md)
* [org.usemoonai.moonsdk.models.GetSupportedOnRampsResponseMessageInnerIconsPng](getsupportedonrampsresponsemessageinnericonspng.md)
* [org.usemoonai.moonsdk.models.GetSwapDto](getswapdto.md)
* [org.usemoonai.moonsdk.models.InputBody](inputbody.md)
* [org.usemoonai.moonsdk.models.LitecoinAPIResponse](litecoinapiresponse.md)
* [org.usemoonai.moonsdk.models.LitecoinInput](litecoininput.md)
* [org.usemoonai.moonsdk.models.LitecoinTransactionInput](litecointransactioninput.md)
* [org.usemoonai.moonsdk.models.LitecoinTransactionOutput](litecointransactionoutput.md)
* [org.usemoonai.moonsdk.models.Message](message.md)
* [org.usemoonai.moonsdk.models.NonceAPIResponse](nonceapiresponse.md)
* [org.usemoonai.moonsdk.models.NonceResponse](nonceresponse.md)
* [org.usemoonai.moonsdk.models.PaymentType](paymenttype.md)
* [org.usemoonai.moonsdk.models.PingResponse](pingresponse.md)
* [org.usemoonai.moonsdk.models.Quote](quote.md)
* [org.usemoonai.moonsdk.models.RippleAPIResponse](rippleapiresponse.md)
* [org.usemoonai.moonsdk.models.RippleInput](rippleinput.md)
* [org.usemoonai.moonsdk.models.RippleTransactionInput](rippletransactioninput.md)
* [org.usemoonai.moonsdk.models.RippleTransactionOutput](rippletransactionoutput.md)
* [org.usemoonai.moonsdk.models.SellQuote](sellquote.md)
* [org.usemoonai.moonsdk.models.SignMessage](signmessage.md)
* [org.usemoonai.moonsdk.models.SignMessageAPIResponse](signmessageapiresponse.md)
* [org.usemoonai.moonsdk.models.SignTypedData](signtypeddata.md)
* [org.usemoonai.moonsdk.models.SolanaAPIResponse](solanaapiresponse.md)
* [org.usemoonai.moonsdk.models.SolanaInput](solanainput.md)
* [org.usemoonai.moonsdk.models.SolanaTransactionInput](solanatransactioninput.md)
* [org.usemoonai.moonsdk.models.SolanaTransactionOutput](solanatransactionoutput.md)
* [org.usemoonai.moonsdk.models.SupportedAssetResponse](supportedassetresponse.md)
* [org.usemoonai.moonsdk.models.SupportedAssetResponseAssetsInner](supportedassetresponseassetsinner.md)
* [org.usemoonai.moonsdk.models.SupportedCurrenciesResponse](supportedcurrenciesresponse.md)
* [org.usemoonai.moonsdk.models.SupportedDefaultResponse](supporteddefaultresponse.md)
* [org.usemoonai.moonsdk.models.SupportedDefaultResponseDefaults](supporteddefaultresponsedefaults.md)
* [org.usemoonai.moonsdk.models.SupportedDefaultResponseDefaultsId](supporteddefaultresponsedefaultsid.md)
* [org.usemoonai.moonsdk.models.SupportedPaymentTypesCurrencyResponse](supportedpaymenttypescurrencyresponse.md)
* [org.usemoonai.moonsdk.models.SupportedPaymentTypesMessage](supportedpaymenttypesmessage.md)
* [org.usemoonai.moonsdk.models.TokenSwapParams](tokenswapparams.md)
* [org.usemoonai.moonsdk.models.Transaction](transaction.md)
* [org.usemoonai.moonsdk.models.TransactionAPIResponse](transactionapiresponse.md)
* [org.usemoonai.moonsdk.models.TransactionData](transactiondata.md)
* [org.usemoonai.moonsdk.models.TransactionInput](transactioninput.md)
* [org.usemoonai.moonsdk.models.TransactionInputMetaData](transactioninputmetadata.md)
* [org.usemoonai.moonsdk.models.TransactionInputSupportedParams](transactioninputsupportedparams.md)
* [org.usemoonai.moonsdk.models.TransactionInputSupportedParamsPartnerData](transactioninputsupportedparamspartnerdata.md)
* [org.usemoonai.moonsdk.models.TransactionInputSupportedParamsPartnerDataRedirectUrl](transactioninputsupportedparamspartnerdataredirecturl.md)
* [org.usemoonai.moonsdk.models.TransactionInputSupportedParamsTheme](transactioninputsupportedparamstheme.md)
* [org.usemoonai.moonsdk.models.TransactionInputWallet](transactioninputwallet.md)
* [org.usemoonai.moonsdk.models.TransactionRequest](transactionrequest.md)
* [org.usemoonai.moonsdk.models.TransactionResponse](transactionresponse.md)
* [org.usemoonai.moonsdk.models.TransactionResponseInfo](transactionresponseinfo.md)
* [org.usemoonai.moonsdk.models.TransactionResponseTx](transactionresponsetx.md)
* [org.usemoonai.moonsdk.models.TronAPIResponse](tronapiresponse.md)
* [org.usemoonai.moonsdk.models.TronInput](troninput.md)
* [org.usemoonai.moonsdk.models.TronTransactionInput](trontransactioninput.md)
* [org.usemoonai.moonsdk.models.TronTransactionOutput](trontransactionoutput.md)
* [org.usemoonai.moonsdk.models.Tx](tx.md)
* [org.usemoonai.moonsdk.models.UniswapInput](uniswapinput.md)

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
