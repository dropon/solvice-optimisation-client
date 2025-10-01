# JobAssignment

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Job** | **string** | Job | 
**Resource** | **string** | Resource | 
**SuggestedArrival** | Pointer to **NullableString** | Suggested arrival date-time | [optional] 
**LatestArrival** | Pointer to **NullableString** | Latest arrival date-time | [optional] 
**ExecutedAfter** | **string** | Executed after date-time | 
**Score** | Pointer to [**NullableJobAssignmentScore**](JobAssignmentScore.md) |  | [optional] 
**ScoreExplanation** | Pointer to [**NullableJobAssignmentScoreExplanation**](JobAssignmentScoreExplanation.md) |  | [optional] 
**SuggestedInitialArrival** | Pointer to **NullableTime** |  | [optional] 
**Violations** | Pointer to [**[]Unresolved**](Unresolved.md) |  | [optional] 

## Methods

### NewJobAssignment

`func NewJobAssignment(job string, resource string, executedAfter string, ) *JobAssignment`

NewJobAssignment instantiates a new JobAssignment object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewJobAssignmentWithDefaults

`func NewJobAssignmentWithDefaults() *JobAssignment`

NewJobAssignmentWithDefaults instantiates a new JobAssignment object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetJob

`func (o *JobAssignment) GetJob() string`

GetJob returns the Job field if non-nil, zero value otherwise.

### GetJobOk

`func (o *JobAssignment) GetJobOk() (*string, bool)`

GetJobOk returns a tuple with the Job field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJob

`func (o *JobAssignment) SetJob(v string)`

SetJob sets Job field to given value.


### GetResource

`func (o *JobAssignment) GetResource() string`

GetResource returns the Resource field if non-nil, zero value otherwise.

### GetResourceOk

`func (o *JobAssignment) GetResourceOk() (*string, bool)`

GetResourceOk returns a tuple with the Resource field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResource

`func (o *JobAssignment) SetResource(v string)`

SetResource sets Resource field to given value.


### GetSuggestedArrival

`func (o *JobAssignment) GetSuggestedArrival() string`

GetSuggestedArrival returns the SuggestedArrival field if non-nil, zero value otherwise.

### GetSuggestedArrivalOk

`func (o *JobAssignment) GetSuggestedArrivalOk() (*string, bool)`

GetSuggestedArrivalOk returns a tuple with the SuggestedArrival field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuggestedArrival

`func (o *JobAssignment) SetSuggestedArrival(v string)`

SetSuggestedArrival sets SuggestedArrival field to given value.

### HasSuggestedArrival

`func (o *JobAssignment) HasSuggestedArrival() bool`

HasSuggestedArrival returns a boolean if a field has been set.

### SetSuggestedArrivalNil

`func (o *JobAssignment) SetSuggestedArrivalNil(b bool)`

 SetSuggestedArrivalNil sets the value for SuggestedArrival to be an explicit nil

### UnsetSuggestedArrival
`func (o *JobAssignment) UnsetSuggestedArrival()`

UnsetSuggestedArrival ensures that no value is present for SuggestedArrival, not even an explicit nil
### GetLatestArrival

`func (o *JobAssignment) GetLatestArrival() string`

GetLatestArrival returns the LatestArrival field if non-nil, zero value otherwise.

### GetLatestArrivalOk

`func (o *JobAssignment) GetLatestArrivalOk() (*string, bool)`

GetLatestArrivalOk returns a tuple with the LatestArrival field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLatestArrival

`func (o *JobAssignment) SetLatestArrival(v string)`

SetLatestArrival sets LatestArrival field to given value.

### HasLatestArrival

`func (o *JobAssignment) HasLatestArrival() bool`

HasLatestArrival returns a boolean if a field has been set.

### SetLatestArrivalNil

`func (o *JobAssignment) SetLatestArrivalNil(b bool)`

 SetLatestArrivalNil sets the value for LatestArrival to be an explicit nil

### UnsetLatestArrival
`func (o *JobAssignment) UnsetLatestArrival()`

UnsetLatestArrival ensures that no value is present for LatestArrival, not even an explicit nil
### GetExecutedAfter

`func (o *JobAssignment) GetExecutedAfter() string`

GetExecutedAfter returns the ExecutedAfter field if non-nil, zero value otherwise.

### GetExecutedAfterOk

`func (o *JobAssignment) GetExecutedAfterOk() (*string, bool)`

GetExecutedAfterOk returns a tuple with the ExecutedAfter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExecutedAfter

`func (o *JobAssignment) SetExecutedAfter(v string)`

SetExecutedAfter sets ExecutedAfter field to given value.


### GetScore

`func (o *JobAssignment) GetScore() JobAssignmentScore`

GetScore returns the Score field if non-nil, zero value otherwise.

### GetScoreOk

`func (o *JobAssignment) GetScoreOk() (*JobAssignmentScore, bool)`

GetScoreOk returns a tuple with the Score field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScore

`func (o *JobAssignment) SetScore(v JobAssignmentScore)`

SetScore sets Score field to given value.

### HasScore

`func (o *JobAssignment) HasScore() bool`

HasScore returns a boolean if a field has been set.

### SetScoreNil

`func (o *JobAssignment) SetScoreNil(b bool)`

 SetScoreNil sets the value for Score to be an explicit nil

### UnsetScore
`func (o *JobAssignment) UnsetScore()`

UnsetScore ensures that no value is present for Score, not even an explicit nil
### GetScoreExplanation

`func (o *JobAssignment) GetScoreExplanation() JobAssignmentScoreExplanation`

GetScoreExplanation returns the ScoreExplanation field if non-nil, zero value otherwise.

### GetScoreExplanationOk

`func (o *JobAssignment) GetScoreExplanationOk() (*JobAssignmentScoreExplanation, bool)`

GetScoreExplanationOk returns a tuple with the ScoreExplanation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScoreExplanation

`func (o *JobAssignment) SetScoreExplanation(v JobAssignmentScoreExplanation)`

SetScoreExplanation sets ScoreExplanation field to given value.

### HasScoreExplanation

`func (o *JobAssignment) HasScoreExplanation() bool`

HasScoreExplanation returns a boolean if a field has been set.

### SetScoreExplanationNil

`func (o *JobAssignment) SetScoreExplanationNil(b bool)`

 SetScoreExplanationNil sets the value for ScoreExplanation to be an explicit nil

### UnsetScoreExplanation
`func (o *JobAssignment) UnsetScoreExplanation()`

UnsetScoreExplanation ensures that no value is present for ScoreExplanation, not even an explicit nil
### GetSuggestedInitialArrival

`func (o *JobAssignment) GetSuggestedInitialArrival() time.Time`

GetSuggestedInitialArrival returns the SuggestedInitialArrival field if non-nil, zero value otherwise.

### GetSuggestedInitialArrivalOk

`func (o *JobAssignment) GetSuggestedInitialArrivalOk() (*time.Time, bool)`

GetSuggestedInitialArrivalOk returns a tuple with the SuggestedInitialArrival field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuggestedInitialArrival

`func (o *JobAssignment) SetSuggestedInitialArrival(v time.Time)`

SetSuggestedInitialArrival sets SuggestedInitialArrival field to given value.

### HasSuggestedInitialArrival

`func (o *JobAssignment) HasSuggestedInitialArrival() bool`

HasSuggestedInitialArrival returns a boolean if a field has been set.

### SetSuggestedInitialArrivalNil

`func (o *JobAssignment) SetSuggestedInitialArrivalNil(b bool)`

 SetSuggestedInitialArrivalNil sets the value for SuggestedInitialArrival to be an explicit nil

### UnsetSuggestedInitialArrival
`func (o *JobAssignment) UnsetSuggestedInitialArrival()`

UnsetSuggestedInitialArrival ensures that no value is present for SuggestedInitialArrival, not even an explicit nil
### GetViolations

`func (o *JobAssignment) GetViolations() []Unresolved`

GetViolations returns the Violations field if non-nil, zero value otherwise.

### GetViolationsOk

`func (o *JobAssignment) GetViolationsOk() (*[]Unresolved, bool)`

GetViolationsOk returns a tuple with the Violations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetViolations

`func (o *JobAssignment) SetViolations(v []Unresolved)`

SetViolations sets Violations field to given value.

### HasViolations

`func (o *JobAssignment) HasViolations() bool`

HasViolations returns a boolean if a field has been set.

### SetViolationsNil

`func (o *JobAssignment) SetViolationsNil(b bool)`

 SetViolationsNil sets the value for Violations to be an explicit nil

### UnsetViolations
`func (o *JobAssignment) UnsetViolations()`

UnsetViolations ensures that no value is present for Violations, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


