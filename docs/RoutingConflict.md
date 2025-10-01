# RoutingConflict

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Constraint** | **string** | Constraint type. | 
**Score** | **string** | Score impact of this conflict. | 
**Job** | Pointer to **NullableString** | Job id. | [optional] 
**Resource** | Pointer to **NullableString** | Resource id. | [optional] 
**Tag** | Pointer to **NullableString** | Tag id. | [optional] 
**Relation** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewRoutingConflict

`func NewRoutingConflict(constraint string, score string, ) *RoutingConflict`

NewRoutingConflict instantiates a new RoutingConflict object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRoutingConflictWithDefaults

`func NewRoutingConflictWithDefaults() *RoutingConflict`

NewRoutingConflictWithDefaults instantiates a new RoutingConflict object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetConstraint

`func (o *RoutingConflict) GetConstraint() string`

GetConstraint returns the Constraint field if non-nil, zero value otherwise.

### GetConstraintOk

`func (o *RoutingConflict) GetConstraintOk() (*string, bool)`

GetConstraintOk returns a tuple with the Constraint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConstraint

`func (o *RoutingConflict) SetConstraint(v string)`

SetConstraint sets Constraint field to given value.


### GetScore

`func (o *RoutingConflict) GetScore() string`

GetScore returns the Score field if non-nil, zero value otherwise.

### GetScoreOk

`func (o *RoutingConflict) GetScoreOk() (*string, bool)`

GetScoreOk returns a tuple with the Score field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScore

`func (o *RoutingConflict) SetScore(v string)`

SetScore sets Score field to given value.


### GetJob

`func (o *RoutingConflict) GetJob() string`

GetJob returns the Job field if non-nil, zero value otherwise.

### GetJobOk

`func (o *RoutingConflict) GetJobOk() (*string, bool)`

GetJobOk returns a tuple with the Job field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJob

`func (o *RoutingConflict) SetJob(v string)`

SetJob sets Job field to given value.

### HasJob

`func (o *RoutingConflict) HasJob() bool`

HasJob returns a boolean if a field has been set.

### SetJobNil

`func (o *RoutingConflict) SetJobNil(b bool)`

 SetJobNil sets the value for Job to be an explicit nil

### UnsetJob
`func (o *RoutingConflict) UnsetJob()`

UnsetJob ensures that no value is present for Job, not even an explicit nil
### GetResource

`func (o *RoutingConflict) GetResource() string`

GetResource returns the Resource field if non-nil, zero value otherwise.

### GetResourceOk

`func (o *RoutingConflict) GetResourceOk() (*string, bool)`

GetResourceOk returns a tuple with the Resource field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResource

`func (o *RoutingConflict) SetResource(v string)`

SetResource sets Resource field to given value.

### HasResource

`func (o *RoutingConflict) HasResource() bool`

HasResource returns a boolean if a field has been set.

### SetResourceNil

`func (o *RoutingConflict) SetResourceNil(b bool)`

 SetResourceNil sets the value for Resource to be an explicit nil

### UnsetResource
`func (o *RoutingConflict) UnsetResource()`

UnsetResource ensures that no value is present for Resource, not even an explicit nil
### GetTag

`func (o *RoutingConflict) GetTag() string`

GetTag returns the Tag field if non-nil, zero value otherwise.

### GetTagOk

`func (o *RoutingConflict) GetTagOk() (*string, bool)`

GetTagOk returns a tuple with the Tag field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTag

`func (o *RoutingConflict) SetTag(v string)`

SetTag sets Tag field to given value.

### HasTag

`func (o *RoutingConflict) HasTag() bool`

HasTag returns a boolean if a field has been set.

### SetTagNil

`func (o *RoutingConflict) SetTagNil(b bool)`

 SetTagNil sets the value for Tag to be an explicit nil

### UnsetTag
`func (o *RoutingConflict) UnsetTag()`

UnsetTag ensures that no value is present for Tag, not even an explicit nil
### GetRelation

`func (o *RoutingConflict) GetRelation() string`

GetRelation returns the Relation field if non-nil, zero value otherwise.

### GetRelationOk

`func (o *RoutingConflict) GetRelationOk() (*string, bool)`

GetRelationOk returns a tuple with the Relation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRelation

`func (o *RoutingConflict) SetRelation(v string)`

SetRelation sets Relation field to given value.

### HasRelation

`func (o *RoutingConflict) HasRelation() bool`

HasRelation returns a boolean if a field has been set.

### SetRelationNil

`func (o *RoutingConflict) SetRelationNil(b bool)`

 SetRelationNil sets the value for Relation to be an explicit nil

### UnsetRelation
`func (o *RoutingConflict) UnsetRelation()`

UnsetRelation ensures that no value is present for Relation, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


