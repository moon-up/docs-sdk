# LitecoinInput

## Properties

| Name           | Type                  | Description | Notes       |
| -------------- | --------------------- | ----------- | ----------- |
| **Network**    | Pointer to **string** |             | \[optional] |
| **PrivateKey** | Pointer to **string** |             | \[optional] |

## Methods

### NewLitecoinInput

`func NewLitecoinInput() *LitecoinInput`

NewLitecoinInput instantiates a new LitecoinInput object This constructor will assign default values to properties that have it defined, and makes sure properties required by API are set, but the set of arguments will change when the set of required properties is changed

### NewLitecoinInputWithDefaults

`func NewLitecoinInputWithDefaults() *LitecoinInput`

NewLitecoinInputWithDefaults instantiates a new LitecoinInput object This constructor will only assign default values to properties that have it defined, but it doesn't guarantee that properties required by API are set

### GetNetwork

`func (o *LitecoinInput) GetNetwork() string`

GetNetwork returns the Network field if non-nil, zero value otherwise.

### GetNetworkOk

`func (o *LitecoinInput) GetNetworkOk() (*string, bool)`

GetNetworkOk returns a tuple with the Network field if it's non-nil, zero value otherwise and a boolean to check if the value has been set.

### SetNetwork

`func (o *LitecoinInput) SetNetwork(v string)`

SetNetwork sets Network field to given value.

### HasNetwork

`func (o *LitecoinInput) HasNetwork() bool`

HasNetwork returns a boolean if a field has been set.

### GetPrivateKey

`func (o *LitecoinInput) GetPrivateKey() string`

GetPrivateKey returns the PrivateKey field if non-nil, zero value otherwise.

### GetPrivateKeyOk

`func (o *LitecoinInput) GetPrivateKeyOk() (*string, bool)`

GetPrivateKeyOk returns a tuple with the PrivateKey field if it's non-nil, zero value otherwise and a boolean to check if the value has been set.

### SetPrivateKey

`func (o *LitecoinInput) SetPrivateKey(v string)`

SetPrivateKey sets PrivateKey field to given value.

### HasPrivateKey

`func (o *LitecoinInput) HasPrivateKey() bool`

HasPrivateKey returns a boolean if a field has been set.

\[Back to Model list] \[Back to API list] \[Back to README]
