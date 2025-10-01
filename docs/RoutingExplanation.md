# RoutingExplanation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Score** | [**NullableRoutingExplanationScore**](RoutingExplanationScore.md) |  | 
**Conflicts** | Pointer to  | Conflicts in the solution | [optional] 
**Unresolved** | Pointer to  | Unresolved constraints in the solution | [optional] 
**Alternatives** | Pointer to **map[string]map[string]interface{}** | When &#x60;options.explanation.enabled&#x60; is set to &#x60;true&#x60;, this field will contain the alternatives for the solution.The key is the job name and the value is the list of assignments. Each assignment contains the resource, the date, and the score. In this way, you can check the impact of the alternative on the score. | [optional] 

## Methods

### NewRoutingExplanation

`func NewRoutingExplanation(score NullableRoutingExplanationScore, ) *RoutingExplanation`

NewRoutingExplanation instantiates a new RoutingExplanation object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRoutingExplanationWithDefaults

`func NewRoutingExplanationWithDefaults() *RoutingExplanation`

NewRoutingExplanationWithDefaults instantiates a new RoutingExplanation object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetScore

`func (o *RoutingExplanation) GetScore() RoutingExplanationScore`

GetScore returns the Score field if non-nil, zero value otherwise.

### GetScoreOk

`func (o *RoutingExplanation) GetScoreOk() (*RoutingExplanationScore, bool)`

GetScoreOk returns a tuple with the Score field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScore

`func (o *RoutingExplanation) SetScore(v RoutingExplanationScore)`

SetScore sets Score field to given value.


### SetScoreNil

`func (o *RoutingExplanation) SetScoreNil(b bool)`

 SetScoreNil sets the value for Score to be an explicit nil

### UnsetScore
`func (o *RoutingExplanation) UnsetScore()`

UnsetScore ensures that no value is present for Score, not even an explicit nil
### GetConflicts

`func (o *RoutingExplanation) GetConflicts() []RoutingConflict`

GetConflicts returns the Conflicts field if non-nil, zero value otherwise.

### GetConflictsOk

`func (o *RoutingExplanation) GetConflictsOk() (*[]RoutingConflict, bool)`

GetConflictsOk returns a tuple with the Conflicts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConflicts

`func (o *RoutingExplanation) SetConflicts(v []RoutingConflict)`

SetConflicts sets Conflicts field to given value.

### HasConflicts

`func (o *RoutingExplanation) HasConflicts() bool`

HasConflicts returns a boolean if a field has been set.

### SetConflictsNil

`func (o *RoutingExplanation) SetConflictsNil(b bool)`

 SetConflictsNil sets the value for Conflicts to be an explicit nil

### UnsetConflicts
`func (o *RoutingExplanation) UnsetConflicts()`

UnsetConflicts ensures that no value is present for Conflicts, not even an explicit nil
### GetUnresolved

`func (o *RoutingExplanation) GetUnresolved() []Unresolved`

GetUnresolved returns the Unresolved field if non-nil, zero value otherwise.

### GetUnresolvedOk

`func (o *RoutingExplanation) GetUnresolvedOk() (*[]Unresolved, bool)`

GetUnresolvedOk returns a tuple with the Unresolved field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnresolved

`func (o *RoutingExplanation) SetUnresolved(v []Unresolved)`

SetUnresolved sets Unresolved field to given value.

### HasUnresolved

`func (o *RoutingExplanation) HasUnresolved() bool`

HasUnresolved returns a boolean if a field has been set.

### SetUnresolvedNil

`func (o *RoutingExplanation) SetUnresolvedNil(b bool)`

 SetUnresolvedNil sets the value for Unresolved to be an explicit nil

### UnsetUnresolved
`func (o *RoutingExplanation) UnsetUnresolved()`

UnsetUnresolved ensures that no value is present for Unresolved, not even an explicit nil
### GetAlternatives

`func (o *RoutingExplanation) GetAlternatives() map[string]map[string]interface{}`

GetAlternatives returns the Alternatives field if non-nil, zero value otherwise.

### GetAlternativesOk

`func (o *RoutingExplanation) GetAlternativesOk() (*map[string]map[string]interface{}, bool)`

GetAlternativesOk returns a tuple with the Alternatives field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAlternatives

`func (o *RoutingExplanation) SetAlternatives(v map[string]map[string]interface{})`

SetAlternatives sets Alternatives field to given value.

### HasAlternatives

`func (o *RoutingExplanation) HasAlternatives() bool`

HasAlternatives returns a boolean if a field has been set.

### SetAlternativesNil

`func (o *RoutingExplanation) SetAlternativesNil(b bool)`

 SetAlternativesNil sets the value for Alternatives to be an explicit nil

### UnsetAlternatives
`func (o *RoutingExplanation) UnsetAlternatives()`

UnsetAlternatives ensures that no value is present for Alternatives, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


