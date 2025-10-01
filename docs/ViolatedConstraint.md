# ViolatedConstraint

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **NullableString** | Name of the constraint. | 
**Value** | **NullableInt32** | Value of the unresolved constraint. The higher, the more deviation from perfection this constraint has. | 
**Level** | [**NullableLevel**](Level.md) | Level of unresolved constraint. | 

## Methods

### NewViolatedConstraint

`func NewViolatedConstraint(name NullableString, value NullableInt32, level NullableLevel, ) *ViolatedConstraint`

NewViolatedConstraint instantiates a new ViolatedConstraint object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewViolatedConstraintWithDefaults

`func NewViolatedConstraintWithDefaults() *ViolatedConstraint`

NewViolatedConstraintWithDefaults instantiates a new ViolatedConstraint object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *ViolatedConstraint) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ViolatedConstraint) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ViolatedConstraint) SetName(v string)`

SetName sets Name field to given value.


### SetNameNil

`func (o *ViolatedConstraint) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *ViolatedConstraint) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil
### GetValue

`func (o *ViolatedConstraint) GetValue() int32`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *ViolatedConstraint) GetValueOk() (*int32, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *ViolatedConstraint) SetValue(v int32)`

SetValue sets Value field to given value.


### SetValueNil

`func (o *ViolatedConstraint) SetValueNil(b bool)`

 SetValueNil sets the value for Value to be an explicit nil

### UnsetValue
`func (o *ViolatedConstraint) UnsetValue()`

UnsetValue ensures that no value is present for Value, not even an explicit nil
### GetLevel

`func (o *ViolatedConstraint) GetLevel() Level`

GetLevel returns the Level field if non-nil, zero value otherwise.

### GetLevelOk

`func (o *ViolatedConstraint) GetLevelOk() (*Level, bool)`

GetLevelOk returns a tuple with the Level field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLevel

`func (o *ViolatedConstraint) SetLevel(v Level)`

SetLevel sets Level field to given value.


### SetLevelNil

`func (o *ViolatedConstraint) SetLevelNil(b bool)`

 SetLevelNil sets the value for Level to be an explicit nil

### UnsetLevel
`func (o *ViolatedConstraint) UnsetLevel()`

UnsetLevel ensures that no value is present for Level, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


