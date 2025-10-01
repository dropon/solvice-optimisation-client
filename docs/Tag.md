# Tag

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** | Tag name that defines a skill, capability, or requirement. This creates a matching constraint between jobs and resources - only resources with this tag can be assigned to jobs that require it. Common examples include &#39;plumbing&#39;, &#39;electrical&#39;, &#39;certified-technician&#39;, or &#39;heavy-lifting&#39;. | 
**Hard** | Pointer to **NullableBool** | Constraint type for this tag requirement. When true (default), creates a hard constraint - jobs can only be assigned to resources with matching tags. When false, creates a soft constraint - jobs prefer resources with matching tags but can be assigned to others if needed, with a score penalty. | [optional] [default to true]
**Weight** | Pointer to **NullableInt32** | Penalty weight applied when this tag constraint is violated (soft constraints only). The weight is measured in the same units as travel time - a weight of 3600 means violating this tag constraint is equivalent to 1 hour of additional travel time. Higher weights make the constraint more important. | [optional] 

## Methods

### NewTag

`func NewTag(name string, ) *Tag`

NewTag instantiates a new Tag object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTagWithDefaults

`func NewTagWithDefaults() *Tag`

NewTagWithDefaults instantiates a new Tag object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *Tag) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Tag) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Tag) SetName(v string)`

SetName sets Name field to given value.


### GetHard

`func (o *Tag) GetHard() bool`

GetHard returns the Hard field if non-nil, zero value otherwise.

### GetHardOk

`func (o *Tag) GetHardOk() (*bool, bool)`

GetHardOk returns a tuple with the Hard field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHard

`func (o *Tag) SetHard(v bool)`

SetHard sets Hard field to given value.

### HasHard

`func (o *Tag) HasHard() bool`

HasHard returns a boolean if a field has been set.

### SetHardNil

`func (o *Tag) SetHardNil(b bool)`

 SetHardNil sets the value for Hard to be an explicit nil

### UnsetHard
`func (o *Tag) UnsetHard()`

UnsetHard ensures that no value is present for Hard, not even an explicit nil
### GetWeight

`func (o *Tag) GetWeight() int32`

GetWeight returns the Weight field if non-nil, zero value otherwise.

### GetWeightOk

`func (o *Tag) GetWeightOk() (*int32, bool)`

GetWeightOk returns a tuple with the Weight field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWeight

`func (o *Tag) SetWeight(v int32)`

SetWeight sets Weight field to given value.

### HasWeight

`func (o *Tag) HasWeight() bool`

HasWeight returns a boolean if a field has been set.

### SetWeightNil

`func (o *Tag) SetWeightNil(b bool)`

 SetWeightNil sets the value for Weight to be an explicit nil

### UnsetWeight
`func (o *Tag) UnsetWeight()`

UnsetWeight ensures that no value is present for Weight, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


