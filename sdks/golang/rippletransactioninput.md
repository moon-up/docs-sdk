# RippleTransactionInput

## Properties

| Name         | Type                   | Description | Notes       |
| ------------ | ---------------------- | ----------- | ----------- |
| **To**       | Pointer to **string**  |             | \[optional] |
| **Value**    | Pointer to **float64** |             | \[optional] |
| **Network**  | Pointer to **string**  |             | \[optional] |
| **Compress** | Pointer to **bool**    |             | \[optional] |

## Methods

### NewRippleTransactionInput

`func NewRippleTransactionInput() *RippleTransactionInput`

NewRippleTransactionInput instantiates a new RippleTransactionInput object This constructor will assign default values to properties that have it defined, and makes sure properties required by API are set, but the set of arguments will change when the set of required properties is changed

### NewRippleTransactionInputWithDefaults

`func NewRippleTransactionInputWithDefaults() *RippleTransactionInput`

NewRippleTransactionInputWithDefaults instantiates a new RippleTransactionInput object This constructor will only assign default values to properties that have it defined, but it doesn't guarantee that properties required by API are set

### GetTo

`func (o *RippleTransactionInput) GetTo() string`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *RippleTransactionInput) GetToOk() (*string, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise and a boolean to check if the value has been set.

### SetTo

`func (o *RippleTransactionInput) SetTo(v string)`

SetTo sets To field to given value.

### HasTo

`func (o *RippleTransactionInput) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetValue

`func (o *RippleTransactionInput) GetValue() float64`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *RippleTransactionInput) GetValueOk() (*float64, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise and a boolean to check if the value has been set.

### SetValue

`func (o *RippleTransactionInput) SetValue(v float64)`

SetValue sets Value field to given value.

### HasValue

`func (o *RippleTransactionInput) HasValue() bool`

HasValue returns a boolean if a field has been set.

### GetNetwork

`func (o *RippleTransactionInput) GetNetwork() string`

GetNetwork returns the Network field if non-nil, zero value otherwise.

### GetNetworkOk

`func (o *RippleTransactionInput) GetNetworkOk() (*string, bool)`

GetNetworkOk returns a tuple with the Network field if it's non-nil, zero value otherwise and a boolean to check if the value has been set.

### SetNetwork

`func (o *RippleTransactionInput) SetNetwork(v string)`

SetNetwork sets Network field to given value.

### HasNetwork

`func (o *RippleTransactionInput) HasNetwork() bool`

HasNetwork returns a boolean if a field has been set.

### GetCompress

`func (o *RippleTransactionInput) GetCompress() bool`

GetCompress returns the Compress field if non-nil, zero value otherwise.

### GetCompressOk

`func (o *RippleTransactionInput) GetCompressOk() (*bool, bool)`

GetCompressOk returns a tuple with the Compress field if it's non-nil, zero value otherwise and a boolean to check if the value has been set.

### SetCompress

`func (o *RippleTransactionInput) SetCompress(v bool)`

SetCompress sets Compress field to given value.

### HasCompress

`func (o *RippleTransactionInput) HasCompress() bool`

HasCompress returns a boolean if a field has been set.

\[Back to Model list] \[Back to API list] \[Back to README]
