# CustomDistanceMatrices

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ProfileMatrices** | Pointer to **map[string]map[string]string** | Map of vehicle profile names (CAR, BIKE, TRUCK) to time slice hour mappings. Each time slice hour maps to a matrix ID that should be fetched from the distance matrix service. Time slice hours correspond to: 6&#x3D;MORNING_RUSH, 9&#x3D;MORNING, 12&#x3D;MIDDAY, 14&#x3D;AFTERNOON, 16&#x3D;EVENING_RUSH, 20&#x3D;NIGHT. | [optional] 
**MatrixServiceUrl** | Pointer to **NullableString** | Optional URL for external distance matrix service endpoint. If not provided, uses the default system service. | [optional] 

## Methods

### NewCustomDistanceMatrices

`func NewCustomDistanceMatrices() *CustomDistanceMatrices`

NewCustomDistanceMatrices instantiates a new CustomDistanceMatrices object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCustomDistanceMatricesWithDefaults

`func NewCustomDistanceMatricesWithDefaults() *CustomDistanceMatrices`

NewCustomDistanceMatricesWithDefaults instantiates a new CustomDistanceMatrices object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetProfileMatrices

`func (o *CustomDistanceMatrices) GetProfileMatrices() map[string]map[string]string`

GetProfileMatrices returns the ProfileMatrices field if non-nil, zero value otherwise.

### GetProfileMatricesOk

`func (o *CustomDistanceMatrices) GetProfileMatricesOk() (*map[string]map[string]string, bool)`

GetProfileMatricesOk returns a tuple with the ProfileMatrices field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProfileMatrices

`func (o *CustomDistanceMatrices) SetProfileMatrices(v map[string]map[string]string)`

SetProfileMatrices sets ProfileMatrices field to given value.

### HasProfileMatrices

`func (o *CustomDistanceMatrices) HasProfileMatrices() bool`

HasProfileMatrices returns a boolean if a field has been set.

### SetProfileMatricesNil

`func (o *CustomDistanceMatrices) SetProfileMatricesNil(b bool)`

 SetProfileMatricesNil sets the value for ProfileMatrices to be an explicit nil

### UnsetProfileMatrices
`func (o *CustomDistanceMatrices) UnsetProfileMatrices()`

UnsetProfileMatrices ensures that no value is present for ProfileMatrices, not even an explicit nil
### GetMatrixServiceUrl

`func (o *CustomDistanceMatrices) GetMatrixServiceUrl() string`

GetMatrixServiceUrl returns the MatrixServiceUrl field if non-nil, zero value otherwise.

### GetMatrixServiceUrlOk

`func (o *CustomDistanceMatrices) GetMatrixServiceUrlOk() (*string, bool)`

GetMatrixServiceUrlOk returns a tuple with the MatrixServiceUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMatrixServiceUrl

`func (o *CustomDistanceMatrices) SetMatrixServiceUrl(v string)`

SetMatrixServiceUrl sets MatrixServiceUrl field to given value.

### HasMatrixServiceUrl

`func (o *CustomDistanceMatrices) HasMatrixServiceUrl() bool`

HasMatrixServiceUrl returns a boolean if a field has been set.

### SetMatrixServiceUrlNil

`func (o *CustomDistanceMatrices) SetMatrixServiceUrlNil(b bool)`

 SetMatrixServiceUrlNil sets the value for MatrixServiceUrl to be an explicit nil

### UnsetMatrixServiceUrl
`func (o *CustomDistanceMatrices) UnsetMatrixServiceUrl()`

UnsetMatrixServiceUrl ensures that no value is present for MatrixServiceUrl, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


