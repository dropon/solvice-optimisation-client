# JobAssignmentScoreExplanation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Constraint** | [**OnrouteConstraint**](OnrouteConstraint.md) | Constraint type. | 
**Score** | **string** | Score impact of this conflict. | 

## Methods

### NewJobAssignmentScoreExplanation

`func NewJobAssignmentScoreExplanation(constraint OnrouteConstraint, score string, ) *JobAssignmentScoreExplanation`

NewJobAssignmentScoreExplanation instantiates a new JobAssignmentScoreExplanation object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewJobAssignmentScoreExplanationWithDefaults

`func NewJobAssignmentScoreExplanationWithDefaults() *JobAssignmentScoreExplanation`

NewJobAssignmentScoreExplanationWithDefaults instantiates a new JobAssignmentScoreExplanation object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetConstraint

`func (o *JobAssignmentScoreExplanation) GetConstraint() OnrouteConstraint`

GetConstraint returns the Constraint field if non-nil, zero value otherwise.

### GetConstraintOk

`func (o *JobAssignmentScoreExplanation) GetConstraintOk() (*OnrouteConstraint, bool)`

GetConstraintOk returns a tuple with the Constraint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConstraint

`func (o *JobAssignmentScoreExplanation) SetConstraint(v OnrouteConstraint)`

SetConstraint sets Constraint field to given value.


### GetScore

`func (o *JobAssignmentScoreExplanation) GetScore() string`

GetScore returns the Score field if non-nil, zero value otherwise.

### GetScoreOk

`func (o *JobAssignmentScoreExplanation) GetScoreOk() (*string, bool)`

GetScoreOk returns a tuple with the Score field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScore

`func (o *JobAssignmentScoreExplanation) SetScore(v string)`

SetScore sets Score field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


