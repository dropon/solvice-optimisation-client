# Relation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | [**RelationType**](RelationType.md) | Type of relationship constraint between jobs. SAME_TRIP: jobs must be on the same vehicle/day. SEQUENCE: jobs must be done in order with optional time intervals. DIRECT_SEQUENCE: jobs must be consecutive with no other jobs between them. NEIGHBOR: jobs must be geographically close. SAME_TIME: jobs must be done simultaneously. PICKUP_AND_DELIVERY: first job is pickup, second is delivery. SAME_RESOURCE: jobs must use the same resource. SAME_DAY: jobs must be on the same day. GROUP_SEQUENCE: jobs with matching tags must be in sequence. | 
**Jobs** | **[]string** | List of job names involved in this relation. For sequence-based relations, the order matters - jobs will be executed in the order specified. For other relations, order may be irrelevant. All job names must exist in the request&#39;s jobs list. | 
**Resource** | Pointer to **NullableString** | Optional resource constraint for this relation. When specified, all jobs in the relation must be assigned to this specific resource. This creates a hard constraint that can help enforce resource-specific workflows or capabilities. | [optional] 
**MinTimeInterval** | Pointer to **NullableInt32** | Minimum time interval in seconds that must pass between consecutive jobs in sequence relations. This ensures adequate time for travel, setup, or processing between related jobs. Only applies to SEQUENCE, DIRECT_SEQUENCE, and SAME_TIME relations. | [optional] 
**MaxTimeInterval** | Pointer to **NullableInt32** | Maximum time interval in seconds allowed between consecutive jobs in sequence relations. This prevents excessive delays between related jobs and ensures timely completion of job sequences. Only applies to SEQUENCE, DIRECT_SEQUENCE, and SAME_TIME relations. | [optional] 
**PartialPlanning** | Pointer to **bool** | Allows the solver to include only some jobs from this relation in the final solution when the full relation cannot be satisfied due to constraints. When false, either all jobs in the relation are assigned or none are, maintaining the relation&#39;s integrity. | [optional] 
**MaxWaitingTime** | Pointer to **NullableInt32** | Maximum waiting time in seconds between jobs in a SAME_TIME relation. This defines how much time synchronization tolerance is allowed - jobs can start within this time window of each other. Defaults to 1200 seconds (20 minutes) if not specified. | [optional] 
**TimeInterval** | [**TimeInterval**](TimeInterval.md) | Reference point for measuring time intervals between jobs in sequence relations. FROM_ARRIVAL (default) measures from when the first job&#39;s service begins to when the second job&#39;s service begins. FROM_DEPARTURE measures from when the first job&#39;s service ends to when the second job&#39;s service begins. | 
**Tags** | Pointer to **[]string** | List of tag names used to define job groups in GROUP_SEQUENCE relations. Jobs with matching tags form groups that must be executed in sequence. This allows for complex sequencing rules based on job characteristics rather than explicit job names. | [optional] 
**EnforceCompatibility** | Pointer to **bool** | When true, enforces resource compatibility checking for SAME_TIME relations. Only compatible resources can work together on linked jobs. | [optional] 
**HardMinWait** | Pointer to **bool** | When true (default), the minimum time interval constraint is enforced as a hard constraint. When false, it becomes a soft constraint that can be violated with penalty. Useful for SEQUENCE and SAME_TIME relations where timing flexibility is acceptable. | [optional] 
**Weight** | Pointer to **NullableInt32** | Weight modifier for this relation. This can be used to modify the weight of a relation to make it more or less important than other relations. | [optional] 

## Methods

### NewRelation

`func NewRelation(type_ RelationType, jobs []string, timeInterval TimeInterval, ) *Relation`

NewRelation instantiates a new Relation object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRelationWithDefaults

`func NewRelationWithDefaults() *Relation`

NewRelationWithDefaults instantiates a new Relation object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *Relation) GetType() RelationType`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *Relation) GetTypeOk() (*RelationType, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *Relation) SetType(v RelationType)`

SetType sets Type field to given value.


### GetJobs

`func (o *Relation) GetJobs() []string`

GetJobs returns the Jobs field if non-nil, zero value otherwise.

### GetJobsOk

`func (o *Relation) GetJobsOk() (*[]string, bool)`

GetJobsOk returns a tuple with the Jobs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJobs

`func (o *Relation) SetJobs(v []string)`

SetJobs sets Jobs field to given value.


### GetResource

`func (o *Relation) GetResource() string`

GetResource returns the Resource field if non-nil, zero value otherwise.

### GetResourceOk

`func (o *Relation) GetResourceOk() (*string, bool)`

GetResourceOk returns a tuple with the Resource field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResource

`func (o *Relation) SetResource(v string)`

SetResource sets Resource field to given value.

### HasResource

`func (o *Relation) HasResource() bool`

HasResource returns a boolean if a field has been set.

### SetResourceNil

`func (o *Relation) SetResourceNil(b bool)`

 SetResourceNil sets the value for Resource to be an explicit nil

### UnsetResource
`func (o *Relation) UnsetResource()`

UnsetResource ensures that no value is present for Resource, not even an explicit nil
### GetMinTimeInterval

`func (o *Relation) GetMinTimeInterval() int32`

GetMinTimeInterval returns the MinTimeInterval field if non-nil, zero value otherwise.

### GetMinTimeIntervalOk

`func (o *Relation) GetMinTimeIntervalOk() (*int32, bool)`

GetMinTimeIntervalOk returns a tuple with the MinTimeInterval field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMinTimeInterval

`func (o *Relation) SetMinTimeInterval(v int32)`

SetMinTimeInterval sets MinTimeInterval field to given value.

### HasMinTimeInterval

`func (o *Relation) HasMinTimeInterval() bool`

HasMinTimeInterval returns a boolean if a field has been set.

### SetMinTimeIntervalNil

`func (o *Relation) SetMinTimeIntervalNil(b bool)`

 SetMinTimeIntervalNil sets the value for MinTimeInterval to be an explicit nil

### UnsetMinTimeInterval
`func (o *Relation) UnsetMinTimeInterval()`

UnsetMinTimeInterval ensures that no value is present for MinTimeInterval, not even an explicit nil
### GetMaxTimeInterval

`func (o *Relation) GetMaxTimeInterval() int32`

GetMaxTimeInterval returns the MaxTimeInterval field if non-nil, zero value otherwise.

### GetMaxTimeIntervalOk

`func (o *Relation) GetMaxTimeIntervalOk() (*int32, bool)`

GetMaxTimeIntervalOk returns a tuple with the MaxTimeInterval field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxTimeInterval

`func (o *Relation) SetMaxTimeInterval(v int32)`

SetMaxTimeInterval sets MaxTimeInterval field to given value.

### HasMaxTimeInterval

`func (o *Relation) HasMaxTimeInterval() bool`

HasMaxTimeInterval returns a boolean if a field has been set.

### SetMaxTimeIntervalNil

`func (o *Relation) SetMaxTimeIntervalNil(b bool)`

 SetMaxTimeIntervalNil sets the value for MaxTimeInterval to be an explicit nil

### UnsetMaxTimeInterval
`func (o *Relation) UnsetMaxTimeInterval()`

UnsetMaxTimeInterval ensures that no value is present for MaxTimeInterval, not even an explicit nil
### GetPartialPlanning

`func (o *Relation) GetPartialPlanning() bool`

GetPartialPlanning returns the PartialPlanning field if non-nil, zero value otherwise.

### GetPartialPlanningOk

`func (o *Relation) GetPartialPlanningOk() (*bool, bool)`

GetPartialPlanningOk returns a tuple with the PartialPlanning field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPartialPlanning

`func (o *Relation) SetPartialPlanning(v bool)`

SetPartialPlanning sets PartialPlanning field to given value.

### HasPartialPlanning

`func (o *Relation) HasPartialPlanning() bool`

HasPartialPlanning returns a boolean if a field has been set.

### GetMaxWaitingTime

`func (o *Relation) GetMaxWaitingTime() int32`

GetMaxWaitingTime returns the MaxWaitingTime field if non-nil, zero value otherwise.

### GetMaxWaitingTimeOk

`func (o *Relation) GetMaxWaitingTimeOk() (*int32, bool)`

GetMaxWaitingTimeOk returns a tuple with the MaxWaitingTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxWaitingTime

`func (o *Relation) SetMaxWaitingTime(v int32)`

SetMaxWaitingTime sets MaxWaitingTime field to given value.

### HasMaxWaitingTime

`func (o *Relation) HasMaxWaitingTime() bool`

HasMaxWaitingTime returns a boolean if a field has been set.

### SetMaxWaitingTimeNil

`func (o *Relation) SetMaxWaitingTimeNil(b bool)`

 SetMaxWaitingTimeNil sets the value for MaxWaitingTime to be an explicit nil

### UnsetMaxWaitingTime
`func (o *Relation) UnsetMaxWaitingTime()`

UnsetMaxWaitingTime ensures that no value is present for MaxWaitingTime, not even an explicit nil
### GetTimeInterval

`func (o *Relation) GetTimeInterval() TimeInterval`

GetTimeInterval returns the TimeInterval field if non-nil, zero value otherwise.

### GetTimeIntervalOk

`func (o *Relation) GetTimeIntervalOk() (*TimeInterval, bool)`

GetTimeIntervalOk returns a tuple with the TimeInterval field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimeInterval

`func (o *Relation) SetTimeInterval(v TimeInterval)`

SetTimeInterval sets TimeInterval field to given value.


### GetTags

`func (o *Relation) GetTags() []string`

GetTags returns the Tags field if non-nil, zero value otherwise.

### GetTagsOk

`func (o *Relation) GetTagsOk() (*[]string, bool)`

GetTagsOk returns a tuple with the Tags field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTags

`func (o *Relation) SetTags(v []string)`

SetTags sets Tags field to given value.

### HasTags

`func (o *Relation) HasTags() bool`

HasTags returns a boolean if a field has been set.

### SetTagsNil

`func (o *Relation) SetTagsNil(b bool)`

 SetTagsNil sets the value for Tags to be an explicit nil

### UnsetTags
`func (o *Relation) UnsetTags()`

UnsetTags ensures that no value is present for Tags, not even an explicit nil
### GetEnforceCompatibility

`func (o *Relation) GetEnforceCompatibility() bool`

GetEnforceCompatibility returns the EnforceCompatibility field if non-nil, zero value otherwise.

### GetEnforceCompatibilityOk

`func (o *Relation) GetEnforceCompatibilityOk() (*bool, bool)`

GetEnforceCompatibilityOk returns a tuple with the EnforceCompatibility field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnforceCompatibility

`func (o *Relation) SetEnforceCompatibility(v bool)`

SetEnforceCompatibility sets EnforceCompatibility field to given value.

### HasEnforceCompatibility

`func (o *Relation) HasEnforceCompatibility() bool`

HasEnforceCompatibility returns a boolean if a field has been set.

### GetHardMinWait

`func (o *Relation) GetHardMinWait() bool`

GetHardMinWait returns the HardMinWait field if non-nil, zero value otherwise.

### GetHardMinWaitOk

`func (o *Relation) GetHardMinWaitOk() (*bool, bool)`

GetHardMinWaitOk returns a tuple with the HardMinWait field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHardMinWait

`func (o *Relation) SetHardMinWait(v bool)`

SetHardMinWait sets HardMinWait field to given value.

### HasHardMinWait

`func (o *Relation) HasHardMinWait() bool`

HasHardMinWait returns a boolean if a field has been set.

### GetWeight

`func (o *Relation) GetWeight() int32`

GetWeight returns the Weight field if non-nil, zero value otherwise.

### GetWeightOk

`func (o *Relation) GetWeightOk() (*int32, bool)`

GetWeightOk returns a tuple with the Weight field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWeight

`func (o *Relation) SetWeight(v int32)`

SetWeight sets Weight field to given value.

### HasWeight

`func (o *Relation) HasWeight() bool`

HasWeight returns a boolean if a field has been set.

### SetWeightNil

`func (o *Relation) SetWeightNil(b bool)`

 SetWeightNil sets the value for Weight to be an explicit nil

### UnsetWeight
`func (o *Relation) UnsetWeight()`

UnsetWeight ensures that no value is present for Weight, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


