# SolviceStatusJob

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Job ID | 
**Status** | Pointer to **NullableString** | Status of the solve. | [optional] 
**SolveDuration** | Pointer to **NullableInt32** | Duration of the solve in seconds | [optional] 
**Errors** | Pointer to [**[]Message**](Message.md) | List of errors | [optional] 
**Warnings** | Pointer to [**[]Message**](Message.md) | List of warnings | [optional] 

## Methods

### NewSolviceStatusJob

`func NewSolviceStatusJob(id string, ) *SolviceStatusJob`

NewSolviceStatusJob instantiates a new SolviceStatusJob object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSolviceStatusJobWithDefaults

`func NewSolviceStatusJobWithDefaults() *SolviceStatusJob`

NewSolviceStatusJobWithDefaults instantiates a new SolviceStatusJob object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *SolviceStatusJob) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *SolviceStatusJob) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *SolviceStatusJob) SetId(v string)`

SetId sets Id field to given value.


### GetStatus

`func (o *SolviceStatusJob) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *SolviceStatusJob) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *SolviceStatusJob) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *SolviceStatusJob) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### SetStatusNil

`func (o *SolviceStatusJob) SetStatusNil(b bool)`

 SetStatusNil sets the value for Status to be an explicit nil

### UnsetStatus
`func (o *SolviceStatusJob) UnsetStatus()`

UnsetStatus ensures that no value is present for Status, not even an explicit nil
### GetSolveDuration

`func (o *SolviceStatusJob) GetSolveDuration() int32`

GetSolveDuration returns the SolveDuration field if non-nil, zero value otherwise.

### GetSolveDurationOk

`func (o *SolviceStatusJob) GetSolveDurationOk() (*int32, bool)`

GetSolveDurationOk returns a tuple with the SolveDuration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSolveDuration

`func (o *SolviceStatusJob) SetSolveDuration(v int32)`

SetSolveDuration sets SolveDuration field to given value.

### HasSolveDuration

`func (o *SolviceStatusJob) HasSolveDuration() bool`

HasSolveDuration returns a boolean if a field has been set.

### SetSolveDurationNil

`func (o *SolviceStatusJob) SetSolveDurationNil(b bool)`

 SetSolveDurationNil sets the value for SolveDuration to be an explicit nil

### UnsetSolveDuration
`func (o *SolviceStatusJob) UnsetSolveDuration()`

UnsetSolveDuration ensures that no value is present for SolveDuration, not even an explicit nil
### GetErrors

`func (o *SolviceStatusJob) GetErrors() []Message`

GetErrors returns the Errors field if non-nil, zero value otherwise.

### GetErrorsOk

`func (o *SolviceStatusJob) GetErrorsOk() (*[]Message, bool)`

GetErrorsOk returns a tuple with the Errors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrors

`func (o *SolviceStatusJob) SetErrors(v []Message)`

SetErrors sets Errors field to given value.

### HasErrors

`func (o *SolviceStatusJob) HasErrors() bool`

HasErrors returns a boolean if a field has been set.

### SetErrorsNil

`func (o *SolviceStatusJob) SetErrorsNil(b bool)`

 SetErrorsNil sets the value for Errors to be an explicit nil

### UnsetErrors
`func (o *SolviceStatusJob) UnsetErrors()`

UnsetErrors ensures that no value is present for Errors, not even an explicit nil
### GetWarnings

`func (o *SolviceStatusJob) GetWarnings() []Message`

GetWarnings returns the Warnings field if non-nil, zero value otherwise.

### GetWarningsOk

`func (o *SolviceStatusJob) GetWarningsOk() (*[]Message, bool)`

GetWarningsOk returns a tuple with the Warnings field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWarnings

`func (o *SolviceStatusJob) SetWarnings(v []Message)`

SetWarnings sets Warnings field to given value.

### HasWarnings

`func (o *SolviceStatusJob) HasWarnings() bool`

HasWarnings returns a boolean if a field has been set.

### SetWarningsNil

`func (o *SolviceStatusJob) SetWarningsNil(b bool)`

 SetWarningsNil sets the value for Warnings to be an explicit nil

### UnsetWarnings
`func (o *SolviceStatusJob) UnsetWarnings()`

UnsetWarnings ensures that no value is present for Warnings, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


