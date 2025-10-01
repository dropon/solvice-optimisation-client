# DateWindow

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**From** | **string** | Date time start of window | 
**To** | **string** | Date time end of window | 
**Weight** | Pointer to **NullableInt32** | Weight constraint modifier | [optional] [default to 1]
**Hard** | Pointer to **NullableBool** | Hard constraint violation of DateWindow | [optional] [default to true]

## Methods

### NewDateWindow

`func NewDateWindow(from string, to string, ) *DateWindow`

NewDateWindow instantiates a new DateWindow object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDateWindowWithDefaults

`func NewDateWindowWithDefaults() *DateWindow`

NewDateWindowWithDefaults instantiates a new DateWindow object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFrom

`func (o *DateWindow) GetFrom() string`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *DateWindow) GetFromOk() (*string, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *DateWindow) SetFrom(v string)`

SetFrom sets From field to given value.


### GetTo

`func (o *DateWindow) GetTo() string`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *DateWindow) GetToOk() (*string, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *DateWindow) SetTo(v string)`

SetTo sets To field to given value.


### GetWeight

`func (o *DateWindow) GetWeight() int32`

GetWeight returns the Weight field if non-nil, zero value otherwise.

### GetWeightOk

`func (o *DateWindow) GetWeightOk() (*int32, bool)`

GetWeightOk returns a tuple with the Weight field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWeight

`func (o *DateWindow) SetWeight(v int32)`

SetWeight sets Weight field to given value.

### HasWeight

`func (o *DateWindow) HasWeight() bool`

HasWeight returns a boolean if a field has been set.

### SetWeightNil

`func (o *DateWindow) SetWeightNil(b bool)`

 SetWeightNil sets the value for Weight to be an explicit nil

### UnsetWeight
`func (o *DateWindow) UnsetWeight()`

UnsetWeight ensures that no value is present for Weight, not even an explicit nil
### GetHard

`func (o *DateWindow) GetHard() bool`

GetHard returns the Hard field if non-nil, zero value otherwise.

### GetHardOk

`func (o *DateWindow) GetHardOk() (*bool, bool)`

GetHardOk returns a tuple with the Hard field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHard

`func (o *DateWindow) SetHard(v bool)`

SetHard sets Hard field to given value.

### HasHard

`func (o *DateWindow) HasHard() bool`

HasHard returns a boolean if a field has been set.

### SetHardNil

`func (o *DateWindow) SetHardNil(b bool)`

 SetHardNil sets the value for Hard to be an explicit nil

### UnsetHard
`func (o *DateWindow) UnsetHard()`

UnsetHard ensures that no value is present for Hard, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


