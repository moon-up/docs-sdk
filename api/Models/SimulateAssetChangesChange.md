# SimulateAssetChangesChange
## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
| **assetType** | [**SimulateAssetType**](SimulateAssetType.md) |  | [default to null] |
| **changeType** | [**SimulateChangeType**](SimulateChangeType.md) |  | [default to null] |
| **from** | **String** | The from address. | [default to null] |
| **to** | **String** | The to address. | [default to null] |
| **rawAmount** | **String** | The raw amount as an integer string. Only available on TRANSFER changes for NATIVE and ERC20 assets, or ERC721/ERC1155 disapprove changes (field set to &#39;0&#39;). | [optional] [default to null] |
| **amount** | **String** | The amount as an integer string. This value is calculated by applying the &#x60;decimals&#x60; field to the &#x60;rawAmount&#x60; field. Only available on TRANSFER changes for NATIVE and ERC20 assets, or ERC721/ERC1155 disapprove changes (field set to &#39;0&#39;). | [optional] [default to null] |
| **name** | **String** | The name of the asset transferred, if available. | [optional] [default to null] |
| **symbol** | **String** | The symbol of the asset transferred if available. | [optional] [default to null] |
| **decimals** | **Double** | The number of decimals used by the ERC20 token. Set to 0 for APPROVE changes. Field is undefined if it&#39;s not defined in the contract and not available from other sources. | [optional] [default to null] |
| **contractAddress** | **String** | The contract address of the asset. Only applicable to ERC20, ERC721, ERC1155, NFT and SPECIAL_NFT transactions. | [optional] [default to null] |
| **logo** | **String** | URL for the logo of the asset, if available. Only applicable to ERC20 transactions. | [optional] [default to null] |
| **tokenId** | **String** | The token id of the asset transferred. Only applicable to ERC721, ERC1155 and SPECIAL_NFT NFTs. | [optional] [default to null] |

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

