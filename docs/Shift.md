# Shift

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**From** | **string** | Start of the shift datetime  | 
**To** | **string** | End of the shift datetime | 
**Start** | Pointer to [**NullableLocation**](Location.md) | Start location | [optional] 
**End** | Pointer to [**NullableLocation**](Location.md) | End location | [optional] 
**IgnoreTravelTimeToFirstJob** | Pointer to **NullableBool** | Ignore the travel time from the start location to the first order | [optional] 
**IgnoreTravelTimeFromLastJob** | Pointer to **NullableBool** | Ignore the travel time from the last order to the optional end location | [optional] 
**Overtime** | Pointer to **interface{}** | Can go into overtime. | [optional] 
**OvertimeEnd** | Pointer to **NullableString** | Maximum overtime time. | [optional] 
**Breaks** | Pointer to [**[]BreakDto1**](BreakDto1.md) | Windowed breaks definitions. | [optional] 
**Tags** | Pointer to **[]string** | Shift tags will ensure that this resource can only do Jobs of this tag during this shift. This allows for tag based availability. | [optional] 
**JobTypeLimitations** | Pointer to **map[string]int32** | Map of job type to maximum count allowed per shift. Null means no limitations. | [optional] 

## Methods

### NewShift

`func NewShift(from string, to string, ) *Shift`

NewShift instantiates a new Shift object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewShiftWithDefaults

`func NewShiftWithDefaults() *Shift`

NewShiftWithDefaults instantiates a new Shift object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFrom

`func (o *Shift) GetFrom() string`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *Shift) GetFromOk() (*string, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *Shift) SetFrom(v string)`

SetFrom sets From field to given value.


### GetTo

`func (o *Shift) GetTo() string`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *Shift) GetToOk() (*string, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *Shift) SetTo(v string)`

SetTo sets To field to given value.


### GetStart

`func (o *Shift) GetStart() Location`

GetStart returns the Start field if non-nil, zero value otherwise.

### GetStartOk

`func (o *Shift) GetStartOk() (*Location, bool)`

GetStartOk returns a tuple with the Start field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStart

`func (o *Shift) SetStart(v Location)`

SetStart sets Start field to given value.

### HasStart

`func (o *Shift) HasStart() bool`

HasStart returns a boolean if a field has been set.

### SetStartNil

`func (o *Shift) SetStartNil(b bool)`

 SetStartNil sets the value for Start to be an explicit nil

### UnsetStart
`func (o *Shift) UnsetStart()`

UnsetStart ensures that no value is present for Start, not even an explicit nil
### GetEnd

`func (o *Shift) GetEnd() Location`

GetEnd returns the End field if non-nil, zero value otherwise.

### GetEndOk

`func (o *Shift) GetEndOk() (*Location, bool)`

GetEndOk returns a tuple with the End field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnd

`func (o *Shift) SetEnd(v Location)`

SetEnd sets End field to given value.

### HasEnd

`func (o *Shift) HasEnd() bool`

HasEnd returns a boolean if a field has been set.

### SetEndNil

`func (o *Shift) SetEndNil(b bool)`

 SetEndNil sets the value for End to be an explicit nil

### UnsetEnd
`func (o *Shift) UnsetEnd()`

UnsetEnd ensures that no value is present for End, not even an explicit nil
### GetIgnoreTravelTimeToFirstJob

`func (o *Shift) GetIgnoreTravelTimeToFirstJob() bool`

GetIgnoreTravelTimeToFirstJob returns the IgnoreTravelTimeToFirstJob field if non-nil, zero value otherwise.

### GetIgnoreTravelTimeToFirstJobOk

`func (o *Shift) GetIgnoreTravelTimeToFirstJobOk() (*bool, bool)`

GetIgnoreTravelTimeToFirstJobOk returns a tuple with the IgnoreTravelTimeToFirstJob field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIgnoreTravelTimeToFirstJob

`func (o *Shift) SetIgnoreTravelTimeToFirstJob(v bool)`

SetIgnoreTravelTimeToFirstJob sets IgnoreTravelTimeToFirstJob field to given value.

### HasIgnoreTravelTimeToFirstJob

`func (o *Shift) HasIgnoreTravelTimeToFirstJob() bool`

HasIgnoreTravelTimeToFirstJob returns a boolean if a field has been set.

### SetIgnoreTravelTimeToFirstJobNil

`func (o *Shift) SetIgnoreTravelTimeToFirstJobNil(b bool)`

 SetIgnoreTravelTimeToFirstJobNil sets the value for IgnoreTravelTimeToFirstJob to be an explicit nil

### UnsetIgnoreTravelTimeToFirstJob
`func (o *Shift) UnsetIgnoreTravelTimeToFirstJob()`

UnsetIgnoreTravelTimeToFirstJob ensures that no value is present for IgnoreTravelTimeToFirstJob, not even an explicit nil
### GetIgnoreTravelTimeFromLastJob

`func (o *Shift) GetIgnoreTravelTimeFromLastJob() bool`

GetIgnoreTravelTimeFromLastJob returns the IgnoreTravelTimeFromLastJob field if non-nil, zero value otherwise.

### GetIgnoreTravelTimeFromLastJobOk

`func (o *Shift) GetIgnoreTravelTimeFromLastJobOk() (*bool, bool)`

GetIgnoreTravelTimeFromLastJobOk returns a tuple with the IgnoreTravelTimeFromLastJob field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIgnoreTravelTimeFromLastJob

`func (o *Shift) SetIgnoreTravelTimeFromLastJob(v bool)`

SetIgnoreTravelTimeFromLastJob sets IgnoreTravelTimeFromLastJob field to given value.

### HasIgnoreTravelTimeFromLastJob

`func (o *Shift) HasIgnoreTravelTimeFromLastJob() bool`

HasIgnoreTravelTimeFromLastJob returns a boolean if a field has been set.

### SetIgnoreTravelTimeFromLastJobNil

`func (o *Shift) SetIgnoreTravelTimeFromLastJobNil(b bool)`

 SetIgnoreTravelTimeFromLastJobNil sets the value for IgnoreTravelTimeFromLastJob to be an explicit nil

### UnsetIgnoreTravelTimeFromLastJob
`func (o *Shift) UnsetIgnoreTravelTimeFromLastJob()`

UnsetIgnoreTravelTimeFromLastJob ensures that no value is present for IgnoreTravelTimeFromLastJob, not even an explicit nil
### GetOvertime

`func (o *Shift) GetOvertime() interface{}`

GetOvertime returns the Overtime field if non-nil, zero value otherwise.

### GetOvertimeOk

`func (o *Shift) GetOvertimeOk() (*interface{}, bool)`

GetOvertimeOk returns a tuple with the Overtime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOvertime

`func (o *Shift) SetOvertime(v interface{})`

SetOvertime sets Overtime field to given value.

### HasOvertime

`func (o *Shift) HasOvertime() bool`

HasOvertime returns a boolean if a field has been set.

### SetOvertimeNil

`func (o *Shift) SetOvertimeNil(b bool)`

 SetOvertimeNil sets the value for Overtime to be an explicit nil

### UnsetOvertime
`func (o *Shift) UnsetOvertime()`

UnsetOvertime ensures that no value is present for Overtime, not even an explicit nil
### GetOvertimeEnd

`func (o *Shift) GetOvertimeEnd() string`

GetOvertimeEnd returns the OvertimeEnd field if non-nil, zero value otherwise.

### GetOvertimeEndOk

`func (o *Shift) GetOvertimeEndOk() (*string, bool)`

GetOvertimeEndOk returns a tuple with the OvertimeEnd field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOvertimeEnd

`func (o *Shift) SetOvertimeEnd(v string)`

SetOvertimeEnd sets OvertimeEnd field to given value.

### HasOvertimeEnd

`func (o *Shift) HasOvertimeEnd() bool`

HasOvertimeEnd returns a boolean if a field has been set.

### SetOvertimeEndNil

`func (o *Shift) SetOvertimeEndNil(b bool)`

 SetOvertimeEndNil sets the value for OvertimeEnd to be an explicit nil

### UnsetOvertimeEnd
`func (o *Shift) UnsetOvertimeEnd()`

UnsetOvertimeEnd ensures that no value is present for OvertimeEnd, not even an explicit nil
### GetBreaks

`func (o *Shift) GetBreaks() []BreakDto1`

GetBreaks returns the Breaks field if non-nil, zero value otherwise.

### GetBreaksOk

`func (o *Shift) GetBreaksOk() (*[]BreakDto1, bool)`

GetBreaksOk returns a tuple with the Breaks field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBreaks

`func (o *Shift) SetBreaks(v []BreakDto1)`

SetBreaks sets Breaks field to given value.

### HasBreaks

`func (o *Shift) HasBreaks() bool`

HasBreaks returns a boolean if a field has been set.

### SetBreaksNil

`func (o *Shift) SetBreaksNil(b bool)`

 SetBreaksNil sets the value for Breaks to be an explicit nil

### UnsetBreaks
`func (o *Shift) UnsetBreaks()`

UnsetBreaks ensures that no value is present for Breaks, not even an explicit nil
### GetTags

`func (o *Shift) GetTags() []string`

GetTags returns the Tags field if non-nil, zero value otherwise.

### GetTagsOk

`func (o *Shift) GetTagsOk() (*[]string, bool)`

GetTagsOk returns a tuple with the Tags field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTags

`func (o *Shift) SetTags(v []string)`

SetTags sets Tags field to given value.

### HasTags

`func (o *Shift) HasTags() bool`

HasTags returns a boolean if a field has been set.

### SetTagsNil

`func (o *Shift) SetTagsNil(b bool)`

 SetTagsNil sets the value for Tags to be an explicit nil

### UnsetTags
`func (o *Shift) UnsetTags()`

UnsetTags ensures that no value is present for Tags, not even an explicit nil
### GetJobTypeLimitations

`func (o *Shift) GetJobTypeLimitations() map[string]int32`

GetJobTypeLimitations returns the JobTypeLimitations field if non-nil, zero value otherwise.

### GetJobTypeLimitationsOk

`func (o *Shift) GetJobTypeLimitationsOk() (*map[string]int32, bool)`

GetJobTypeLimitationsOk returns a tuple with the JobTypeLimitations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJobTypeLimitations

`func (o *Shift) SetJobTypeLimitations(v map[string]int32)`

SetJobTypeLimitations sets JobTypeLimitations field to given value.

### HasJobTypeLimitations

`func (o *Shift) HasJobTypeLimitations() bool`

HasJobTypeLimitations returns a boolean if a field has been set.

### SetJobTypeLimitationsNil

`func (o *Shift) SetJobTypeLimitationsNil(b bool)`

 SetJobTypeLimitationsNil sets the value for JobTypeLimitations to be an explicit nil

### UnsetJobTypeLimitations
`func (o *Shift) UnsetJobTypeLimitations()`

UnsetJobTypeLimitations ensures that no value is present for JobTypeLimitations, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


