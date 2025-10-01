# OnRouteRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Resources** | [**[]Resource**](Resource.md) | List of available resources (vehicles, drivers, workers) that can be assigned to perform jobs. Each resource defines their working schedules, location constraints, capacity limits, and capabilities. At least one resource is required, with a maximum of 2000 resources per request. | 
**Jobs** | [**[]Job**](Job.md) | List of jobs/tasks to be assigned to resources. Each job specifies service requirements, location, time constraints, duration, and resource preferences. Jobs represent the work that needs to be scheduled and optimized. At least one job is required, with a maximum of 10,000 jobs per request. | 
**Options** | Pointer to [**NullableOptions**](Options.md) | Configuration options that control the solver&#39;s behavior, optimization strategy, and output format. These settings affect how the solver approaches the problem, what data is included in responses, and performance characteristics. | [optional] 
**Weights** | Pointer to [**NullableWeights**](Weights.md) | Relative importance weights for different optimization objectives and constraint violations. These weights allow you to balance competing priorities such as travel time vs. resource utilization, or to emphasize certain constraints like customer preferences or service urgency. | [optional] 
**Hook** | Pointer to **NullableString** | Optional webhook URL that will receive a POST request with the job ID when the optimization is complete. This enables asynchronous processing where you can submit a request and be notified when results are ready, rather than waiting for the synchronous response. | [optional] 
**CustomDistanceMatrices** | Pointer to [**NullableCustomDistanceMatrices**](CustomDistanceMatrices.md) | Optional configuration for custom distance matrices supporting multiple vehicle profiles and time slices. When provided, these matrix IDs will be used instead of calculating distances through routing engines. This is useful for scenarios requiring pre-computed distance matrices with specific routing constraints or for improved performance. | [optional] 
**Label** | Pointer to **NullableString** |  | [optional] 
**Relations** | Pointer to [**[]Relation**](Relation.md) |  | [optional] 

## Methods

### NewOnRouteRequest

`func NewOnRouteRequest(resources []Resource, jobs []Job, ) *OnRouteRequest`

NewOnRouteRequest instantiates a new OnRouteRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewOnRouteRequestWithDefaults

`func NewOnRouteRequestWithDefaults() *OnRouteRequest`

NewOnRouteRequestWithDefaults instantiates a new OnRouteRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetResources

`func (o *OnRouteRequest) GetResources() []Resource`

GetResources returns the Resources field if non-nil, zero value otherwise.

### GetResourcesOk

`func (o *OnRouteRequest) GetResourcesOk() (*[]Resource, bool)`

GetResourcesOk returns a tuple with the Resources field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResources

`func (o *OnRouteRequest) SetResources(v []Resource)`

SetResources sets Resources field to given value.


### GetJobs

`func (o *OnRouteRequest) GetJobs() []Job`

GetJobs returns the Jobs field if non-nil, zero value otherwise.

### GetJobsOk

`func (o *OnRouteRequest) GetJobsOk() (*[]Job, bool)`

GetJobsOk returns a tuple with the Jobs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJobs

`func (o *OnRouteRequest) SetJobs(v []Job)`

SetJobs sets Jobs field to given value.


### GetOptions

`func (o *OnRouteRequest) GetOptions() Options`

GetOptions returns the Options field if non-nil, zero value otherwise.

### GetOptionsOk

`func (o *OnRouteRequest) GetOptionsOk() (*Options, bool)`

GetOptionsOk returns a tuple with the Options field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOptions

`func (o *OnRouteRequest) SetOptions(v Options)`

SetOptions sets Options field to given value.

### HasOptions

`func (o *OnRouteRequest) HasOptions() bool`

HasOptions returns a boolean if a field has been set.

### SetOptionsNil

`func (o *OnRouteRequest) SetOptionsNil(b bool)`

 SetOptionsNil sets the value for Options to be an explicit nil

### UnsetOptions
`func (o *OnRouteRequest) UnsetOptions()`

UnsetOptions ensures that no value is present for Options, not even an explicit nil
### GetWeights

`func (o *OnRouteRequest) GetWeights() Weights`

GetWeights returns the Weights field if non-nil, zero value otherwise.

### GetWeightsOk

`func (o *OnRouteRequest) GetWeightsOk() (*Weights, bool)`

GetWeightsOk returns a tuple with the Weights field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWeights

`func (o *OnRouteRequest) SetWeights(v Weights)`

SetWeights sets Weights field to given value.

### HasWeights

`func (o *OnRouteRequest) HasWeights() bool`

HasWeights returns a boolean if a field has been set.

### SetWeightsNil

`func (o *OnRouteRequest) SetWeightsNil(b bool)`

 SetWeightsNil sets the value for Weights to be an explicit nil

### UnsetWeights
`func (o *OnRouteRequest) UnsetWeights()`

UnsetWeights ensures that no value is present for Weights, not even an explicit nil
### GetHook

`func (o *OnRouteRequest) GetHook() string`

GetHook returns the Hook field if non-nil, zero value otherwise.

### GetHookOk

`func (o *OnRouteRequest) GetHookOk() (*string, bool)`

GetHookOk returns a tuple with the Hook field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHook

`func (o *OnRouteRequest) SetHook(v string)`

SetHook sets Hook field to given value.

### HasHook

`func (o *OnRouteRequest) HasHook() bool`

HasHook returns a boolean if a field has been set.

### SetHookNil

`func (o *OnRouteRequest) SetHookNil(b bool)`

 SetHookNil sets the value for Hook to be an explicit nil

### UnsetHook
`func (o *OnRouteRequest) UnsetHook()`

UnsetHook ensures that no value is present for Hook, not even an explicit nil
### GetCustomDistanceMatrices

`func (o *OnRouteRequest) GetCustomDistanceMatrices() CustomDistanceMatrices`

GetCustomDistanceMatrices returns the CustomDistanceMatrices field if non-nil, zero value otherwise.

### GetCustomDistanceMatricesOk

`func (o *OnRouteRequest) GetCustomDistanceMatricesOk() (*CustomDistanceMatrices, bool)`

GetCustomDistanceMatricesOk returns a tuple with the CustomDistanceMatrices field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomDistanceMatrices

`func (o *OnRouteRequest) SetCustomDistanceMatrices(v CustomDistanceMatrices)`

SetCustomDistanceMatrices sets CustomDistanceMatrices field to given value.

### HasCustomDistanceMatrices

`func (o *OnRouteRequest) HasCustomDistanceMatrices() bool`

HasCustomDistanceMatrices returns a boolean if a field has been set.

### SetCustomDistanceMatricesNil

`func (o *OnRouteRequest) SetCustomDistanceMatricesNil(b bool)`

 SetCustomDistanceMatricesNil sets the value for CustomDistanceMatrices to be an explicit nil

### UnsetCustomDistanceMatrices
`func (o *OnRouteRequest) UnsetCustomDistanceMatrices()`

UnsetCustomDistanceMatrices ensures that no value is present for CustomDistanceMatrices, not even an explicit nil
### GetLabel

`func (o *OnRouteRequest) GetLabel() string`

GetLabel returns the Label field if non-nil, zero value otherwise.

### GetLabelOk

`func (o *OnRouteRequest) GetLabelOk() (*string, bool)`

GetLabelOk returns a tuple with the Label field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabel

`func (o *OnRouteRequest) SetLabel(v string)`

SetLabel sets Label field to given value.

### HasLabel

`func (o *OnRouteRequest) HasLabel() bool`

HasLabel returns a boolean if a field has been set.

### SetLabelNil

`func (o *OnRouteRequest) SetLabelNil(b bool)`

 SetLabelNil sets the value for Label to be an explicit nil

### UnsetLabel
`func (o *OnRouteRequest) UnsetLabel()`

UnsetLabel ensures that no value is present for Label, not even an explicit nil
### GetRelations

`func (o *OnRouteRequest) GetRelations() []Relation`

GetRelations returns the Relations field if non-nil, zero value otherwise.

### GetRelationsOk

`func (o *OnRouteRequest) GetRelationsOk() (*[]Relation, bool)`

GetRelationsOk returns a tuple with the Relations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRelations

`func (o *OnRouteRequest) SetRelations(v []Relation)`

SetRelations sets Relations field to given value.

### HasRelations

`func (o *OnRouteRequest) HasRelations() bool`

HasRelations returns a boolean if a field has been set.

### SetRelationsNil

`func (o *OnRouteRequest) SetRelationsNil(b bool)`

 SetRelationsNil sets the value for Relations to be an explicit nil

### UnsetRelations
`func (o *OnRouteRequest) UnsetRelations()`

UnsetRelations ensures that no value is present for Relations, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


