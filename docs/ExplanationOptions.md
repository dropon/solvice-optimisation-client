# ExplanationOptions

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | Pointer to **NullableBool** | When enabled the explanation will contain a map of all the alternative positions for each job | [optional] 
**FilterHardConstraints** | Pointer to **NullableBool** | When true the map of alternative positions will contain only feasible alternatives | [optional] 
**OnlyUnassigned** | Pointer to **NullableBool** |  | [optional] 

## Methods

### NewExplanationOptions

`func NewExplanationOptions() *ExplanationOptions`

NewExplanationOptions instantiates a new ExplanationOptions object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewExplanationOptionsWithDefaults

`func NewExplanationOptionsWithDefaults() *ExplanationOptions`

NewExplanationOptionsWithDefaults instantiates a new ExplanationOptions object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEnabled

`func (o *ExplanationOptions) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *ExplanationOptions) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *ExplanationOptions) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *ExplanationOptions) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### SetEnabledNil

`func (o *ExplanationOptions) SetEnabledNil(b bool)`

 SetEnabledNil sets the value for Enabled to be an explicit nil

### UnsetEnabled
`func (o *ExplanationOptions) UnsetEnabled()`

UnsetEnabled ensures that no value is present for Enabled, not even an explicit nil
### GetFilterHardConstraints

`func (o *ExplanationOptions) GetFilterHardConstraints() bool`

GetFilterHardConstraints returns the FilterHardConstraints field if non-nil, zero value otherwise.

### GetFilterHardConstraintsOk

`func (o *ExplanationOptions) GetFilterHardConstraintsOk() (*bool, bool)`

GetFilterHardConstraintsOk returns a tuple with the FilterHardConstraints field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilterHardConstraints

`func (o *ExplanationOptions) SetFilterHardConstraints(v bool)`

SetFilterHardConstraints sets FilterHardConstraints field to given value.

### HasFilterHardConstraints

`func (o *ExplanationOptions) HasFilterHardConstraints() bool`

HasFilterHardConstraints returns a boolean if a field has been set.

### SetFilterHardConstraintsNil

`func (o *ExplanationOptions) SetFilterHardConstraintsNil(b bool)`

 SetFilterHardConstraintsNil sets the value for FilterHardConstraints to be an explicit nil

### UnsetFilterHardConstraints
`func (o *ExplanationOptions) UnsetFilterHardConstraints()`

UnsetFilterHardConstraints ensures that no value is present for FilterHardConstraints, not even an explicit nil
### GetOnlyUnassigned

`func (o *ExplanationOptions) GetOnlyUnassigned() bool`

GetOnlyUnassigned returns the OnlyUnassigned field if non-nil, zero value otherwise.

### GetOnlyUnassignedOk

`func (o *ExplanationOptions) GetOnlyUnassignedOk() (*bool, bool)`

GetOnlyUnassignedOk returns a tuple with the OnlyUnassigned field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOnlyUnassigned

`func (o *ExplanationOptions) SetOnlyUnassigned(v bool)`

SetOnlyUnassigned sets OnlyUnassigned field to given value.

### HasOnlyUnassigned

`func (o *ExplanationOptions) HasOnlyUnassigned() bool`

HasOnlyUnassigned returns a boolean if a field has been set.

### SetOnlyUnassignedNil

`func (o *ExplanationOptions) SetOnlyUnassignedNil(b bool)`

 SetOnlyUnassignedNil sets the value for OnlyUnassigned to be an explicit nil

### UnsetOnlyUnassigned
`func (o *ExplanationOptions) UnsetOnlyUnassigned()`

UnsetOnlyUnassigned ensures that no value is present for OnlyUnassigned, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


