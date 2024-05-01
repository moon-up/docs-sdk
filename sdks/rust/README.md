# Rust

No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)

## Overview

This API client was generated by the [OpenAPI Generator](https://openapi-generator.tech) project. By using the [openapi-spec](https://openapis.org) from a remote server, you can easily generate an API client.

* API version: 1.0.0
* Package version: 1.0.0
* Build package: `org.openapitools.codegen.languages.RustClientCodegen`

## Installation

Put the package under your project folder in a directory named `moonsdk` and add the following to `Cargo.toml` under `[dependencies]`:

```
moonsdk = { path = "./moonsdk" }
```

## Documentation for API Endpoints

All URIs are relative to _https://beta.usemoon.ai_

| Class                | Method                                                                                                                  | HTTP request                                          | Description |
| -------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------- | ----------- |
| _AaveApi_            | [**borrow**](aaveapi.md#borrow)                                                                                         | **POST** /aave/{name}/borrow                          |             |
| _AaveApi_            | [**lend**](aaveapi.md#lend)                                                                                             | **POST** /aave/{name}/lend                            |             |
| _AaveApi_            | [**repay**](aaveapi.md#repay)                                                                                           | **POST** /aave/{name}/repay                           |             |
| _AaveApi_            | [**user\_reserve\_data**](aaveapi.md#user\_reserve\_data)                                                               | **POST** /aave/{name}/user-reserve-data               |             |
| _AccountsApi_        | [**broadcast\_tx**](accountsapi.md#broadcast\_tx)                                                                       | **POST** /accounts/{accountName}/broadcast-tx         |             |
| _AccountsApi_        | [**create\_account**](accountsapi.md#create\_account)                                                                   | **POST** /accounts                                    |             |
| _AccountsApi_        | [**delete\_account**](accountsapi.md#delete\_account)                                                                   | **DELETE** /accounts/{accountName}                    |             |
| _AccountsApi_        | [**deploy\_contract**](accountsapi.md#deploy\_contract)                                                                 | **POST** /accounts/{accountName}/deploy               |             |
| _AccountsApi_        | [**get\_account**](accountsapi.md#get\_account)                                                                         | **GET** /accounts/{accountName}                       |             |
| _AccountsApi_        | [**get\_balance**](accountsapi.md#get\_balance)                                                                         | **GET** /accounts/{accountName}/balance               |             |
| _AccountsApi_        | [**get\_nonce**](accountsapi.md#get\_nonce)                                                                             | **GET** /accounts/{accountName}/nonce                 |             |
| _AccountsApi_        | [**list\_accounts**](accountsapi.md#list\_accounts)                                                                     | **GET** /accounts                                     |             |
| _AccountsApi_        | [**sign\_message**](accountsapi.md#sign\_message)                                                                       | **POST** /accounts/{accountName}/sign-message         |             |
| _AccountsApi_        | [**sign\_transaction**](accountsapi.md#sign\_transaction)                                                               | **POST** /accounts/{accountName}/sign-transaction     |             |
| _AccountsApi_        | [**sign\_typed\_data**](accountsapi.md#sign\_typed\_data)                                                               | **POST** /accounts/{accountName}/sign-typed-data      |             |
| _AccountsApi_        | [**transfer\_eth**](accountsapi.md#transfer\_eth)                                                                       | **POST** /accounts/{accountName}/transfer-eth         |             |
| _BitcoinApi_         | [**create\_bitcoin\_account**](bitcoinapi.md#create\_bitcoin\_account)                                                  | **POST** /bitcoin                                     |             |
| _BitcoinApi_         | [**get\_bitcoin\_account**](bitcoinapi.md#get\_bitcoin\_account)                                                        | **GET** /bitcoin/{accountName}                        |             |
| _BitcoinApi_         | [**list\_bitcoin\_accounts**](bitcoinapi.md#list\_bitcoin\_accounts)                                                    | **GET** /bitcoin                                      |             |
| _BitcoinApi_         | [**sign\_bitcoin\_transaction**](bitcoinapi.md#sign\_bitcoin\_transaction)                                              | **POST** /bitcoin/{accountName}/sign-tx               |             |
| _BitcoincashApi_     | [**create\_bitcoin\_cash\_account**](bitcoincashapi.md#create\_bitcoin\_cash\_account)                                  | **POST** /bitcoincash                                 |             |
| _BitcoincashApi_     | [**get\_bitcoin\_cash\_account**](bitcoincashapi.md#get\_bitcoin\_cash\_account)                                        | **GET** /bitcoincash/{accountName}                    |             |
| _BitcoincashApi_     | [**list\_bitcoin\_cash\_accounts**](bitcoincashapi.md#list\_bitcoin\_cash\_accounts)                                    | **GET** /bitcoincash                                  |             |
| _BitcoincashApi_     | [**sign\_bitcoin\_cash\_transaction**](bitcoincashapi.md#sign\_bitcoin\_cash\_transaction)                              | **POST** /bitcoincash/{accountName}/sign-tx           |             |
| _ConveyorFinanceApi_ | [**swap**](conveyorfinanceapi.md#swap)                                                                                  | **POST** /conveyorfinance/{name}/swap                 |             |
| _CosmosApi_          | [**create\_cosmos\_account**](cosmosapi.md#create\_cosmos\_account)                                                     | **POST** /cosmos                                      |             |
| _CosmosApi_          | [**get\_cosmos\_account**](cosmosapi.md#get\_cosmos\_account)                                                           | **GET** /cosmos/{accountName}                         |             |
| _CosmosApi_          | [**list\_cosmos\_accounts**](cosmosapi.md#list\_cosmos\_accounts)                                                       | **GET** /cosmos                                       |             |
| _CosmosApi_          | [**sign\_cosmos\_transaction**](cosmosapi.md#sign\_cosmos\_transaction)                                                 | **POST** /cosmos/{accountName}/sign-tx                |             |
| _DefaultApi_         | [**get\_message**](defaultapi.md#get\_message)                                                                          | **GET** /ping                                         |             |
| _DogeCoinApi_        | [**create\_doge\_coin\_account**](dogecoinapi.md#create\_doge\_coin\_account)                                           | **POST** /dogecoin                                    |             |
| _DogeCoinApi_        | [**get\_doge\_coin\_account**](dogecoinapi.md#get\_doge\_coin\_account)                                                 | **GET** /dogecoin/{accountName}                       |             |
| _DogeCoinApi_        | [**list\_doge\_coin\_accounts**](dogecoinapi.md#list\_doge\_coin\_accounts)                                             | **GET** /dogecoin                                     |             |
| _DogeCoinApi_        | [**sign\_doge\_coin\_transaction**](dogecoinapi.md#sign\_doge\_coin\_transaction)                                       | **POST** /dogecoin/{accountName}/sign-tx              |             |
| _EnsApi_             | [**resolve**](ensapi.md#resolve)                                                                                        | **POST** /ens/resolve                                 |             |
| _Erc1155Api_         | [**balance\_of**](erc1155api.md#balance\_of)                                                                            | **POST** /erc1155/{name}/balance-of                   |             |
| _Erc1155Api_         | [**balance\_of\_batch**](erc1155api.md#balance\_of\_batch)                                                              | **POST** /erc1155/{name}/balance-of-batch             |             |
| _Erc1155Api_         | [**is\_approved\_for\_all**](erc1155api.md#is\_approved\_for\_all)                                                      | **POST** /erc1155/{name}/is-approved-for-all          |             |
| _Erc1155Api_         | [**safe\_batch\_transfer\_from**](erc1155api.md#safe\_batch\_transfer\_from)                                            | **POST** /erc1155/{name}/safe-batch-transfer-from     |             |
| _Erc1155Api_         | [**safe\_transfer\_from**](erc1155api.md#safe\_transfer\_from)                                                          | **POST** /erc1155/{name}/safe-transfer-from           |             |
| _Erc1155Api_         | [**set\_approval\_for\_all**](erc1155api.md#set\_approval\_for\_all)                                                    | **POST** /erc1155/{name}/set-approval-for-all         |             |
| _EosApi_             | [**create\_eos\_account**](eosapi.md#create\_eos\_account)                                                              | **POST** /eos                                         |             |
| _EosApi_             | [**get\_eos\_account**](eosapi.md#get\_eos\_account)                                                                    | **GET** /eos/{accountName}                            |             |
| _EosApi_             | [**list\_eos\_accounts**](eosapi.md#list\_eos\_accounts)                                                                | **GET** /eos                                          |             |
| _EosApi_             | [**sign\_eos\_transaction**](eosapi.md#sign\_eos\_transaction)                                                          | **POST** /eos/{accountName}/sign-tx                   |             |
| _Erc20Api_           | [**allowance\_erc20**](erc20api.md#allowance\_erc20)                                                                    | **POST** /erc20/{name}/allowance                      |             |
| _Erc20Api_           | [**approve\_erc20**](erc20api.md#approve\_erc20)                                                                        | **POST** /erc20/{name}/approve                        |             |
| _Erc20Api_           | [**balance\_of\_erc20**](erc20api.md#balance\_of\_erc20)                                                                | **POST** /erc20/{name}/balance-of                     |             |
| _Erc20Api_           | [**decimals\_erc20**](erc20api.md#decimals\_erc20)                                                                      | **POST** /erc20/{name}/decimals                       |             |
| _Erc20Api_           | [**name\_erc20**](erc20api.md#name\_erc20)                                                                              | **POST** /erc20/{name}/name                           |             |
| _Erc20Api_           | [**symbol\_erc20**](erc20api.md#symbol\_erc20)                                                                          | **POST** /erc20/{name}/symbol                         |             |
| _Erc20Api_           | [**total\_supply\_erc20**](erc20api.md#total\_supply\_erc20)                                                            | **POST** /erc20/{name}/total-supply                   |             |
| _Erc20Api_           | [**transfer\_erc20**](erc20api.md#transfer\_erc20)                                                                      | **POST** /erc20/{name}/transfer                       |             |
| _Erc20Api_           | [**transfer\_from\_erc20**](erc20api.md#transfer\_from\_erc20)                                                          | **POST** /erc20/{name}/transfer-from                  |             |
| _Erc721Api_          | [**approve**](erc721api.md#approve)                                                                                     | **POST** /erc721/{name}/approve                       |             |
| _Erc721Api_          | [**balance\_of**](erc721api.md#balance\_of)                                                                             | **POST** /erc721/{name}/balance-of                    |             |
| _Erc721Api_          | [**get\_approved**](erc721api.md#get\_approved)                                                                         | **POST** /erc721/{name}/get-approved                  |             |
| _Erc721Api_          | [**is\_approved\_for\_all**](erc721api.md#is\_approved\_for\_all)                                                       | **POST** /erc721/{name}/is-approved-for-all           |             |
| _Erc721Api_          | [**name**](erc721api.md#name)                                                                                           | **POST** /erc721/{name}/name                          |             |
| _Erc721Api_          | [**owner\_of**](erc721api.md#owner\_of)                                                                                 | **POST** /erc721/{name}/owner-of                      |             |
| _Erc721Api_          | [**safe\_transfer\_from**](erc721api.md#safe\_transfer\_from)                                                           | **POST** /erc721/{name}/safe-transfer-from            |             |
| _Erc721Api_          | [**set\_approval\_for\_all**](erc721api.md#set\_approval\_for\_all)                                                     | **POST** /erc721/{name}/set-approval-for-all          |             |
| _Erc721Api_          | [**symbol**](erc721api.md#symbol)                                                                                       | **POST** /erc721/{name}/symbol                        |             |
| _Erc721Api_          | [**token\_uri**](erc721api.md#token\_uri)                                                                               | **POST** /erc721/{name}/token-uri                     |             |
| _Erc721Api_          | [**transfer**](erc721api.md#transfer)                                                                                   | **POST** /erc721/{name}/transfer                      |             |
| _Erc721Api_          | [**transfer\_from**](erc721api.md#transfer\_from)                                                                       | **POST** /erc721/{name}/transfer-from                 |             |
| _LitecoinApi_        | [**create\_litecoin\_account**](litecoinapi.md#create\_litecoin\_account)                                               | **POST** /litecoin                                    |             |
| _LitecoinApi_        | [**get\_litecoin\_account**](litecoinapi.md#get\_litecoin\_account)                                                     | **GET** /litecoin/{accountName}                       |             |
| _LitecoinApi_        | [**list\_litecoin\_accounts**](litecoinapi.md#list\_litecoin\_accounts)                                                 | **GET** /litecoin                                     |             |
| _LitecoinApi_        | [**sign\_litecoin\_transaction**](litecoinapi.md#sign\_litecoin\_transaction)                                           | **POST** /litecoin/{accountName}/sign-tx              |             |
| _OneinchApi_         | [**approve\_call\_data**](oneinchapi.md#approve\_call\_data)                                                            | **POST** /oneinch/approve-call-data                   |             |
| _OneinchApi_         | [**approve\_spender**](oneinchapi.md#approve\_spender)                                                                  | **POST** /oneinch/approve-spender                     |             |
| _OneinchApi_         | [**protocols**](oneinchapi.md#protocols)                                                                                | **POST** /oneinch/protocols                           |             |
| _OneinchApi_         | [**quote**](oneinchapi.md#quote)                                                                                        | **POST** /oneinch/quote                               |             |
| _OneinchApi_         | [**swap**](oneinchapi.md#swap)                                                                                          | **POST** /oneinch/{accountName}/swap                  |             |
| _OneinchApi_         | [**tokens**](oneinchapi.md#tokens)                                                                                      | **POST** /oneinch/tokens                              |             |
| _OnramperApi_        | [**on\_ramper\_checkout**](onramperapi.md#on\_ramper\_checkout)                                                         | **POST** /onramper/fund/${accountName}                |             |
| _OnramperApi_        | [**on\_ramper\_get\_quotes\_buy**](onramperapi.md#on\_ramper\_get\_quotes\_buy)                                         | **GET** /onramper/quotes/buy                          |             |
| _OnramperApi_        | [**on\_ramper\_get\_quotes\_sell**](onramperapi.md#on\_ramper\_get\_quotes\_sell)                                       | **GET** /onramper/quotes/sell                         |             |
| _OnramperApi_        | [**on\_ramper\_get\_supported\_assets**](onramperapi.md#on\_ramper\_get\_supported\_assets)                             | **GET** /onramper/assets                              |             |
| _OnramperApi_        | [**on\_ramper\_get\_supported\_currencies**](onramperapi.md#on\_ramper\_get\_supported\_currencies)                     | **GET** /onramper/currencies                          |             |
| _OnramperApi_        | [**on\_ramper\_get\_supported\_defaults\_all**](onramperapi.md#on\_ramper\_get\_supported\_defaults\_all)               | **GET** /onramper/defaults                            |             |
| _OnramperApi_        | [**on\_ramper\_get\_supported\_on\_ramps\_all**](onramperapi.md#on\_ramper\_get\_supported\_on\_ramps\_all)             | **GET** /onramper/onramps                             |             |
| _OnramperApi_        | [**on\_ramper\_get\_supported\_payment\_types**](onramperapi.md#on\_ramper\_get\_supported\_payment\_types)             | **GET** /onramper/payment-types                       |             |
| _OnramperApi_        | [**on\_ramper\_get\_supported\_payment\_types\_fiat**](onramperapi.md#on\_ramper\_get\_supported\_payment\_types\_fiat) | **GET** /onramper/payment-types/fiat                  |             |
| _RippleApi_          | [**create\_ripple\_account**](rippleapi.md#create\_ripple\_account)                                                     | **POST** /ripple                                      |             |
| _RippleApi_          | [**get\_ripple\_account**](rippleapi.md#get\_ripple\_account)                                                           | **GET** /ripple/{accountName}                         |             |
| _RippleApi_          | [**list\_ripple\_accounts**](rippleapi.md#list\_ripple\_accounts)                                                       | **GET** /ripple                                       |             |
| _RippleApi_          | [**sign\_ripple\_transaction**](rippleapi.md#sign\_ripple\_transaction)                                                 | **POST** /ripple/{accountName}/sign-tx                |             |
| _SolanaApi_          | [**create\_solana\_account**](solanaapi.md#create\_solana\_account)                                                     | **POST** /solana                                      |             |
| _SolanaApi_          | [**get\_solana\_account**](solanaapi.md#get\_solana\_account)                                                           | **GET** /solana/{accountName}                         |             |
| _SolanaApi_          | [**list\_solana\_accounts**](solanaapi.md#list\_solana\_accounts)                                                       | **GET** /solana                                       |             |
| _SolanaApi_          | [**sign\_solana\_transaction**](solanaapi.md#sign\_solana\_transaction)                                                 | **POST** /solana/{accountName}/sign-tx                |             |
| _TronApi_            | [**create\_tron\_account**](tronapi.md#create\_tron\_account)                                                           | **POST** /tron                                        |             |
| _TronApi_            | [**get\_tron\_account**](tronapi.md#get\_tron\_account)                                                                 | **GET** /tron/{accountName}                           |             |
| _TronApi_            | [**list\_tron\_accounts**](tronapi.md#list\_tron\_accounts)                                                             | **GET** /tron                                         |             |
| _TronApi_            | [**sign\_tron\_transaction**](tronapi.md#sign\_tron\_transaction)                                                       | **POST** /tron/{accountName}/sign-tx                  |             |
| _UniSwapApi_         | [**add\_liquidity**](uniswapapi.md#add\_liquidity)                                                                      | **POST** /uniswap/{name}/add-liquidity                |             |
| _UniSwapApi_         | [**remove\_liquidity**](uniswapapi.md#remove\_liquidity)                                                                | **POST** /uniswap/{name}/remove-liquidity             |             |
| _UniSwapApi_         | [**swap\_exact\_eth\_for\_tokens**](uniswapapi.md#swap\_exact\_eth\_for\_tokens)                                        | **POST** /uniswap/{name}/swap-exact-eth-for-tokens    |             |
| _UniSwapApi_         | [**swap\_exact\_tokens\_for\_tokens**](uniswapapi.md#swap\_exact\_tokens\_for\_tokens)                                  | **POST** /uniswap/{name}/swap-exact-tokens-for-tokens |             |
| _YearnApi_           | [**add\_liquidity**](yearnapi.md#add\_liquidity)                                                                        | **POST** /yearn/{name}/add-liquidity                  |             |
| _YearnApi_           | [**add\_liquidity\_weth**](yearnapi.md#add\_liquidity\_weth)                                                            | **POST** /yearn/{name}/add-liquidity-weth             |             |
| _YearnApi_           | [**remove\_liquidity**](yearnapi.md#remove\_liquidity)                                                                  | **POST** /yearn/{name}/remove-liquidity               |             |
| _YearnApi_           | [**remove\_liquidity\_weth**](yearnapi.md#remove\_liquidity\_weth)                                                      | **POST** /yearn/{name}/remove-liquidity-weth          |             |

## Documentation For Models

* [AaveInput](aaveinput.md)
* [AaveReservesApiResponse](aavereservesapiresponse.md)
* [AaveReservesData](aavereservesdata.md)
* [AccountApiResponse](accountapiresponse.md)
* [AccountData](accountdata.md)
* [AccountResponse](accountresponse.md)
* [AvailablePaymentMethod](availablepaymentmethod.md)
* [BalanceApiResponse](balanceapiresponse.md)
* [BalanceResponse](balanceresponse.md)
* [BitcoinApiResponse](bitcoinapiresponse.md)
* [BitcoinCashApiResponse](bitcoincashapiresponse.md)
* [BitcoinCashInput](bitcoincashinput.md)
* [BitcoinCashTransactionInput](bitcoincashtransactioninput.md)
* [BitcoinCashTransactionOutput](bitcoincashtransactionoutput.md)
* [BitcoinInput](bitcoininput.md)
* [BitcoinTransactionInput](bitcointransactioninput.md)
* [BitcoinTransactionOutput](bitcointransactionoutput.md)
* [BroadCastRawTransactionApiResponse](broadcastrawtransactionapiresponse.md)
* [BroadCastRawTransactionResponse](broadcastrawtransactionresponse.md)
* [BroadcastInput](broadcastinput.md)
* [ConveyorFinanceControllerResponse](conveyorfinancecontrollerresponse.md)
* [CosmosApiResponse](cosmosapiresponse.md)
* [CosmosInput](cosmosinput.md)
* [CosmosTransactionInput](cosmostransactioninput.md)
* [CosmosTransactionOutput](cosmostransactionoutput.md)
* [CreateAccountInput](createaccountinput.md)
* [CryptoCurrency](cryptocurrency.md)
* [DeployInput](deployinput.md)
* [DogeCoinApiResponse](dogecoinapiresponse.md)
* [DogeCoinInput](dogecoininput.md)
* [DogeCoinTransactionInput](dogecointransactioninput.md)
* [DogeCoinTransactionOutput](dogecointransactionoutput.md)
* [EnsResolveApiResponse](ensresolveapiresponse.md)
* [EnsResolveInput](ensresolveinput.md)
* [EnsResolveResponse](ensresolveresponse.md)
* [EosApiResponse](eosapiresponse.md)
* [EosInput](eosinput.md)
* [EosTransactionInput](eostransactioninput.md)
* [EosTransactionOutput](eostransactionoutput.md)
* [Erc1155Request](erc1155request.md)
* [Erc721Request](erc721request.md)
* [FiatCurrency](fiatcurrency.md)
* [GetSupportedOnRampsResponse](getsupportedonrampsresponse.md)
* [GetSupportedOnRampsResponseMessageInner](getsupportedonrampsresponsemessageinner.md)
* [GetSupportedOnRampsResponseMessageInnerIcons](getsupportedonrampsresponsemessageinnericons.md)
* [GetSupportedOnRampsResponseMessageInnerIconsPng](getsupportedonrampsresponsemessageinnericonspng.md)
* [GetSwapDto](getswapdto.md)
* [InputBody](inputbody.md)
* [LitecoinApiResponse](litecoinapiresponse.md)
* [LitecoinInput](litecoininput.md)
* [LitecoinTransactionInput](litecointransactioninput.md)
* [LitecoinTransactionOutput](litecointransactionoutput.md)
* [Message](message.md)
* [NonceApiResponse](nonceapiresponse.md)
* [NonceResponse](nonceresponse.md)
* [PaymentType](paymenttype.md)
* [PingResponse](pingresponse.md)
* [Quote](quote.md)
* [RippleApiResponse](rippleapiresponse.md)
* [RippleInput](rippleinput.md)
* [RippleTransactionInput](rippletransactioninput.md)
* [RippleTransactionOutput](rippletransactionoutput.md)
* [SellQuote](sellquote.md)
* [SignMessage](signmessage.md)
* [SignMessageApiResponse](signmessageapiresponse.md)
* [SignTypedData](signtypeddata.md)
* [SolanaApiResponse](solanaapiresponse.md)
* [SolanaInput](solanainput.md)
* [SolanaTransactionInput](solanatransactioninput.md)
* [SolanaTransactionOutput](solanatransactionoutput.md)
* [SupportedAssetResponse](supportedassetresponse.md)
* [SupportedAssetResponseAssetsInner](supportedassetresponseassetsinner.md)
* [SupportedCurrenciesResponse](supportedcurrenciesresponse.md)
* [SupportedDefaultResponse](supporteddefaultresponse.md)
* [SupportedDefaultResponseDefaults](supporteddefaultresponsedefaults.md)
* [SupportedDefaultResponseDefaultsId](supporteddefaultresponsedefaultsid.md)
* [SupportedPaymentTypesCurrencyResponse](supportedpaymenttypescurrencyresponse.md)
* [SupportedPaymentTypesMessage](supportedpaymenttypesmessage.md)
* [TokenSwapParams](tokenswapparams.md)
* [Transaction](transaction.md)
* [TransactionApiResponse](transactionapiresponse.md)
* [TransactionData](transactiondata.md)
* [TransactionInput](transactioninput.md)
* [TransactionInputMetaData](transactioninputmetadata.md)
* [TransactionInputSupportedParams](transactioninputsupportedparams.md)
* [TransactionInputSupportedParamsPartnerData](transactioninputsupportedparamspartnerdata.md)
* [TransactionInputSupportedParamsPartnerDataRedirectUrl](transactioninputsupportedparamspartnerdataredirecturl.md)
* [TransactionInputSupportedParamsTheme](transactioninputsupportedparamstheme.md)
* [TransactionInputWallet](transactioninputwallet.md)
* [TransactionRequest](transactionrequest.md)
* [TransactionResponse](transactionresponse.md)
* [TransactionResponseInfo](transactionresponseinfo.md)
* [TransactionResponseTx](transactionresponsetx.md)
* [TronApiResponse](tronapiresponse.md)
* [TronInput](troninput.md)
* [TronTransactionInput](trontransactioninput.md)
* [TronTransactionOutput](trontransactionoutput.md)
* [Tx](tx.md)
* [UniswapInput](uniswapinput.md)

To get access to the crate's generated documentation, use:

```
cargo doc --open
```

## Author