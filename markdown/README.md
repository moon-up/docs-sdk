# Documentation for moon-vault-api

<a name="documentation-for-api-endpoints"></a>
## Documentation for API Endpoints

All URIs are relative to *https://beta.usemoon.ai*

| Class | Method | HTTP request | Description |
|------------ | ------------- | ------------- | -------------|
| *AaveApi* | [**borrow**](Apis/AaveApi.md#borrow) | **POST** /aave/{name}/borrow |  |
*AaveApi* | [**lend**](Apis/AaveApi.md#lend) | **POST** /aave/{name}/lend |  |
*AaveApi* | [**repay**](Apis/AaveApi.md#repay) | **POST** /aave/{name}/repay |  |
*AaveApi* | [**userReserveData**](Apis/AaveApi.md#userreservedata) | **POST** /aave/{name}/user-reserve-data |  |
| *AccountsApi* | [**broadcastTx**](Apis/AccountsApi.md#broadcasttx) | **POST** /accounts/{accountName}/broadcast-tx |  |
*AccountsApi* | [**createAccount**](Apis/AccountsApi.md#createaccount) | **POST** /accounts |  |
*AccountsApi* | [**deleteAccount**](Apis/AccountsApi.md#deleteaccount) | **DELETE** /accounts/{accountName} |  |
*AccountsApi* | [**deployContract**](Apis/AccountsApi.md#deploycontract) | **POST** /accounts/{accountName}/deploy |  |
*AccountsApi* | [**getAccount**](Apis/AccountsApi.md#getaccount) | **GET** /accounts/{accountName} |  |
*AccountsApi* | [**getBalance**](Apis/AccountsApi.md#getbalance) | **GET** /accounts/{accountName}/balance |  |
*AccountsApi* | [**getNonce**](Apis/AccountsApi.md#getnonce) | **GET** /accounts/{accountName}/nonce |  |
*AccountsApi* | [**listAccounts**](Apis/AccountsApi.md#listaccounts) | **GET** /accounts |  |
*AccountsApi* | [**signMessage**](Apis/AccountsApi.md#signmessage) | **POST** /accounts/{accountName}/sign-message |  |
*AccountsApi* | [**signTransaction**](Apis/AccountsApi.md#signtransaction) | **POST** /accounts/{accountName}/sign-transaction |  |
*AccountsApi* | [**signTypedData**](Apis/AccountsApi.md#signtypeddata) | **POST** /accounts/{accountName}/sign-typed-data |  |
*AccountsApi* | [**transferEth**](Apis/AccountsApi.md#transfereth) | **POST** /accounts/{accountName}/transfer-eth |  |
| *BitcoinApi* | [**createBitcoinAccount**](Apis/BitcoinApi.md#createbitcoinaccount) | **POST** /bitcoin |  |
*BitcoinApi* | [**getBitcoinAccount**](Apis/BitcoinApi.md#getbitcoinaccount) | **GET** /bitcoin/{accountName} |  |
*BitcoinApi* | [**listBitcoinAccounts**](Apis/BitcoinApi.md#listbitcoinaccounts) | **GET** /bitcoin |  |
*BitcoinApi* | [**signBitcoinTransaction**](Apis/BitcoinApi.md#signbitcointransaction) | **POST** /bitcoin/{accountName}/sign-tx |  |
| *BitcoincashApi* | [**createBitcoinCashAccount**](Apis/BitcoincashApi.md#createbitcoincashaccount) | **POST** /bitcoincash |  |
*BitcoincashApi* | [**getBitcoinCashAccount**](Apis/BitcoincashApi.md#getbitcoincashaccount) | **GET** /bitcoincash/{accountName} |  |
*BitcoincashApi* | [**listBitcoinCashAccounts**](Apis/BitcoincashApi.md#listbitcoincashaccounts) | **GET** /bitcoincash |  |
*BitcoincashApi* | [**signBitcoinCashTransaction**](Apis/BitcoincashApi.md#signbitcoincashtransaction) | **POST** /bitcoincash/{accountName}/sign-tx |  |
| *ConveyorFinanceApi* | [**swap**](Apis/ConveyorFinanceApi.md#swap) | **POST** /conveyorfinance/{name}/swap |  |
| *CosmosApi* | [**createCosmosAccount**](Apis/CosmosApi.md#createcosmosaccount) | **POST** /cosmos |  |
*CosmosApi* | [**getCosmosAccount**](Apis/CosmosApi.md#getcosmosaccount) | **GET** /cosmos/{accountName} |  |
*CosmosApi* | [**listCosmosAccounts**](Apis/CosmosApi.md#listcosmosaccounts) | **GET** /cosmos |  |
*CosmosApi* | [**signCosmosTransaction**](Apis/CosmosApi.md#signcosmostransaction) | **POST** /cosmos/{accountName}/sign-tx |  |
| *DefaultApi* | [**getMessage**](Apis/DefaultApi.md#getmessage) | **GET** /ping |  |
| *DogeCoinApi* | [**createDogeCoinAccount**](Apis/DogeCoinApi.md#createdogecoinaccount) | **POST** /dogecoin |  |
*DogeCoinApi* | [**getDogeCoinAccount**](Apis/DogeCoinApi.md#getdogecoinaccount) | **GET** /dogecoin/{accountName} |  |
*DogeCoinApi* | [**listDogeCoinAccounts**](Apis/DogeCoinApi.md#listdogecoinaccounts) | **GET** /dogecoin |  |
*DogeCoinApi* | [**signDogeCoinTransaction**](Apis/DogeCoinApi.md#signdogecointransaction) | **POST** /dogecoin/{accountName}/sign-tx |  |
| *ENSApi* | [**resolve**](Apis/ENSApi.md#resolve) | **POST** /ens/resolve |  |
| *ERC1155Api* | [**balanceOf**](Apis/ERC1155Api.md#balanceof) | **POST** /erc1155/{name}/balance-of |  |
*ERC1155Api* | [**balanceOfBatch**](Apis/ERC1155Api.md#balanceofbatch) | **POST** /erc1155/{name}/balance-of-batch |  |
*ERC1155Api* | [**isApprovedForAll**](Apis/ERC1155Api.md#isapprovedforall) | **POST** /erc1155/{name}/is-approved-for-all |  |
*ERC1155Api* | [**safeBatchTransferFrom**](Apis/ERC1155Api.md#safebatchtransferfrom) | **POST** /erc1155/{name}/safe-batch-transfer-from |  |
*ERC1155Api* | [**safeTransferFrom**](Apis/ERC1155Api.md#safetransferfrom) | **POST** /erc1155/{name}/safe-transfer-from |  |
*ERC1155Api* | [**setApprovalForAll**](Apis/ERC1155Api.md#setapprovalforall) | **POST** /erc1155/{name}/set-approval-for-all |  |
| *EosApi* | [**createEosAccount**](Apis/EosApi.md#createeosaccount) | **POST** /eos |  |
*EosApi* | [**getEosAccount**](Apis/EosApi.md#geteosaccount) | **GET** /eos/{accountName} |  |
*EosApi* | [**listEosAccounts**](Apis/EosApi.md#listeosaccounts) | **GET** /eos |  |
*EosApi* | [**signEosTransaction**](Apis/EosApi.md#signeostransaction) | **POST** /eos/{accountName}/sign-tx |  |
| *Erc20Api* | [**allowanceErc20**](Apis/Erc20Api.md#allowanceerc20) | **POST** /erc20/{name}/allowance |  |
*Erc20Api* | [**approveErc20**](Apis/Erc20Api.md#approveerc20) | **POST** /erc20/{name}/approve |  |
*Erc20Api* | [**balanceOfErc20**](Apis/Erc20Api.md#balanceoferc20) | **POST** /erc20/{name}/balance-of |  |
*Erc20Api* | [**decimalsErc20**](Apis/Erc20Api.md#decimalserc20) | **POST** /erc20/{name}/decimals |  |
*Erc20Api* | [**nameErc20**](Apis/Erc20Api.md#nameerc20) | **POST** /erc20/{name}/name |  |
*Erc20Api* | [**symbolErc20**](Apis/Erc20Api.md#symbolerc20) | **POST** /erc20/{name}/symbol |  |
*Erc20Api* | [**totalSupplyErc20**](Apis/Erc20Api.md#totalsupplyerc20) | **POST** /erc20/{name}/total-supply |  |
*Erc20Api* | [**transferErc20**](Apis/Erc20Api.md#transfererc20) | **POST** /erc20/{name}/transfer |  |
*Erc20Api* | [**transferFromErc20**](Apis/Erc20Api.md#transferfromerc20) | **POST** /erc20/{name}/transfer-from |  |
| *Erc721Api* | [**approve**](Apis/Erc721Api.md#approve) | **POST** /erc721/{name}/approve |  |
*Erc721Api* | [**balanceOf**](Apis/Erc721Api.md#balanceof) | **POST** /erc721/{name}/balance-of |  |
*Erc721Api* | [**getApproved**](Apis/Erc721Api.md#getapproved) | **POST** /erc721/{name}/get-approved |  |
*Erc721Api* | [**isApprovedForAll**](Apis/Erc721Api.md#isapprovedforall) | **POST** /erc721/{name}/is-approved-for-all |  |
*Erc721Api* | [**name**](Apis/Erc721Api.md#name) | **POST** /erc721/{name}/name |  |
*Erc721Api* | [**ownerOf**](Apis/Erc721Api.md#ownerof) | **POST** /erc721/{name}/owner-of |  |
*Erc721Api* | [**safeTransferFrom**](Apis/Erc721Api.md#safetransferfrom) | **POST** /erc721/{name}/safe-transfer-from |  |
*Erc721Api* | [**setApprovalForAll**](Apis/Erc721Api.md#setapprovalforall) | **POST** /erc721/{name}/set-approval-for-all |  |
*Erc721Api* | [**symbol**](Apis/Erc721Api.md#symbol) | **POST** /erc721/{name}/symbol |  |
*Erc721Api* | [**tokenUri**](Apis/Erc721Api.md#tokenuri) | **POST** /erc721/{name}/token-uri |  |
*Erc721Api* | [**transfer**](Apis/Erc721Api.md#transfer) | **POST** /erc721/{name}/transfer |  |
*Erc721Api* | [**transferFrom**](Apis/Erc721Api.md#transferfrom) | **POST** /erc721/{name}/transfer-from |  |
| *LitecoinApi* | [**createLitecoinAccount**](Apis/LitecoinApi.md#createlitecoinaccount) | **POST** /litecoin |  |
*LitecoinApi* | [**getLitecoinAccount**](Apis/LitecoinApi.md#getlitecoinaccount) | **GET** /litecoin/{accountName} |  |
*LitecoinApi* | [**listLitecoinAccounts**](Apis/LitecoinApi.md#listlitecoinaccounts) | **GET** /litecoin |  |
*LitecoinApi* | [**signLitecoinTransaction**](Apis/LitecoinApi.md#signlitecointransaction) | **POST** /litecoin/{accountName}/sign-tx |  |
| *OneinchApi* | [**approveCallData**](Apis/OneinchApi.md#approvecalldata) | **POST** /oneinch/approve-call-data |  |
*OneinchApi* | [**approveSpender**](Apis/OneinchApi.md#approvespender) | **POST** /oneinch/approve-spender |  |
*OneinchApi* | [**protocols**](Apis/OneinchApi.md#protocols) | **POST** /oneinch/protocols |  |
*OneinchApi* | [**quote**](Apis/OneinchApi.md#quote) | **POST** /oneinch/quote |  |
*OneinchApi* | [**swap**](Apis/OneinchApi.md#swap) | **POST** /oneinch/{accountName}/swap |  |
*OneinchApi* | [**tokens**](Apis/OneinchApi.md#tokens) | **POST** /oneinch/tokens |  |
| *OnramperApi* | [**onRamperCheckout**](Apis/OnramperApi.md#onrampercheckout) | **POST** /onramper/fund/${accountName} |  |
*OnramperApi* | [**onRamperGetQuotesBuy**](Apis/OnramperApi.md#onrampergetquotesbuy) | **GET** /onramper/quotes/buy |  |
*OnramperApi* | [**onRamperGetQuotesSell**](Apis/OnramperApi.md#onrampergetquotessell) | **GET** /onramper/quotes/sell |  |
*OnramperApi* | [**onRamperGetSupportedAssets**](Apis/OnramperApi.md#onrampergetsupportedassets) | **GET** /onramper/assets |  |
*OnramperApi* | [**onRamperGetSupportedCurrencies**](Apis/OnramperApi.md#onrampergetsupportedcurrencies) | **GET** /onramper/currencies |  |
*OnramperApi* | [**onRamperGetSupportedDefaultsAll**](Apis/OnramperApi.md#onrampergetsupporteddefaultsall) | **GET** /onramper/defaults |  |
*OnramperApi* | [**onRamperGetSupportedOnRampsAll**](Apis/OnramperApi.md#onrampergetsupportedonrampsall) | **GET** /onramper/onramps |  |
*OnramperApi* | [**onRamperGetSupportedPaymentTypes**](Apis/OnramperApi.md#onrampergetsupportedpaymenttypes) | **GET** /onramper/payment-types |  |
*OnramperApi* | [**onRamperGetSupportedPaymentTypesFiat**](Apis/OnramperApi.md#onrampergetsupportedpaymenttypesfiat) | **GET** /onramper/payment-types/fiat |  |
| *RippleApi* | [**createRippleAccount**](Apis/RippleApi.md#createrippleaccount) | **POST** /ripple |  |
*RippleApi* | [**getRippleAccount**](Apis/RippleApi.md#getrippleaccount) | **GET** /ripple/{accountName} |  |
*RippleApi* | [**listRippleAccounts**](Apis/RippleApi.md#listrippleaccounts) | **GET** /ripple |  |
*RippleApi* | [**signRippleTransaction**](Apis/RippleApi.md#signrippletransaction) | **POST** /ripple/{accountName}/sign-tx |  |
| *SolanaApi* | [**createSolanaAccount**](Apis/SolanaApi.md#createsolanaaccount) | **POST** /solana |  |
*SolanaApi* | [**getSolanaAccount**](Apis/SolanaApi.md#getsolanaaccount) | **GET** /solana/{accountName} |  |
*SolanaApi* | [**listSolanaAccounts**](Apis/SolanaApi.md#listsolanaaccounts) | **GET** /solana |  |
*SolanaApi* | [**signSolanaTransaction**](Apis/SolanaApi.md#signsolanatransaction) | **POST** /solana/{accountName}/sign-tx |  |
| *TronApi* | [**createTronAccount**](Apis/TronApi.md#createtronaccount) | **POST** /tron |  |
*TronApi* | [**getTronAccount**](Apis/TronApi.md#gettronaccount) | **GET** /tron/{accountName} |  |
*TronApi* | [**listTronAccounts**](Apis/TronApi.md#listtronaccounts) | **GET** /tron |  |
*TronApi* | [**signTronTransaction**](Apis/TronApi.md#signtrontransaction) | **POST** /tron/{accountName}/sign-tx |  |
| *UniSwapApi* | [**addLiquidity**](Apis/UniSwapApi.md#addliquidity) | **POST** /uniswap/{name}/add-liquidity |  |
*UniSwapApi* | [**removeLiquidity**](Apis/UniSwapApi.md#removeliquidity) | **POST** /uniswap/{name}/remove-liquidity |  |
*UniSwapApi* | [**swapExactETHForTokens**](Apis/UniSwapApi.md#swapexactethfortokens) | **POST** /uniswap/{name}/swap-exact-eth-for-tokens |  |
*UniSwapApi* | [**swapExactTokensForTokens**](Apis/UniSwapApi.md#swapexacttokensfortokens) | **POST** /uniswap/{name}/swap-exact-tokens-for-tokens |  |
| *YearnApi* | [**addLiquidity**](Apis/YearnApi.md#addliquidity) | **POST** /yearn/{name}/add-liquidity |  |
*YearnApi* | [**addLiquidityWeth**](Apis/YearnApi.md#addliquidityweth) | **POST** /yearn/{name}/add-liquidity-weth |  |
*YearnApi* | [**removeLiquidity**](Apis/YearnApi.md#removeliquidity) | **POST** /yearn/{name}/remove-liquidity |  |
*YearnApi* | [**removeLiquidityWeth**](Apis/YearnApi.md#removeliquidityweth) | **POST** /yearn/{name}/remove-liquidity-weth |  |


<a name="documentation-for-models"></a>
## Documentation for Models

 - [AaveInput](./Models/AaveInput.md)
 - [AaveReservesAPIResponse](./Models/AaveReservesAPIResponse.md)
 - [AaveReservesData](./Models/AaveReservesData.md)
 - [AccountAPIResponse](./Models/AccountAPIResponse.md)
 - [AccountData](./Models/AccountData.md)
 - [AccountResponse](./Models/AccountResponse.md)
 - [AvailablePaymentMethod](./Models/AvailablePaymentMethod.md)
 - [BalanceAPIResponse](./Models/BalanceAPIResponse.md)
 - [BalanceResponse](./Models/BalanceResponse.md)
 - [BitcoinAPIResponse](./Models/BitcoinAPIResponse.md)
 - [BitcoinCashAPIResponse](./Models/BitcoinCashAPIResponse.md)
 - [BitcoinCashInput](./Models/BitcoinCashInput.md)
 - [BitcoinCashTransactionInput](./Models/BitcoinCashTransactionInput.md)
 - [BitcoinCashTransactionOutput](./Models/BitcoinCashTransactionOutput.md)
 - [BitcoinInput](./Models/BitcoinInput.md)
 - [BitcoinTransactionInput](./Models/BitcoinTransactionInput.md)
 - [BitcoinTransactionOutput](./Models/BitcoinTransactionOutput.md)
 - [BroadCastRawTransactionAPIResponse](./Models/BroadCastRawTransactionAPIResponse.md)
 - [BroadCastRawTransactionResponse](./Models/BroadCastRawTransactionResponse.md)
 - [BroadcastInput](./Models/BroadcastInput.md)
 - [ConveyorFinanceControllerResponse](./Models/ConveyorFinanceControllerResponse.md)
 - [CosmosAPIResponse](./Models/CosmosAPIResponse.md)
 - [CosmosInput](./Models/CosmosInput.md)
 - [CosmosTransactionInput](./Models/CosmosTransactionInput.md)
 - [CosmosTransactionOutput](./Models/CosmosTransactionOutput.md)
 - [CreateAccountInput](./Models/CreateAccountInput.md)
 - [CryptoCurrency](./Models/CryptoCurrency.md)
 - [DeployInput](./Models/DeployInput.md)
 - [DogeCoinAPIResponse](./Models/DogeCoinAPIResponse.md)
 - [DogeCoinInput](./Models/DogeCoinInput.md)
 - [DogeCoinTransactionInput](./Models/DogeCoinTransactionInput.md)
 - [DogeCoinTransactionOutput](./Models/DogeCoinTransactionOutput.md)
 - [EnsResolveAPIResponse](./Models/EnsResolveAPIResponse.md)
 - [EnsResolveInput](./Models/EnsResolveInput.md)
 - [EnsResolveResponse](./Models/EnsResolveResponse.md)
 - [EosAPIResponse](./Models/EosAPIResponse.md)
 - [EosInput](./Models/EosInput.md)
 - [EosTransactionInput](./Models/EosTransactionInput.md)
 - [EosTransactionOutput](./Models/EosTransactionOutput.md)
 - [Erc1155Request](./Models/Erc1155Request.md)
 - [Erc721Request](./Models/Erc721Request.md)
 - [FiatCurrency](./Models/FiatCurrency.md)
 - [GetSupportedOnRampsResponse](./Models/GetSupportedOnRampsResponse.md)
 - [GetSupportedOnRampsResponse_message_inner](./Models/GetSupportedOnRampsResponse_message_inner.md)
 - [GetSupportedOnRampsResponse_message_inner_icons](./Models/GetSupportedOnRampsResponse_message_inner_icons.md)
 - [GetSupportedOnRampsResponse_message_inner_icons_png](./Models/GetSupportedOnRampsResponse_message_inner_icons_png.md)
 - [GetSwapDto](./Models/GetSwapDto.md)
 - [InputBody](./Models/InputBody.md)
 - [LitecoinAPIResponse](./Models/LitecoinAPIResponse.md)
 - [LitecoinInput](./Models/LitecoinInput.md)
 - [LitecoinTransactionInput](./Models/LitecoinTransactionInput.md)
 - [LitecoinTransactionOutput](./Models/LitecoinTransactionOutput.md)
 - [Message](./Models/Message.md)
 - [NonceAPIResponse](./Models/NonceAPIResponse.md)
 - [NonceResponse](./Models/NonceResponse.md)
 - [PaymentType](./Models/PaymentType.md)
 - [PingResponse](./Models/PingResponse.md)
 - [Quote](./Models/Quote.md)
 - [RippleAPIResponse](./Models/RippleAPIResponse.md)
 - [RippleInput](./Models/RippleInput.md)
 - [RippleTransactionInput](./Models/RippleTransactionInput.md)
 - [RippleTransactionOutput](./Models/RippleTransactionOutput.md)
 - [SellQuote](./Models/SellQuote.md)
 - [SignMessage](./Models/SignMessage.md)
 - [SignMessageAPIResponse](./Models/SignMessageAPIResponse.md)
 - [SignTypedData](./Models/SignTypedData.md)
 - [SolanaAPIResponse](./Models/SolanaAPIResponse.md)
 - [SolanaInput](./Models/SolanaInput.md)
 - [SolanaTransactionInput](./Models/SolanaTransactionInput.md)
 - [SolanaTransactionOutput](./Models/SolanaTransactionOutput.md)
 - [SupportedAssetResponse](./Models/SupportedAssetResponse.md)
 - [SupportedAssetResponse_assets_inner](./Models/SupportedAssetResponse_assets_inner.md)
 - [SupportedCurrenciesResponse](./Models/SupportedCurrenciesResponse.md)
 - [SupportedDefaultResponse](./Models/SupportedDefaultResponse.md)
 - [SupportedDefaultResponse_defaults](./Models/SupportedDefaultResponse_defaults.md)
 - [SupportedDefaultResponse_defaults_id](./Models/SupportedDefaultResponse_defaults_id.md)
 - [SupportedPaymentTypesCurrencyResponse](./Models/SupportedPaymentTypesCurrencyResponse.md)
 - [SupportedPaymentTypesMessage](./Models/SupportedPaymentTypesMessage.md)
 - [TokenSwapParams](./Models/TokenSwapParams.md)
 - [Transaction](./Models/Transaction.md)
 - [TransactionAPIResponse](./Models/TransactionAPIResponse.md)
 - [TransactionData](./Models/TransactionData.md)
 - [TransactionInput](./Models/TransactionInput.md)
 - [TransactionInput_metaData](./Models/TransactionInput_metaData.md)
 - [TransactionInput_supportedParams](./Models/TransactionInput_supportedParams.md)
 - [TransactionInput_supportedParams_partnerData](./Models/TransactionInput_supportedParams_partnerData.md)
 - [TransactionInput_supportedParams_partnerData_redirectUrl](./Models/TransactionInput_supportedParams_partnerData_redirectUrl.md)
 - [TransactionInput_supportedParams_theme](./Models/TransactionInput_supportedParams_theme.md)
 - [TransactionInput_wallet](./Models/TransactionInput_wallet.md)
 - [TransactionRequest](./Models/TransactionRequest.md)
 - [TransactionResponse](./Models/TransactionResponse.md)
 - [TransactionResponse_info](./Models/TransactionResponse_info.md)
 - [TransactionResponse_tx](./Models/TransactionResponse_tx.md)
 - [TronAPIResponse](./Models/TronAPIResponse.md)
 - [TronInput](./Models/TronInput.md)
 - [TronTransactionInput](./Models/TronTransactionInput.md)
 - [TronTransactionOutput](./Models/TronTransactionOutput.md)
 - [Tx](./Models/Tx.md)
 - [UniswapInput](./Models/UniswapInput.md)


<a name="documentation-for-authorization"></a>
## Documentation for Authorization

<a name="BearerAuth"></a>
### BearerAuth

- **Type**: API key
- **API key parameter name**: Authorization
- **Location**: HTTP header

<a name="OAuth2"></a>
### OAuth2

- **Type**: OAuth
- **Flow**: password
- **Authorization URL**: 
- **Scopes**: 
  - authorization_code: grants authorization_code

<a name="ApiKeyAuth"></a>
### ApiKeyAuth

- **Type**: API key
- **API key parameter name**: x-api-key
- **Location**: HTTP header

