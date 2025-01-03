# Documentation for moon-vault-api

<a name="documentation-for-api-endpoints"></a>
## Documentation for API Endpoints

All URIs are relative to *https://beta.usemoon.ai*

| Class | Method | HTTP request | Description |
|------------ | ------------- | ------------- | -------------|
| *AAVEV3UIIncentiveDataProviderApi* | [**aAVEv3IncentiveDataProviderGetFullReservesData**](Apis/AAVEV3UIIncentiveDataProviderApi.md#aavev3incentivedataprovidergetfullreservesdata) | **GET** /aave/v3/incentives/fullReservesIncentiveData | Retrieves full incentive data for all reserves and user positions |
*AAVEV3UIIncentiveDataProviderApi* | [**aAVEv3IncentiveDataProviderGetReservesData**](Apis/AAVEV3UIIncentiveDataProviderApi.md#aavev3incentivedataprovidergetreservesdata) | **GET** /aave/v3/incentives/reservesIncentivesData | Retrieves incentive data for all reserves in the pool |
*AAVEV3UIIncentiveDataProviderApi* | [**aAVEv3IncentiveDataProviderGetUserReservesData**](Apis/AAVEV3UIIncentiveDataProviderApi.md#aavev3incentivedataprovidergetuserreservesdata) | **GET** /aave/v3/incentives/userReservesIncentivesData | Retrieves incentive data for a user's positions in all reserves |
| *AAVEV3UIPoolDataProviderApi* | [**aaveV3UiPoolDataProviderEthCurrencyUnit**](Apis/AAVEV3UIPoolDataProviderApi.md#aavev3uipooldataproviderethcurrencyunit) | **GET** /aave/v3/pool-data/eth-currency-unit | Retrieves the ETH currency unit from the AAVE V3 UI Pool Data Provider. |
*AAVEV3UIPoolDataProviderApi* | [**aaveV3UiPoolDataProviderMarketReferenceCurrencyPriceInUsdProxyAggregator**](Apis/AAVEV3UIPoolDataProviderApi.md#aavev3uipooldataprovidermarketreferencecurrencypriceinusdproxyaggregator) | **GET** /aave/v3/pool-data/market-reference-currency-price-in-usd-proxy-aggregator | Retrieves the market reference currency price in USD using the proxy aggregator. |
*AAVEV3UIPoolDataProviderApi* | [**aaveV3UiPoolDataProviderNetworkBaseTokenPriceInUsdProxyAggregator**](Apis/AAVEV3UIPoolDataProviderApi.md#aavev3uipooldataprovidernetworkbasetokenpriceinusdproxyaggregator) | **GET** /aave/v3/pool-data/network-base-token-price-in-usd-proxy-aggregator |  Retrieves the network base token price in USD using the proxy aggregator. |
*AAVEV3UIPoolDataProviderApi* | [**aaveV3UiPoolDataProviderReservesList**](Apis/AAVEV3UIPoolDataProviderApi.md#aavev3uipooldataproviderreserveslist) | **GET** /aave/v3/pool-data/reserves-list | Retrieves the list of reserves from the AAVE V3 UI Pool Data Provider. |
*AAVEV3UIPoolDataProviderApi* | [**aaveV3UiPoolDataProviderUserReservesData**](Apis/AAVEV3UIPoolDataProviderApi.md#aavev3uipooldataprovideruserreservesdata) | **GET** /aave/v3/pool-data/user-reserves-data | Retrieves the user's reserve data from the AAVE v3 UI Pool Data Provider. |
*AAVEV3UIPoolDataProviderApi* | [**getReservesData**](Apis/AAVEV3UIPoolDataProviderApi.md#getreservesdata) | **GET** /aave/v3/pool-data/reserves-data |  |
| *AAVEV3WalletBalanceProviderApi* | [**aaveV3WalletBalanceOf**](Apis/AAVEV3WalletBalanceProviderApi.md#aavev3walletbalanceof) | **GET** /aave/v3/wallet-balance/balance-of | Retrieves the balance of a specific token for a user from the AAVE v3 Wallet Balance Provider. |
*AAVEV3WalletBalanceProviderApi* | [**aaveV3WalletBatchBalanceOf**](Apis/AAVEV3WalletBalanceProviderApi.md#aavev3walletbatchbalanceof) | **GET** /aave/v3/wallet-balance/batch-balance-of | Retrieves the batch balance of multiple users for specified tokens. |
*AAVEV3WalletBalanceProviderApi* | [**aaveV3WalletUserWalletBalances**](Apis/AAVEV3WalletBalanceProviderApi.md#aavev3walletuserwalletbalances) | **GET** /aave/v3/wallet-balance/user-wallet-balances | Retrieves the wallet balances for a user from the AAVE v3 Wallet Balance Provider. |
| *AAVEv3PoolApi* | [**aavev3PoolBorrow**](Apis/AAVEv3PoolApi.md#aavev3poolborrow) | **POST** /aave/v3/pool/{address}/borrow | Borrows assets from the Aave pool. |
*AAVEv3PoolApi* | [**aavev3PoolGetReserveData**](Apis/AAVEv3PoolApi.md#aavev3poolgetreservedata) | **GET** /aave/v3/pool/{account}/getReserveData | Retrieves reserve data for a specific asset from the Aave pool. |
*AAVEv3PoolApi* | [**aavev3PoolGetUserAccountData**](Apis/AAVEv3PoolApi.md#aavev3poolgetuseraccountdata) | **GET** /aave/v3/pool/{account}/getUserAccountData | Retrieves user account data from the Aave pool. |
*AAVEv3PoolApi* | [**aavev3PoolLiquidationCall**](Apis/AAVEv3PoolApi.md#aavev3poolliquidationcall) | **POST** /aave/v3/pool/{address}/liquidationCall | Handles the liquidation call to the Aave pool. |
*AAVEv3PoolApi* | [**aavev3PoolRepay**](Apis/AAVEv3PoolApi.md#aavev3poolrepay) | **POST** /aave/v3/pool/{address}/repay | Repays a loan on the Aave protocol. |
*AAVEv3PoolApi* | [**aavev3PoolSetUserUseReserveAsCollateral**](Apis/AAVEv3PoolApi.md#aavev3poolsetuserusereserveascollateral) | **POST** /aave/v3/pool/{address}/setUserUseReserveAsCollateral | Sets the user's reserve as collateral in the Aave pool. |
*AAVEv3PoolApi* | [**aavev3PoolSupply**](Apis/AAVEv3PoolApi.md#aavev3poolsupply) | **POST** /aave/v3/pool/{address}/supply | Supplies assets to the Aave pool. |
*AAVEv3PoolApi* | [**aavev3PoolWithdraw**](Apis/AAVEv3PoolApi.md#aavev3poolwithdraw) | **POST** /aave/v3/pool/{address}/withdraw | Withdraws assets from the Aave pool. |
| *AAVEv3RewardsApi* | [**aAVEv3RewardsClaimAllRewards**](Apis/AAVEv3RewardsApi.md#aavev3rewardsclaimallrewards) | **POST** /aave/v3/rewards/{address}/claimAllRewards | Claims all available rewards for the specified assets |
*AAVEv3RewardsApi* | [**aAVEv3RewardsClaimAllRewardsOnBehalf**](Apis/AAVEv3RewardsApi.md#aavev3rewardsclaimallrewardsonbehalf) | **POST** /aave/v3/rewards/{address}/claimAllRewardsOnBehalf | Claims all rewards on behalf of another address |
*AAVEv3RewardsApi* | [**aAVEv3RewardsClaimAllRewardsToSelf**](Apis/AAVEv3RewardsApi.md#aavev3rewardsclaimallrewardstoself) | **POST** /aave/v3/rewards/{address}/claimAllRewardsToSelf | Claims all rewards to the calling address |
*AAVEv3RewardsApi* | [**aAVEv3RewardsClaimRewards**](Apis/AAVEv3RewardsApi.md#aavev3rewardsclaimrewards) | **POST** /aave/v3/rewards/{address}/claimRewards | Claims rewards for the specified assets and rewards |
*AAVEv3RewardsApi* | [**aAVEv3RewardsClaimRewardsOnBehalf**](Apis/AAVEv3RewardsApi.md#aavev3rewardsclaimrewardsonbehalf) | **POST** /aave/v3/rewards/{address}/claimRewardsOnBehalf | Claims rewards on behalf of another address |
*AAVEv3RewardsApi* | [**aAVEv3RewardsClaimRewardsToSelf**](Apis/AAVEv3RewardsApi.md#aavev3rewardsclaimrewardstoself) | **POST** /aave/v3/rewards/{address}/claimRewardsToSelf | Claims rewards to the calling address |
*AAVEv3RewardsApi* | [**aAVEv3RewardsGetRewardsByAsset**](Apis/AAVEv3RewardsApi.md#aavev3rewardsgetrewardsbyasset) | **GET** /aave/v3/rewards/{account}/rewardsByAsset | Retrieves all rewards for a specific asset |
*AAVEv3RewardsApi* | [**aAVEv3RewardsGetRewardsData**](Apis/AAVEv3RewardsApi.md#aavev3rewardsgetrewardsdata) | **GET** /aave/v3/rewards/{account}/rewardsData | Retrieves rewards configuration data for an asset |
*AAVEv3RewardsApi* | [**aAVEv3RewardsGetUserRewards**](Apis/AAVEv3RewardsApi.md#aavev3rewardsgetuserrewards) | **GET** /aave/v3/rewards/{account}/userRewards | Gets reward data for a specific user |
| *AccountsApi* | [**accountsBroadcastEthreeumTransaction**](Apis/AccountsApi.md#accountsbroadcastethreeumtransaction) | **POST** /accounts/{accountName}/broadcast-tx | Broadcasts a transaction using the provided account name and transaction details. |
*AccountsApi* | [**accountsCreateEthereumAccount**](Apis/AccountsApi.md#accountscreateethereumaccount) | **POST** /accounts | Creates a new account using the provided authorization token and account input data. |
*AccountsApi* | [**accountsDeleteEthereumAccount**](Apis/AccountsApi.md#accountsdeleteethereumaccount) | **DELETE** /accounts/{accountName} | Deletes an account based on the provided account name. |
*AccountsApi* | [**accountsDeployContract**](Apis/AccountsApi.md#accountsdeploycontract) | **POST** /accounts/{accountName}/deploy | Deploys a contract using the provided account name and deployment input. |
*AccountsApi* | [**accountsEncodeAbiData**](Apis/AccountsApi.md#accountsencodeabidata) | **POST** /accounts/encode-data | Encodes data using the provided ABI and function parameters. |
*AccountsApi* | [**accountsEstimateGas**](Apis/AccountsApi.md#accountsestimategas) | **POST** /accounts/{accountName}/estimate | Estimates the gas required for a transaction. |
*AccountsApi* | [**accountsEthereumGetNativeBalance**](Apis/AccountsApi.md#accountsethereumgetnativebalance) | **GET** /accounts/{accountName}/balance | Retrieves the balance of a specified account. |
*AccountsApi* | [**accountsEthereumGetNonce**](Apis/AccountsApi.md#accountsethereumgetnonce) | **GET** /accounts/{accountName}/nonce | Retrieves the nonce for a given account. |
*AccountsApi* | [**accountsExportEthreumAccount**](Apis/AccountsApi.md#accountsexportethreumaccount) | **GET** /accounts/{accountName}/export | Exports the account details including address, private key, and public key. |
*AccountsApi* | [**accountsGetEthreumAccount**](Apis/AccountsApi.md#accountsgetethreumaccount) | **GET** /accounts/{accountName} |   Retrieves the account details for a given account name. |
*AccountsApi* | [**accountsListEthereumAccounts**](Apis/AccountsApi.md#accountslistethereumaccounts) | **GET** /accounts | Lists accounts using the provided authorization token. |
*AccountsApi* | [**accountsSignEthereumTransaction**](Apis/AccountsApi.md#accountssignethereumtransaction) | **POST** /accounts/{accountName}/sign-transaction | Signs a transaction for the specified account. |
*AccountsApi* | [**accountsSignEthereumTypedData**](Apis/AccountsApi.md#accountssignethereumtypeddata) | **POST** /accounts/{accountName}/sign-typed-data | Handles the signing of typed data for a given account. |
*AccountsApi* | [**accountsSignEthreumMessage**](Apis/AccountsApi.md#accountssignethreummessage) | **POST** /accounts/{accountName}/sign-message | Signs a message using the provided account name and authorization token. |
*AccountsApi* | [**accountsSuggestGasPrice**](Apis/AccountsApi.md#accountssuggestgasprice) | **GET** /accounts/{accountName}/suggest-gas | Suggests the gas price for a given account and chain ID. |
*AccountsApi* | [**accountsTransferEth**](Apis/AccountsApi.md#accountstransfereth) | **POST** /accounts/{accountName}/transfer-eth | Transfers Ethereum from one account to another. |
| *AlloraApi* | [**getPriceInference**](Apis/AlloraApi.md#getpriceinference) | **GET** /allora/inference | Get price inference for a specific asset and timeframe |
*AlloraApi* | [**impliedFuturePrice**](Apis/AlloraApi.md#impliedfutureprice) | **GET** /allora/implied-future-price | Calculate implied future price |
*AlloraApi* | [**logReturnToPercentage**](Apis/AlloraApi.md#logreturntopercentage) | **GET** /allora/log-return-to-percentage | Convert log return to percentage |
| *BitcoinApi* | [**bitcoinBitcoinCreateAccount**](Apis/BitcoinApi.md#bitcoinbitcoincreateaccount) | **POST** /bitcoin | Creates a new Bitcoin account. |
*BitcoinApi* | [**bitcoinBitcoinCreateBRC20Transaction**](Apis/BitcoinApi.md#bitcoinbitcoincreatebrc20transaction) | **POST** /bitcoin/{accountName}/brc20-tx | Creates a BRC20 transaction. |
*BitcoinApi* | [**bitcoinBitcoinCreateSRC20Inscription**](Apis/BitcoinApi.md#bitcoinbitcoincreatesrc20inscription) | **POST** /bitcoin/{accountName}/src20-inscription | Creates an SRC20 inscription using the provided account name and inscription input. |
*BitcoinApi* | [**bitcoinBitcoinDeleteAccount**](Apis/BitcoinApi.md#bitcoinbitcoindeleteaccount) | **POST** /bitcoin/{accountName}/delete | Deletes a Bitcoin account. |
*BitcoinApi* | [**bitcoinBitcoinExportAccount**](Apis/BitcoinApi.md#bitcoinbitcoinexportaccount) | **POST** /bitcoin/{accountName}/export | Exports the account details for the specified account name. |
*BitcoinApi* | [**bitcoinBitcoinGenerateUnsignedPSBTHex**](Apis/BitcoinApi.md#bitcoinbitcoingenerateunsignedpsbthex) | **POST** /bitcoin/{accountName}/generate-unsigned-psbt | Generates an unsigned PSBT (Partially Signed Bitcoin Transaction) hex string. |
*BitcoinApi* | [**bitcoinBitcoinGetAccount**](Apis/BitcoinApi.md#bitcoinbitcoingetaccount) | **GET** /bitcoin/{accountName} | Retrieves the account information for a given account name. |
*BitcoinApi* | [**bitcoinBitcoinSignTransaction**](Apis/BitcoinApi.md#bitcoinbitcoinsigntransaction) | **POST** /bitcoin/{accountName}/sign-tx | Signs a Bitcoin transaction using the provided account name and transaction input. |
*BitcoinApi* | [**bitcoinListAccounts**](Apis/BitcoinApi.md#bitcoinlistaccounts) | **GET** /bitcoin | Lists the accounts associated with the provided authorization token. |
| *BitcoinCashApi* | [**bitcoinCashBitcoinCashCreateAccount**](Apis/BitcoinCashApi.md#bitcoincashbitcoincashcreateaccount) | **POST** /bitcoincash/accounts | Creates a new Bitcoin Cash account. |
*BitcoinCashApi* | [**bitcoinCashBitcoinCashDeleteAccount**](Apis/BitcoinCashApi.md#bitcoincashbitcoincashdeleteaccount) | **POST** /bitcoincash/accounts/{accountName}/delete | Deletes a Bitcoin Cash account. |
*BitcoinCashApi* | [**bitcoinCashBitcoinCashExportAccount**](Apis/BitcoinCashApi.md#bitcoincashbitcoincashexportaccount) | **POST** /bitcoincash/accounts/{accountName}/export | Exports the account details for the specified account name. |
*BitcoinCashApi* | [**bitcoinCashBitcoinCashGenerateUnsignedPSBTHex**](Apis/BitcoinCashApi.md#bitcoincashbitcoincashgenerateunsignedpsbthex) | **POST** /bitcoincash/accounts/{accountName}/generate-unsigned-psbt | Generates an unsigned PSBT (Partially Signed Bitcoin Transaction) hex string. |
*BitcoinCashApi* | [**bitcoinCashBitcoinCashGetAccount**](Apis/BitcoinCashApi.md#bitcoincashbitcoincashgetaccount) | **GET** /bitcoincash/accounts/{accountName} | Reads the account information for a given account name. |
*BitcoinCashApi* | [**bitcoinCashBitcoinCashSignBitcoinTransaction**](Apis/BitcoinCashApi.md#bitcoincashbitcoincashsignbitcointransaction) | **POST** /bitcoincash/accounts/{accountName}/sign-btc-tx | Signs a Bitcoin transaction for the specified account. |
*BitcoinCashApi* | [**bitcoinCashBitcoinCashSignPSBTWithKeyPathAndScriptPath**](Apis/BitcoinCashApi.md#bitcoincashbitcoincashsignpsbtwithkeypathandscriptpath) | **POST** /bitcoincash/accounts/{accountName}/sign-psbt-with-key-path-and-script-path | Signs a Partially Signed Bitcoin Transaction (PSBT) using a key path and script path. |
*BitcoinCashApi* | [**bitcoinCashBitcoinCashSignTransaction**](Apis/BitcoinCashApi.md#bitcoincashbitcoincashsigntransaction) | **POST** /bitcoincash/accounts/{accountName}/sign-tx | Signs a Bitcoin Cash transaction. |
*BitcoinCashApi* | [**bitcoinCashBitcoinCashSignTransactionWithMemo**](Apis/BitcoinCashApi.md#bitcoincashbitcoincashsigntransactionwithmemo) | **POST** /bitcoincash/accounts/{accountName}/memo-sign-tx | Signs a Bitcoin Cash transaction with a memo. |
*BitcoinCashApi* | [**bitcoinCashListAccounts**](Apis/BitcoinCashApi.md#bitcoincashlistaccounts) | **GET** /bitcoincash/accounts | Lists Bitcoin Cash accounts associated with the provided authorization token. |
| *ComponentsApi* | [**componentsCreateComponent**](Apis/ComponentsApi.md#componentscreatecomponent) | **POST** /components | Creates a new component in the database. |
*ComponentsApi* | [**componentsForceEmbedding**](Apis/ComponentsApi.md#componentsforceembedding) | **POST** /components/{id}/embedding/force | Forces the embedding of a description for a component. |
*ComponentsApi* | [**componentsGetComponent**](Apis/ComponentsApi.md#componentsgetcomponent) | **GET** /components/{id} | Retrieves a component by its ID. |
*ComponentsApi* | [**componentsGetComponentCapabilitiesDescription**](Apis/ComponentsApi.md#componentsgetcomponentcapabilitiesdescription) | **GET** /components/capabilities | Retrieves the capabilities description of components from the database. |
*ComponentsApi* | [**componentsGetComponents**](Apis/ComponentsApi.md#componentsgetcomponents) | **GET** /components | Retrieves a list of components from the database. |
*ComponentsApi* | [**componentsSearchComponents**](Apis/ComponentsApi.md#componentssearchcomponents) | **GET** /components/search | Searches for components similar to the specified query. |
*ComponentsApi* | [**componentsUpdateComponent**](Apis/ComponentsApi.md#componentsupdatecomponent) | **POST** /components/{id} |  Updates a component in the database. |
*ComponentsApi* | [**componentsUpdateEmbedding**](Apis/ComponentsApi.md#componentsupdateembedding) | **POST** /components/{id}/embedding | Updates the embedding of a component's description. |
| *CookieFunApi* | [**cookieFunGetKOLCommunity**](Apis/CookieFunApi.md#cookiefungetkolcommunity) | **GET** /cookiefun/kols/{username}/community | Retrieves community metrics for a specific KOL. |
*CookieFunApi* | [**cookieFunGetKOLList**](Apis/CookieFunApi.md#cookiefungetkollist) | **GET** /cookiefun/kols | Retrieves a list of key opinion leaders (KOLs). |
*CookieFunApi* | [**cookieFunGetKOLNetwork**](Apis/CookieFunApi.md#cookiefungetkolnetwork) | **GET** /cookiefun/kols/{username}/network | Retrieves the network information for a specific KOL. |
*CookieFunApi* | [**cookieFunGetPredictiveMetrics**](Apis/CookieFunApi.md#cookiefungetpredictivemetrics) | **GET** /cookiefun/predictive/{metric} | Retrieves predictive metrics. |
*CookieFunApi* | [**cookieFunGetTokenAnalytics**](Apis/CookieFunApi.md#cookiefungettokenanalytics) | **GET** /cookiefun/tokens/{tokenId}/analytics | Retrieves token analytics. |
*CookieFunApi* | [**cookieFunGetTrendingNarratives**](Apis/CookieFunApi.md#cookiefungettrendingnarratives) | **GET** /cookiefun/narratives/trending | Retrieves trending narratives. |
*CookieFunApi* | [**cookieFunGetTrendingTokens**](Apis/CookieFunApi.md#cookiefungettrendingtokens) | **GET** /cookiefun/tokens/trending | Retrieves trending tokens. |
*CookieFunApi* | [**cookieFunGetTrendingTweets**](Apis/CookieFunApi.md#cookiefungettrendingtweets) | **GET** /cookiefun/tweets/trending | Retrieves trending tweets. |
| *CosmosApi* | [**cosmosCosmosCreateAccount**](Apis/CosmosApi.md#cosmoscosmoscreateaccount) | **POST** /cosmos | Creates a new Cosmos account. |
*CosmosApi* | [**cosmosCosmosDeleteAccount**](Apis/CosmosApi.md#cosmoscosmosdeleteaccount) | **DELETE** /cosmos/{accountName} | Deletes an account in the Cosmos SDK. |
*CosmosApi* | [**cosmosCosmosExportAccount**](Apis/CosmosApi.md#cosmoscosmosexportaccount) | **POST** /cosmos/{accountName}/export | Exports a Cosmos account. |
*CosmosApi* | [**cosmosCosmosGetAccount**](Apis/CosmosApi.md#cosmoscosmosgetaccount) | **GET** /cosmos/{accountName} | Retrieves account information from the Cosmos SDK. |
*CosmosApi* | [**cosmosCosmosListAccounts**](Apis/CosmosApi.md#cosmoscosmoslistaccounts) | **GET** /cosmos | Lists Cosmos accounts associated with the provided authorization token. |
*CosmosApi* | [**cosmosCosmosSignIBCTransferTransaction**](Apis/CosmosApi.md#cosmoscosmossignibctransfertransaction) | **POST** /cosmos/{accountName}/sign-ibc-transfer | Signs an IBC transfer transaction for a given account. |
*CosmosApi* | [**cosmosCosmosSignMessage**](Apis/CosmosApi.md#cosmoscosmossignmessage) | **POST** /cosmos/{accountName}/sign-message | Signs a message using the Cosmos SDK. |
*CosmosApi* | [**cosmosCosmosSignTransferTransaction**](Apis/CosmosApi.md#cosmoscosmossigntransfertransaction) | **POST** /cosmos/{accountName}/sign-transfer | Signs a transfer transaction using the provided authorization token and account name. |
| *DataApi* | [**chartsGetChartAnalysis**](Apis/DataApi.md#chartsgetchartanalysis) | **GET** /data/analysis/{symbol}/{timeframe} | Retrieves the chart analysis for a given trading symbol and timeframe. |
*DataApi* | [**dataExecuteCustomSupabaseQuery**](Apis/DataApi.md#dataexecutecustomsupabasequery) | **POST** /data/query | Executes a query using the LLMSupabaseQueryGenerator and returns the result. |
*DataApi* | [**dataGetPortfolioFetchStatus**](Apis/DataApi.md#datagetportfoliofetchstatus) | **GET** /data/portfolio/status/{jobId} | Retrieves the status of a portfolio job. |
*DataApi* | [**dataGetTokensMetadata**](Apis/DataApi.md#datagettokensmetadata) | **GET** /data/token-metadata | Retrieves token metadata from the Moralis service. |
*DataApi* | [**dataGetUserDebankComplexProtocolList**](Apis/DataApi.md#datagetuserdebankcomplexprotocollist) | **GET** /data/{address}/debank/complex-protocols | Retrieves the user's complex protocol list from Debank, with Supabase caching. |
*DataApi* | [**dataGetUserDebankTokenList**](Apis/DataApi.md#datagetuserdebanktokenlist) | **GET** /data/{address}/debank/tokens | Retrieves the user's token list from Debank, with Supabase caching. |
*DataApi* | [**dataGetUserDebankTotalBalance**](Apis/DataApi.md#datagetuserdebanktotalbalance) | **GET** /data/{address}/debank/total-balance |  |
*DataApi* | [**dataGetUserWalletPortfolio**](Apis/DataApi.md#datagetuserwalletportfolio) | **GET** /data/{address}/portfolio | Retrieves the user's portfolio based on the provided wallet address. |
*DataApi* | [**dataGetWalletNFTs**](Apis/DataApi.md#datagetwalletnfts) | **GET** /data/{address}/nfts |  |
*DataApi* | [**dataGetWalletTokenBalances**](Apis/DataApi.md#datagetwallettokenbalances) | **GET** /data/{address}/balance | Retrieves the wallet balance for a given address. |
*DataApi* | [**dataGetWalletTransactionHistory**](Apis/DataApi.md#datagetwallettransactionhistory) | **GET** /data/{address}/history | Retrieves the wallet history for a given address and blockchain chain. |
*DataApi* | [**getAllDebankUserTokens**](Apis/DataApi.md#getalldebankusertokens) | **GET** /data/{address}/debank/all-tokens |  |
| *DefaultApi* | [**getMessage**](Apis/DefaultApi.md#getmessage) | **GET** /ping |  |
*DefaultApi* | [**getTools**](Apis/DefaultApi.md#gettools) | **GET** /lifi/tools | Retrieves tools based on the provided chains. |
*DefaultApi* | [**lIFIGetAllPossibleConnections**](Apis/DefaultApi.md#lifigetallpossibleconnections) | **GET** /lifi/allPossibleConnections | Retrieves all possible connections for a given chain and token. |
*DefaultApi* | [**lIFIGetChains**](Apis/DefaultApi.md#lifigetchains) | **GET** /lifi/chains | Retrieves a list of supported chains. |
*DefaultApi* | [**lIFIGetConnections**](Apis/DefaultApi.md#lifigetconnections) | **GET** /lifi/connections | Retrieves connections between specified chains and tokens. |
*DefaultApi* | [**lIFIGetQuote**](Apis/DefaultApi.md#lifigetquote) | **GET** /lifi/quote | Retrieves a quote for a token swap between different chains. |
*DefaultApi* | [**lIFIGetStatus**](Apis/DefaultApi.md#lifigetstatus) | **GET** /lifi/status | Retrieves the status of a transaction based on the provided transaction hash. |
*DefaultApi* | [**lIFIGetTokenDetails**](Apis/DefaultApi.md#lifigettokendetails) | **GET** /lifi/token | Fetches the details of a specified token on a given blockchain. |
*DefaultApi* | [**lIFIGetTokens**](Apis/DefaultApi.md#lifigettokens) | **GET** /lifi/tokens | Fetches tokens from the LiFi service. |
*DefaultApi* | [**lIFIPostQuote**](Apis/DefaultApi.md#lifipostquote) | **POST** /lifi/{accountName}/quote | Handles the retrieval of a quote for a token swap between different chains. |
| *DogeCoinApi* | [**dogeCoinListAccounts**](Apis/DogeCoinApi.md#dogecoinlistaccounts) | **GET** /dogecoin | Lists the accounts associated with the provided Dogecoin token. |
*DogeCoinApi* | [**dogecoinDogeCoinCreateNewAccount**](Apis/DogeCoinApi.md#dogecoindogecoincreatenewaccount) | **POST** /dogecoin | Creates a new Dogecoin account. |
*DogeCoinApi* | [**dogecoinDogeCoinDeleteAccount**](Apis/DogeCoinApi.md#dogecoindogecoindeleteaccount) | **POST** /dogecoin/{accountName}/delete | Deletes a Dogecoin account. |
*DogeCoinApi* | [**dogecoinDogeCoinExportAccountDetails**](Apis/DogeCoinApi.md#dogecoindogecoinexportaccountdetails) | **POST** /dogecoin/{accountName}/export | Exports the account details for a given account name. |
*DogeCoinApi* | [**dogecoinDogeCoinGetAccountDetails**](Apis/DogeCoinApi.md#dogecoindogecoingetaccountdetails) | **GET** /dogecoin/{accountName} | Retrieves the account information for a given account name. |
*DogeCoinApi* | [**dogecoinDogeCoinSignTransaction**](Apis/DogeCoinApi.md#dogecoindogecoinsigntransaction) | **POST** /dogecoin/{accountName}/sign-tx | Signs a Dogecoin transaction. |
*DogeCoinApi* | [**dogecoinDogeCoinSignTransactionWithMemo**](Apis/DogeCoinApi.md#dogecoindogecoinsigntransactionwithmemo) | **POST** /dogecoin/{accountName}/memo-sign-tx | Signs a Dogecoin transaction with a memo. |
| *ENSApi* | [**eNSResolve**](Apis/ENSApi.md#ensresolve) | **POST** /ens/resolve | Resolves an ENS (Ethereum Name Service) name to its corresponding address. |
*ENSApi* | [**eNSReverseResolve**](Apis/ENSApi.md#ensreverseresolve) | **POST** /ens/reverse | Resolves an ENS (Ethereum Name Service) address to its corresponding name. |
| *ERC1155Api* | [**erc1155Erc1155BalanceOf**](Apis/ERC1155Api.md#erc1155erc1155balanceof) | **POST** /erc1155/{name}/balance-of | Retrieves the balance of an ERC1155 token for a specific account. |
*ERC1155Api* | [**erc1155Erc1155BalanceOfBatch**](Apis/ERC1155Api.md#erc1155erc1155balanceofbatch) | **POST** /erc1155/{name}/balance-of-batch | Retrieves balances for multiple token IDs and accounts in a batch operation. |
*ERC1155Api* | [**erc1155Erc1155IsApprovedForAll**](Apis/ERC1155Api.md#erc1155erc1155isapprovedforall) | **POST** /erc1155/{name}/is-approved-for-all | Queries if an address is approved to manage all tokens of another address. |
*ERC1155Api* | [**erc1155Erc1155SafeBatchTransferFrom**](Apis/ERC1155Api.md#erc1155erc1155safebatchtransferfrom) | **POST** /erc1155/{name}/safe-batch-transfer-from | Safely transfers multiple tokens between addresses in a batch operation. |
*ERC1155Api* | [**erc1155Erc1155SafeTransferFrom**](Apis/ERC1155Api.md#erc1155erc1155safetransferfrom) | **POST** /erc1155/{name}/safe-transfer-from | Safely transfers a single token between addresses. |
*ERC1155Api* | [**erc1155Erc1155SetApprovalForAll**](Apis/ERC1155Api.md#erc1155erc1155setapprovalforall) | **POST** /erc1155/{name}/set-approval-for-all | Enables or disables approval for a third party (\"operator\") to manage all tokens. |
| *ERC20Api* | [**erc20ApproveERC20TokenSpending**](Apis/ERC20Api.md#erc20approveerc20tokenspending) | **POST** /erc20/{address}/approve | Approves a specified address to spend tokens on behalf of the user. |
*ERC20Api* | [**erc20GetERC20TokenAllowance**](Apis/ERC20Api.md#erc20geterc20tokenallowance) | **GET** /erc20/{account}/allowance | Retrieves the allowance of a specified ERC20 token for a given owner and spender. |
*ERC20Api* | [**erc20GetERC20TokenBalance**](Apis/ERC20Api.md#erc20geterc20tokenbalance) | **GET** /erc20/{account}/balanceOf | Retrieves the balance of a specified ERC20 token for a given account. |
*ERC20Api* | [**erc20GetERC20TokenDecimals**](Apis/ERC20Api.md#erc20geterc20tokendecimals) | **GET** /erc20/{account}/decimals | Retrieves the number of decimals for the provided ERC20 token. |
*ERC20Api* | [**erc20GetERC20TokenName**](Apis/ERC20Api.md#erc20geterc20tokenname) | **GET** /erc20/{account}/name | Retrieves the name of an ERC20 token. |
*ERC20Api* | [**erc20GetERC20TokenSymbol**](Apis/ERC20Api.md#erc20geterc20tokensymbol) | **GET** /erc20/{account}/symbol | Retrieves the symbol of an ERC20 token. |
*ERC20Api* | [**erc20GetERC20TokenTotalSupply**](Apis/ERC20Api.md#erc20geterc20tokentotalsupply) | **GET** /erc20/{account}/totalSupply | Retrieves the total supply of an ERC20 token. |
*ERC20Api* | [**erc20TransferERC20Token**](Apis/ERC20Api.md#erc20transfererc20token) | **POST** /erc20/{address}/transfer | Transfers ERC20 tokens to a specified address. |
*ERC20Api* | [**erc20TransferFromERC20Token**](Apis/ERC20Api.md#erc20transferfromerc20token) | **POST** /erc20/{address}/transferFrom | Transfers tokens from one address to another. |
| *ERC4626Api* | [**erc4626ApproveERC4626**](Apis/ERC4626Api.md#erc4626approveerc4626) | **POST** /erc4626/{address}/approve | Approves a spender to transfer a specific amount of shares. |
*ERC4626Api* | [**erc4626DepositToERC4626**](Apis/ERC4626Api.md#erc4626deposittoerc4626) | **POST** /erc4626/{address}/deposit | Deposits assets into the vault and mints shares to the receiver. |
*ERC4626Api* | [**erc4626GetERC4626Allowance**](Apis/ERC4626Api.md#erc4626geterc4626allowance) | **GET** /erc4626/{account}/allowance | Gets the amount of shares that an owner has allowed a spender to use. |
*ERC4626Api* | [**erc4626GetERC4626Asset**](Apis/ERC4626Api.md#erc4626geterc4626asset) | **GET** /erc4626/{account}/asset | Retrieves the underlying asset address of the ERC4626 vault. |
*ERC4626Api* | [**erc4626GetERC4626BalanceOf**](Apis/ERC4626Api.md#erc4626geterc4626balanceof) | **GET** /erc4626/{account}/balanceOf | Gets the balance of shares for an account. |
*ERC4626Api* | [**erc4626GetERC4626ConvertToAssets**](Apis/ERC4626Api.md#erc4626geterc4626converttoassets) | **GET** /erc4626/{account}/convertToAssets | Calculates the amount of assets that would be withdrawn for a given amount of shares. |
*ERC4626Api* | [**erc4626GetERC4626ConvertToShares**](Apis/ERC4626Api.md#erc4626geterc4626converttoshares) | **GET** /erc4626/{account}/convertToShares | Calculates the amount of shares that would be minted for a given amount of assets. |
*ERC4626Api* | [**erc4626GetERC4626MaxDeposit**](Apis/ERC4626Api.md#erc4626geterc4626maxdeposit) | **GET** /erc4626/{account}/maxDeposit | Returns the maximum amount of assets that can be deposited in a single transaction. |
*ERC4626Api* | [**erc4626GetERC4626MaxMint**](Apis/ERC4626Api.md#erc4626geterc4626maxmint) | **GET** /erc4626/{account}/maxMint | Returns the maximum amount of shares that can be minted in a single transaction. |
*ERC4626Api* | [**erc4626GetERC4626MaxRedeem**](Apis/ERC4626Api.md#erc4626geterc4626maxredeem) | **GET** /erc4626/{account}/maxRedeem | Returns the maximum amount of shares that can be redeemed in a single transaction. |
*ERC4626Api* | [**erc4626GetERC4626MaxWithdraw**](Apis/ERC4626Api.md#erc4626geterc4626maxwithdraw) | **GET** /erc4626/{account}/maxWithdraw | Returns the maximum amount of assets that can be withdrawn in a single transaction. |
*ERC4626Api* | [**erc4626GetERC4626PreviewDeposit**](Apis/ERC4626Api.md#erc4626geterc4626previewdeposit) | **GET** /erc4626/{account}/previewDeposit | Simulates the amount of shares that would be received for a deposit of assets. |
*ERC4626Api* | [**erc4626GetERC4626PreviewMint**](Apis/ERC4626Api.md#erc4626geterc4626previewmint) | **GET** /erc4626/{account}/previewMint | Simulates the amount of assets needed for minting a specific amount of shares. |
*ERC4626Api* | [**erc4626GetERC4626PreviewRedeem**](Apis/ERC4626Api.md#erc4626geterc4626previewredeem) | **GET** /erc4626/{account}/previewRedeem | Simulates the amount of assets that would be received for redeeming shares. |
*ERC4626Api* | [**erc4626GetERC4626PreviewWithdraw**](Apis/ERC4626Api.md#erc4626geterc4626previewwithdraw) | **GET** /erc4626/{account}/previewWithdraw | Simulates the amount of shares needed to withdraw a specific amount of assets. |
*ERC4626Api* | [**erc4626GetERC4626TotalAssets**](Apis/ERC4626Api.md#erc4626geterc4626totalassets) | **GET** /erc4626/{account}/totalAssets | Gets the total amount of underlying assets held by the vault. |
*ERC4626Api* | [**erc4626GetERC4626TotalSupply**](Apis/ERC4626Api.md#erc4626geterc4626totalsupply) | **GET** /erc4626/{account}/totalSupply | Gets the total supply of shares. |
*ERC4626Api* | [**erc4626MintERC4626Shares**](Apis/ERC4626Api.md#erc4626minterc4626shares) | **POST** /erc4626/{address}/mint | Mints shares to the receiver by depositing exact amount of assets. |
*ERC4626Api* | [**erc4626RedeemERC4626Shares**](Apis/ERC4626Api.md#erc4626redeemerc4626shares) | **POST** /erc4626/{address}/redeem | Redeems shares from owner and sends exact amount of assets to receiver. |
*ERC4626Api* | [**erc4626TransferERC4626**](Apis/ERC4626Api.md#erc4626transfererc4626) | **POST** /erc4626/{address}/transfer | Transfers shares to a specified address. |
*ERC4626Api* | [**erc4626TransferFromERC4626**](Apis/ERC4626Api.md#erc4626transferfromerc4626) | **POST** /erc4626/{address}/transferFrom | Transfers shares from one address to another. |
*ERC4626Api* | [**erc4626WithdrawFromERC4626**](Apis/ERC4626Api.md#erc4626withdrawfromerc4626) | **POST** /erc4626/{address}/withdraw | Withdraws assets from the vault to the receiver. |
| *ERC721Api* | [**erc721ApproveERC721**](Apis/ERC721Api.md#erc721approveerc721) | **POST** /erc721/{address}/approve | Approves an ERC721 token for a given address. |
*ERC721Api* | [**erc721GetERC721Approved**](Apis/ERC721Api.md#erc721geterc721approved) | **GET** /erc721/{tokenId}/getApproved | Retrieves the approved address for a specific ERC721 token. |
*ERC721Api* | [**erc721GetERC721BalanceOf**](Apis/ERC721Api.md#erc721geterc721balanceof) | **GET** /erc721/{account}/balanceOf | Retrieves the balance of ERC721 tokens for a given account. |
*ERC721Api* | [**erc721GetERC721IsApprovedForAll**](Apis/ERC721Api.md#erc721geterc721isapprovedforall) | **GET** /erc721/{owner}/{operator}/isApprovedForAll | Checks if an operator is approved to manage all assets of a given owner. |
*ERC721Api* | [**erc721GetERC721Name**](Apis/ERC721Api.md#erc721geterc721name) | **GET** /erc721/name | Retrieves the name of an ERC721 token. |
*ERC721Api* | [**erc721GetERC721OwnerOf**](Apis/ERC721Api.md#erc721geterc721ownerof) | **GET** /erc721/{tokenId}/ownerOf | Retrieves the owner of a specified ERC721 token. |
*ERC721Api* | [**erc721GetERC721Symbol**](Apis/ERC721Api.md#erc721geterc721symbol) | **GET** /erc721/symbol | Retrieves the symbol of an ERC721 token. |
*ERC721Api* | [**erc721GetERC721TokenURI**](Apis/ERC721Api.md#erc721geterc721tokenuri) | **GET** /erc721/{tokenId}/tokenURI | Retrieves the token URI for a given ERC721 token. |
*ERC721Api* | [**erc721SafeTransferFromERC721**](Apis/ERC721Api.md#erc721safetransferfromerc721) | **POST** /erc721/{address}/safeTransferFrom | Safely transfers an ERC721 token from one address to another. |
*ERC721Api* | [**erc721SafeTransferFromWithDataERC721**](Apis/ERC721Api.md#erc721safetransferfromwithdataerc721) | **POST** /erc721/{address}/safeTransferFromWithData | Safely transfers an ERC721 token from one address to another with additional data. |
*ERC721Api* | [**erc721SetApprovalForAllERC721**](Apis/ERC721Api.md#erc721setapprovalforallerc721) | **POST** /erc721/{address}/setApprovalForAll | Sets approval for all ERC721 tokens for a given address. |
*ERC721Api* | [**erc721TransferFromERC721**](Apis/ERC721Api.md#erc721transferfromerc721) | **POST** /erc721/{address}/transferFrom | Transfers an ERC721 token from one address to another. |
| *EosApi* | [**createEosAccount**](Apis/EosApi.md#createeosaccount) | **POST** /eos | Creates a new EOS account. |
*EosApi* | [**deleteEosAccount**](Apis/EosApi.md#deleteeosaccount) | **POST** /eos/{accountName}/delete | Deletes an EOS account. |
*EosApi* | [**exportEosAccount**](Apis/EosApi.md#exporteosaccount) | **POST** /eos/{accountName}/export | Exports the account information for a given EOS account name. |
*EosApi* | [**getEosAccount**](Apis/EosApi.md#geteosaccount) | **GET** /eos/{accountName} | Retrieves account information from the EOS blockchain. |
*EosApi* | [**listEosAccounts**](Apis/EosApi.md#listeosaccounts) | **GET** /eos | Lists EOS accounts associated with the provided authorization token. |
*EosApi* | [**signEosTransaction**](Apis/EosApi.md#signeostransaction) | **POST** /eos/{accountName}/sign-tx | Signs an EOS transaction. |
| *FinancialDatasetsApi* | [**financialDatasetsGetAllFinancials**](Apis/FinancialDatasetsApi.md#financialdatasetsgetallfinancials) | **GET** /financial-datasets/all-financials/{ticker} | Retrieves all financials for a given ticker symbol. |
*FinancialDatasetsApi* | [**financialDatasetsGetAvailableTickers**](Apis/FinancialDatasetsApi.md#financialdatasetsgetavailabletickers) | **GET** /financial-datasets/available-tickers | Retrieves the available tickers. |
*FinancialDatasetsApi* | [**financialDatasetsGetBalanceSheets**](Apis/FinancialDatasetsApi.md#financialdatasetsgetbalancesheets) | **GET** /financial-datasets/balance-sheets/{ticker} | Retrieves the balance sheets for a given ticker symbol. |
*FinancialDatasetsApi* | [**financialDatasetsGetCashFlowStatements**](Apis/FinancialDatasetsApi.md#financialdatasetsgetcashflowstatements) | **GET** /financial-datasets/cash-flow-statements/{ticker} | Retrieves the cash flow statements for a given ticker symbol. |
*FinancialDatasetsApi* | [**financialDatasetsGetCompanyFacts**](Apis/FinancialDatasetsApi.md#financialdatasetsgetcompanyfacts) | **GET** /financial-datasets/company-facts/{ticker} | Retrieves the company facts for a given ticker symbol. |
*FinancialDatasetsApi* | [**financialDatasetsGetIncomeStatements**](Apis/FinancialDatasetsApi.md#financialdatasetsgetincomestatements) | **GET** /financial-datasets/income-statements/{ticker} | Retrieves the income statements for a given ticker symbol. |
*FinancialDatasetsApi* | [**financialDatasetsGetInsiderTransactions**](Apis/FinancialDatasetsApi.md#financialdatasetsgetinsidertransactions) | **GET** /financial-datasets/insider-transactions/{ticker} | Retrieves the insider transactions for a given ticker symbol. |
*FinancialDatasetsApi* | [**financialDatasetsGetOptionsChain**](Apis/FinancialDatasetsApi.md#financialdatasetsgetoptionschain) | **GET** /financial-datasets/options-chain/{ticker} | Retrieves the options chain for a given ticker symbol. |
*FinancialDatasetsApi* | [**financialDatasetsGetPriceSnapshot**](Apis/FinancialDatasetsApi.md#financialdatasetsgetpricesnapshot) | **GET** /financial-datasets/price-snapshot/{ticker} | Retrieves the price snapshot for a given ticker symbol. |
*FinancialDatasetsApi* | [**financialDatasetsGetPrices**](Apis/FinancialDatasetsApi.md#financialdatasetsgetprices) | **GET** /financial-datasets/prices/{ticker} | Retrieves the price data for a given ticker symbol. |
*FinancialDatasetsApi* | [**financialDatasetsGetSegmentedRevenues**](Apis/FinancialDatasetsApi.md#financialdatasetsgetsegmentedrevenues) | **GET** /financial-datasets/segmented-revenues/{ticker} | Retrieves the segmented revenues for a given ticker symbol. |
*FinancialDatasetsApi* | [**financialDatasetsSearchFinancials**](Apis/FinancialDatasetsApi.md#financialdatasetssearchfinancials) | **POST** /financial-datasets/search-financials | Searches financials for a given search request. |
*FinancialDatasetsApi* | [**financialDatasetsSearchFinancialsByLineItems**](Apis/FinancialDatasetsApi.md#financialdatasetssearchfinancialsbylineitems) | **POST** /financial-datasets/search-line-items | Searches financials by line items. |
| *JupiterApi* | [**jUPITERCancelLimitOrders**](Apis/JupiterApi.md#jupitercancellimitorders) | **POST** /jupiter/{accountName}/cancelLimitOrders | Cancels limit orders for a given account. |
*JupiterApi* | [**jUPITERCreateLimitOrder**](Apis/JupiterApi.md#jupitercreatelimitorder) | **POST** /jupiter/{accountName}/createLimitOrder | Creates a limit order for a given account. |
*JupiterApi* | [**jUPITERGetIndexedRouteMap**](Apis/JupiterApi.md#jupitergetindexedroutemap) | **GET** /jupiter/indexedRouteMap | Retrieves the indexed route map. |
*JupiterApi* | [**jUPITERGetOpenOrders**](Apis/JupiterApi.md#jupitergetopenorders) | **GET** /jupiter/openOrders | Retrieves open orders for a given wallet address. |
*JupiterApi* | [**jUPITERGetOrderHistory**](Apis/JupiterApi.md#jupitergetorderhistory) | **GET** /jupiter/orderHistory | Retrieves order history for a given wallet address. |
*JupiterApi* | [**jUPITERGetProgramIdToLabel**](Apis/JupiterApi.md#jupitergetprogramidtolabel) | **GET** /jupiter/programIdToLabel | Retrieves the program ID to label mapping. |
*JupiterApi* | [**jUPITERGetQuote**](Apis/JupiterApi.md#jupitergetquote) | **POST** /jupiter/{accountName}/quote | Retrieves the tokens available on the Jupiter platform. |
*JupiterApi* | [**jUPITERGetSwapInstructions**](Apis/JupiterApi.md#jupitergetswapinstructions) | **POST** /jupiter/{accountName}/swapInstructions | Retrieves swap instructions for a given account. |
*JupiterApi* | [**jUPITERGetTokens**](Apis/JupiterApi.md#jupitergettokens) | **GET** /jupiter/tokens | Retrieves the tokens available on the Jupiter platform. |
*JupiterApi* | [**jUPITERSwap**](Apis/JupiterApi.md#jupiterswap) | **POST** /jupiter/{accountName}/swap | Handles the swap operation for a given account. |
| *LendingPoolApi* | [**lendingPoolBorrow**](Apis/LendingPoolApi.md#lendingpoolborrow) | **POST** /lending-pool/{accountName}/borrow | Handles the borrowing process from the lending pool. |
*LendingPoolApi* | [**lendingPoolDeposit**](Apis/LendingPoolApi.md#lendingpooldeposit) | **POST** /lending-pool/{accountName}/deposit | Handles the deposit operation for a lending pool. |
*LendingPoolApi* | [**lendingPoolFlashLoan**](Apis/LendingPoolApi.md#lendingpoolflashloan) | **POST** /lending-pool/{accountName}/flash-loan | Executes a flash loan operation on the lending pool. |
*LendingPoolApi* | [**lendingPoolGetAddressesProvider**](Apis/LendingPoolApi.md#lendingpoolgetaddressesprovider) | **GET** /lending-pool/addresses-provider | Retrieves the addresses provider from the lending pool instance. |
*LendingPoolApi* | [**lendingPoolGetFlashLoanPremiumTotal**](Apis/LendingPoolApi.md#lendingpoolgetflashloanpremiumtotal) | **GET** /lending-pool/flash-loan-premium | Retrieves the total flash loan premium for a given lending pool. |
*LendingPoolApi* | [**lendingPoolGetLendingPoolRevision**](Apis/LendingPoolApi.md#lendingpoolgetlendingpoolrevision) | **GET** /lending-pool/revision | Retrieves the revision number of a lending pool. |
*LendingPoolApi* | [**lendingPoolGetMaxNumberReserves**](Apis/LendingPoolApi.md#lendingpoolgetmaxnumberreserves) | **GET** /lending-pool/max-reserves | Retrieves the maximum number of reserves from the lending pool. |
*LendingPoolApi* | [**lendingPoolGetMaxStableRateBorrowSizePercent**](Apis/LendingPoolApi.md#lendingpoolgetmaxstablerateborrowsizepercent) | **GET** /lending-pool/max-stable-rate-borrow-size-percent | Retrieves the maximum stable rate borrow size percentage from the lending pool. |
*LendingPoolApi* | [**lendingPoolGetReserveData**](Apis/LendingPoolApi.md#lendingpoolgetreservedata) | **GET** /lending-pool/reserve-data | Retrieves reserve data for a specific asset from the lending pool. |
*LendingPoolApi* | [**lendingPoolGetReservesList**](Apis/LendingPoolApi.md#lendingpoolgetreserveslist) | **GET** /lending-pool/reserves-list | Retrieves the list of reserves from the lending pool. |
*LendingPoolApi* | [**lendingPoolGetUserAccountData**](Apis/LendingPoolApi.md#lendingpoolgetuseraccountdata) | **GET** /lending-pool/user-account-data | Retrieves user account data from the lending pool. |
*LendingPoolApi* | [**lendingPoolIsPaused**](Apis/LendingPoolApi.md#lendingpoolispaused) | **GET** /lending-pool/paused | Checks if the lending pool is paused. |
*LendingPoolApi* | [**lendingPoolLiquidationCall**](Apis/LendingPoolApi.md#lendingpoolliquidationcall) | **POST** /lending-pool/{accountName}/liquidation-call | Handles the liquidation call for a lending pool. |
*LendingPoolApi* | [**lendingPoolRepay**](Apis/LendingPoolApi.md#lendingpoolrepay) | **POST** /lending-pool/{accountName}/repay | Repays a loan in the lending pool. |
*LendingPoolApi* | [**lendingPoolSetUserUseReserveAsCollateral**](Apis/LendingPoolApi.md#lendingpoolsetuserusereserveascollateral) | **POST** /lending-pool/{accountName}/set-user-use-reserve-as-collateral | Sets the user's reserve as collateral. |
*LendingPoolApi* | [**lendingPoolSwapBorrowRateMode**](Apis/LendingPoolApi.md#lendingpoolswapborrowratemode) | **POST** /lending-pool/{accountName}/swap-borrow-rate-mode | Swaps the borrow rate mode for a given account in the lending pool. |
| *LeveragerApi* | [**leveragerDeleverageERC20**](Apis/LeveragerApi.md#leveragerdeleverageerc20) | **POST** /leverager/{accountName}/deleverage-erc20 |  |
*LeveragerApi* | [**leveragerDeleverageNative**](Apis/LeveragerApi.md#leveragerdeleveragenative) | **POST** /leverager/{accountName}/deleverage-native |  |
*LeveragerApi* | [**leveragerExecuteOperation**](Apis/LeveragerApi.md#leveragerexecuteoperation) | **POST** /leverager/{accountName}/execute-operation |  |
*LeveragerApi* | [**leveragerGetAddressesProvider**](Apis/LeveragerApi.md#leveragergetaddressesprovider) | **GET** /leverager/addresses-provider |  |
*LeveragerApi* | [**leveragerGetDefaultAdminRole**](Apis/LeveragerApi.md#leveragergetdefaultadminrole) | **GET** /leverager/default-admin-role |  |
*LeveragerApi* | [**leveragerGetLendingPool**](Apis/LeveragerApi.md#leveragergetlendingpool) | **GET** /leverager/lending-pool |  |
*LeveragerApi* | [**leveragerGetMinHF**](Apis/LeveragerApi.md#leveragergetminhf) | **GET** /leverager/min-hf |  |
*LeveragerApi* | [**leveragerGetRoleAdmin**](Apis/LeveragerApi.md#leveragergetroleadmin) | **GET** /leverager/role-admin |  |
*LeveragerApi* | [**leveragerGetWETH**](Apis/LeveragerApi.md#leveragergetweth) | **GET** /leverager/weth |  |
*LeveragerApi* | [**leveragerGrantRole**](Apis/LeveragerApi.md#leveragergrantrole) | **POST** /leverager/{accountName}/grant-role |  |
*LeveragerApi* | [**leveragerHasRole**](Apis/LeveragerApi.md#leveragerhasrole) | **GET** /leverager/has-role |  |
*LeveragerApi* | [**leveragerIsPaused**](Apis/LeveragerApi.md#leveragerispaused) | **GET** /leverager/paused |  |
*LeveragerApi* | [**leveragerLeverageERC20**](Apis/LeveragerApi.md#leveragerleverageerc20) | **POST** /leverager/{accountName}/leverage-erc20 |  |
*LeveragerApi* | [**leveragerLeverageNative**](Apis/LeveragerApi.md#leveragerleveragenative) | **POST** /leverager/{accountName}/leverage-native |  |
*LeveragerApi* | [**leveragerPause**](Apis/LeveragerApi.md#leveragerpause) | **POST** /leverager/{accountName}/pause |  |
*LeveragerApi* | [**leveragerRenounceRole**](Apis/LeveragerApi.md#leveragerrenouncerole) | **POST** /leverager/{accountName}/renounce-role |  |
*LeveragerApi* | [**leveragerRevokeRole**](Apis/LeveragerApi.md#leveragerrevokerole) | **POST** /leverager/{accountName}/revoke-role |  |
*LeveragerApi* | [**leveragerSupportsInterface**](Apis/LeveragerApi.md#leveragersupportsinterface) | **GET** /leverager/supports-interface |  |
*LeveragerApi* | [**leveragerUnpause**](Apis/LeveragerApi.md#leveragerunpause) | **POST** /leverager/{accountName}/unpause |  |
| *LitecoinApi* | [**listLitecoinAccounts**](Apis/LitecoinApi.md#listlitecoinaccounts) | **GET** /litecoin | Lists the accounts associated with the provided authorization token. |
*LitecoinApi* | [**litecoinCreateLitecoinAccount**](Apis/LitecoinApi.md#litecoincreatelitecoinaccount) | **POST** /litecoin | Creates a new Litecoin account. |
*LitecoinApi* | [**litecoinDeleteLitecoinAccount**](Apis/LitecoinApi.md#litecoindeletelitecoinaccount) | **POST** /litecoin/{accountName}/delete | Deletes a Litecoin account. |
*LitecoinApi* | [**litecoinExportLitecoinAccount**](Apis/LitecoinApi.md#litecoinexportlitecoinaccount) | **POST** /litecoin/{accountName}/export | Exports the account information for a given account name. |
*LitecoinApi* | [**litecoinGetLitecoinAccount**](Apis/LitecoinApi.md#litecoingetlitecoinaccount) | **GET** /litecoin/{accountName} | Retrieves account information for a specified account name. |
*LitecoinApi* | [**litecoinSignLitecoinTransaction**](Apis/LitecoinApi.md#litecoinsignlitecointransaction) | **POST** /litecoin/{accountName}/sign-tx | Signs a Litecoin transaction. |
*LitecoinApi* | [**litecoinSignLitecoinTransactionWithMemo**](Apis/LitecoinApi.md#litecoinsignlitecointransactionwithmemo) | **POST** /litecoin/{accountName}/memo-sign-tx | Signs a Litecoin transaction with a memo. |
| *LynexApi* | [**calculateOptimalVoteDistribution**](Apis/LynexApi.md#calculateoptimalvotedistribution) | **GET** /lynex/data/vote-distribution |  |
*LynexApi* | [**getAssetByAddress**](Apis/LynexApi.md#getassetbyaddress) | **GET** /lynex/data/assets/{address} | Retrieves an asset by its address. |
*LynexApi* | [**getAssets**](Apis/LynexApi.md#getassets) | **GET** /lynex/data/assets | Retrieves the assets using the provided authorization token. |
*LynexApi* | [**getPoolByAddress**](Apis/LynexApi.md#getpoolbyaddress) | **GET** /lynex/data/pools/{address} |  |
*LynexApi* | [**getPools**](Apis/LynexApi.md#getpools) | **GET** /lynex/data/pools |  |
*LynexApi* | [**getPoolsByType**](Apis/LynexApi.md#getpoolsbytype) | **GET** /lynex/data/pools/type/{type} |  |
*LynexApi* | [**getTopAPRPools**](Apis/LynexApi.md#gettopaprpools) | **GET** /lynex/data/pools/top-apr |  |
*LynexApi* | [**getTotalValueLocked**](Apis/LynexApi.md#gettotalvaluelocked) | **GET** /lynex/data/tvl |  |
| *LynexNFTApi* | [**approve**](Apis/LynexNFTApi.md#approve) | **POST** /lynex/nft/{address}/approve |  |
*LynexNFTApi* | [**burn**](Apis/LynexNFTApi.md#burn) | **POST** /lynex/nft/{address}/burn |  |
*LynexNFTApi* | [**checkpoint**](Apis/LynexNFTApi.md#checkpoint) | **POST** /lynex/nft/{address}/checkpoint |  |
*LynexNFTApi* | [**checkpointDelegatee**](Apis/LynexNFTApi.md#checkpointdelegatee) | **POST** /lynex/nft/{address}/checkpointDelegatee |  |
*LynexNFTApi* | [**claim**](Apis/LynexNFTApi.md#claim) | **POST** /lynex/nft/{address}/claim |  |
*LynexNFTApi* | [**createDelegatedLockFor**](Apis/LynexNFTApi.md#createdelegatedlockfor) | **POST** /lynex/nft/{address}/createDelegatedLockFor |  |
*LynexNFTApi* | [**createLock**](Apis/LynexNFTApi.md#createlock) | **POST** /lynex/nft/{address}/createLock |  |
*LynexNFTApi* | [**createLockFor**](Apis/LynexNFTApi.md#createlockfor) | **POST** /lynex/nft/{address}/createLockFor |  |
*LynexNFTApi* | [**delegate**](Apis/LynexNFTApi.md#delegate) | **POST** /lynex/nft/{address}/delegate |  |
*LynexNFTApi* | [**delegateBySig**](Apis/LynexNFTApi.md#delegatebysig) | **POST** /lynex/nft/{address}/delegateBySig |  |
*LynexNFTApi* | [**getApproved**](Apis/LynexNFTApi.md#getapproved) | **GET** /lynex/nft/getApproved |  |
*LynexNFTApi* | [**getBalanceOf**](Apis/LynexNFTApi.md#getbalanceof) | **GET** /lynex/nft/balanceOf |  |
*LynexNFTApi* | [**getBalanceOfNFT**](Apis/LynexNFTApi.md#getbalanceofnft) | **GET** /lynex/nft/balanceOfNFT |  |
*LynexNFTApi* | [**getBalanceOfNFTAt**](Apis/LynexNFTApi.md#getbalanceofnftat) | **GET** /lynex/nft/balanceOfNFTAt |  |
*LynexNFTApi* | [**getDelegates**](Apis/LynexNFTApi.md#getdelegates) | **GET** /lynex/nft/delegates |  |
*LynexNFTApi* | [**getLockDetails**](Apis/LynexNFTApi.md#getlockdetails) | **GET** /lynex/nft/lockDetails |  |
*LynexNFTApi* | [**getName**](Apis/LynexNFTApi.md#getname) | **GET** /lynex/nft/name |  |
*LynexNFTApi* | [**getOwnerOf**](Apis/LynexNFTApi.md#getownerof) | **GET** /lynex/nft/ownerOf |  |
*LynexNFTApi* | [**getPastVotes**](Apis/LynexNFTApi.md#getpastvotes) | **GET** /lynex/nft/getPastVotes |  |
*LynexNFTApi* | [**getSymbol**](Apis/LynexNFTApi.md#getsymbol) | **GET** /lynex/nft/symbol |  |
*LynexNFTApi* | [**getTokenByIndex**](Apis/LynexNFTApi.md#gettokenbyindex) | **GET** /lynex/nft/tokenByIndex |  |
*LynexNFTApi* | [**getTokenOfOwnerByIndex**](Apis/LynexNFTApi.md#gettokenofownerbyindex) | **GET** /lynex/nft/tokenOfOwnerByIndex |  |
*LynexNFTApi* | [**getTokenURI**](Apis/LynexNFTApi.md#gettokenuri) | **GET** /lynex/nft/tokenURI |  |
*LynexNFTApi* | [**getTotalNftsMinted**](Apis/LynexNFTApi.md#gettotalnftsminted) | **GET** /lynex/nft/totalNftsMinted |  |
*LynexNFTApi* | [**getTotalSupply**](Apis/LynexNFTApi.md#gettotalsupply) | **GET** /lynex/nft/totalSupply |  |
*LynexNFTApi* | [**getVestedPayout**](Apis/LynexNFTApi.md#getvestedpayout) | **GET** /lynex/nft/vestedPayout |  |
*LynexNFTApi* | [**getVestedPayoutAtTime**](Apis/LynexNFTApi.md#getvestedpayoutattime) | **GET** /lynex/nft/vestedPayoutAtTime |  |
*LynexNFTApi* | [**getVestingPayout**](Apis/LynexNFTApi.md#getvestingpayout) | **GET** /lynex/nft/vestingPayout |  |
*LynexNFTApi* | [**getVestingPeriod**](Apis/LynexNFTApi.md#getvestingperiod) | **GET** /lynex/nft/vestingPeriod |  |
*LynexNFTApi* | [**getVotes**](Apis/LynexNFTApi.md#getvotes) | **GET** /lynex/nft/getVotes |  |
*LynexNFTApi* | [**globalCheckpoint**](Apis/LynexNFTApi.md#globalcheckpoint) | **POST** /lynex/nft/{address}/globalCheckpoint |  |
*LynexNFTApi* | [**increaseLockAmount**](Apis/LynexNFTApi.md#increaselockamount) | **POST** /lynex/nft/{address}/increaseLockAmount |  |
*LynexNFTApi* | [**increaseUnlockTime**](Apis/LynexNFTApi.md#increaseunlocktime) | **POST** /lynex/nft/{address}/increaseUnlockTime |  |
*LynexNFTApi* | [**isApprovedForAll**](Apis/LynexNFTApi.md#isapprovedforall) | **GET** /lynex/nft/isApprovedForAll |  |
*LynexNFTApi* | [**merge**](Apis/LynexNFTApi.md#merge) | **POST** /lynex/nft/{address}/merge |  |
*LynexNFTApi* | [**safeTransferFrom**](Apis/LynexNFTApi.md#safetransferfrom) | **POST** /lynex/nft/{address}/safeTransferFrom |  |
*LynexNFTApi* | [**setApprovalForAll**](Apis/LynexNFTApi.md#setapprovalforall) | **POST** /lynex/nft/{address}/setApprovalForAll |  |
*LynexNFTApi* | [**setClaimApproval**](Apis/LynexNFTApi.md#setclaimapproval) | **POST** /lynex/nft/{address}/setClaimApproval |  |
*LynexNFTApi* | [**setClaimApprovalForAll**](Apis/LynexNFTApi.md#setclaimapprovalforall) | **POST** /lynex/nft/{address}/setClaimApprovalForAll |  |
*LynexNFTApi* | [**split**](Apis/LynexNFTApi.md#split) | **POST** /lynex/nft/{address}/split |  |
*LynexNFTApi* | [**transferFrom**](Apis/LynexNFTApi.md#transferfrom) | **POST** /lynex/nft/{address}/transferFrom |  |
*LynexNFTApi* | [**unlockPermanent**](Apis/LynexNFTApi.md#unlockpermanent) | **POST** /lynex/nft/{address}/unlockPermanent |  |
| *LynexRouterApi* | [**addLiquidity**](Apis/LynexRouterApi.md#addliquidity) | **POST** /lynex/router/{address}/addLiquidity |  |
*LynexRouterApi* | [**addLiquidityETH**](Apis/LynexRouterApi.md#addliquidityeth) | **POST** /lynex/router/{address}/addLiquidityETH |  |
*LynexRouterApi* | [**getAmountOut**](Apis/LynexRouterApi.md#getamountout) | **GET** /lynex/router/getAmountOut |  |
*LynexRouterApi* | [**getAmountsOut**](Apis/LynexRouterApi.md#getamountsout) | **GET** /lynex/router/getAmountsOut |  |
*LynexRouterApi* | [**getFactory**](Apis/LynexRouterApi.md#getfactory) | **GET** /lynex/router/factory |  |
*LynexRouterApi* | [**getWETH**](Apis/LynexRouterApi.md#getweth) | **GET** /lynex/router/wETH |  |
*LynexRouterApi* | [**swapExactETHForTokens**](Apis/LynexRouterApi.md#swapexactethfortokens) | **POST** /lynex/router/{address}/swapExactETHForTokens |  |
*LynexRouterApi* | [**swapExactTokensForETH**](Apis/LynexRouterApi.md#swapexacttokensforeth) | **POST** /lynex/router/{address}/swapExactTokensForETH |  |
*LynexRouterApi* | [**swapExactTokensForTokens**](Apis/LynexRouterApi.md#swapexacttokensfortokens) | **POST** /lynex/router/{address}/swapExactTokensForTokens |  |
| *LynexVoterApi* | [**claimBribes**](Apis/LynexVoterApi.md#claimbribes) | **POST** /lynex/voter/{address}/claimBribes |  |
*LynexVoterApi* | [**claimFees**](Apis/LynexVoterApi.md#claimfees) | **POST** /lynex/voter/{address}/claimFees |  |
*LynexVoterApi* | [**claimRewards**](Apis/LynexVoterApi.md#claimrewards) | **POST** /lynex/voter/{address}/claimRewards |  |
*LynexVoterApi* | [**createGauge**](Apis/LynexVoterApi.md#creategauge) | **POST** /lynex/voter/{address}/createGauge |  |
*LynexVoterApi* | [**distribute**](Apis/LynexVoterApi.md#distribute) | **POST** /lynex/voter/{address}/distribute |  |
*LynexVoterApi* | [**getLastVoted**](Apis/LynexVoterApi.md#getlastvoted) | **GET** /lynex/voter/lastVoted |  |
*LynexVoterApi* | [**getPoolVoteLength**](Apis/LynexVoterApi.md#getpoolvotelength) | **GET** /lynex/voter/poolVoteLength |  |
*LynexVoterApi* | [**getTotalWeight**](Apis/LynexVoterApi.md#gettotalweight) | **GET** /lynex/voter/totalWeight |  |
*LynexVoterApi* | [**getWeights**](Apis/LynexVoterApi.md#getweights) | **GET** /lynex/voter/weights |  |
*LynexVoterApi* | [**isGauge**](Apis/LynexVoterApi.md#isgauge) | **GET** /lynex/voter/isGauge |  |
*LynexVoterApi* | [**isWhitelisted**](Apis/LynexVoterApi.md#iswhitelisted) | **GET** /lynex/voter/isWhitelisted |  |
*LynexVoterApi* | [**killGauge**](Apis/LynexVoterApi.md#killgauge) | **POST** /lynex/voter/{address}/killGauge |  |
*LynexVoterApi* | [**notifyRewardAmount**](Apis/LynexVoterApi.md#notifyrewardamount) | **POST** /lynex/voter/{address}/notifyRewardAmount |  |
*LynexVoterApi* | [**poke**](Apis/LynexVoterApi.md#poke) | **POST** /lynex/voter/{address}/poke |  |
*LynexVoterApi* | [**reset**](Apis/LynexVoterApi.md#reset) | **POST** /lynex/voter/{address}/reset |  |
*LynexVoterApi* | [**reviveGauge**](Apis/LynexVoterApi.md#revivegauge) | **POST** /lynex/voter/{address}/reviveGauge |  |
*LynexVoterApi* | [**vote**](Apis/LynexVoterApi.md#vote) | **POST** /lynex/voter/{address}/vote |  |
*LynexVoterApi* | [**voteWithOptimalDistribution**](Apis/LynexVoterApi.md#votewithoptimaldistribution) | **POST** /lynex/voter/{address}/voteWithOptimalDistribution |  |
*LynexVoterApi* | [**whitelist**](Apis/LynexVoterApi.md#whitelist) | **POST** /lynex/voter/{address}/whitelist |  |
| *MakeFunTokenApi* | [**makeFunTokenGetCLFactory**](Apis/MakeFunTokenApi.md#makefuntokengetclfactory) | **GET** /makefuntoken/{account}/CLFactory |  |
*MakeFunTokenApi* | [**makeFunTokenGetMaxTick**](Apis/MakeFunTokenApi.md#makefuntokengetmaxtick) | **GET** /makefuntoken/{account}/maxTick |  |
*MakeFunTokenApi* | [**makeFunTokenGetMinTick**](Apis/MakeFunTokenApi.md#makefuntokengetmintick) | **GET** /makefuntoken/{account}/minTick |  |
*MakeFunTokenApi* | [**makeFunTokenMakeToken**](Apis/MakeFunTokenApi.md#makefuntokenmaketoken) | **POST** /makefuntoken/{address}/makeToken |  |
*MakeFunTokenApi* | [**makeFunTokenSetSupplyLimits**](Apis/MakeFunTokenApi.md#makefuntokensetsupplylimits) | **POST** /makefuntoken/{address}/setSupplyLimits |  |
*MakeFunTokenApi* | [**makeFunTokenSetTickLimits**](Apis/MakeFunTokenApi.md#makefuntokensetticklimits) | **POST** /makefuntoken/{address}/setTickLimits |  |
| *MultiCallApi* | [**createFlow**](Apis/MultiCallApi.md#createflow) | **POST** /multicall/flows |  |
*MultiCallApi* | [**createJob**](Apis/MultiCallApi.md#createjob) | **POST** /multicall/create-job |  |
*MultiCallApi* | [**createUserDefinedFunction**](Apis/MultiCallApi.md#createuserdefinedfunction) | **POST** /multicall/user-defined-functions |  |
*MultiCallApi* | [**deleteFlow**](Apis/MultiCallApi.md#deleteflow) | **DELETE** /multicall/flows/{flowId} |  |
*MultiCallApi* | [**deleteJob**](Apis/MultiCallApi.md#deletejob) | **DELETE** /multicall/job/{jobId} |  |
*MultiCallApi* | [**deleteUserDefinedFunction**](Apis/MultiCallApi.md#deleteuserdefinedfunction) | **DELETE** /multicall/user-defined-functions/{functionId} |  |
*MultiCallApi* | [**executeJob**](Apis/MultiCallApi.md#executejob) | **POST** /multicall/execute-job/{jobId} |  |
*MultiCallApi* | [**getFlow**](Apis/MultiCallApi.md#getflow) | **GET** /multicall/flows/{flowId} |  |
*MultiCallApi* | [**getJob**](Apis/MultiCallApi.md#getjob) | **GET** /multicall/job/{jobId} |  |
*MultiCallApi* | [**getJobResult**](Apis/MultiCallApi.md#getjobresult) | **GET** /multicall/job-result/{jobId} |  |
*MultiCallApi* | [**getNotifications**](Apis/MultiCallApi.md#getnotifications) | **GET** /multicall/notifications |  |
*MultiCallApi* | [**getScheduledJobs**](Apis/MultiCallApi.md#getscheduledjobs) | **GET** /multicall/scheduled-jobs |  |
*MultiCallApi* | [**listFlows**](Apis/MultiCallApi.md#listflows) | **GET** /multicall/flows |  |
*MultiCallApi* | [**listJobs**](Apis/MultiCallApi.md#listjobs) | **GET** /multicall/jobs |  |
*MultiCallApi* | [**listUserDefinedFunctions**](Apis/MultiCallApi.md#listuserdefinedfunctions) | **GET** /multicall/user-defined-functions |  |
*MultiCallApi* | [**markNotificationAsRead**](Apis/MultiCallApi.md#marknotificationasread) | **POST** /multicall/notifications/{notificationId}/mark-as-read |  |
*MultiCallApi* | [**scheduleJob**](Apis/MultiCallApi.md#schedulejob) | **POST** /multicall/schedule-job |  |
*MultiCallApi* | [**unscheduleJob**](Apis/MultiCallApi.md#unschedulejob) | **POST** /multicall/unschedule-job/{jobId} |  |
*MultiCallApi* | [**updateFlow**](Apis/MultiCallApi.md#updateflow) | **PUT** /multicall/flows/{flowId} |  |
| *OdosApi* | [**getZapQuote**](Apis/OdosApi.md#getzapquote) | **POST** /odos/{accountName}/get-zap-quote |  |
*OdosApi* | [**oDOSAssembleTransaction**](Apis/OdosApi.md#odosassembletransaction) | **POST** /odos/assemble-transaction | Assembles a transaction using the provided authorization token and request body. |
*OdosApi* | [**oDOSGetContractInfo**](Apis/OdosApi.md#odosgetcontractinfo) | **GET** /odos/contract-info | Retrieves contract information from the Odos API. |
*OdosApi* | [**oDOSGetCurrentBlock**](Apis/OdosApi.md#odosgetcurrentblock) | **GET** /odos/current-block | Retrieves the current block information for a given blockchain. |
*OdosApi* | [**oDOSGetExecutorAddress**](Apis/OdosApi.md#odosgetexecutoraddress) | **GET** /odos/executor-address | Retrieves the executor address from the Odos API. |
*OdosApi* | [**oDOSGetLiquiditySources**](Apis/OdosApi.md#odosgetliquiditysources) | **GET** /odos/liquidity-sources | Retrieves liquidity sources for a given chain ID. |
*OdosApi* | [**oDOSGetQuote**](Apis/OdosApi.md#odosgetquote) | **POST** /odos/{accountName}/get-quote | Retrieves a quote for a given account and input body. |
*OdosApi* | [**oDOSGetRouterAddress**](Apis/OdosApi.md#odosgetrouteraddress) | **GET** /odos/router-address | Retrieves the router address for the specified version and chain ID. |
*OdosApi* | [**oDOSGetSupportedChains**](Apis/OdosApi.md#odosgetsupportedchains) | **GET** /odos/supported-chains | Retrieves the supported blockchain networks from the Odos API. |
*OdosApi* | [**oDOSGetSupportedTokens**](Apis/OdosApi.md#odosgetsupportedtokens) | **GET** /odos/supported-tokens | Retrieves the supported tokens for a given blockchain network. |
*OdosApi* | [**oDOSSwapTokens**](Apis/OdosApi.md#odosswaptokens) | **POST** /odos/{accountName}/swap | Handles the swap operation for the given account. |
*OdosApi* | [**zap**](Apis/OdosApi.md#zap) | **POST** /odos/{accountName}/zap |  |
| *OnramperApi* | [**onRamperCheckout**](Apis/OnramperApi.md#onrampercheckout) | **POST** /onramper/fund/${accountName} |  |
*OnramperApi* | [**onRamperGetQuotesBuy**](Apis/OnramperApi.md#onrampergetquotesbuy) | **GET** /onramper/quotes/buy |  |
*OnramperApi* | [**onRamperGetQuotesSell**](Apis/OnramperApi.md#onrampergetquotessell) | **GET** /onramper/quotes/sell |  |
*OnramperApi* | [**onRamperGetSupportedAssets**](Apis/OnramperApi.md#onrampergetsupportedassets) | **GET** /onramper/assets |  |
*OnramperApi* | [**onRamperGetSupportedCurrencies**](Apis/OnramperApi.md#onrampergetsupportedcurrencies) | **GET** /onramper/currencies |  |
*OnramperApi* | [**onRamperGetSupportedDefaultsAll**](Apis/OnramperApi.md#onrampergetsupporteddefaultsall) | **GET** /onramper/defaults |  |
*OnramperApi* | [**onRamperGetSupportedOnRampsAll**](Apis/OnramperApi.md#onrampergetsupportedonrampsall) | **GET** /onramper/onramps |  |
*OnramperApi* | [**onRamperGetSupportedPaymentTypes**](Apis/OnramperApi.md#onrampergetsupportedpaymenttypes) | **GET** /onramper/payment-types |  |
*OnramperApi* | [**onRamperGetSupportedPaymentTypesFiat**](Apis/OnramperApi.md#onrampergetsupportedpaymenttypesfiat) | **GET** /onramper/payment-types/fiat |  |
| *OpenSeaApi* | [**createCollectionOffer**](Apis/OpenSeaApi.md#createcollectionoffer) | **POST** /opensea/{account}/createCollectionOffer |  |
*OpenSeaApi* | [**createOffer**](Apis/OpenSeaApi.md#createoffer) | **POST** /opensea/{account}/createOffer |  |
*OpenSeaApi* | [**getCollection**](Apis/OpenSeaApi.md#getcollection) | **GET** /opensea/{account}/collection/{slug} |  |
*OpenSeaApi* | [**getNFT**](Apis/OpenSeaApi.md#getnft) | **GET** /opensea/{account}/nft/{address}/{tokenId} |  |
*OpenSeaApi* | [**unwrapWeth**](Apis/OpenSeaApi.md#unwrapweth) | **POST** /opensea/{account}/unwrapWeth |  |
*OpenSeaApi* | [**wrapEth**](Apis/OpenSeaApi.md#wrapeth) | **POST** /opensea/{account}/wrapEth |  |
| *PolymarketApi* | [**approveForPolymarket**](Apis/PolymarketApi.md#approveforpolymarket) | **POST** /polymarket/{account}/approveForPolymarket |  |
*PolymarketApi* | [**cancelMarketOrders**](Apis/PolymarketApi.md#cancelmarketorders) | **POST** /polymarket/{account}/cancelMarketOrders |  |
*PolymarketApi* | [**cancelOrder**](Apis/PolymarketApi.md#cancelorder) | **POST** /polymarket/{account}/cancelOrder |  |
*PolymarketApi* | [**cancelOrders**](Apis/PolymarketApi.md#cancelorders) | **POST** /polymarket/{account}/cancelOrders |  |
*PolymarketApi* | [**createMarketBuyOrder**](Apis/PolymarketApi.md#createmarketbuyorder) | **POST** /polymarket/{account}/createMarketBuyOrder |  |
*PolymarketApi* | [**createOrder**](Apis/PolymarketApi.md#createorder) | **POST** /polymarket/{account}/createOrder |  |
*PolymarketApi* | [**dropNotifications**](Apis/PolymarketApi.md#dropnotifications) | **POST** /polymarket/{account}/dropNotifications |  |
*PolymarketApi* | [**getBalanceAllowance**](Apis/PolymarketApi.md#getbalanceallowance) | **GET** /polymarket/{account}/balanceAllowance |  |
*PolymarketApi* | [**getMarket**](Apis/PolymarketApi.md#getmarket) | **GET** /polymarket/{account}/market/{conditionID} |  |
*PolymarketApi* | [**getMarketTradeEvents**](Apis/PolymarketApi.md#getmarkettradeevents) | **GET** /polymarket/{account}/marketTradeEvents/{conditionID} |  |
*PolymarketApi* | [**getMarkets**](Apis/PolymarketApi.md#getmarkets) | **GET** /polymarket/{account}/markets |  |
*PolymarketApi* | [**getNotifications**](Apis/PolymarketApi.md#getnotifications) | **GET** /polymarket/{account}/notifications |  |
*PolymarketApi* | [**getOpenOrders**](Apis/PolymarketApi.md#getopenorders) | **GET** /polymarket/{account}/openOrders |  |
*PolymarketApi* | [**getOrder**](Apis/PolymarketApi.md#getorder) | **GET** /polymarket/{account}/order/{orderID} |  |
*PolymarketApi* | [**getOrderBook**](Apis/PolymarketApi.md#getorderbook) | **GET** /polymarket/{account}/orderBook |  |
*PolymarketApi* | [**getPricesHistory**](Apis/PolymarketApi.md#getpriceshistory) | **GET** /polymarket/{account}/pricesHistory |  |
*PolymarketApi* | [**getTrades**](Apis/PolymarketApi.md#gettrades) | **GET** /polymarket/{account}/trades |  |
*PolymarketApi* | [**postOrder**](Apis/PolymarketApi.md#postorder) | **POST** /polymarket/{account}/postOrder |  |
*PolymarketApi* | [**updateBalanceAllowance**](Apis/PolymarketApi.md#updatebalanceallowance) | **POST** /polymarket/{account}/updateBalanceAllowance |  |
| *PoolAddressProviderApi* | [**aavev3PoolAddressProviderGetACLAdmin**](Apis/PoolAddressProviderApi.md#aavev3pooladdressprovidergetacladmin) | **GET** /aave/v3/poolAddressProvider/{account}/getACLAdmin | Retrieves the ACL (Access Control List) admin address for a given account. |
*PoolAddressProviderApi* | [**aavev3PoolAddressProviderGetACLManager**](Apis/PoolAddressProviderApi.md#aavev3pooladdressprovidergetaclmanager) | **GET** /aave/v3/poolAddressProvider/{account}/getACLManager | Retrieves the ACL Manager address from the Pool Address Provider. |
*PoolAddressProviderApi* | [**aavev3PoolAddressProviderGetAddress**](Apis/PoolAddressProviderApi.md#aavev3pooladdressprovidergetaddress) | **GET** /aave/v3/poolAddressProvider/{account}/getAddress | Retrieves an address from the Pool Address Provider. |
*PoolAddressProviderApi* | [**aavev3PoolAddressProviderGetMarketId**](Apis/PoolAddressProviderApi.md#aavev3pooladdressprovidergetmarketid) | **GET** /aave/v3/poolAddressProvider/{account}/getMarketId | Retrieves the market ID from the Pool Address Provider. |
*PoolAddressProviderApi* | [**aavev3PoolAddressProviderGetPool**](Apis/PoolAddressProviderApi.md#aavev3pooladdressprovidergetpool) | **GET** /aave/v3/poolAddressProvider/{account}/getPool | Retrieves the pool address from the Aave protocol. |
*PoolAddressProviderApi* | [**aavev3PoolAddressProviderGetPoolConfigurator**](Apis/PoolAddressProviderApi.md#aavev3pooladdressprovidergetpoolconfigurator) | **GET** /aave/v3/poolAddressProvider/{account}/getPoolConfigurator | Retrieves the pool configurator for a given account. |
*PoolAddressProviderApi* | [**aavev3PoolAddressProviderGetPriceOracle**](Apis/PoolAddressProviderApi.md#aavev3pooladdressprovidergetpriceoracle) | **GET** /aave/v3/poolAddressProvider/{account}/getPriceOracle | Retrieves the price oracle address from the Aave pool address provider. |
*PoolAddressProviderApi* | [**aavev3PoolAddressProviderSetACLAdmin**](Apis/PoolAddressProviderApi.md#aavev3pooladdressprovidersetacladmin) | **POST** /aave/v3/poolAddressProvider/{address}/setACLAdmin | Sets the ACL (Access Control List) admin for the specified address. |
*PoolAddressProviderApi* | [**aavev3PoolAddressProviderSetACLManager**](Apis/PoolAddressProviderApi.md#aavev3pooladdressprovidersetaclmanager) | **POST** /aave/v3/poolAddressProvider/{address}/setACLManager | Sets the ACL Manager for the specified pool address provider. |
*PoolAddressProviderApi* | [**aavev3PoolAddressProviderSetAddress**](Apis/PoolAddressProviderApi.md#aavev3pooladdressprovidersetaddress) | **POST** /aave/v3/poolAddressProvider/{address}/setAddress | Sets the address for the Pool Address Provider. |
*PoolAddressProviderApi* | [**aavev3PoolAddressProviderSetMarketId**](Apis/PoolAddressProviderApi.md#aavev3pooladdressprovidersetmarketid) | **POST** /aave/v3/poolAddressProvider/{address}/setMarketId | Sets the market ID for the given pool address provider. |
*PoolAddressProviderApi* | [**aavev3PoolAddressProviderSetPoolConfiguratorImpl**](Apis/PoolAddressProviderApi.md#aavev3pooladdressprovidersetpoolconfiguratorimpl) | **POST** /aave/v3/poolAddressProvider/{address}/setPoolConfiguratorImpl | Sets the Pool Configurator implementation for the given address. |
*PoolAddressProviderApi* | [**aavev3PoolAddressProviderSetPoolImpl**](Apis/PoolAddressProviderApi.md#aavev3pooladdressprovidersetpoolimpl) | **POST** /aave/v3/poolAddressProvider/{address}/setPoolImpl | Sets the pool implementation address for the given address. |
| *PoolAddressProviderRegistryApi* | [**aavev3PoolAddressProviderRegistryGetATokenTotalSupply**](Apis/PoolAddressProviderRegistryApi.md#aavev3pooladdressproviderregistrygetatokentotalsupply) | **GET** /aave/v3/poolAddressProviderRegistry/{account}/getATokenTotalSupply | Retrieves the total supply of a specific AToken. |
*PoolAddressProviderRegistryApi* | [**aavev3PoolAddressProviderRegistryGetAddressesProvider**](Apis/PoolAddressProviderRegistryApi.md#aavev3pooladdressproviderregistrygetaddressesprovider) | **GET** /aave/v3/poolAddressProviderRegistry/{account}/getAddressesProvider | Retrieves the addresses provider from the Aave V3 Pool Address Provider Registry. |
*PoolAddressProviderRegistryApi* | [**aavev3PoolAddressProviderRegistryGetAllATokens**](Apis/PoolAddressProviderRegistryApi.md#aavev3pooladdressproviderregistrygetallatokens) | **GET** /aave/v3/poolAddressProviderRegistry/{account}/getAllATokens | Retrieves all ATokens associated with the specified account. |
*PoolAddressProviderRegistryApi* | [**aavev3PoolAddressProviderRegistryGetDebtCeiling**](Apis/PoolAddressProviderRegistryApi.md#aavev3pooladdressproviderregistrygetdebtceiling) | **GET** /aave/v3/poolAddressProviderRegistry/{account}/getDebtCeiling | Retrieves the debt ceiling for a specified asset from the Aave V3 Pool Address Provider Registry. |
*PoolAddressProviderRegistryApi* | [**getAllReservesTokens**](Apis/PoolAddressProviderRegistryApi.md#getallreservestokens) | **GET** /aave/v3/poolAddressProviderRegistry/{account}/getAllReservesTokens |  |
| *RamsesApi* | [**calculateOptimalVoteDistribution**](Apis/RamsesApi.md#calculateoptimalvotedistribution) | **GET** /ramses/data/vote-distribution |  |
*RamsesApi* | [**getInfo**](Apis/RamsesApi.md#getinfo) | **GET** /ramses/data/info |  |
*RamsesApi* | [**getPoolByAddress**](Apis/RamsesApi.md#getpoolbyaddress) | **GET** /ramses/data/pools/{address} |  |
*RamsesApi* | [**getPools**](Apis/RamsesApi.md#getpools) | **GET** /ramses/data/pools |  |
*RamsesApi* | [**getPoolsByType**](Apis/RamsesApi.md#getpoolsbytype) | **GET** /ramses/data/pools/type/{type} |  |
*RamsesApi* | [**getTokens**](Apis/RamsesApi.md#gettokens) | **GET** /ramses/data/tokens |  |
*RamsesApi* | [**getTopAPRPools**](Apis/RamsesApi.md#gettopaprpools) | **GET** /ramses/data/pools/top-apr |  |
*RamsesApi* | [**getTotalValueLocked**](Apis/RamsesApi.md#gettotalvaluelocked) | **GET** /ramses/data/tvl |  |
| *RamsesNFTApi* | [**abstain**](Apis/RamsesNFTApi.md#abstain) | **POST** /ramses/nft/{address}/abstain |  |
*RamsesNFTApi* | [**approve**](Apis/RamsesNFTApi.md#approve) | **POST** /ramses/nft/{address}/approve |  |
*RamsesNFTApi* | [**attach**](Apis/RamsesNFTApi.md#attach) | **POST** /ramses/nft/{address}/attach |  |
*RamsesNFTApi* | [**createLock**](Apis/RamsesNFTApi.md#createlock) | **POST** /ramses/nft/{address}/createLock |  |
*RamsesNFTApi* | [**delegate**](Apis/RamsesNFTApi.md#delegate) | **POST** /ramses/nft/{address}/delegate |  |
*RamsesNFTApi* | [**detach**](Apis/RamsesNFTApi.md#detach) | **POST** /ramses/nft/{address}/detach |  |
*RamsesNFTApi* | [**getBalanceOf**](Apis/RamsesNFTApi.md#getbalanceof) | **GET** /ramses/nft/balanceOf |  |
*RamsesNFTApi* | [**getBalanceOfNFT**](Apis/RamsesNFTApi.md#getbalanceofnft) | **GET** /ramses/nft/balanceOfNFT |  |
*RamsesNFTApi* | [**getDelegates**](Apis/RamsesNFTApi.md#getdelegates) | **GET** /ramses/nft/delegates |  |
*RamsesNFTApi* | [**getLocked**](Apis/RamsesNFTApi.md#getlocked) | **GET** /ramses/nft/locked |  |
*RamsesNFTApi* | [**getOwnerOf**](Apis/RamsesNFTApi.md#getownerof) | **GET** /ramses/nft/ownerOf |  |
*RamsesNFTApi* | [**getPastVotes**](Apis/RamsesNFTApi.md#getpastvotes) | **GET** /ramses/nft/getPastVotes |  |
*RamsesNFTApi* | [**getTokenURI**](Apis/RamsesNFTApi.md#gettokenuri) | **GET** /ramses/nft/tokenURI |  |
*RamsesNFTApi* | [**getTotalSupply**](Apis/RamsesNFTApi.md#gettotalsupply) | **GET** /ramses/nft/totalSupply |  |
*RamsesNFTApi* | [**getVotes**](Apis/RamsesNFTApi.md#getvotes) | **GET** /ramses/nft/getVotes |  |
*RamsesNFTApi* | [**increaseAmount**](Apis/RamsesNFTApi.md#increaseamount) | **POST** /ramses/nft/{address}/increaseAmount |  |
*RamsesNFTApi* | [**increaseUnlockTime**](Apis/RamsesNFTApi.md#increaseunlocktime) | **POST** /ramses/nft/{address}/increaseUnlockTime |  |
*RamsesNFTApi* | [**merge**](Apis/RamsesNFTApi.md#merge) | **POST** /ramses/nft/{address}/merge |  |
*RamsesNFTApi* | [**split**](Apis/RamsesNFTApi.md#split) | **POST** /ramses/nft/{address}/split |  |
*RamsesNFTApi* | [**transferFrom**](Apis/RamsesNFTApi.md#transferfrom) | **POST** /ramses/nft/{address}/transferFrom |  |
*RamsesNFTApi* | [**withdraw**](Apis/RamsesNFTApi.md#withdraw) | **POST** /ramses/nft/{address}/withdraw |  |
| *RamsesRouterApi* | [**addLiquidity**](Apis/RamsesRouterApi.md#addliquidity) | **POST** /ramses/router/{address}/addLiquidity |  |
*RamsesRouterApi* | [**addLiquidityETH**](Apis/RamsesRouterApi.md#addliquidityeth) | **POST** /ramses/router/{address}/addLiquidityETH |  |
*RamsesRouterApi* | [**getAmountOut**](Apis/RamsesRouterApi.md#getamountout) | **GET** /ramses/router/getAmountOut |  |
*RamsesRouterApi* | [**getAmountsOut**](Apis/RamsesRouterApi.md#getamountsout) | **GET** /ramses/router/getAmountsOut |  |
*RamsesRouterApi* | [**getFactory**](Apis/RamsesRouterApi.md#getfactory) | **GET** /ramses/router/factory |  |
*RamsesRouterApi* | [**getReserves**](Apis/RamsesRouterApi.md#getreserves) | **GET** /ramses/router/getReserves |  |
*RamsesRouterApi* | [**getWeth**](Apis/RamsesRouterApi.md#getweth) | **GET** /ramses/router/weth |  |
*RamsesRouterApi* | [**isPair**](Apis/RamsesRouterApi.md#ispair) | **GET** /ramses/router/isPair |  |
*RamsesRouterApi* | [**pairFor**](Apis/RamsesRouterApi.md#pairfor) | **GET** /ramses/router/pairFor |  |
*RamsesRouterApi* | [**quoteAddLiquidity**](Apis/RamsesRouterApi.md#quoteaddliquidity) | **GET** /ramses/router/quoteAddLiquidity |  |
*RamsesRouterApi* | [**quoteRemoveLiquidity**](Apis/RamsesRouterApi.md#quoteremoveliquidity) | **GET** /ramses/router/quoteRemoveLiquidity |  |
*RamsesRouterApi* | [**removeLiquidity**](Apis/RamsesRouterApi.md#removeliquidity) | **POST** /ramses/router/{address}/removeLiquidity |  |
*RamsesRouterApi* | [**removeLiquidityETH**](Apis/RamsesRouterApi.md#removeliquidityeth) | **POST** /ramses/router/{address}/removeLiquidityETH |  |
*RamsesRouterApi* | [**sortTokens**](Apis/RamsesRouterApi.md#sorttokens) | **GET** /ramses/router/sortTokens |  |
*RamsesRouterApi* | [**swapExactETHForTokens**](Apis/RamsesRouterApi.md#swapexactethfortokens) | **POST** /ramses/router/{address}/swapExactETHForTokens |  |
*RamsesRouterApi* | [**swapExactTokensForETH**](Apis/RamsesRouterApi.md#swapexacttokensforeth) | **POST** /ramses/router/{address}/swapExactTokensForETH |  |
*RamsesRouterApi* | [**swapExactTokensForTokens**](Apis/RamsesRouterApi.md#swapexacttokensfortokens) | **POST** /ramses/router/{address}/swapExactTokensForTokens |  |
*RamsesRouterApi* | [**uNSAFESwapExactTokensForTokens**](Apis/RamsesRouterApi.md#unsafeswapexacttokensfortokens) | **POST** /ramses/router/{address}/UNSAFE_swapExactTokensForTokens |  |
| *RamsesVoterApi* | [**attachTokenToGauge**](Apis/RamsesVoterApi.md#attachtokentogauge) | **POST** /ramses/voter/{address}/attachTokenToGauge |  |
*RamsesVoterApi* | [**claimBribes**](Apis/RamsesVoterApi.md#claimbribes) | **POST** /ramses/voter/{address}/claimBribes |  |
*RamsesVoterApi* | [**claimFees**](Apis/RamsesVoterApi.md#claimfees) | **POST** /ramses/voter/{address}/claimFees |  |
*RamsesVoterApi* | [**claimRewards**](Apis/RamsesVoterApi.md#claimrewards) | **POST** /ramses/voter/{address}/claimRewards |  |
*RamsesVoterApi* | [**createGauge**](Apis/RamsesVoterApi.md#creategauge) | **POST** /ramses/voter/{address}/createGauge |  |
*RamsesVoterApi* | [**detachTokenFromGauge**](Apis/RamsesVoterApi.md#detachtokenfromgauge) | **POST** /ramses/voter/{address}/detachTokenFromGauge |  |
*RamsesVoterApi* | [**distribute**](Apis/RamsesVoterApi.md#distribute) | **POST** /ramses/voter/{address}/distribute |  |
*RamsesVoterApi* | [**getLastVoted**](Apis/RamsesVoterApi.md#getlastvoted) | **GET** /ramses/voter/lastVoted |  |
*RamsesVoterApi* | [**getTotalWeight**](Apis/RamsesVoterApi.md#gettotalweight) | **GET** /ramses/voter/totalWeight |  |
*RamsesVoterApi* | [**getWeights**](Apis/RamsesVoterApi.md#getweights) | **GET** /ramses/voter/weights |  |
*RamsesVoterApi* | [**isGauge**](Apis/RamsesVoterApi.md#isgauge) | **GET** /ramses/voter/isGauge |  |
*RamsesVoterApi* | [**isWhitelisted**](Apis/RamsesVoterApi.md#iswhitelisted) | **GET** /ramses/voter/isWhitelisted |  |
*RamsesVoterApi* | [**killGauge**](Apis/RamsesVoterApi.md#killgauge) | **POST** /ramses/voter/{address}/killGauge |  |
*RamsesVoterApi* | [**notifyRewardAmount**](Apis/RamsesVoterApi.md#notifyrewardamount) | **POST** /ramses/voter/{address}/notifyRewardAmount |  |
*RamsesVoterApi* | [**poke**](Apis/RamsesVoterApi.md#poke) | **POST** /ramses/voter/{address}/poke |  |
*RamsesVoterApi* | [**reset**](Apis/RamsesVoterApi.md#reset) | **POST** /ramses/voter/{address}/reset |  |
*RamsesVoterApi* | [**reviveGauge**](Apis/RamsesVoterApi.md#revivegauge) | **POST** /ramses/voter/{address}/reviveGauge |  |
*RamsesVoterApi* | [**vote**](Apis/RamsesVoterApi.md#vote) | **POST** /ramses/voter/{address}/vote |  |
*RamsesVoterApi* | [**voteWithOptimalDistribution**](Apis/RamsesVoterApi.md#votewithoptimaldistribution) | **POST** /ramses/voter/{address}/voteWithOptimalDistribution |  |
*RamsesVoterApi* | [**whitelist**](Apis/RamsesVoterApi.md#whitelist) | **POST** /ramses/voter/{address}/whitelist |  |
| *RippleApi* | [**createRippleAccount**](Apis/RippleApi.md#createrippleaccount) | **POST** /ripple |  |
*RippleApi* | [**deleteRippleAccount**](Apis/RippleApi.md#deleterippleaccount) | **POST** /ripple/{accountName}/delete |  |
*RippleApi* | [**exportRippleAccount**](Apis/RippleApi.md#exportrippleaccount) | **POST** /ripple/{accountName}/export |  |
*RippleApi* | [**getRippleAccount**](Apis/RippleApi.md#getrippleaccount) | **GET** /ripple/{accountName} |  |
*RippleApi* | [**listRippleAccounts**](Apis/RippleApi.md#listrippleaccounts) | **GET** /ripple |  |
*RippleApi* | [**signRippleTransaction**](Apis/RippleApi.md#signrippletransaction) | **POST** /ripple/{accountName}/sign-tx |  |
| *SolanaApi* | [**createSolanaAccount**](Apis/SolanaApi.md#createsolanaaccount) | **POST** /solana |  |
*SolanaApi* | [**deleteSolanaAccount**](Apis/SolanaApi.md#deletesolanaaccount) | **POST** /solana/{accountName}/delete |  |
*SolanaApi* | [**exportSolanaAccount**](Apis/SolanaApi.md#exportsolanaaccount) | **POST** /solana/{accountName}/export |  |
*SolanaApi* | [**getSolanaAccount**](Apis/SolanaApi.md#getsolanaaccount) | **GET** /solana/{accountName} |  |
*SolanaApi* | [**listSolanaAccounts**](Apis/SolanaApi.md#listsolanaaccounts) | **GET** /solana |  |
*SolanaApi* | [**multiSignSolanaTransaction**](Apis/SolanaApi.md#multisignsolanatransaction) | **POST** /solana/{accountName}/multi-sign-tx |  |
*SolanaApi* | [**signSolanaTransaction**](Apis/SolanaApi.md#signsolanatransaction) | **POST** /solana/{accountName}/sign-tx |  |
*SolanaApi* | [**transferSolanaTransaction**](Apis/SolanaApi.md#transfersolanatransaction) | **POST** /solana/{accountName}/transfer |  |
*SolanaApi* | [**transferTokensSignSolanaTransaction**](Apis/SolanaApi.md#transfertokenssignsolanatransaction) | **POST** /solana/{accountName}/transfer-tokens |  |
| *ThenaApi* | [**calculateOptimalVoteDistribution**](Apis/ThenaApi.md#calculateoptimalvotedistribution) | **GET** /thena/data/vote-distribution |  |
*ThenaApi* | [**getFusionByAddress**](Apis/ThenaApi.md#getfusionbyaddress) | **GET** /thena/data/fusions/{address} |  |
*ThenaApi* | [**getFusions**](Apis/ThenaApi.md#getfusions) | **GET** /thena/data/fusions |  |
*ThenaApi* | [**getFusionsByType**](Apis/ThenaApi.md#getfusionsbytype) | **GET** /thena/data/fusions/type/{type} |  |
*ThenaApi* | [**getTopAPRFusions**](Apis/ThenaApi.md#gettopaprfusions) | **GET** /thena/data/fusions/top-apr |  |
*ThenaApi* | [**getTopPairs**](Apis/ThenaApi.md#gettoppairs) | **GET** /thena/data/pairs/top |  |
*ThenaApi* | [**getTopTokens**](Apis/ThenaApi.md#gettoptokens) | **GET** /thena/data/tokens/top |  |
*ThenaApi* | [**getTotalValueLocked**](Apis/ThenaApi.md#gettotalvaluelocked) | **GET** /thena/data/tvl |  |
| *ThorSwapApi* | [**getGasPrice**](Apis/ThorSwapApi.md#getgasprice) | **GET** /thorswap/gasPrice |  |
*ThorSwapApi* | [**getQuote**](Apis/ThorSwapApi.md#getquote) | **GET** /thorswap/quote |  |
*ThorSwapApi* | [**getSupportedChains**](Apis/ThorSwapApi.md#getsupportedchains) | **GET** /thorswap/supportedChains |  |
*ThorSwapApi* | [**getSupportedProviders**](Apis/ThorSwapApi.md#getsupportedproviders) | **GET** /thorswap/supportedProviders |  |
*ThorSwapApi* | [**swap**](Apis/ThorSwapApi.md#swap) | **POST** /thorswap/swap |  |
| *TradingBotApi* | [**activateBot**](Apis/TradingBotApi.md#activatebot) | **GET** /tradingBot/{botId}/activate |  |
*TradingBotApi* | [**conversation**](Apis/TradingBotApi.md#conversation) | **GET** /tradingBot/{botId}/twitter/conversation/{tweetId} |  |
*TradingBotApi* | [**createTweet**](Apis/TradingBotApi.md#createtweet) | **POST** /tradingBot/{botId}/twitter/createTweet |  |
*TradingBotApi* | [**deactivateBot**](Apis/TradingBotApi.md#deactivatebot) | **GET** /tradingBot/{botId}/deactivate |  |
*TradingBotApi* | [**followingTimeline**](Apis/TradingBotApi.md#followingtimeline) | **GET** /tradingBot/{botId}/twitter/followingTimeline |  |
*TradingBotApi* | [**getBotLastRunResults**](Apis/TradingBotApi.md#getbotlastrunresults) | **GET** /tradingBot/{botId}/lastRunResults |  |
*TradingBotApi* | [**getBotStatus**](Apis/TradingBotApi.md#getbotstatus) | **GET** /tradingBot/{botId}/status |  |
*TradingBotApi* | [**getConfigs**](Apis/TradingBotApi.md#getconfigs) | **GET** /tradingBot/configs |  |
*TradingBotApi* | [**restartBot**](Apis/TradingBotApi.md#restartbot) | **GET** /tradingBot/{botId}/restart |  |
*TradingBotApi* | [**startBot**](Apis/TradingBotApi.md#startbot) | **GET** /tradingBot/{botId}/start |  |
*TradingBotApi* | [**stopBot**](Apis/TradingBotApi.md#stopbot) | **GET** /tradingBot/{botId}/stop |  |
*TradingBotApi* | [**triggerBot**](Apis/TradingBotApi.md#triggerbot) | **GET** /tradingBot/{botId}/trigger |  |
*TradingBotApi* | [**tweetHistory**](Apis/TradingBotApi.md#tweethistory) | **GET** /tradingBot/{botId}/twitter/tweet/history |  |
*TradingBotApi* | [**tweetReplyTest**](Apis/TradingBotApi.md#tweetreplytest) | **POST** /tradingBot/{botId}/tweetReplyTest |  |
*TradingBotApi* | [**updatePersonality**](Apis/TradingBotApi.md#updatepersonality) | **PATCH** /tradingBot/{botId}/personality |  |
| *TronApi* | [**tronCreateTronAccount**](Apis/TronApi.md#troncreatetronaccount) | **POST** /tron | Creates a new account using the provided TronInput data. |
*TronApi* | [**tronDeleteTronAccount**](Apis/TronApi.md#trondeletetronaccount) | **POST** /tron/{accountName}/delete | Deletes an account using the provided account name and authorization token. |
*TronApi* | [**tronExportTronAccount**](Apis/TronApi.md#tronexporttronaccount) | **POST** /tron/{accountName}/export | Exports the account details for the specified account name. |
*TronApi* | [**tronGetTronAccount**](Apis/TronApi.md#trongettronaccount) | **GET** /tron/{accountName} | Retrieves account information from the Tron blockchain. |
*TronApi* | [**tronListTronAccounts**](Apis/TronApi.md#tronlisttronaccounts) | **GET** /tron | Lists accounts using the provided authorization token. |
*TronApi* | [**tronSignTronTransaction**](Apis/TronApi.md#tronsigntrontransaction) | **POST** /tron/{accountName}/sign-tx | Signs a Tron transaction using the provided account name and transaction input. |
| *UniswapV2RouterApi* | [**addLiquidity**](Apis/UniswapV2RouterApi.md#addliquidity) | **POST** /uniswap/v2/router/{account}/addLiquidity |  |
*UniswapV2RouterApi* | [**addLiquidityETH**](Apis/UniswapV2RouterApi.md#addliquidityeth) | **POST** /uniswap/v2/router/{account}/addLiquidityETH |  |
*UniswapV2RouterApi* | [**getAmountIn**](Apis/UniswapV2RouterApi.md#getamountin) | **POST** /uniswap/v2/router/{account}/getAmountIn |  |
*UniswapV2RouterApi* | [**getAmountOut**](Apis/UniswapV2RouterApi.md#getamountout) | **POST** /uniswap/v2/router/{account}/getAmountOut |  |
*UniswapV2RouterApi* | [**getAmountsIn**](Apis/UniswapV2RouterApi.md#getamountsin) | **POST** /uniswap/v2/router/{account}/getAmountsIn |  |
*UniswapV2RouterApi* | [**getAmountsOut**](Apis/UniswapV2RouterApi.md#getamountsout) | **POST** /uniswap/v2/router/{account}/getAmountsOut |  |
*UniswapV2RouterApi* | [**getWETH**](Apis/UniswapV2RouterApi.md#getweth) | **GET** /uniswap/v2/router/{account}/WETH |  |
*UniswapV2RouterApi* | [**quote**](Apis/UniswapV2RouterApi.md#quote) | **POST** /uniswap/v2/router/{account}/quote |  |
*UniswapV2RouterApi* | [**removeLiquidity**](Apis/UniswapV2RouterApi.md#removeliquidity) | **POST** /uniswap/v2/router/{account}/removeLiquidity |  |
*UniswapV2RouterApi* | [**removeLiquidityETH**](Apis/UniswapV2RouterApi.md#removeliquidityeth) | **POST** /uniswap/v2/router/{account}/removeLiquidityETH |  |
*UniswapV2RouterApi* | [**removeLiquidityETHSupportingFeeOnTransferTokens**](Apis/UniswapV2RouterApi.md#removeliquidityethsupportingfeeontransfertokens) | **POST** /uniswap/v2/router/{account}/removeLiquidityETHSupportingFeeOnTransferTokens |  |
*UniswapV2RouterApi* | [**removeLiquidityETHWithPermit**](Apis/UniswapV2RouterApi.md#removeliquidityethwithpermit) | **POST** /uniswap/v2/router/{account}/removeLiquidityETHWithPermit |  |
*UniswapV2RouterApi* | [**removeLiquidityETHWithPermitSupportingFeeOnTransferTokens**](Apis/UniswapV2RouterApi.md#removeliquidityethwithpermitsupportingfeeontransfertokens) | **POST** /uniswap/v2/router/{account}/removeLiquidityETHWithPermitSupportingFeeOnTransferTokens |  |
*UniswapV2RouterApi* | [**removeLiquidityWithPermit**](Apis/UniswapV2RouterApi.md#removeliquiditywithpermit) | **POST** /uniswap/v2/router/{account}/removeLiquidityWithPermit |  |
*UniswapV2RouterApi* | [**swapETHForExactTokens**](Apis/UniswapV2RouterApi.md#swapethforexacttokens) | **POST** /uniswap/v2/router/{account}/swapETHForExactTokens |  |
*UniswapV2RouterApi* | [**swapExactETHForTokens**](Apis/UniswapV2RouterApi.md#swapexactethfortokens) | **POST** /uniswap/v2/router/{account}/swapExactETHForTokens |  |
*UniswapV2RouterApi* | [**swapExactETHForTokensSupportingFeeOnTransferTokens**](Apis/UniswapV2RouterApi.md#swapexactethfortokenssupportingfeeontransfertokens) | **POST** /uniswap/v2/router/{account}/swapExactETHForTokensSupportingFeeOnTransferTokens |  |
*UniswapV2RouterApi* | [**swapExactTokensForETH**](Apis/UniswapV2RouterApi.md#swapexacttokensforeth) | **POST** /uniswap/v2/router/{account}/swapExactTokensForETH |  |
*UniswapV2RouterApi* | [**swapExactTokensForETHSupportingFeeOnTransferTokens**](Apis/UniswapV2RouterApi.md#swapexacttokensforethsupportingfeeontransfertokens) | **POST** /uniswap/v2/router/{account}/swapExactTokensForETHSupportingFeeOnTransferTokens |  |
*UniswapV2RouterApi* | [**swapExactTokensForTokens**](Apis/UniswapV2RouterApi.md#swapexacttokensfortokens) | **POST** /uniswap/v2/router/{account}/swapExactTokensForTokens |  |
*UniswapV2RouterApi* | [**swapExactTokensForTokensSupportingFeeOnTransferTokens**](Apis/UniswapV2RouterApi.md#swapexacttokensfortokenssupportingfeeontransfertokens) | **POST** /uniswap/v2/router/{account}/swapExactTokensForTokensSupportingFeeOnTransferTokens |  |
*UniswapV2RouterApi* | [**swapTokensForExactETH**](Apis/UniswapV2RouterApi.md#swaptokensforexacteth) | **POST** /uniswap/v2/router/{account}/swapTokensForExactETH |  |
*UniswapV2RouterApi* | [**swapTokensForExactTokens**](Apis/UniswapV2RouterApi.md#swaptokensforexacttokens) | **POST** /uniswap/v2/router/{account}/swapTokensForExactTokens |  |
| *UniswapV3NFTApi* | [**approve**](Apis/UniswapV3NFTApi.md#approve) | **POST** /uniswap/v3/nft/{address}/approve |  |
*UniswapV3NFTApi* | [**balanceOf**](Apis/UniswapV3NFTApi.md#balanceof) | **GET** /uniswap/v3/nft/balanceOf |  |
*UniswapV3NFTApi* | [**baseURI**](Apis/UniswapV3NFTApi.md#baseuri) | **GET** /uniswap/v3/nft/baseURI |  |
*UniswapV3NFTApi* | [**burn**](Apis/UniswapV3NFTApi.md#burn) | **POST** /uniswap/v3/nft/{address}/burn |  |
*UniswapV3NFTApi* | [**collect**](Apis/UniswapV3NFTApi.md#collect) | **POST** /uniswap/v3/nft/{address}/collect |  |
*UniswapV3NFTApi* | [**createAndInitializePoolIfNecessary**](Apis/UniswapV3NFTApi.md#createandinitializepoolifnecessary) | **POST** /uniswap/v3/nft/{address}/createAndInitializePoolIfNecessary |  |
*UniswapV3NFTApi* | [**dOMAINSEPARATOR**](Apis/UniswapV3NFTApi.md#domainseparator) | **GET** /uniswap/v3/nft/DOMAIN_SEPARATOR |  |
*UniswapV3NFTApi* | [**decreaseLiquidity**](Apis/UniswapV3NFTApi.md#decreaseliquidity) | **POST** /uniswap/v3/nft/{address}/decreaseLiquidity |  |
*UniswapV3NFTApi* | [**factory**](Apis/UniswapV3NFTApi.md#factory) | **GET** /uniswap/v3/nft/factory |  |
*UniswapV3NFTApi* | [**getApproved**](Apis/UniswapV3NFTApi.md#getapproved) | **GET** /uniswap/v3/nft/getApproved |  |
*UniswapV3NFTApi* | [**increaseLiquidity**](Apis/UniswapV3NFTApi.md#increaseliquidity) | **POST** /uniswap/v3/nft/{address}/increaseLiquidity |  |
*UniswapV3NFTApi* | [**isApprovedForAll**](Apis/UniswapV3NFTApi.md#isapprovedforall) | **GET** /uniswap/v3/nft/isApprovedForAll |  |
*UniswapV3NFTApi* | [**mint**](Apis/UniswapV3NFTApi.md#mint) | **POST** /uniswap/v3/nft/{address}/mint |  |
*UniswapV3NFTApi* | [**multicall**](Apis/UniswapV3NFTApi.md#multicall) | **POST** /uniswap/v3/nft/{address}/multicall |  |
*UniswapV3NFTApi* | [**name**](Apis/UniswapV3NFTApi.md#name) | **GET** /uniswap/v3/nft/name |  |
*UniswapV3NFTApi* | [**ownerOf**](Apis/UniswapV3NFTApi.md#ownerof) | **GET** /uniswap/v3/nft/ownerOf |  |
*UniswapV3NFTApi* | [**pERMITTYPEHASH**](Apis/UniswapV3NFTApi.md#permittypehash) | **GET** /uniswap/v3/nft/PERMIT_TYPEHASH |  |
*UniswapV3NFTApi* | [**permit**](Apis/UniswapV3NFTApi.md#permit) | **POST** /uniswap/v3/nft/{address}/permit |  |
*UniswapV3NFTApi* | [**positions**](Apis/UniswapV3NFTApi.md#positions) | **GET** /uniswap/v3/nft/positions |  |
*UniswapV3NFTApi* | [**refundETH**](Apis/UniswapV3NFTApi.md#refundeth) | **POST** /uniswap/v3/nft/{address}/refundETH |  |
*UniswapV3NFTApi* | [**setApprovalForAll**](Apis/UniswapV3NFTApi.md#setapprovalforall) | **POST** /uniswap/v3/nft/{address}/setApprovalForAll |  |
*UniswapV3NFTApi* | [**supportsInterface**](Apis/UniswapV3NFTApi.md#supportsinterface) | **GET** /uniswap/v3/nft/supportsInterface |  |
*UniswapV3NFTApi* | [**sweepToken**](Apis/UniswapV3NFTApi.md#sweeptoken) | **POST** /uniswap/v3/nft/{address}/sweepToken |  |
*UniswapV3NFTApi* | [**symbol**](Apis/UniswapV3NFTApi.md#symbol) | **GET** /uniswap/v3/nft/symbol |  |
*UniswapV3NFTApi* | [**tokenByIndex**](Apis/UniswapV3NFTApi.md#tokenbyindex) | **GET** /uniswap/v3/nft/tokenByIndex |  |
*UniswapV3NFTApi* | [**tokenOfOwnerByIndex**](Apis/UniswapV3NFTApi.md#tokenofownerbyindex) | **GET** /uniswap/v3/nft/tokenOfOwnerByIndex |  |
*UniswapV3NFTApi* | [**tokenURI**](Apis/UniswapV3NFTApi.md#tokenuri) | **GET** /uniswap/v3/nft/tokenURI |  |
*UniswapV3NFTApi* | [**totalSupply**](Apis/UniswapV3NFTApi.md#totalsupply) | **GET** /uniswap/v3/nft/totalSupply |  |
*UniswapV3NFTApi* | [**transferFrom**](Apis/UniswapV3NFTApi.md#transferfrom) | **POST** /uniswap/v3/nft/{address}/transferFrom |  |
*UniswapV3NFTApi* | [**unwrapWETH9**](Apis/UniswapV3NFTApi.md#unwrapweth9) | **POST** /uniswap/v3/nft/{address}/unwrapWETH9 |  |
*UniswapV3NFTApi* | [**wETH9**](Apis/UniswapV3NFTApi.md#weth9) | **GET** /uniswap/v3/nft/WETH9 |  |
| *UniswapV3RouterApi* | [**exactInput**](Apis/UniswapV3RouterApi.md#exactinput) | **POST** /uniswap/v3/router/{address}/exactInput |  |
*UniswapV3RouterApi* | [**exactInputSingle**](Apis/UniswapV3RouterApi.md#exactinputsingle) | **POST** /uniswap/v3/router/{address}/exactInputSingle |  |
*UniswapV3RouterApi* | [**exactOutput**](Apis/UniswapV3RouterApi.md#exactoutput) | **POST** /uniswap/v3/router/{address}/exactOutput |  |
*UniswapV3RouterApi* | [**exactOutputSingle**](Apis/UniswapV3RouterApi.md#exactoutputsingle) | **POST** /uniswap/v3/router/{address}/exactOutputSingle |  |
*UniswapV3RouterApi* | [**factory**](Apis/UniswapV3RouterApi.md#factory) | **GET** /uniswap/v3/router/factory |  |
*UniswapV3RouterApi* | [**multicall**](Apis/UniswapV3RouterApi.md#multicall) | **POST** /uniswap/v3/router/{address}/multicall |  |
*UniswapV3RouterApi* | [**refundETH**](Apis/UniswapV3RouterApi.md#refundeth) | **POST** /uniswap/v3/router/{address}/refundETH |  |
*UniswapV3RouterApi* | [**selfPermit**](Apis/UniswapV3RouterApi.md#selfpermit) | **POST** /uniswap/v3/router/{address}/selfPermit |  |
*UniswapV3RouterApi* | [**selfPermitAllowed**](Apis/UniswapV3RouterApi.md#selfpermitallowed) | **POST** /uniswap/v3/router/{address}/selfPermitAllowed |  |
*UniswapV3RouterApi* | [**selfPermitAllowedIfNecessary**](Apis/UniswapV3RouterApi.md#selfpermitallowedifnecessary) | **POST** /uniswap/v3/router/{address}/selfPermitAllowedIfNecessary |  |
*UniswapV3RouterApi* | [**selfPermitIfNecessary**](Apis/UniswapV3RouterApi.md#selfpermitifnecessary) | **POST** /uniswap/v3/router/{address}/selfPermitIfNecessary |  |
*UniswapV3RouterApi* | [**sweepToken**](Apis/UniswapV3RouterApi.md#sweeptoken) | **POST** /uniswap/v3/router/{address}/sweepToken |  |
*UniswapV3RouterApi* | [**sweepTokenWithFee**](Apis/UniswapV3RouterApi.md#sweeptokenwithfee) | **POST** /uniswap/v3/router/{address}/sweepTokenWithFee |  |
*UniswapV3RouterApi* | [**unwrapWETH9**](Apis/UniswapV3RouterApi.md#unwrapweth9) | **POST** /uniswap/v3/router/{address}/unwrapWETH9 |  |
*UniswapV3RouterApi* | [**unwrapWETH9WithFee**](Apis/UniswapV3RouterApi.md#unwrapweth9withfee) | **POST** /uniswap/v3/router/{address}/unwrapWETH9WithFee |  |
*UniswapV3RouterApi* | [**wETH9**](Apis/UniswapV3RouterApi.md#weth9) | **GET** /uniswap/v3/router/WETH9 |  |
| *VeTheNFTApi* | [**abstain**](Apis/VeTheNFTApi.md#abstain) | **POST** /thena/nft/{address}/abstain |  |
*VeTheNFTApi* | [**approve**](Apis/VeTheNFTApi.md#approve) | **POST** /thena/nft/{address}/approve |  |
*VeTheNFTApi* | [**attach**](Apis/VeTheNFTApi.md#attach) | **POST** /thena/nft/{address}/attach |  |
*VeTheNFTApi* | [**checkpoint**](Apis/VeTheNFTApi.md#checkpoint) | **POST** /thena/nft/{address}/checkpoint |  |
*VeTheNFTApi* | [**createLock**](Apis/VeTheNFTApi.md#createlock) | **POST** /thena/nft/{address}/createLock |  |
*VeTheNFTApi* | [**createLockFor**](Apis/VeTheNFTApi.md#createlockfor) | **POST** /thena/nft/{address}/createLockFor |  |
*VeTheNFTApi* | [**delegate**](Apis/VeTheNFTApi.md#delegate) | **POST** /thena/nft/{address}/delegate |  |
*VeTheNFTApi* | [**delegateBySig**](Apis/VeTheNFTApi.md#delegatebysig) | **POST** /thena/nft/{address}/delegateBySig |  |
*VeTheNFTApi* | [**depositFor**](Apis/VeTheNFTApi.md#depositfor) | **POST** /thena/nft/{address}/depositFor |  |
*VeTheNFTApi* | [**detach**](Apis/VeTheNFTApi.md#detach) | **POST** /thena/nft/{address}/detach |  |
*VeTheNFTApi* | [**getApproved**](Apis/VeTheNFTApi.md#getapproved) | **GET** /thena/nft/{tokenId}/getApproved |  |
*VeTheNFTApi* | [**getBalanceOf**](Apis/VeTheNFTApi.md#getbalanceof) | **GET** /thena/nft/{account}/balanceOf |  |
*VeTheNFTApi* | [**getBalanceOfAtNFT**](Apis/VeTheNFTApi.md#getbalanceofatnft) | **GET** /thena/nft/{tokenId}/balanceOfAtNFT |  |
*VeTheNFTApi* | [**getBalanceOfNFT**](Apis/VeTheNFTApi.md#getbalanceofnft) | **GET** /thena/nft/{tokenId}/balanceOfNFT |  |
*VeTheNFTApi* | [**getDelegates**](Apis/VeTheNFTApi.md#getdelegates) | **GET** /thena/nft/{delegator}/delegates |  |
*VeTheNFTApi* | [**getLastUserSlope**](Apis/VeTheNFTApi.md#getlastuserslope) | **GET** /thena/nft/{tokenId}/getLastUserSlope |  |
*VeTheNFTApi* | [**getLocked**](Apis/VeTheNFTApi.md#getlocked) | **GET** /thena/nft/{tokenId}/locked |  |
*VeTheNFTApi* | [**getLockedEnd**](Apis/VeTheNFTApi.md#getlockedend) | **GET** /thena/nft/{tokenId}/lockedEnd |  |
*VeTheNFTApi* | [**getOwnerOf**](Apis/VeTheNFTApi.md#getownerof) | **GET** /thena/nft/{tokenId}/ownerOf |  |
*VeTheNFTApi* | [**getPastTotalSupply**](Apis/VeTheNFTApi.md#getpasttotalsupply) | **GET** /thena/nft/getPastTotalSupply |  |
*VeTheNFTApi* | [**getPastVotes**](Apis/VeTheNFTApi.md#getpastvotes) | **GET** /thena/nft/{account}/getPastVotes |  |
*VeTheNFTApi* | [**getTokenURI**](Apis/VeTheNFTApi.md#gettokenuri) | **GET** /thena/nft/{tokenId}/tokenURI |  |
*VeTheNFTApi* | [**getTotalSupply**](Apis/VeTheNFTApi.md#gettotalsupply) | **GET** /thena/nft/totalSupply |  |
*VeTheNFTApi* | [**getTotalSupplyAt**](Apis/VeTheNFTApi.md#gettotalsupplyat) | **GET** /thena/nft/totalSupplyAt |  |
*VeTheNFTApi* | [**getTotalSupplyAtT**](Apis/VeTheNFTApi.md#gettotalsupplyatt) | **GET** /thena/nft/totalSupplyAtT |  |
*VeTheNFTApi* | [**getUserPointHistory**](Apis/VeTheNFTApi.md#getuserpointhistory) | **GET** /thena/nft/{tokenId}/userPointHistory |  |
*VeTheNFTApi* | [**getUserPointHistoryTS**](Apis/VeTheNFTApi.md#getuserpointhistoryts) | **GET** /thena/nft/{tokenId}/userPointHistoryTS |  |
*VeTheNFTApi* | [**getVotes**](Apis/VeTheNFTApi.md#getvotes) | **GET** /thena/nft/{account}/getVotes |  |
*VeTheNFTApi* | [**increaseLockAmount**](Apis/VeTheNFTApi.md#increaselockamount) | **POST** /thena/nft/{address}/increaseLockAmount |  |
*VeTheNFTApi* | [**increaseUnlockTime**](Apis/VeTheNFTApi.md#increaseunlocktime) | **POST** /thena/nft/{address}/increaseUnlockTime |  |
*VeTheNFTApi* | [**isApprovedForAll**](Apis/VeTheNFTApi.md#isapprovedforall) | **GET** /thena/nft/{owner}/isApprovedForAll |  |
*VeTheNFTApi* | [**merge**](Apis/VeTheNFTApi.md#merge) | **POST** /thena/nft/{address}/merge |  |
*VeTheNFTApi* | [**safeTransferFrom**](Apis/VeTheNFTApi.md#safetransferfrom) | **POST** /thena/nft/{address}/safeTransferFrom |  |
*VeTheNFTApi* | [**setApprovalForAll**](Apis/VeTheNFTApi.md#setapprovalforall) | **POST** /thena/nft/{address}/setApprovalForAll |  |
*VeTheNFTApi* | [**split**](Apis/VeTheNFTApi.md#split) | **POST** /thena/nft/{address}/split |  |
*VeTheNFTApi* | [**transferFrom**](Apis/VeTheNFTApi.md#transferfrom) | **POST** /thena/nft/{address}/transferFrom |  |
*VeTheNFTApi* | [**voting**](Apis/VeTheNFTApi.md#voting) | **POST** /thena/nft/{address}/voting |  |
*VeTheNFTApi* | [**withdraw**](Apis/VeTheNFTApi.md#withdraw) | **POST** /thena/nft/{address}/withdraw |  |
| *VeTheNftVoterApi* | [**attachTokenToGauge**](Apis/VeTheNftVoterApi.md#attachtokentogauge) | **POST** /thena/voter/{address}/attachTokenToGauge |  |
*VeTheNftVoterApi* | [**claimBribes**](Apis/VeTheNftVoterApi.md#claimbribes) | **POST** /thena/voter/{address}/claimBribes |  |
*VeTheNftVoterApi* | [**claimFees**](Apis/VeTheNftVoterApi.md#claimfees) | **POST** /thena/voter/{address}/claimFees |  |
*VeTheNftVoterApi* | [**claimRewards**](Apis/VeTheNftVoterApi.md#claimrewards) | **POST** /thena/voter/{address}/claimRewards |  |
*VeTheNftVoterApi* | [**createGauge**](Apis/VeTheNftVoterApi.md#creategauge) | **POST** /thena/voter/{address}/createGauge |  |
*VeTheNftVoterApi* | [**detachTokenFromGauge**](Apis/VeTheNftVoterApi.md#detachtokenfromgauge) | **POST** /thena/voter/{address}/detachTokenFromGauge |  |
*VeTheNftVoterApi* | [**distribute**](Apis/VeTheNftVoterApi.md#distribute) | **POST** /thena/voter/{address}/distribute |  |
*VeTheNftVoterApi* | [**getTotalWeight**](Apis/VeTheNftVoterApi.md#gettotalweight) | **GET** /thena/voter/totalWeight |  |
*VeTheNftVoterApi* | [**getWeights**](Apis/VeTheNftVoterApi.md#getweights) | **GET** /thena/voter/weights |  |
*VeTheNftVoterApi* | [**isGauge**](Apis/VeTheNftVoterApi.md#isgauge) | **GET** /thena/voter/isGauge |  |
*VeTheNftVoterApi* | [**isWhitelisted**](Apis/VeTheNftVoterApi.md#iswhitelisted) | **GET** /thena/voter/isWhitelisted |  |
*VeTheNftVoterApi* | [**killGauge**](Apis/VeTheNftVoterApi.md#killgauge) | **POST** /thena/voter/{address}/killGauge |  |
*VeTheNftVoterApi* | [**lastVoted**](Apis/VeTheNftVoterApi.md#lastvoted) | **GET** /thena/voter/lastVoted |  |
*VeTheNftVoterApi* | [**notifyRewardAmount**](Apis/VeTheNftVoterApi.md#notifyrewardamount) | **POST** /thena/voter/{address}/notifyRewardAmount |  |
*VeTheNftVoterApi* | [**poke**](Apis/VeTheNftVoterApi.md#poke) | **POST** /thena/voter/{address}/poke |  |
*VeTheNftVoterApi* | [**poolVoteLength**](Apis/VeTheNftVoterApi.md#poolvotelength) | **GET** /thena/voter/poolVoteLength |  |
*VeTheNftVoterApi* | [**reset**](Apis/VeTheNftVoterApi.md#reset) | **POST** /thena/voter/{address}/reset |  |
*VeTheNftVoterApi* | [**reviveGauge**](Apis/VeTheNftVoterApi.md#revivegauge) | **POST** /thena/voter/{address}/reviveGauge |  |
*VeTheNftVoterApi* | [**vote**](Apis/VeTheNftVoterApi.md#vote) | **POST** /thena/voter/{address}/vote |  |
*VeTheNftVoterApi* | [**voteWithOptimalDistribution**](Apis/VeTheNftVoterApi.md#votewithoptimaldistribution) | **POST** /thena/voter/{address}/voteWithOptimalDistribution |  |
*VeTheNftVoterApi* | [**whitelist**](Apis/VeTheNftVoterApi.md#whitelist) | **POST** /thena/voter/{address}/whitelist |  |


<a name="documentation-for-models"></a>
## Documentation for Models

 - [AAVEv3RewardsAPIResponse_AAVEv3RewardsExecuteFunctionResult_](./Models/AAVEv3RewardsAPIResponse_AAVEv3RewardsExecuteFunctionResult_.md)
 - [AAVEv3RewardsAPIResponse_string-Array_](./Models/AAVEv3RewardsAPIResponse_string-Array_.md)
 - [AAVEv3RewardsAPIResponse_string_](./Models/AAVEv3RewardsAPIResponse_string_.md)
 - [AAVEv3RewardsExecuteFunctionResult](./Models/AAVEv3RewardsExecuteFunctionResult.md)
 - [AAVEv3RewardsInputBody](./Models/AAVEv3RewardsInputBody.md)
 - [AAVEv3RewardsTransaction](./Models/AAVEv3RewardsTransaction.md)
 - [AAVEv3UiIncentiveDataProviderAPIResponse_AggregatedReserveIncentiveData-Array_](./Models/AAVEv3UiIncentiveDataProviderAPIResponse_AggregatedReserveIncentiveData-Array_.md)
 - [AAVEv3UiIncentiveDataProviderAPIResponse_FullReservesIncentiveData_](./Models/AAVEv3UiIncentiveDataProviderAPIResponse_FullReservesIncentiveData_.md)
 - [AAVEv3UiIncentiveDataProviderAPIResponse_UserReserveIncentiveData-Array_](./Models/AAVEv3UiIncentiveDataProviderAPIResponse_UserReserveIncentiveData-Array_.md)
 - [AAVEv3UiPoolDataProviderAPIResponse_UserReserveData-Array_](./Models/AAVEv3UiPoolDataProviderAPIResponse_UserReserveData-Array_.md)
 - [AAVEv3UiPoolDataProviderAPIResponse_any_](./Models/AAVEv3UiPoolDataProviderAPIResponse_any_.md)
 - [AAVEv3UiPoolDataProviderAPIResponse_string-Array_](./Models/AAVEv3UiPoolDataProviderAPIResponse_string-Array_.md)
 - [AAVEv3UiPoolDataProviderAPIResponse_string_](./Models/AAVEv3UiPoolDataProviderAPIResponse_string_.md)
 - [AAVEv3WalletBalanceProviderAPIResponse__tokens-string-Array--balances-string-Array--__](./Models/AAVEv3WalletBalanceProviderAPIResponse__tokens-string-Array--balances-string-Array--__.md)
 - [AAVEv3WalletBalanceProviderAPIResponse__tokens_string_Array__balances_string_Array_____data](./Models/AAVEv3WalletBalanceProviderAPIResponse__tokens_string_Array__balances_string_Array_____data.md)
 - [AAVEv3WalletBalanceProviderAPIResponse_string-Array_](./Models/AAVEv3WalletBalanceProviderAPIResponse_string-Array_.md)
 - [AAVEv3WalletBalanceProviderAPIResponse_string_](./Models/AAVEv3WalletBalanceProviderAPIResponse_string_.md)
 - [AavePoolAPIResponse_AavePoolExecuteFunctionResult_](./Models/AavePoolAPIResponse_AavePoolExecuteFunctionResult_.md)
 - [AavePoolAPIResponse_any_](./Models/AavePoolAPIResponse_any_.md)
 - [AavePoolExecuteFunctionResult](./Models/AavePoolExecuteFunctionResult.md)
 - [AavePoolInputBody](./Models/AavePoolInputBody.md)
 - [AavePoolInputBody_borrowAmount](./Models/AavePoolInputBody_borrowAmount.md)
 - [AavePoolInputBody_initialDeposit](./Models/AavePoolInputBody_initialDeposit.md)
 - [AavePoolInputBody_minHealthFactor](./Models/AavePoolInputBody_minHealthFactor.md)
 - [AavePoolInputBody_premiums](./Models/AavePoolInputBody_premiums.md)
 - [AavePoolTransaction](./Models/AavePoolTransaction.md)
 - [AbiEncodeInput](./Models/AbiEncodeInput.md)
 - [AbiEncodeOutput](./Models/AbiEncodeOutput.md)
 - [AbiEncodeOutput_data](./Models/AbiEncodeOutput_data.md)
 - [AccessTuple](./Models/AccessTuple.md)
 - [AccountAPIResponse](./Models/AccountAPIResponse.md)
 - [AccountData](./Models/AccountData.md)
 - [AccountResponse](./Models/AccountResponse.md)
 - [Action](./Models/Action.md)
 - [AggregatedReserveIncentiveData](./Models/AggregatedReserveIncentiveData.md)
 - [AllFinancials](./Models/AllFinancials.md)
 - [AllFinancialsAPIResponse](./Models/AllFinancialsAPIResponse.md)
 - [AlloraInferenceResponse](./Models/AlloraInferenceResponse.md)
 - [AlloraInferenceResponse_data](./Models/AlloraInferenceResponse_data.md)
 - [AlloraInferenceResponse_data_confidenceIntervals](./Models/AlloraInferenceResponse_data_confidenceIntervals.md)
 - [ApiResponse_ChainsResponse_](./Models/ApiResponse_ChainsResponse_.md)
 - [ApiResponse_ConnectionsResponse_](./Models/ApiResponse_ConnectionsResponse_.md)
 - [ApiResponse_PostQuote_](./Models/ApiResponse_PostQuote_.md)
 - [ApiResponse_Quote_](./Models/ApiResponse_Quote_.md)
 - [ApiResponse_StatusResponse_](./Models/ApiResponse_StatusResponse_.md)
 - [ApiResponse_TokenDetails_](./Models/ApiResponse_TokenDetails_.md)
 - [ApiResponse_TokenInfoByChainId_](./Models/ApiResponse_TokenInfoByChainId_.md)
 - [ApiResponse_TokensResponse_](./Models/ApiResponse_TokensResponse_.md)
 - [ApiResponse_ToolsResponse_](./Models/ApiResponse_ToolsResponse_.md)
 - [ApproveForPolymarketBody](./Models/ApproveForPolymarketBody.md)
 - [AssembleRequest](./Models/AssembleRequest.md)
 - [Asset](./Models/Asset.md)
 - [AvailableTickersAPIResponse](./Models/AvailableTickersAPIResponse.md)
 - [BRC20TransactionInput](./Models/BRC20TransactionInput.md)
 - [BRC20TransactionOutput](./Models/BRC20TransactionOutput.md)
 - [BalanceAPIResponse](./Models/BalanceAPIResponse.md)
 - [BalanceAllowanceResponse](./Models/BalanceAllowanceResponse.md)
 - [BalanceResponse](./Models/BalanceResponse.md)
 - [BalanceSheet](./Models/BalanceSheet.md)
 - [BalanceSheetsAPIResponse](./Models/BalanceSheetsAPIResponse.md)
 - [BaseCosmosAPIResponse](./Models/BaseCosmosAPIResponse.md)
 - [BitcoinAPIResponse](./Models/BitcoinAPIResponse.md)
 - [BitcoinAPIResponse_data](./Models/BitcoinAPIResponse_data.md)
 - [BitcoinCashAPIResponse_AccountResponse_](./Models/BitcoinCashAPIResponse_AccountResponse_.md)
 - [BitcoinCashAPIResponse_BitcoinCashTransactionOutput_](./Models/BitcoinCashAPIResponse_BitcoinCashTransactionOutput_.md)
 - [BitcoinCashAPIResponse__psbt_hex-string__](./Models/BitcoinCashAPIResponse__psbt_hex-string__.md)
 - [BitcoinCashAPIResponse__psbt_hex_string___data](./Models/BitcoinCashAPIResponse__psbt_hex_string___data.md)
 - [BitcoinCashAPIResponse__signed_psbt_hex-string__](./Models/BitcoinCashAPIResponse__signed_psbt_hex-string__.md)
 - [BitcoinCashAPIResponse__signed_psbt_hex_string___data](./Models/BitcoinCashAPIResponse__signed_psbt_hex_string___data.md)
 - [BitcoinCashAPIResponse__signed_tx-string__](./Models/BitcoinCashAPIResponse__signed_tx-string__.md)
 - [BitcoinCashAPIResponse__signed_tx_string___data](./Models/BitcoinCashAPIResponse__signed_tx_string___data.md)
 - [BitcoinCashInput](./Models/BitcoinCashInput.md)
 - [BitcoinCashTransactionInput](./Models/BitcoinCashTransactionInput.md)
 - [BitcoinCashTransactionOutput](./Models/BitcoinCashTransactionOutput.md)
 - [BitcoinCash_BitcoinCashSignBitcoinTransaction_request](./Models/BitcoinCash_BitcoinCashSignBitcoinTransaction_request.md)
 - [BitcoinCash_BitcoinCashSignPSBTWithKeyPathAndScriptPath_request](./Models/BitcoinCash_BitcoinCashSignPSBTWithKeyPathAndScriptPath_request.md)
 - [BitcoinInput](./Models/BitcoinInput.md)
 - [BitcoinTransactionInput](./Models/BitcoinTransactionInput.md)
 - [BitcoinTransactionOutput](./Models/BitcoinTransactionOutput.md)
 - [BotConfigType](./Models/BotConfigType.md)
 - [Bridge](./Models/Bridge.md)
 - [BridgeSupportedChain](./Models/BridgeSupportedChain.md)
 - [BroadCastRawTransactionAPIResponse](./Models/BroadCastRawTransactionAPIResponse.md)
 - [BroadCastRawTransactionResponse](./Models/BroadCastRawTransactionResponse.md)
 - [BroadcastInput](./Models/BroadcastInput.md)
 - [CancelMarketOrdersBody](./Models/CancelMarketOrdersBody.md)
 - [CancelMarketOrdersBody_payload](./Models/CancelMarketOrdersBody_payload.md)
 - [CancelMarketOrdersResponse](./Models/CancelMarketOrdersResponse.md)
 - [CancelOrderBody](./Models/CancelOrderBody.md)
 - [CancelOrderResponse](./Models/CancelOrderResponse.md)
 - [CancelOrdersBody](./Models/CancelOrdersBody.md)
 - [CancelOrdersResponse](./Models/CancelOrdersResponse.md)
 - [CashFlowStatement](./Models/CashFlowStatement.md)
 - [CashFlowStatementsAPIResponse](./Models/CashFlowStatementsAPIResponse.md)
 - [Chain](./Models/Chain.md)
 - [Chain_metamask](./Models/Chain_metamask.md)
 - [Chain_metamask_nativeCurrency](./Models/Chain_metamask_nativeCurrency.md)
 - [Chain_nativeToken](./Models/Chain_nativeToken.md)
 - [ChainsResponse](./Models/ChainsResponse.md)
 - [ChartAnalysisAPIResponse](./Models/ChartAnalysisAPIResponse.md)
 - [CommunityMetrics](./Models/CommunityMetrics.md)
 - [CommunityMetricsAPIResponse](./Models/CommunityMetricsAPIResponse.md)
 - [CompanyFacts](./Models/CompanyFacts.md)
 - [CompanyFactsAPIResponse](./Models/CompanyFactsAPIResponse.md)
 - [ComponentAPIResponse_ComponentDefinition-Array_](./Models/ComponentAPIResponse_ComponentDefinition-Array_.md)
 - [ComponentAPIResponse_ComponentDefinition_](./Models/ComponentAPIResponse_ComponentDefinition_.md)
 - [ComponentAPIResponse_ComponentMatch-Array_](./Models/ComponentAPIResponse_ComponentMatch-Array_.md)
 - [ComponentAPIResponse_Partial_ComponentDefinition_-Array_](./Models/ComponentAPIResponse_Partial_ComponentDefinition_-Array_.md)
 - [ComponentAPIResponse_void_](./Models/ComponentAPIResponse_void_.md)
 - [ComponentDefinition](./Models/ComponentDefinition.md)
 - [ComponentMatch](./Models/ComponentMatch.md)
 - [Components_updateEmbedding_request](./Models/Components_updateEmbedding_request.md)
 - [Connection](./Models/Connection.md)
 - [ConnectionsResponse](./Models/ConnectionsResponse.md)
 - [CosmosAccount](./Models/CosmosAccount.md)
 - [CosmosAccountAPIResponse](./Models/CosmosAccountAPIResponse.md)
 - [CosmosAccountListAPIResponse](./Models/CosmosAccountListAPIResponse.md)
 - [CosmosAccountListResponse](./Models/CosmosAccountListResponse.md)
 - [CosmosAccountListResponse_data](./Models/CosmosAccountListResponse_data.md)
 - [CosmosAccountResponse](./Models/CosmosAccountResponse.md)
 - [CosmosAccountResponse_data](./Models/CosmosAccountResponse_data.md)
 - [CosmosIBCTransferInput](./Models/CosmosIBCTransferInput.md)
 - [CosmosSignMessageInput](./Models/CosmosSignMessageInput.md)
 - [CosmosSignedMessageAPIResponse](./Models/CosmosSignedMessageAPIResponse.md)
 - [CosmosSignedMessageResponse](./Models/CosmosSignedMessageResponse.md)
 - [CosmosTransactionAPIResponse](./Models/CosmosTransactionAPIResponse.md)
 - [CosmosTransactionResponse](./Models/CosmosTransactionResponse.md)
 - [CosmosTransferInput](./Models/CosmosTransferInput.md)
 - [Cosmos_CosmosCreateAccount_request](./Models/Cosmos_CosmosCreateAccount_request.md)
 - [CreateAccountInput](./Models/CreateAccountInput.md)
 - [CreateFlowBody](./Models/CreateFlowBody.md)
 - [CreateLimitOrderBody](./Models/CreateLimitOrderBody.md)
 - [CreateMarketBuyOrderBody](./Models/CreateMarketBuyOrderBody.md)
 - [CreateMarketBuyOrderBody_options](./Models/CreateMarketBuyOrderBody_options.md)
 - [CreateMarketBuyOrderBody_userMarketOrder](./Models/CreateMarketBuyOrderBody_userMarketOrder.md)
 - [CreateMarketBuyOrderResponse](./Models/CreateMarketBuyOrderResponse.md)
 - [CreateOrderBody](./Models/CreateOrderBody.md)
 - [CreateOrderBody_options](./Models/CreateOrderBody_options.md)
 - [CreateOrderBody_userOrder](./Models/CreateOrderBody_userOrder.md)
 - [CreateOrderResponse](./Models/CreateOrderResponse.md)
 - [CreateUserDefinedFunction_request](./Models/CreateUserDefinedFunction_request.md)
 - [CryptoCurrency](./Models/CryptoCurrency.md)
 - [DebankPortfolioAPIResponse](./Models/DebankPortfolioAPIResponse.md)
 - [DeployInput](./Models/DeployInput.md)
 - [DogeCoinAPIResponse](./Models/DogeCoinAPIResponse.md)
 - [DogeCoinInput](./Models/DogeCoinInput.md)
 - [DogeCoinTransactionInput](./Models/DogeCoinTransactionInput.md)
 - [DogeCoinTransactionOutput](./Models/DogeCoinTransactionOutput.md)
 - [DropNotificationsBody](./Models/DropNotificationsBody.md)
 - [DropNotificationsBody_params](./Models/DropNotificationsBody_params.md)
 - [DropNotificationsResponse](./Models/DropNotificationsResponse.md)
 - [ENSReverseResolveAPIResponse](./Models/ENSReverseResolveAPIResponse.md)
 - [ENSReverseResolveInput](./Models/ENSReverseResolveInput.md)
 - [ENSReverseResolveResponse](./Models/ENSReverseResolveResponse.md)
 - [ERC20APIResponse_ERC20ExecuteFunctionResult_](./Models/ERC20APIResponse_ERC20ExecuteFunctionResult_.md)
 - [ERC20APIResponse_number_](./Models/ERC20APIResponse_number_.md)
 - [ERC20APIResponse_string_](./Models/ERC20APIResponse_string_.md)
 - [ERC20ExecuteFunctionResult](./Models/ERC20ExecuteFunctionResult.md)
 - [ERC20InputBody](./Models/ERC20InputBody.md)
 - [ERC20Transaction](./Models/ERC20Transaction.md)
 - [ERC4626APIResponse](./Models/ERC4626APIResponse.md)
 - [ERC721APIResponse](./Models/ERC721APIResponse.md)
 - [EmotionalState](./Models/EmotionalState.md)
 - [EnsResolveAPIResponse](./Models/EnsResolveAPIResponse.md)
 - [EnsResolveInput](./Models/EnsResolveInput.md)
 - [EnsResolveResponse](./Models/EnsResolveResponse.md)
 - [EosAPIResponse](./Models/EosAPIResponse.md)
 - [EosInput](./Models/EosInput.md)
 - [EosTransactionInput](./Models/EosTransactionInput.md)
 - [EosTransactionOutput](./Models/EosTransactionOutput.md)
 - [Erc1155Request](./Models/Erc1155Request.md)
 - [Estimate](./Models/Estimate.md)
 - [EvmCommonContractDataJSON](./Models/EvmCommonContractDataJSON.md)
 - [EvmContractSpenderDetailsJSON](./Models/EvmContractSpenderDetailsJSON.md)
 - [EvmContractTokenDetailsJSON](./Models/EvmContractTokenDetailsJSON.md)
 - [EvmDecodedEventJSON](./Models/EvmDecodedEventJSON.md)
 - [EvmDecodedEventParamsItemJSON](./Models/EvmDecodedEventParamsItemJSON.md)
 - [EvmETransactionCategoryJSON](./Models/EvmETransactionCategoryJSON.md)
 - [EvmInternalTransactionJSON](./Models/EvmInternalTransactionJSON.md)
 - [EvmLogVerboseJSON](./Models/EvmLogVerboseJSON.md)
 - [EvmNativeTransferJSON](./Models/EvmNativeTransferJSON.md)
 - [EvmNormalizedMetadataAttributeJSON](./Models/EvmNormalizedMetadataAttributeJSON.md)
 - [EvmNormalizedMetadataJSON](./Models/EvmNormalizedMetadataJSON.md)
 - [EvmResolveContractInteractionResponseJSON](./Models/EvmResolveContractInteractionResponseJSON.md)
 - [EvmWalletHistoryErc20TransferJSON](./Models/EvmWalletHistoryErc20TransferJSON.md)
 - [EvmWalletHistoryNftTransferJSON](./Models/EvmWalletHistoryNftTransferJSON.md)
 - [EvmWalletHistoryTransactionJSON](./Models/EvmWalletHistoryTransactionJSON.md)
 - [Exchange](./Models/Exchange.md)
 - [ExportAccountAPIResponse](./Models/ExportAccountAPIResponse.md)
 - [ExportAccountAPIResponse_data](./Models/ExportAccountAPIResponse_data.md)
 - [FeeCost](./Models/FeeCost.md)
 - [FiatCurrency](./Models/FiatCurrency.md)
 - [FinancialDatasets_SearchFinancialsByLineItems_request](./Models/FinancialDatasets_SearchFinancialsByLineItems_request.md)
 - [Flow](./Models/Flow.md)
 - [FlowEdge](./Models/FlowEdge.md)
 - [FlowNode](./Models/FlowNode.md)
 - [FlowNode_data](./Models/FlowNode_data.md)
 - [FullReservesIncentiveData](./Models/FullReservesIncentiveData.md)
 - [GasCost](./Models/GasCost.md)
 - [GasPrice](./Models/GasPrice.md)
 - [GasPrice_history_inner](./Models/GasPrice_history_inner.md)
 - [GeneratedTweet](./Models/GeneratedTweet.md)
 - [GetAllDebankUserTokens_200_response](./Models/GetAllDebankUserTokens_200_response.md)
 - [GetAllDebankUserTokens_200_response_anyOf](./Models/GetAllDebankUserTokens_200_response_anyOf.md)
 - [GetAllDebankUserTokens_200_response_anyOf_1](./Models/GetAllDebankUserTokens_200_response_anyOf_1.md)
 - [GetSupportedOnRampsResponse](./Models/GetSupportedOnRampsResponse.md)
 - [GetSupportedOnRampsResponse_message_inner](./Models/GetSupportedOnRampsResponse_message_inner.md)
 - [GetSupportedOnRampsResponse_message_inner_icons](./Models/GetSupportedOnRampsResponse_message_inner_icons.md)
 - [GetSupportedOnRampsResponse_message_inner_icons_png](./Models/GetSupportedOnRampsResponse_message_inner_icons_png.md)
 - [ImpliedFuturePrice_200_response](./Models/ImpliedFuturePrice_200_response.md)
 - [ImpliedFuturePrice_200_response_data](./Models/ImpliedFuturePrice_200_response_data.md)
 - [IncentiveData](./Models/IncentiveData.md)
 - [IncomeStatement](./Models/IncomeStatement.md)
 - [IncomeStatementsAPIResponse](./Models/IncomeStatementsAPIResponse.md)
 - [InputBody](./Models/InputBody.md)
 - [InsiderTransaction](./Models/InsiderTransaction.md)
 - [InsiderTransactionsAPIResponse](./Models/InsiderTransactionsAPIResponse.md)
 - [JUPITER_cancelLimitOrders_request](./Models/JUPITER_cancelLimitOrders_request.md)
 - [Jobs](./Models/Jobs.md)
 - [Json](./Models/Json.md)
 - [JupiterAPIResponse_JupiterExecuteFunctionResult_](./Models/JupiterAPIResponse_JupiterExecuteFunctionResult_.md)
 - [JupiterAPIResponse_Record_string.string__](./Models/JupiterAPIResponse_Record_string.string__.md)
 - [JupiterAPIResponse_any_](./Models/JupiterAPIResponse_any_.md)
 - [JupiterAPIResponse_string-Array_](./Models/JupiterAPIResponse_string-Array_.md)
 - [JupiterExecuteFunctionResult](./Models/JupiterExecuteFunctionResult.md)
 - [KOL](./Models/KOL.md)
 - [KOLListAPIResponse](./Models/KOLListAPIResponse.md)
 - [KOLNetwork](./Models/KOLNetwork.md)
 - [KOLNetworkAPIResponse](./Models/KOLNetworkAPIResponse.md)
 - [LendingPoolAPIResponse_LendingPoolExecuteFunctionResult_](./Models/LendingPoolAPIResponse_LendingPoolExecuteFunctionResult_.md)
 - [LendingPoolAPIResponse_any_](./Models/LendingPoolAPIResponse_any_.md)
 - [LendingPoolAPIResponse_boolean_](./Models/LendingPoolAPIResponse_boolean_.md)
 - [LendingPoolAPIResponse_number_](./Models/LendingPoolAPIResponse_number_.md)
 - [LendingPoolAPIResponse_string-Array_](./Models/LendingPoolAPIResponse_string-Array_.md)
 - [LendingPoolAPIResponse_string_](./Models/LendingPoolAPIResponse_string_.md)
 - [LendingPoolExecuteFunctionResult](./Models/LendingPoolExecuteFunctionResult.md)
 - [LendingPoolInputBody](./Models/LendingPoolInputBody.md)
 - [LendingPoolTransaction](./Models/LendingPoolTransaction.md)
 - [LeveragerAPIResponse_LeveragerExecuteFunctionResult_](./Models/LeveragerAPIResponse_LeveragerExecuteFunctionResult_.md)
 - [LeveragerAPIResponse_boolean_](./Models/LeveragerAPIResponse_boolean_.md)
 - [LeveragerAPIResponse_string_](./Models/LeveragerAPIResponse_string_.md)
 - [LeveragerExecuteFunctionResult](./Models/LeveragerExecuteFunctionResult.md)
 - [LeveragerInputBody](./Models/LeveragerInputBody.md)
 - [LeveragerTransaction](./Models/LeveragerTransaction.md)
 - [LineItemsSearchAPIResponse](./Models/LineItemsSearchAPIResponse.md)
 - [LineItemsSearchResult](./Models/LineItemsSearchResult.md)
 - [LitecoinAPIResponse](./Models/LitecoinAPIResponse.md)
 - [LitecoinInput](./Models/LitecoinInput.md)
 - [LitecoinTransactionInput](./Models/LitecoinTransactionInput.md)
 - [LitecoinTransactionOutput](./Models/LitecoinTransactionOutput.md)
 - [LockedData](./Models/LockedData.md)
 - [LogReturnToPercentage_200_response](./Models/LogReturnToPercentage_200_response.md)
 - [LogReturnToPercentage_200_response_data](./Models/LogReturnToPercentage_200_response_data.md)
 - [LynexAPIResponse](./Models/LynexAPIResponse.md)
 - [LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_](./Models/LynexNFTAPIResponse_LynexNFTExecuteFunctionResult_.md)
 - [LynexNFTAPIResponse_VestingPeriodData_](./Models/LynexNFTAPIResponse_VestingPeriodData_.md)
 - [LynexNFTAPIResponse_any_](./Models/LynexNFTAPIResponse_any_.md)
 - [LynexNFTAPIResponse_boolean_](./Models/LynexNFTAPIResponse_boolean_.md)
 - [LynexNFTAPIResponse_string_](./Models/LynexNFTAPIResponse_string_.md)
 - [LynexNFTExecuteFunctionResult](./Models/LynexNFTExecuteFunctionResult.md)
 - [LynexNFTInputBody](./Models/LynexNFTInputBody.md)
 - [LynexNFTTransaction](./Models/LynexNFTTransaction.md)
 - [LynexRouterAPIResponse_LynexRouterExecuteFunctionResult_](./Models/LynexRouterAPIResponse_LynexRouterExecuteFunctionResult_.md)
 - [LynexRouterAPIResponse__amountOut-string--stable-boolean__](./Models/LynexRouterAPIResponse__amountOut-string--stable-boolean__.md)
 - [LynexRouterAPIResponse__amountOut_string__stable_boolean___data](./Models/LynexRouterAPIResponse__amountOut_string__stable_boolean___data.md)
 - [LynexRouterAPIResponse_string-Array_](./Models/LynexRouterAPIResponse_string-Array_.md)
 - [LynexRouterAPIResponse_string_](./Models/LynexRouterAPIResponse_string_.md)
 - [LynexRouterExecuteFunctionResult](./Models/LynexRouterExecuteFunctionResult.md)
 - [LynexRouterInputBody](./Models/LynexRouterInputBody.md)
 - [LynexRouterTransaction](./Models/LynexRouterTransaction.md)
 - [LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_](./Models/LynexVoterAPIResponse_LynexVoterExecuteFunctionResult_.md)
 - [LynexVoterAPIResponse_boolean_](./Models/LynexVoterAPIResponse_boolean_.md)
 - [LynexVoterAPIResponse_string_](./Models/LynexVoterAPIResponse_string_.md)
 - [LynexVoterExecuteFunctionResult](./Models/LynexVoterExecuteFunctionResult.md)
 - [LynexVoterInputBody](./Models/LynexVoterInputBody.md)
 - [LynexVoterTransaction](./Models/LynexVoterTransaction.md)
 - [MakeFunTokenHelperAPIResponse_MakeFunTokenHelperExecuteFunctionResult_](./Models/MakeFunTokenHelperAPIResponse_MakeFunTokenHelperExecuteFunctionResult_.md)
 - [MakeFunTokenHelperAPIResponse_number_](./Models/MakeFunTokenHelperAPIResponse_number_.md)
 - [MakeFunTokenHelperAPIResponse_string_](./Models/MakeFunTokenHelperAPIResponse_string_.md)
 - [MakeFunTokenHelperExecuteFunctionResult](./Models/MakeFunTokenHelperExecuteFunctionResult.md)
 - [MakeFunTokenHelperInputBody](./Models/MakeFunTokenHelperInputBody.md)
 - [MakeFunTokenHelperTransaction](./Models/MakeFunTokenHelperTransaction.md)
 - [MakerOrder](./Models/MakerOrder.md)
 - [MarketPrice](./Models/MarketPrice.md)
 - [MarketTradeEvent](./Models/MarketTradeEvent.md)
 - [MarketTradeEvent_market](./Models/MarketTradeEvent_market.md)
 - [MarketTradeEvent_user](./Models/MarketTradeEvent_user.md)
 - [Message](./Models/Message.md)
 - [MultiCallAPIResponse](./Models/MultiCallAPIResponse.md)
 - [MultiCallAPIResponse_Flow-Array_](./Models/MultiCallAPIResponse_Flow-Array_.md)
 - [MultiCallAPIResponse_Flow_](./Models/MultiCallAPIResponse_Flow_.md)
 - [MultiCallAPIResponse_Jobs-Array_](./Models/MultiCallAPIResponse_Jobs-Array_.md)
 - [MultiCallAPIResponse_Jobs_](./Models/MultiCallAPIResponse_Jobs_.md)
 - [MultiCallAPIResponse_any-Array_](./Models/MultiCallAPIResponse_any-Array_.md)
 - [MultiCallAPIResponse_any_](./Models/MultiCallAPIResponse_any_.md)
 - [MultiCallAPIResponse_string_](./Models/MultiCallAPIResponse_string_.md)
 - [MultiCallInputBody](./Models/MultiCallInputBody.md)
 - [MultiCallInputBody_calls_inner](./Models/MultiCallInputBody_calls_inner.md)
 - [MultiCallInputBody_flow](./Models/MultiCallInputBody_flow.md)
 - [NFTsAPIResponse](./Models/NFTsAPIResponse.md)
 - [NarrativeTrend](./Models/NarrativeTrend.md)
 - [NarrativeTrendsAPIResponse](./Models/NarrativeTrendsAPIResponse.md)
 - [NonceAPIResponse](./Models/NonceAPIResponse.md)
 - [NonceResponse](./Models/NonceResponse.md)
 - [Notification](./Models/Notification.md)
 - [OdosAPIResponse_OdosExecuteFunctionResult_](./Models/OdosAPIResponse_OdosExecuteFunctionResult_.md)
 - [OdosExecuteFunctionResult](./Models/OdosExecuteFunctionResult.md)
 - [OdosSwapInputBody](./Models/OdosSwapInputBody.md)
 - [OdosTransaction](./Models/OdosTransaction.md)
 - [OpenOrder](./Models/OpenOrder.md)
 - [OpenSeaAPIResponse](./Models/OpenSeaAPIResponse.md)
 - [OpenSeaCollectionInputBody](./Models/OpenSeaCollectionInputBody.md)
 - [OpenSeaNFTInputBody](./Models/OpenSeaNFTInputBody.md)
 - [OptionsChainAPIResponse](./Models/OptionsChainAPIResponse.md)
 - [OptionsChainItem](./Models/OptionsChainItem.md)
 - [OrderBookSummary](./Models/OrderBookSummary.md)
 - [OrderSummary](./Models/OrderSummary.md)
 - [PaginationPayload](./Models/PaginationPayload.md)
 - [Partial_ComponentDefinition_](./Models/Partial_ComponentDefinition_.md)
 - [PathVizImageConfig](./Models/PathVizImageConfig.md)
 - [PaymentType](./Models/PaymentType.md)
 - [PersonalityInput](./Models/PersonalityInput.md)
 - [PersonalityTraits](./Models/PersonalityTraits.md)
 - [Pick_ComponentDefinition.Exclude_keyofComponentDefinition.id__](./Models/Pick_ComponentDefinition.Exclude_keyofComponentDefinition.id__.md)
 - [Pick_JupiterInputBody.Exclude_keyofJupiterInputBody.accountName__](./Models/Pick_JupiterInputBody.Exclude_keyofJupiterInputBody.accountName__.md)
 - [PingResponse](./Models/PingResponse.md)
 - [PolymarketAPIResponse_BalanceAllowanceResponse_](./Models/PolymarketAPIResponse_BalanceAllowanceResponse_.md)
 - [PolymarketAPIResponse_CancelMarketOrdersResponse_](./Models/PolymarketAPIResponse_CancelMarketOrdersResponse_.md)
 - [PolymarketAPIResponse_CancelOrderResponse_](./Models/PolymarketAPIResponse_CancelOrderResponse_.md)
 - [PolymarketAPIResponse_CancelOrdersResponse_](./Models/PolymarketAPIResponse_CancelOrdersResponse_.md)
 - [PolymarketAPIResponse_CreateMarketBuyOrderResponse_](./Models/PolymarketAPIResponse_CreateMarketBuyOrderResponse_.md)
 - [PolymarketAPIResponse_CreateOrderResponse_](./Models/PolymarketAPIResponse_CreateOrderResponse_.md)
 - [PolymarketAPIResponse_DropNotificationsResponse_](./Models/PolymarketAPIResponse_DropNotificationsResponse_.md)
 - [PolymarketAPIResponse_MarketPrice-Array_](./Models/PolymarketAPIResponse_MarketPrice-Array_.md)
 - [PolymarketAPIResponse_MarketTradeEvent-Array_](./Models/PolymarketAPIResponse_MarketTradeEvent-Array_.md)
 - [PolymarketAPIResponse_Notification-Array_](./Models/PolymarketAPIResponse_Notification-Array_.md)
 - [PolymarketAPIResponse_OpenOrder_](./Models/PolymarketAPIResponse_OpenOrder_.md)
 - [PolymarketAPIResponse_OpenOrdersResponse_](./Models/PolymarketAPIResponse_OpenOrdersResponse_.md)
 - [PolymarketAPIResponse_OrderBookSummary_](./Models/PolymarketAPIResponse_OrderBookSummary_.md)
 - [PolymarketAPIResponse_PaginationPayload_](./Models/PolymarketAPIResponse_PaginationPayload_.md)
 - [PolymarketAPIResponse_PostOrderResponse_](./Models/PolymarketAPIResponse_PostOrderResponse_.md)
 - [PolymarketAPIResponse_Trade-Array_](./Models/PolymarketAPIResponse_Trade-Array_.md)
 - [PolymarketAPIResponse_UpdateBalanceAllowanceResponse_](./Models/PolymarketAPIResponse_UpdateBalanceAllowanceResponse_.md)
 - [PolymarketAPIResponse_any_](./Models/PolymarketAPIResponse_any_.md)
 - [PolymarketWrapperNewOrder_string_](./Models/PolymarketWrapperNewOrder_string_.md)
 - [PolymarketWrapperNewOrder_string__order](./Models/PolymarketWrapperNewOrder_string__order.md)
 - [PolymarketWrapperSignedOrder](./Models/PolymarketWrapperSignedOrder.md)
 - [PoolAddressProviderAPIResponse_PoolAddressProviderExecuteFunctionResult_](./Models/PoolAddressProviderAPIResponse_PoolAddressProviderExecuteFunctionResult_.md)
 - [PoolAddressProviderAPIResponse_string_](./Models/PoolAddressProviderAPIResponse_string_.md)
 - [PoolAddressProviderExecuteFunctionResult](./Models/PoolAddressProviderExecuteFunctionResult.md)
 - [PoolAddressProviderInputBody](./Models/PoolAddressProviderInputBody.md)
 - [PoolAddressProviderRegistryAPIResponse_any-Array_](./Models/PoolAddressProviderRegistryAPIResponse_any-Array_.md)
 - [PoolAddressProviderRegistryAPIResponse_string_](./Models/PoolAddressProviderRegistryAPIResponse_string_.md)
 - [PoolAddressProviderTransaction](./Models/PoolAddressProviderTransaction.md)
 - [PortfolioAPIResponse](./Models/PortfolioAPIResponse.md)
 - [PortfolioAPIResponse_data](./Models/PortfolioAPIResponse_data.md)
 - [PostOrderBody](./Models/PostOrderBody.md)
 - [PostOrderResponse](./Models/PostOrderResponse.md)
 - [PostQuote](./Models/PostQuote.md)
 - [PredictiveMetric](./Models/PredictiveMetric.md)
 - [PredictiveMetricsAPIResponse](./Models/PredictiveMetricsAPIResponse.md)
 - [PriceData](./Models/PriceData.md)
 - [PriceInterval](./Models/PriceInterval.md)
 - [PriceSnapshot](./Models/PriceSnapshot.md)
 - [PriceSnapshotAPIResponse](./Models/PriceSnapshotAPIResponse.md)
 - [PricesAPIResponse](./Models/PricesAPIResponse.md)
 - [Quote](./Models/Quote.md)
 - [RamsesAPIResponse](./Models/RamsesAPIResponse.md)
 - [RamsesNFTAPIResponse_LockedData_](./Models/RamsesNFTAPIResponse_LockedData_.md)
 - [RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_](./Models/RamsesNFTAPIResponse_RamsesNFTExecuteFunctionResult_.md)
 - [RamsesNFTAPIResponse_string_](./Models/RamsesNFTAPIResponse_string_.md)
 - [RamsesNFTExecuteFunctionResult](./Models/RamsesNFTExecuteFunctionResult.md)
 - [RamsesNFTInputBody](./Models/RamsesNFTInputBody.md)
 - [RamsesNFTTransaction](./Models/RamsesNFTTransaction.md)
 - [RamsesRouterAPIResponse_RamsesRouterExecuteFunctionResult_](./Models/RamsesRouterAPIResponse_RamsesRouterExecuteFunctionResult_.md)
 - [RamsesRouterAPIResponse_SortedTokens_](./Models/RamsesRouterAPIResponse_SortedTokens_.md)
 - [RamsesRouterAPIResponse__amountA-string--amountB-string--liquidity-string--__](./Models/RamsesRouterAPIResponse__amountA-string--amountB-string--liquidity-string--__.md)
 - [RamsesRouterAPIResponse__amountA-string--amountB-string__](./Models/RamsesRouterAPIResponse__amountA-string--amountB-string__.md)
 - [RamsesRouterAPIResponse__amountA_string__amountB_string___data](./Models/RamsesRouterAPIResponse__amountA_string__amountB_string___data.md)
 - [RamsesRouterAPIResponse__amountA_string__amountB_string__liquidity_string_____data](./Models/RamsesRouterAPIResponse__amountA_string__amountB_string__liquidity_string_____data.md)
 - [RamsesRouterAPIResponse__amountOut-string--stable-boolean__](./Models/RamsesRouterAPIResponse__amountOut-string--stable-boolean__.md)
 - [RamsesRouterAPIResponse__reserve0%3Astring--reserve1%3Astring__](./Models/RamsesRouterAPIResponse__reserve0%3Astring--reserve1%3Astring__.md)
 - [RamsesRouterAPIResponse__reserve0_3Astring__reserve1_3Astring___data](./Models/RamsesRouterAPIResponse__reserve0_3Astring__reserve1_3Astring___data.md)
 - [RamsesRouterAPIResponse_boolean_](./Models/RamsesRouterAPIResponse_boolean_.md)
 - [RamsesRouterAPIResponse_string-Array_](./Models/RamsesRouterAPIResponse_string-Array_.md)
 - [RamsesRouterAPIResponse_string_](./Models/RamsesRouterAPIResponse_string_.md)
 - [RamsesRouterExecuteFunctionResult](./Models/RamsesRouterExecuteFunctionResult.md)
 - [RamsesRouterInputBody](./Models/RamsesRouterInputBody.md)
 - [RamsesRouterInputBody_routes_inner](./Models/RamsesRouterInputBody_routes_inner.md)
 - [RamsesRouterTransaction](./Models/RamsesRouterTransaction.md)
 - [RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_](./Models/RamsesVoterAPIResponse_RamsesVoterExecuteFunctionResult_.md)
 - [RamsesVoterAPIResponse_boolean_](./Models/RamsesVoterAPIResponse_boolean_.md)
 - [RamsesVoterAPIResponse_string_](./Models/RamsesVoterAPIResponse_string_.md)
 - [RamsesVoterExecuteFunctionResult](./Models/RamsesVoterExecuteFunctionResult.md)
 - [RamsesVoterInputBody](./Models/RamsesVoterInputBody.md)
 - [RamsesVoterTransaction](./Models/RamsesVoterTransaction.md)
 - [Record_string.any_](./Models/Record_string.any_.md)
 - [RewardInfo](./Models/RewardInfo.md)
 - [RippleAPIResponse](./Models/RippleAPIResponse.md)
 - [RippleInput](./Models/RippleInput.md)
 - [RippleTransactionInput](./Models/RippleTransactionInput.md)
 - [RippleTransactionOutput](./Models/RippleTransactionOutput.md)
 - [SRC20InscriptionInput](./Models/SRC20InscriptionInput.md)
 - [SRC20InscriptionOutput](./Models/SRC20InscriptionOutput.md)
 - [ScheduleJobBody](./Models/ScheduleJobBody.md)
 - [SearchFilter](./Models/SearchFilter.md)
 - [SearchFinancialsAPIResponse](./Models/SearchFinancialsAPIResponse.md)
 - [SearchRequest](./Models/SearchRequest.md)
 - [SearchResult](./Models/SearchResult.md)
 - [SegmentedRevenue](./Models/SegmentedRevenue.md)
 - [SegmentedRevenueItem](./Models/SegmentedRevenueItem.md)
 - [SegmentedRevenuesAPIResponse](./Models/SegmentedRevenuesAPIResponse.md)
 - [SellQuote](./Models/SellQuote.md)
 - [Side](./Models/Side.md)
 - [SignMessage](./Models/SignMessage.md)
 - [SignMessageAPIResponse](./Models/SignMessageAPIResponse.md)
 - [SignTypedData](./Models/SignTypedData.md)
 - [SimulateAssetChangesChange](./Models/SimulateAssetChangesChange.md)
 - [SimulateAssetChangesError](./Models/SimulateAssetChangesError.md)
 - [SimulateAssetChangesResponse](./Models/SimulateAssetChangesResponse.md)
 - [SimulateAssetType](./Models/SimulateAssetType.md)
 - [SimulateChangeType](./Models/SimulateChangeType.md)
 - [SolanaAPIResponse](./Models/SolanaAPIResponse.md)
 - [SolanaInput](./Models/SolanaInput.md)
 - [SolanaSignTransactionInput](./Models/SolanaSignTransactionInput.md)
 - [SolanaTransactionInput](./Models/SolanaTransactionInput.md)
 - [SolanaTransactionOutput](./Models/SolanaTransactionOutput.md)
 - [SortedTokens](./Models/SortedTokens.md)
 - [StatusResponse](./Models/StatusResponse.md)
 - [Step](./Models/Step.md)
 - [SuccessResponse_249_inner](./Models/SuccessResponse_249_inner.md)
 - [SupportedAssetResponse](./Models/SupportedAssetResponse.md)
 - [SupportedAssetResponse_assets_inner](./Models/SupportedAssetResponse_assets_inner.md)
 - [SupportedCurrenciesResponse](./Models/SupportedCurrenciesResponse.md)
 - [SupportedDefaultResponse](./Models/SupportedDefaultResponse.md)
 - [SupportedDefaultResponse_defaults](./Models/SupportedDefaultResponse_defaults.md)
 - [SupportedDefaultResponse_defaults_id](./Models/SupportedDefaultResponse_defaults_id.md)
 - [SupportedDefaultResponse_recommended](./Models/SupportedDefaultResponse_recommended.md)
 - [SupportedPaymentTypesCurrencyResponse](./Models/SupportedPaymentTypesCurrencyResponse.md)
 - [SupportedPaymentTypesMessage](./Models/SupportedPaymentTypesMessage.md)
 - [Swap_request](./Models/Swap_request.md)
 - [ThenaAPIResponse](./Models/ThenaAPIResponse.md)
 - [ThorSwapAPIResponse_GasPrice_](./Models/ThorSwapAPIResponse_GasPrice_.md)
 - [ThorSwapAPIResponse_Quote_](./Models/ThorSwapAPIResponse_Quote_.md)
 - [ThorSwapAPIResponse_string-Array_](./Models/ThorSwapAPIResponse_string-Array_.md)
 - [ThorSwapAPIResponse_string_](./Models/ThorSwapAPIResponse_string_.md)
 - [TimeFrame](./Models/TimeFrame.md)
 - [Token](./Models/Token.md)
 - [TokenAmount](./Models/TokenAmount.md)
 - [TokenAnalytics](./Models/TokenAnalytics.md)
 - [TokenAnalyticsAPIResponse](./Models/TokenAnalyticsAPIResponse.md)
 - [TokenConfig](./Models/TokenConfig.md)
 - [TokenDetails](./Models/TokenDetails.md)
 - [TokenInfo](./Models/TokenInfo.md)
 - [TokenMetadataAPIResponse](./Models/TokenMetadataAPIResponse.md)
 - [TokenProportion](./Models/TokenProportion.md)
 - [TokensResponse](./Models/TokensResponse.md)
 - [ToolsResponse](./Models/ToolsResponse.md)
 - [Trade](./Models/Trade.md)
 - [Trade_side](./Models/Trade_side.md)
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
 - [TransactionStatus](./Models/TransactionStatus.md)
 - [TrendingToken](./Models/TrendingToken.md)
 - [TrendingTokensAPIResponse](./Models/TrendingTokensAPIResponse.md)
 - [TrendingTweet](./Models/TrendingTweet.md)
 - [TrendingTweetsAPIResponse](./Models/TrendingTweetsAPIResponse.md)
 - [TronAPIResponse](./Models/TronAPIResponse.md)
 - [TronInput](./Models/TronInput.md)
 - [TronTransactionInput](./Models/TronTransactionInput.md)
 - [TronTransactionOutput](./Models/TronTransactionOutput.md)
 - [Tx](./Models/Tx.md)
 - [UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_](./Models/UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_.md)
 - [UniswapV2ExecuteFunctionResult](./Models/UniswapV2ExecuteFunctionResult.md)
 - [UniswapV2InputBody](./Models/UniswapV2InputBody.md)
 - [UniswapV2Transaction](./Models/UniswapV2Transaction.md)
 - [UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_](./Models/UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_.md)
 - [UniswapV3APIResponse_string_](./Models/UniswapV3APIResponse_string_.md)
 - [UniswapV3ExecuteFunctionResult](./Models/UniswapV3ExecuteFunctionResult.md)
 - [UniswapV3InputBody](./Models/UniswapV3InputBody.md)
 - [UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_](./Models/UniswapV3NFTAPIResponse_UniswapV3ExecuteFunctionResult_.md)
 - [UniswapV3NFTAPIResponse_any_](./Models/UniswapV3NFTAPIResponse_any_.md)
 - [UniswapV3NFTAPIResponse_boolean_](./Models/UniswapV3NFTAPIResponse_boolean_.md)
 - [UniswapV3NFTAPIResponse_string_](./Models/UniswapV3NFTAPIResponse_string_.md)
 - [UniswapV3Transaction](./Models/UniswapV3Transaction.md)
 - [UnsignedPSBTInput](./Models/UnsignedPSBTInput.md)
 - [UnsignedPSBTOutput](./Models/UnsignedPSBTOutput.md)
 - [UpdateBalanceAllowanceBody](./Models/UpdateBalanceAllowanceBody.md)
 - [UpdateBalanceAllowanceBody_params](./Models/UpdateBalanceAllowanceBody_params.md)
 - [UpdateBalanceAllowanceResponse](./Models/UpdateBalanceAllowanceResponse.md)
 - [UpdateFlowBody](./Models/UpdateFlowBody.md)
 - [UserIncentiveData](./Models/UserIncentiveData.md)
 - [UserPointHistoryData](./Models/UserPointHistoryData.md)
 - [UserReserveData](./Models/UserReserveData.md)
 - [UserReserveIncentiveData](./Models/UserReserveIncentiveData.md)
 - [UserRewardInfo](./Models/UserRewardInfo.md)
 - [VeNFTExecuteFunctionResult](./Models/VeNFTExecuteFunctionResult.md)
 - [VeNFTInputBody](./Models/VeNFTInputBody.md)
 - [VeNFTTransaction](./Models/VeNFTTransaction.md)
 - [VeTheNFTAPIResponse_LockedData_](./Models/VeTheNFTAPIResponse_LockedData_.md)
 - [VeTheNFTAPIResponse_UserPointHistoryData_](./Models/VeTheNFTAPIResponse_UserPointHistoryData_.md)
 - [VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_](./Models/VeTheNFTAPIResponse_VeNFTExecuteFunctionResult_.md)
 - [VeTheNFTAPIResponse_boolean_](./Models/VeTheNFTAPIResponse_boolean_.md)
 - [VeTheNFTAPIResponse_string_](./Models/VeTheNFTAPIResponse_string_.md)
 - [VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_](./Models/VeTheNftVoterAPIResponse_VeTheNftVoterExecuteFunctionResult_.md)
 - [VeTheNftVoterAPIResponse_boolean_](./Models/VeTheNftVoterAPIResponse_boolean_.md)
 - [VeTheNftVoterAPIResponse_string_](./Models/VeTheNftVoterAPIResponse_string_.md)
 - [VeTheNftVoterExecuteFunctionResult](./Models/VeTheNftVoterExecuteFunctionResult.md)
 - [VeTheNftVoterInputBody](./Models/VeTheNftVoterInputBody.md)
 - [VeTheNftVoterTransaction](./Models/VeTheNftVoterTransaction.md)
 - [VestingPeriodData](./Models/VestingPeriodData.md)
 - [VoteWithOptimalDistribution_request](./Models/VoteWithOptimalDistribution_request.md)
 - [VoteWithOptimalDistribution_request_1](./Models/VoteWithOptimalDistribution_request_1.md)
 - [VoteWithOptimalDistribution_request_2](./Models/VoteWithOptimalDistribution_request_2.md)
 - [WalletBalanceAPIResponse](./Models/WalletBalanceAPIResponse.md)
 - [WalletHistoryAPIResponse](./Models/WalletHistoryAPIResponse.md)
 - [WrapEth_request](./Models/WrapEth_request.md)


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

