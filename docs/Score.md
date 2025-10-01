# Score

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**HardScore** | Pointer to **NullableInt64** | The score of the constraints that are hard. This should be 0 in order to be feasible. | [optional] 
**MediumScore** | Pointer to **NullableInt64** | The score of the constraints that are medium. | [optional] 
**SoftScore** | Pointer to **NullableInt64** | The score of the constraints that are soft. | [optional] 
**Feasible** | Pointer to **NullableBool** |  | [optional] 

## Methods

### NewScore

`func NewScore() *Score`

NewScore instantiates a new Score object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScoreWithDefaults

`func NewScoreWithDefaults() *Score`

NewScoreWithDefaults instantiates a new Score object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetHardScore

`func (o *Score) GetHardScore() int64`

GetHardScore returns the HardScore field if non-nil, zero value otherwise.

### GetHardScoreOk

`func (o *Score) GetHardScoreOk() (*int64, bool)`

GetHardScoreOk returns a tuple with the HardScore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHardScore

`func (o *Score) SetHardScore(v int64)`

SetHardScore sets HardScore field to given value.

### HasHardScore

`func (o *Score) HasHardScore() bool`

HasHardScore returns a boolean if a field has been set.

### SetHardScoreNil

`func (o *Score) SetHardScoreNil(b bool)`

 SetHardScoreNil sets the value for HardScore to be an explicit nil

### UnsetHardScore
`func (o *Score) UnsetHardScore()`

UnsetHardScore ensures that no value is present for HardScore, not even an explicit nil
### GetMediumScore

`func (o *Score) GetMediumScore() int64`

GetMediumScore returns the MediumScore field if non-nil, zero value otherwise.

### GetMediumScoreOk

`func (o *Score) GetMediumScoreOk() (*int64, bool)`

GetMediumScoreOk returns a tuple with the MediumScore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMediumScore

`func (o *Score) SetMediumScore(v int64)`

SetMediumScore sets MediumScore field to given value.

### HasMediumScore

`func (o *Score) HasMediumScore() bool`

HasMediumScore returns a boolean if a field has been set.

### SetMediumScoreNil

`func (o *Score) SetMediumScoreNil(b bool)`

 SetMediumScoreNil sets the value for MediumScore to be an explicit nil

### UnsetMediumScore
`func (o *Score) UnsetMediumScore()`

UnsetMediumScore ensures that no value is present for MediumScore, not even an explicit nil
### GetSoftScore

`func (o *Score) GetSoftScore() int64`

GetSoftScore returns the SoftScore field if non-nil, zero value otherwise.

### GetSoftScoreOk

`func (o *Score) GetSoftScoreOk() (*int64, bool)`

GetSoftScoreOk returns a tuple with the SoftScore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSoftScore

`func (o *Score) SetSoftScore(v int64)`

SetSoftScore sets SoftScore field to given value.

### HasSoftScore

`func (o *Score) HasSoftScore() bool`

HasSoftScore returns a boolean if a field has been set.

### SetSoftScoreNil

`func (o *Score) SetSoftScoreNil(b bool)`

 SetSoftScoreNil sets the value for SoftScore to be an explicit nil

### UnsetSoftScore
`func (o *Score) UnsetSoftScore()`

UnsetSoftScore ensures that no value is present for SoftScore, not even an explicit nil
### GetFeasible

`func (o *Score) GetFeasible() bool`

GetFeasible returns the Feasible field if non-nil, zero value otherwise.

### GetFeasibleOk

`func (o *Score) GetFeasibleOk() (*bool, bool)`

GetFeasibleOk returns a tuple with the Feasible field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFeasible

`func (o *Score) SetFeasible(v bool)`

SetFeasible sets Feasible field to given value.

### HasFeasible

`func (o *Score) HasFeasible() bool`

HasFeasible returns a boolean if a field has been set.

### SetFeasibleNil

`func (o *Score) SetFeasibleNil(b bool)`

 SetFeasibleNil sets the value for Feasible to be an explicit nil

### UnsetFeasible
`func (o *Score) UnsetFeasible()`

UnsetFeasible ensures that no value is present for Feasible, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


