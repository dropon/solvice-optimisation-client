# Rule

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Period** | Pointer to [**PeriodDto**](PeriodDto.md) | Period of the rule. If null, then it encompasses the entire period. | [optional] 
**MinWorkTime** | Pointer to **NullableInt32** | Minimum work time in seconds. Work time is service time + drive/travel time. | [optional] 
**MaxWorkTime** | Pointer to **NullableInt32** | Maximum work time in seconds. Work time is service time + drive/travel time. | [optional] 
**MinServiceTime** | Pointer to **NullableInt32** | Minimum service time in seconds | [optional] 
**MaxServiceTime** | Pointer to **NullableInt32** | Maximum service time in seconds | [optional] 
**MinDriveTime** | Pointer to **NullableInt32** | Minimum drive time in seconds | [optional] 
**MaxDriveTime** | Pointer to **NullableInt32** | Maximum drive time in seconds | [optional] 
**MinJobComplexity** | Pointer to **NullableInt32** | Sum of the complexity of the jobs completed by this resource should reach this value | [optional] 
**MaxJobComplexity** | Pointer to **NullableInt32** | Sum of the complexity of the jobs completed by this resource should not go over this value | [optional] 
**JobTypeLimitations** | Pointer to **map[string]int32** | Map of job type to maximum count allowed per period. Null means no limitations. | [optional] 

## Methods

### NewRule

`func NewRule() *Rule`

NewRule instantiates a new Rule object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRuleWithDefaults

`func NewRuleWithDefaults() *Rule`

NewRuleWithDefaults instantiates a new Rule object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPeriod

`func (o *Rule) GetPeriod() PeriodDto`

GetPeriod returns the Period field if non-nil, zero value otherwise.

### GetPeriodOk

`func (o *Rule) GetPeriodOk() (*PeriodDto, bool)`

GetPeriodOk returns a tuple with the Period field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPeriod

`func (o *Rule) SetPeriod(v PeriodDto)`

SetPeriod sets Period field to given value.

### HasPeriod

`func (o *Rule) HasPeriod() bool`

HasPeriod returns a boolean if a field has been set.

### GetMinWorkTime

`func (o *Rule) GetMinWorkTime() int32`

GetMinWorkTime returns the MinWorkTime field if non-nil, zero value otherwise.

### GetMinWorkTimeOk

`func (o *Rule) GetMinWorkTimeOk() (*int32, bool)`

GetMinWorkTimeOk returns a tuple with the MinWorkTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMinWorkTime

`func (o *Rule) SetMinWorkTime(v int32)`

SetMinWorkTime sets MinWorkTime field to given value.

### HasMinWorkTime

`func (o *Rule) HasMinWorkTime() bool`

HasMinWorkTime returns a boolean if a field has been set.

### SetMinWorkTimeNil

`func (o *Rule) SetMinWorkTimeNil(b bool)`

 SetMinWorkTimeNil sets the value for MinWorkTime to be an explicit nil

### UnsetMinWorkTime
`func (o *Rule) UnsetMinWorkTime()`

UnsetMinWorkTime ensures that no value is present for MinWorkTime, not even an explicit nil
### GetMaxWorkTime

`func (o *Rule) GetMaxWorkTime() int32`

GetMaxWorkTime returns the MaxWorkTime field if non-nil, zero value otherwise.

### GetMaxWorkTimeOk

`func (o *Rule) GetMaxWorkTimeOk() (*int32, bool)`

GetMaxWorkTimeOk returns a tuple with the MaxWorkTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxWorkTime

`func (o *Rule) SetMaxWorkTime(v int32)`

SetMaxWorkTime sets MaxWorkTime field to given value.

### HasMaxWorkTime

`func (o *Rule) HasMaxWorkTime() bool`

HasMaxWorkTime returns a boolean if a field has been set.

### SetMaxWorkTimeNil

`func (o *Rule) SetMaxWorkTimeNil(b bool)`

 SetMaxWorkTimeNil sets the value for MaxWorkTime to be an explicit nil

### UnsetMaxWorkTime
`func (o *Rule) UnsetMaxWorkTime()`

UnsetMaxWorkTime ensures that no value is present for MaxWorkTime, not even an explicit nil
### GetMinServiceTime

`func (o *Rule) GetMinServiceTime() int32`

GetMinServiceTime returns the MinServiceTime field if non-nil, zero value otherwise.

### GetMinServiceTimeOk

`func (o *Rule) GetMinServiceTimeOk() (*int32, bool)`

GetMinServiceTimeOk returns a tuple with the MinServiceTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMinServiceTime

`func (o *Rule) SetMinServiceTime(v int32)`

SetMinServiceTime sets MinServiceTime field to given value.

### HasMinServiceTime

`func (o *Rule) HasMinServiceTime() bool`

HasMinServiceTime returns a boolean if a field has been set.

### SetMinServiceTimeNil

`func (o *Rule) SetMinServiceTimeNil(b bool)`

 SetMinServiceTimeNil sets the value for MinServiceTime to be an explicit nil

### UnsetMinServiceTime
`func (o *Rule) UnsetMinServiceTime()`

UnsetMinServiceTime ensures that no value is present for MinServiceTime, not even an explicit nil
### GetMaxServiceTime

`func (o *Rule) GetMaxServiceTime() int32`

GetMaxServiceTime returns the MaxServiceTime field if non-nil, zero value otherwise.

### GetMaxServiceTimeOk

`func (o *Rule) GetMaxServiceTimeOk() (*int32, bool)`

GetMaxServiceTimeOk returns a tuple with the MaxServiceTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxServiceTime

`func (o *Rule) SetMaxServiceTime(v int32)`

SetMaxServiceTime sets MaxServiceTime field to given value.

### HasMaxServiceTime

`func (o *Rule) HasMaxServiceTime() bool`

HasMaxServiceTime returns a boolean if a field has been set.

### SetMaxServiceTimeNil

`func (o *Rule) SetMaxServiceTimeNil(b bool)`

 SetMaxServiceTimeNil sets the value for MaxServiceTime to be an explicit nil

### UnsetMaxServiceTime
`func (o *Rule) UnsetMaxServiceTime()`

UnsetMaxServiceTime ensures that no value is present for MaxServiceTime, not even an explicit nil
### GetMinDriveTime

`func (o *Rule) GetMinDriveTime() int32`

GetMinDriveTime returns the MinDriveTime field if non-nil, zero value otherwise.

### GetMinDriveTimeOk

`func (o *Rule) GetMinDriveTimeOk() (*int32, bool)`

GetMinDriveTimeOk returns a tuple with the MinDriveTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMinDriveTime

`func (o *Rule) SetMinDriveTime(v int32)`

SetMinDriveTime sets MinDriveTime field to given value.

### HasMinDriveTime

`func (o *Rule) HasMinDriveTime() bool`

HasMinDriveTime returns a boolean if a field has been set.

### SetMinDriveTimeNil

`func (o *Rule) SetMinDriveTimeNil(b bool)`

 SetMinDriveTimeNil sets the value for MinDriveTime to be an explicit nil

### UnsetMinDriveTime
`func (o *Rule) UnsetMinDriveTime()`

UnsetMinDriveTime ensures that no value is present for MinDriveTime, not even an explicit nil
### GetMaxDriveTime

`func (o *Rule) GetMaxDriveTime() int32`

GetMaxDriveTime returns the MaxDriveTime field if non-nil, zero value otherwise.

### GetMaxDriveTimeOk

`func (o *Rule) GetMaxDriveTimeOk() (*int32, bool)`

GetMaxDriveTimeOk returns a tuple with the MaxDriveTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxDriveTime

`func (o *Rule) SetMaxDriveTime(v int32)`

SetMaxDriveTime sets MaxDriveTime field to given value.

### HasMaxDriveTime

`func (o *Rule) HasMaxDriveTime() bool`

HasMaxDriveTime returns a boolean if a field has been set.

### SetMaxDriveTimeNil

`func (o *Rule) SetMaxDriveTimeNil(b bool)`

 SetMaxDriveTimeNil sets the value for MaxDriveTime to be an explicit nil

### UnsetMaxDriveTime
`func (o *Rule) UnsetMaxDriveTime()`

UnsetMaxDriveTime ensures that no value is present for MaxDriveTime, not even an explicit nil
### GetMinJobComplexity

`func (o *Rule) GetMinJobComplexity() int32`

GetMinJobComplexity returns the MinJobComplexity field if non-nil, zero value otherwise.

### GetMinJobComplexityOk

`func (o *Rule) GetMinJobComplexityOk() (*int32, bool)`

GetMinJobComplexityOk returns a tuple with the MinJobComplexity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMinJobComplexity

`func (o *Rule) SetMinJobComplexity(v int32)`

SetMinJobComplexity sets MinJobComplexity field to given value.

### HasMinJobComplexity

`func (o *Rule) HasMinJobComplexity() bool`

HasMinJobComplexity returns a boolean if a field has been set.

### SetMinJobComplexityNil

`func (o *Rule) SetMinJobComplexityNil(b bool)`

 SetMinJobComplexityNil sets the value for MinJobComplexity to be an explicit nil

### UnsetMinJobComplexity
`func (o *Rule) UnsetMinJobComplexity()`

UnsetMinJobComplexity ensures that no value is present for MinJobComplexity, not even an explicit nil
### GetMaxJobComplexity

`func (o *Rule) GetMaxJobComplexity() int32`

GetMaxJobComplexity returns the MaxJobComplexity field if non-nil, zero value otherwise.

### GetMaxJobComplexityOk

`func (o *Rule) GetMaxJobComplexityOk() (*int32, bool)`

GetMaxJobComplexityOk returns a tuple with the MaxJobComplexity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxJobComplexity

`func (o *Rule) SetMaxJobComplexity(v int32)`

SetMaxJobComplexity sets MaxJobComplexity field to given value.

### HasMaxJobComplexity

`func (o *Rule) HasMaxJobComplexity() bool`

HasMaxJobComplexity returns a boolean if a field has been set.

### SetMaxJobComplexityNil

`func (o *Rule) SetMaxJobComplexityNil(b bool)`

 SetMaxJobComplexityNil sets the value for MaxJobComplexity to be an explicit nil

### UnsetMaxJobComplexity
`func (o *Rule) UnsetMaxJobComplexity()`

UnsetMaxJobComplexity ensures that no value is present for MaxJobComplexity, not even an explicit nil
### GetJobTypeLimitations

`func (o *Rule) GetJobTypeLimitations() map[string]int32`

GetJobTypeLimitations returns the JobTypeLimitations field if non-nil, zero value otherwise.

### GetJobTypeLimitationsOk

`func (o *Rule) GetJobTypeLimitationsOk() (*map[string]int32, bool)`

GetJobTypeLimitationsOk returns a tuple with the JobTypeLimitations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJobTypeLimitations

`func (o *Rule) SetJobTypeLimitations(v map[string]int32)`

SetJobTypeLimitations sets JobTypeLimitations field to given value.

### HasJobTypeLimitations

`func (o *Rule) HasJobTypeLimitations() bool`

HasJobTypeLimitations returns a boolean if a field has been set.

### SetJobTypeLimitationsNil

`func (o *Rule) SetJobTypeLimitationsNil(b bool)`

 SetJobTypeLimitationsNil sets the value for JobTypeLimitations to be an explicit nil

### UnsetJobTypeLimitations
`func (o *Rule) UnsetJobTypeLimitations()`

UnsetJobTypeLimitations ensures that no value is present for JobTypeLimitations, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


