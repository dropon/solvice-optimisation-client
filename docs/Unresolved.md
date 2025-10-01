# Unresolved

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Constraint** | [**OnrouteConstraint**](OnrouteConstraint.md) | Constraint type. | 
**Score** | **string** | Score impact of this conflict. | 

## Methods

### NewUnresolved

`func NewUnresolved(constraint OnrouteConstraint, score string, ) *Unresolved`

NewUnresolved instantiates a new Unresolved object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUnresolvedWithDefaults

`func NewUnresolvedWithDefaults() *Unresolved`

NewUnresolvedWithDefaults instantiates a new Unresolved object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetConstraint

`func (o *Unresolved) GetConstraint() OnrouteConstraint`

GetConstraint returns the Constraint field if non-nil, zero value otherwise.

### GetConstraintOk

`func (o *Unresolved) GetConstraintOk() (*OnrouteConstraint, bool)`

GetConstraintOk returns a tuple with the Constraint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConstraint

`func (o *Unresolved) SetConstraint(v OnrouteConstraint)`

SetConstraint sets Constraint field to given value.


### GetScore

`func (o *Unresolved) GetScore() string`

GetScore returns the Score field if non-nil, zero value otherwise.

### GetScoreOk

`func (o *Unresolved) GetScoreOk() (*string, bool)`

GetScoreOk returns a tuple with the Score field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScore

`func (o *Unresolved) SetScore(v string)`

SetScore sets Score field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


