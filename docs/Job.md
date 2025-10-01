# Job

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** | Unique description | 
**Duration** | Pointer to **NullableInt32** | Service duration of the job | [optional] 
**Location** | Pointer to [**NullableLocation**](Location.md) | Job location | [optional] 
**Priority** | Pointer to **NullableInt32** | Priority level that influences job selection during optimization. Higher priority jobs are more likely to be included in the final solution when not all jobs can be assigned due to resource or time constraints. The priority is multiplied by job duration to calculate the selection weight. Particularly important when partialPlanning is enabled. Default value is 1. | [optional] 
**Urgency** | Pointer to **NullableInt32** | Urgency level that influences the scheduling order of jobs. Higher urgency jobs are preferentially scheduled earlier in the day and earlier in the planning period, helping ensure time-critical tasks are completed first. This affects the sequence of job execution rather than job selection. | [optional] 
**Tags** | Pointer to [**[]Tag**](Tag.md) | List of skill or capability tags that define resource requirements for this job. Tags create hard or soft constraints linking jobs to resources with matching capabilities. For example, a &#39;plumbing&#39; tag ensures only resources with plumbing skills can be assigned to plumbing jobs. | [optional] 
**Rankings** | Pointer to [**[]Ranking**](Ranking.md) | List of resource preference rankings for this job. Each ranking specifies a resource name and a preference score (1-100), where lower values indicate stronger preference. This allows jobs to have preferred resources while still allowing assignment to other resources if needed, with the preference reflected in the optimization score. | [optional] 
**Windows** | Pointer to [**[]DateWindow**](DateWindow.md) | List of time windows during which this job can be started or executed. Each window defines a start and end time, creating temporal constraints for job scheduling. Multiple windows allow for flexible scheduling across different time periods. Jobs can only be assigned within these time boundaries. | [optional] 
**DurationSquash** | Pointer to **NullableInt32** | Reduced service duration when this job is performed at the same location immediately after another job. This optimization recognizes that setup time, travel within a building, or equipment preparation may be shared between consecutive jobs at the same location. For example, if duration&#x3D;600 and durationSquash&#x3D;30, the second job at the same location takes only 30 seconds instead of 600. | [optional] 
**PlannedDate** | Pointer to **NullableString** | Fixed date assignment for this job that must be respected during optimization. When specified, the job can only be scheduled on this specific date, creating a hard constraint that the solver must honor. Useful for jobs that are already committed to customers or have date-specific requirements. | [optional] 
**PlannedResource** | Pointer to **NullableString** | Fixed resource assignment for this job that must be respected during optimization. When specified, only the named resource can be assigned to this job, creating a hard constraint. Combined with plannedArrival, this allows for pre-committed assignments that the solver must work around when optimizing other jobs. | [optional] 
**PlannedArrival** | Pointer to **NullableString** | Fixed arrival time for this job that creates a soft constraint during optimization. The solver will try to schedule the job as close as possible to this time, with deviations penalized in the score according to the plannedWeight. This allows for customer appointment times or preferred scheduling while maintaining optimization flexibility. | [optional] 
**Hard** | Pointer to **NullableBool** | In the case of partialPlanning planning, this indicates whether this order should be integrated into the planning or not. | [optional] 
**HardWeight** | Pointer to **NullableInt32** | In the case of partialPlanning planning, this indicates the weight of this order. | [optional] 
**Padding** | Pointer to **NullableInt32** | Padding time before and after the job. In seconds | [optional] 
**Load** | Pointer to **[]int32** | Load | [optional] 
**AllowedResources** | Pointer to **[]string** | List of vehicle names that are allowed to be assigned to this order. | [optional] 
**InitialResource** | Pointer to **NullableString** | Warm start for the assigned resource: name of the vehicle to which this job is planned. Use this to speed up the solver and to start from an initial solution. | [optional] 
**InitialArrival** | Pointer to **NullableString** | Warm start for the arrival time. Use this to speed up the solver and to start from an initial solution. | [optional] 
**DisallowedResources** | Pointer to **[]string** | List of vehicle names that are allowed to be assigned to this order. | [optional] 
**Complexity** | Pointer to **NullableInt32** | Complexity of the job | [optional] 
**Resumable** | Pointer to **NullableBool** | Enables job interruption by resource unavailability breaks. When true, the job can start before a break, pause during the break, and resume afterward. Default: false. | [optional] 
**JobTypes** | Pointer to **[]string** | List of job types that this job represents. Used to enforce job type limitations per resource per timeframe. | [optional] 

## Methods

### NewJob

`func NewJob(name string, ) *Job`

NewJob instantiates a new Job object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewJobWithDefaults

`func NewJobWithDefaults() *Job`

NewJobWithDefaults instantiates a new Job object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *Job) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Job) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Job) SetName(v string)`

SetName sets Name field to given value.


### GetDuration

`func (o *Job) GetDuration() int32`

GetDuration returns the Duration field if non-nil, zero value otherwise.

### GetDurationOk

`func (o *Job) GetDurationOk() (*int32, bool)`

GetDurationOk returns a tuple with the Duration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDuration

`func (o *Job) SetDuration(v int32)`

SetDuration sets Duration field to given value.

### HasDuration

`func (o *Job) HasDuration() bool`

HasDuration returns a boolean if a field has been set.

### SetDurationNil

`func (o *Job) SetDurationNil(b bool)`

 SetDurationNil sets the value for Duration to be an explicit nil

### UnsetDuration
`func (o *Job) UnsetDuration()`

UnsetDuration ensures that no value is present for Duration, not even an explicit nil
### GetLocation

`func (o *Job) GetLocation() Location`

GetLocation returns the Location field if non-nil, zero value otherwise.

### GetLocationOk

`func (o *Job) GetLocationOk() (*Location, bool)`

GetLocationOk returns a tuple with the Location field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLocation

`func (o *Job) SetLocation(v Location)`

SetLocation sets Location field to given value.

### HasLocation

`func (o *Job) HasLocation() bool`

HasLocation returns a boolean if a field has been set.

### SetLocationNil

`func (o *Job) SetLocationNil(b bool)`

 SetLocationNil sets the value for Location to be an explicit nil

### UnsetLocation
`func (o *Job) UnsetLocation()`

UnsetLocation ensures that no value is present for Location, not even an explicit nil
### GetPriority

`func (o *Job) GetPriority() int32`

GetPriority returns the Priority field if non-nil, zero value otherwise.

### GetPriorityOk

`func (o *Job) GetPriorityOk() (*int32, bool)`

GetPriorityOk returns a tuple with the Priority field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriority

`func (o *Job) SetPriority(v int32)`

SetPriority sets Priority field to given value.

### HasPriority

`func (o *Job) HasPriority() bool`

HasPriority returns a boolean if a field has been set.

### SetPriorityNil

`func (o *Job) SetPriorityNil(b bool)`

 SetPriorityNil sets the value for Priority to be an explicit nil

### UnsetPriority
`func (o *Job) UnsetPriority()`

UnsetPriority ensures that no value is present for Priority, not even an explicit nil
### GetUrgency

`func (o *Job) GetUrgency() int32`

GetUrgency returns the Urgency field if non-nil, zero value otherwise.

### GetUrgencyOk

`func (o *Job) GetUrgencyOk() (*int32, bool)`

GetUrgencyOk returns a tuple with the Urgency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrgency

`func (o *Job) SetUrgency(v int32)`

SetUrgency sets Urgency field to given value.

### HasUrgency

`func (o *Job) HasUrgency() bool`

HasUrgency returns a boolean if a field has been set.

### SetUrgencyNil

`func (o *Job) SetUrgencyNil(b bool)`

 SetUrgencyNil sets the value for Urgency to be an explicit nil

### UnsetUrgency
`func (o *Job) UnsetUrgency()`

UnsetUrgency ensures that no value is present for Urgency, not even an explicit nil
### GetTags

`func (o *Job) GetTags() []Tag`

GetTags returns the Tags field if non-nil, zero value otherwise.

### GetTagsOk

`func (o *Job) GetTagsOk() (*[]Tag, bool)`

GetTagsOk returns a tuple with the Tags field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTags

`func (o *Job) SetTags(v []Tag)`

SetTags sets Tags field to given value.

### HasTags

`func (o *Job) HasTags() bool`

HasTags returns a boolean if a field has been set.

### SetTagsNil

`func (o *Job) SetTagsNil(b bool)`

 SetTagsNil sets the value for Tags to be an explicit nil

### UnsetTags
`func (o *Job) UnsetTags()`

UnsetTags ensures that no value is present for Tags, not even an explicit nil
### GetRankings

`func (o *Job) GetRankings() []Ranking`

GetRankings returns the Rankings field if non-nil, zero value otherwise.

### GetRankingsOk

`func (o *Job) GetRankingsOk() (*[]Ranking, bool)`

GetRankingsOk returns a tuple with the Rankings field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRankings

`func (o *Job) SetRankings(v []Ranking)`

SetRankings sets Rankings field to given value.

### HasRankings

`func (o *Job) HasRankings() bool`

HasRankings returns a boolean if a field has been set.

### SetRankingsNil

`func (o *Job) SetRankingsNil(b bool)`

 SetRankingsNil sets the value for Rankings to be an explicit nil

### UnsetRankings
`func (o *Job) UnsetRankings()`

UnsetRankings ensures that no value is present for Rankings, not even an explicit nil
### GetWindows

`func (o *Job) GetWindows() []DateWindow`

GetWindows returns the Windows field if non-nil, zero value otherwise.

### GetWindowsOk

`func (o *Job) GetWindowsOk() (*[]DateWindow, bool)`

GetWindowsOk returns a tuple with the Windows field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWindows

`func (o *Job) SetWindows(v []DateWindow)`

SetWindows sets Windows field to given value.

### HasWindows

`func (o *Job) HasWindows() bool`

HasWindows returns a boolean if a field has been set.

### SetWindowsNil

`func (o *Job) SetWindowsNil(b bool)`

 SetWindowsNil sets the value for Windows to be an explicit nil

### UnsetWindows
`func (o *Job) UnsetWindows()`

UnsetWindows ensures that no value is present for Windows, not even an explicit nil
### GetDurationSquash

`func (o *Job) GetDurationSquash() int32`

GetDurationSquash returns the DurationSquash field if non-nil, zero value otherwise.

### GetDurationSquashOk

`func (o *Job) GetDurationSquashOk() (*int32, bool)`

GetDurationSquashOk returns a tuple with the DurationSquash field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDurationSquash

`func (o *Job) SetDurationSquash(v int32)`

SetDurationSquash sets DurationSquash field to given value.

### HasDurationSquash

`func (o *Job) HasDurationSquash() bool`

HasDurationSquash returns a boolean if a field has been set.

### SetDurationSquashNil

`func (o *Job) SetDurationSquashNil(b bool)`

 SetDurationSquashNil sets the value for DurationSquash to be an explicit nil

### UnsetDurationSquash
`func (o *Job) UnsetDurationSquash()`

UnsetDurationSquash ensures that no value is present for DurationSquash, not even an explicit nil
### GetPlannedDate

`func (o *Job) GetPlannedDate() string`

GetPlannedDate returns the PlannedDate field if non-nil, zero value otherwise.

### GetPlannedDateOk

`func (o *Job) GetPlannedDateOk() (*string, bool)`

GetPlannedDateOk returns a tuple with the PlannedDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPlannedDate

`func (o *Job) SetPlannedDate(v string)`

SetPlannedDate sets PlannedDate field to given value.

### HasPlannedDate

`func (o *Job) HasPlannedDate() bool`

HasPlannedDate returns a boolean if a field has been set.

### SetPlannedDateNil

`func (o *Job) SetPlannedDateNil(b bool)`

 SetPlannedDateNil sets the value for PlannedDate to be an explicit nil

### UnsetPlannedDate
`func (o *Job) UnsetPlannedDate()`

UnsetPlannedDate ensures that no value is present for PlannedDate, not even an explicit nil
### GetPlannedResource

`func (o *Job) GetPlannedResource() string`

GetPlannedResource returns the PlannedResource field if non-nil, zero value otherwise.

### GetPlannedResourceOk

`func (o *Job) GetPlannedResourceOk() (*string, bool)`

GetPlannedResourceOk returns a tuple with the PlannedResource field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPlannedResource

`func (o *Job) SetPlannedResource(v string)`

SetPlannedResource sets PlannedResource field to given value.

### HasPlannedResource

`func (o *Job) HasPlannedResource() bool`

HasPlannedResource returns a boolean if a field has been set.

### SetPlannedResourceNil

`func (o *Job) SetPlannedResourceNil(b bool)`

 SetPlannedResourceNil sets the value for PlannedResource to be an explicit nil

### UnsetPlannedResource
`func (o *Job) UnsetPlannedResource()`

UnsetPlannedResource ensures that no value is present for PlannedResource, not even an explicit nil
### GetPlannedArrival

`func (o *Job) GetPlannedArrival() string`

GetPlannedArrival returns the PlannedArrival field if non-nil, zero value otherwise.

### GetPlannedArrivalOk

`func (o *Job) GetPlannedArrivalOk() (*string, bool)`

GetPlannedArrivalOk returns a tuple with the PlannedArrival field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPlannedArrival

`func (o *Job) SetPlannedArrival(v string)`

SetPlannedArrival sets PlannedArrival field to given value.

### HasPlannedArrival

`func (o *Job) HasPlannedArrival() bool`

HasPlannedArrival returns a boolean if a field has been set.

### SetPlannedArrivalNil

`func (o *Job) SetPlannedArrivalNil(b bool)`

 SetPlannedArrivalNil sets the value for PlannedArrival to be an explicit nil

### UnsetPlannedArrival
`func (o *Job) UnsetPlannedArrival()`

UnsetPlannedArrival ensures that no value is present for PlannedArrival, not even an explicit nil
### GetHard

`func (o *Job) GetHard() bool`

GetHard returns the Hard field if non-nil, zero value otherwise.

### GetHardOk

`func (o *Job) GetHardOk() (*bool, bool)`

GetHardOk returns a tuple with the Hard field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHard

`func (o *Job) SetHard(v bool)`

SetHard sets Hard field to given value.

### HasHard

`func (o *Job) HasHard() bool`

HasHard returns a boolean if a field has been set.

### SetHardNil

`func (o *Job) SetHardNil(b bool)`

 SetHardNil sets the value for Hard to be an explicit nil

### UnsetHard
`func (o *Job) UnsetHard()`

UnsetHard ensures that no value is present for Hard, not even an explicit nil
### GetHardWeight

`func (o *Job) GetHardWeight() int32`

GetHardWeight returns the HardWeight field if non-nil, zero value otherwise.

### GetHardWeightOk

`func (o *Job) GetHardWeightOk() (*int32, bool)`

GetHardWeightOk returns a tuple with the HardWeight field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHardWeight

`func (o *Job) SetHardWeight(v int32)`

SetHardWeight sets HardWeight field to given value.

### HasHardWeight

`func (o *Job) HasHardWeight() bool`

HasHardWeight returns a boolean if a field has been set.

### SetHardWeightNil

`func (o *Job) SetHardWeightNil(b bool)`

 SetHardWeightNil sets the value for HardWeight to be an explicit nil

### UnsetHardWeight
`func (o *Job) UnsetHardWeight()`

UnsetHardWeight ensures that no value is present for HardWeight, not even an explicit nil
### GetPadding

`func (o *Job) GetPadding() int32`

GetPadding returns the Padding field if non-nil, zero value otherwise.

### GetPaddingOk

`func (o *Job) GetPaddingOk() (*int32, bool)`

GetPaddingOk returns a tuple with the Padding field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPadding

`func (o *Job) SetPadding(v int32)`

SetPadding sets Padding field to given value.

### HasPadding

`func (o *Job) HasPadding() bool`

HasPadding returns a boolean if a field has been set.

### SetPaddingNil

`func (o *Job) SetPaddingNil(b bool)`

 SetPaddingNil sets the value for Padding to be an explicit nil

### UnsetPadding
`func (o *Job) UnsetPadding()`

UnsetPadding ensures that no value is present for Padding, not even an explicit nil
### GetLoad

`func (o *Job) GetLoad() []int32`

GetLoad returns the Load field if non-nil, zero value otherwise.

### GetLoadOk

`func (o *Job) GetLoadOk() (*[]int32, bool)`

GetLoadOk returns a tuple with the Load field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLoad

`func (o *Job) SetLoad(v []int32)`

SetLoad sets Load field to given value.

### HasLoad

`func (o *Job) HasLoad() bool`

HasLoad returns a boolean if a field has been set.

### SetLoadNil

`func (o *Job) SetLoadNil(b bool)`

 SetLoadNil sets the value for Load to be an explicit nil

### UnsetLoad
`func (o *Job) UnsetLoad()`

UnsetLoad ensures that no value is present for Load, not even an explicit nil
### GetAllowedResources

`func (o *Job) GetAllowedResources() []string`

GetAllowedResources returns the AllowedResources field if non-nil, zero value otherwise.

### GetAllowedResourcesOk

`func (o *Job) GetAllowedResourcesOk() (*[]string, bool)`

GetAllowedResourcesOk returns a tuple with the AllowedResources field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAllowedResources

`func (o *Job) SetAllowedResources(v []string)`

SetAllowedResources sets AllowedResources field to given value.

### HasAllowedResources

`func (o *Job) HasAllowedResources() bool`

HasAllowedResources returns a boolean if a field has been set.

### SetAllowedResourcesNil

`func (o *Job) SetAllowedResourcesNil(b bool)`

 SetAllowedResourcesNil sets the value for AllowedResources to be an explicit nil

### UnsetAllowedResources
`func (o *Job) UnsetAllowedResources()`

UnsetAllowedResources ensures that no value is present for AllowedResources, not even an explicit nil
### GetInitialResource

`func (o *Job) GetInitialResource() string`

GetInitialResource returns the InitialResource field if non-nil, zero value otherwise.

### GetInitialResourceOk

`func (o *Job) GetInitialResourceOk() (*string, bool)`

GetInitialResourceOk returns a tuple with the InitialResource field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInitialResource

`func (o *Job) SetInitialResource(v string)`

SetInitialResource sets InitialResource field to given value.

### HasInitialResource

`func (o *Job) HasInitialResource() bool`

HasInitialResource returns a boolean if a field has been set.

### SetInitialResourceNil

`func (o *Job) SetInitialResourceNil(b bool)`

 SetInitialResourceNil sets the value for InitialResource to be an explicit nil

### UnsetInitialResource
`func (o *Job) UnsetInitialResource()`

UnsetInitialResource ensures that no value is present for InitialResource, not even an explicit nil
### GetInitialArrival

`func (o *Job) GetInitialArrival() string`

GetInitialArrival returns the InitialArrival field if non-nil, zero value otherwise.

### GetInitialArrivalOk

`func (o *Job) GetInitialArrivalOk() (*string, bool)`

GetInitialArrivalOk returns a tuple with the InitialArrival field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInitialArrival

`func (o *Job) SetInitialArrival(v string)`

SetInitialArrival sets InitialArrival field to given value.

### HasInitialArrival

`func (o *Job) HasInitialArrival() bool`

HasInitialArrival returns a boolean if a field has been set.

### SetInitialArrivalNil

`func (o *Job) SetInitialArrivalNil(b bool)`

 SetInitialArrivalNil sets the value for InitialArrival to be an explicit nil

### UnsetInitialArrival
`func (o *Job) UnsetInitialArrival()`

UnsetInitialArrival ensures that no value is present for InitialArrival, not even an explicit nil
### GetDisallowedResources

`func (o *Job) GetDisallowedResources() []string`

GetDisallowedResources returns the DisallowedResources field if non-nil, zero value otherwise.

### GetDisallowedResourcesOk

`func (o *Job) GetDisallowedResourcesOk() (*[]string, bool)`

GetDisallowedResourcesOk returns a tuple with the DisallowedResources field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisallowedResources

`func (o *Job) SetDisallowedResources(v []string)`

SetDisallowedResources sets DisallowedResources field to given value.

### HasDisallowedResources

`func (o *Job) HasDisallowedResources() bool`

HasDisallowedResources returns a boolean if a field has been set.

### SetDisallowedResourcesNil

`func (o *Job) SetDisallowedResourcesNil(b bool)`

 SetDisallowedResourcesNil sets the value for DisallowedResources to be an explicit nil

### UnsetDisallowedResources
`func (o *Job) UnsetDisallowedResources()`

UnsetDisallowedResources ensures that no value is present for DisallowedResources, not even an explicit nil
### GetComplexity

`func (o *Job) GetComplexity() int32`

GetComplexity returns the Complexity field if non-nil, zero value otherwise.

### GetComplexityOk

`func (o *Job) GetComplexityOk() (*int32, bool)`

GetComplexityOk returns a tuple with the Complexity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetComplexity

`func (o *Job) SetComplexity(v int32)`

SetComplexity sets Complexity field to given value.

### HasComplexity

`func (o *Job) HasComplexity() bool`

HasComplexity returns a boolean if a field has been set.

### SetComplexityNil

`func (o *Job) SetComplexityNil(b bool)`

 SetComplexityNil sets the value for Complexity to be an explicit nil

### UnsetComplexity
`func (o *Job) UnsetComplexity()`

UnsetComplexity ensures that no value is present for Complexity, not even an explicit nil
### GetResumable

`func (o *Job) GetResumable() bool`

GetResumable returns the Resumable field if non-nil, zero value otherwise.

### GetResumableOk

`func (o *Job) GetResumableOk() (*bool, bool)`

GetResumableOk returns a tuple with the Resumable field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResumable

`func (o *Job) SetResumable(v bool)`

SetResumable sets Resumable field to given value.

### HasResumable

`func (o *Job) HasResumable() bool`

HasResumable returns a boolean if a field has been set.

### SetResumableNil

`func (o *Job) SetResumableNil(b bool)`

 SetResumableNil sets the value for Resumable to be an explicit nil

### UnsetResumable
`func (o *Job) UnsetResumable()`

UnsetResumable ensures that no value is present for Resumable, not even an explicit nil
### GetJobTypes

`func (o *Job) GetJobTypes() []string`

GetJobTypes returns the JobTypes field if non-nil, zero value otherwise.

### GetJobTypesOk

`func (o *Job) GetJobTypesOk() (*[]string, bool)`

GetJobTypesOk returns a tuple with the JobTypes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJobTypes

`func (o *Job) SetJobTypes(v []string)`

SetJobTypes sets JobTypes field to given value.

### HasJobTypes

`func (o *Job) HasJobTypes() bool`

HasJobTypes returns a boolean if a field has been set.

### SetJobTypesNil

`func (o *Job) SetJobTypesNil(b bool)`

 SetJobTypesNil sets the value for JobTypes to be an explicit nil

### UnsetJobTypes
`func (o *Job) UnsetJobTypes()`

UnsetJobTypes ensures that no value is present for JobTypes, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


