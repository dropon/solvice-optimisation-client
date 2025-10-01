# Weights

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**PriorityWeight** | Pointer to **NullableInt32** | Weight modifier for job priority constraints. Higher values make the solver more likely to include high-priority jobs in the solution when not all jobs can be assigned. This affects job selection probability but not scheduling order. The weight is multiplied by the job&#39;s priority value and duration. | [optional] 
**WorkloadSpreadWeight** | Pointer to **NullableInt32** | Weight modifier for workload balancing across resources and time periods. Higher values make the solver more aggressive about equalizing service time distribution. Works with fairWorkloadPerTrip and fairWorkloadPerResource options, and is sensitive to the workloadSensitivity parameter. | [optional] 
**TravelTimeWeight** | Pointer to **NullableInt32** | Weight modifier for total travel time optimization. This is the baseline weight (typically 1) against which all other weights are compared. Higher values make the solver more aggressive about minimizing travel time, potentially at the expense of other objectives. | [optional] 
**PlannedWeight** | Pointer to **NullableInt32** | Weight modifier for deviations from planned arrivals and resource assignments. Higher values make the solver more reluctant to deviate from plannedArrival times and plannedResource assignments. This is crucial for maintaining customer appointments and commitments. | [optional] 
**AsapWeight** | Pointer to **NullableInt32** | Weight modifier for scheduling jobs as early as possible within their time windows and resource availability. Higher values push jobs toward the beginning of shifts and planning periods, useful for front-loading work or maximizing completion rates. | [optional] 
**MinimizeResourcesWeight** | Pointer to **NullableInt32** | Weight modifier for minimizing the number of active resources per day/trip. The weight is measured in the same units as travel time - a weight of 3600 means using an additional resource is equivalent to 1 hour of travel time. Higher values encourage consolidation of jobs onto fewer resources. | [optional] 
**AllowedResourcesWeight** | Pointer to **NullableInt32** | Weight modifier for soft violations of resource assignment constraints. When jobs have allowedResources restrictions and they cannot be satisfied as hard constraints, this weight determines the penalty for assigning jobs to non-allowed resources. | [optional] 
**WaitTimeWeight** | Pointer to **NullableInt32** | Weight modifier for total waiting time across all resources. Waiting time occurs when resources arrive at jobs before their time windows open or when they have idle time between jobs. Higher values make the solver more aggressive about minimizing idle time. | [optional] 
**UrgencyWeight** | Pointer to **NullableInt32** | Weight modifier for job urgency constraints. Higher values make the solver more aggressive about scheduling urgent jobs earlier in the day and planning period. This affects the sequence and timing of job execution based on their urgency values. | [optional] 
**DriveTimeWeight** | Pointer to **NullableInt32** | Weight modifier for total driving time across all resources. Similar to travelTimeWeight but focuses specifically on driving time violations or constraints. Higher values make the solver more concerned with minimizing driving time, useful for fuel efficiency or driver fatigue management. | [optional] 
**RankingWeight** | Pointer to **NullableInt32** | Weight modifier for resource ranking preferences defined in job rankings. Higher values make the solver more aggressive about assigning jobs to their preferred (lower-ranked) resources, even if it increases travel time or other costs. This helps maintain service quality by using optimal resource assignments. | [optional] 

## Methods

### NewWeights

`func NewWeights() *Weights`

NewWeights instantiates a new Weights object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWeightsWithDefaults

`func NewWeightsWithDefaults() *Weights`

NewWeightsWithDefaults instantiates a new Weights object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPriorityWeight

`func (o *Weights) GetPriorityWeight() int32`

GetPriorityWeight returns the PriorityWeight field if non-nil, zero value otherwise.

### GetPriorityWeightOk

`func (o *Weights) GetPriorityWeightOk() (*int32, bool)`

GetPriorityWeightOk returns a tuple with the PriorityWeight field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriorityWeight

`func (o *Weights) SetPriorityWeight(v int32)`

SetPriorityWeight sets PriorityWeight field to given value.

### HasPriorityWeight

`func (o *Weights) HasPriorityWeight() bool`

HasPriorityWeight returns a boolean if a field has been set.

### SetPriorityWeightNil

`func (o *Weights) SetPriorityWeightNil(b bool)`

 SetPriorityWeightNil sets the value for PriorityWeight to be an explicit nil

### UnsetPriorityWeight
`func (o *Weights) UnsetPriorityWeight()`

UnsetPriorityWeight ensures that no value is present for PriorityWeight, not even an explicit nil
### GetWorkloadSpreadWeight

`func (o *Weights) GetWorkloadSpreadWeight() int32`

GetWorkloadSpreadWeight returns the WorkloadSpreadWeight field if non-nil, zero value otherwise.

### GetWorkloadSpreadWeightOk

`func (o *Weights) GetWorkloadSpreadWeightOk() (*int32, bool)`

GetWorkloadSpreadWeightOk returns a tuple with the WorkloadSpreadWeight field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkloadSpreadWeight

`func (o *Weights) SetWorkloadSpreadWeight(v int32)`

SetWorkloadSpreadWeight sets WorkloadSpreadWeight field to given value.

### HasWorkloadSpreadWeight

`func (o *Weights) HasWorkloadSpreadWeight() bool`

HasWorkloadSpreadWeight returns a boolean if a field has been set.

### SetWorkloadSpreadWeightNil

`func (o *Weights) SetWorkloadSpreadWeightNil(b bool)`

 SetWorkloadSpreadWeightNil sets the value for WorkloadSpreadWeight to be an explicit nil

### UnsetWorkloadSpreadWeight
`func (o *Weights) UnsetWorkloadSpreadWeight()`

UnsetWorkloadSpreadWeight ensures that no value is present for WorkloadSpreadWeight, not even an explicit nil
### GetTravelTimeWeight

`func (o *Weights) GetTravelTimeWeight() int32`

GetTravelTimeWeight returns the TravelTimeWeight field if non-nil, zero value otherwise.

### GetTravelTimeWeightOk

`func (o *Weights) GetTravelTimeWeightOk() (*int32, bool)`

GetTravelTimeWeightOk returns a tuple with the TravelTimeWeight field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTravelTimeWeight

`func (o *Weights) SetTravelTimeWeight(v int32)`

SetTravelTimeWeight sets TravelTimeWeight field to given value.

### HasTravelTimeWeight

`func (o *Weights) HasTravelTimeWeight() bool`

HasTravelTimeWeight returns a boolean if a field has been set.

### SetTravelTimeWeightNil

`func (o *Weights) SetTravelTimeWeightNil(b bool)`

 SetTravelTimeWeightNil sets the value for TravelTimeWeight to be an explicit nil

### UnsetTravelTimeWeight
`func (o *Weights) UnsetTravelTimeWeight()`

UnsetTravelTimeWeight ensures that no value is present for TravelTimeWeight, not even an explicit nil
### GetPlannedWeight

`func (o *Weights) GetPlannedWeight() int32`

GetPlannedWeight returns the PlannedWeight field if non-nil, zero value otherwise.

### GetPlannedWeightOk

`func (o *Weights) GetPlannedWeightOk() (*int32, bool)`

GetPlannedWeightOk returns a tuple with the PlannedWeight field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPlannedWeight

`func (o *Weights) SetPlannedWeight(v int32)`

SetPlannedWeight sets PlannedWeight field to given value.

### HasPlannedWeight

`func (o *Weights) HasPlannedWeight() bool`

HasPlannedWeight returns a boolean if a field has been set.

### SetPlannedWeightNil

`func (o *Weights) SetPlannedWeightNil(b bool)`

 SetPlannedWeightNil sets the value for PlannedWeight to be an explicit nil

### UnsetPlannedWeight
`func (o *Weights) UnsetPlannedWeight()`

UnsetPlannedWeight ensures that no value is present for PlannedWeight, not even an explicit nil
### GetAsapWeight

`func (o *Weights) GetAsapWeight() int32`

GetAsapWeight returns the AsapWeight field if non-nil, zero value otherwise.

### GetAsapWeightOk

`func (o *Weights) GetAsapWeightOk() (*int32, bool)`

GetAsapWeightOk returns a tuple with the AsapWeight field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAsapWeight

`func (o *Weights) SetAsapWeight(v int32)`

SetAsapWeight sets AsapWeight field to given value.

### HasAsapWeight

`func (o *Weights) HasAsapWeight() bool`

HasAsapWeight returns a boolean if a field has been set.

### SetAsapWeightNil

`func (o *Weights) SetAsapWeightNil(b bool)`

 SetAsapWeightNil sets the value for AsapWeight to be an explicit nil

### UnsetAsapWeight
`func (o *Weights) UnsetAsapWeight()`

UnsetAsapWeight ensures that no value is present for AsapWeight, not even an explicit nil
### GetMinimizeResourcesWeight

`func (o *Weights) GetMinimizeResourcesWeight() int32`

GetMinimizeResourcesWeight returns the MinimizeResourcesWeight field if non-nil, zero value otherwise.

### GetMinimizeResourcesWeightOk

`func (o *Weights) GetMinimizeResourcesWeightOk() (*int32, bool)`

GetMinimizeResourcesWeightOk returns a tuple with the MinimizeResourcesWeight field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMinimizeResourcesWeight

`func (o *Weights) SetMinimizeResourcesWeight(v int32)`

SetMinimizeResourcesWeight sets MinimizeResourcesWeight field to given value.

### HasMinimizeResourcesWeight

`func (o *Weights) HasMinimizeResourcesWeight() bool`

HasMinimizeResourcesWeight returns a boolean if a field has been set.

### SetMinimizeResourcesWeightNil

`func (o *Weights) SetMinimizeResourcesWeightNil(b bool)`

 SetMinimizeResourcesWeightNil sets the value for MinimizeResourcesWeight to be an explicit nil

### UnsetMinimizeResourcesWeight
`func (o *Weights) UnsetMinimizeResourcesWeight()`

UnsetMinimizeResourcesWeight ensures that no value is present for MinimizeResourcesWeight, not even an explicit nil
### GetAllowedResourcesWeight

`func (o *Weights) GetAllowedResourcesWeight() int32`

GetAllowedResourcesWeight returns the AllowedResourcesWeight field if non-nil, zero value otherwise.

### GetAllowedResourcesWeightOk

`func (o *Weights) GetAllowedResourcesWeightOk() (*int32, bool)`

GetAllowedResourcesWeightOk returns a tuple with the AllowedResourcesWeight field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAllowedResourcesWeight

`func (o *Weights) SetAllowedResourcesWeight(v int32)`

SetAllowedResourcesWeight sets AllowedResourcesWeight field to given value.

### HasAllowedResourcesWeight

`func (o *Weights) HasAllowedResourcesWeight() bool`

HasAllowedResourcesWeight returns a boolean if a field has been set.

### SetAllowedResourcesWeightNil

`func (o *Weights) SetAllowedResourcesWeightNil(b bool)`

 SetAllowedResourcesWeightNil sets the value for AllowedResourcesWeight to be an explicit nil

### UnsetAllowedResourcesWeight
`func (o *Weights) UnsetAllowedResourcesWeight()`

UnsetAllowedResourcesWeight ensures that no value is present for AllowedResourcesWeight, not even an explicit nil
### GetWaitTimeWeight

`func (o *Weights) GetWaitTimeWeight() int32`

GetWaitTimeWeight returns the WaitTimeWeight field if non-nil, zero value otherwise.

### GetWaitTimeWeightOk

`func (o *Weights) GetWaitTimeWeightOk() (*int32, bool)`

GetWaitTimeWeightOk returns a tuple with the WaitTimeWeight field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWaitTimeWeight

`func (o *Weights) SetWaitTimeWeight(v int32)`

SetWaitTimeWeight sets WaitTimeWeight field to given value.

### HasWaitTimeWeight

`func (o *Weights) HasWaitTimeWeight() bool`

HasWaitTimeWeight returns a boolean if a field has been set.

### SetWaitTimeWeightNil

`func (o *Weights) SetWaitTimeWeightNil(b bool)`

 SetWaitTimeWeightNil sets the value for WaitTimeWeight to be an explicit nil

### UnsetWaitTimeWeight
`func (o *Weights) UnsetWaitTimeWeight()`

UnsetWaitTimeWeight ensures that no value is present for WaitTimeWeight, not even an explicit nil
### GetUrgencyWeight

`func (o *Weights) GetUrgencyWeight() int32`

GetUrgencyWeight returns the UrgencyWeight field if non-nil, zero value otherwise.

### GetUrgencyWeightOk

`func (o *Weights) GetUrgencyWeightOk() (*int32, bool)`

GetUrgencyWeightOk returns a tuple with the UrgencyWeight field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrgencyWeight

`func (o *Weights) SetUrgencyWeight(v int32)`

SetUrgencyWeight sets UrgencyWeight field to given value.

### HasUrgencyWeight

`func (o *Weights) HasUrgencyWeight() bool`

HasUrgencyWeight returns a boolean if a field has been set.

### SetUrgencyWeightNil

`func (o *Weights) SetUrgencyWeightNil(b bool)`

 SetUrgencyWeightNil sets the value for UrgencyWeight to be an explicit nil

### UnsetUrgencyWeight
`func (o *Weights) UnsetUrgencyWeight()`

UnsetUrgencyWeight ensures that no value is present for UrgencyWeight, not even an explicit nil
### GetDriveTimeWeight

`func (o *Weights) GetDriveTimeWeight() int32`

GetDriveTimeWeight returns the DriveTimeWeight field if non-nil, zero value otherwise.

### GetDriveTimeWeightOk

`func (o *Weights) GetDriveTimeWeightOk() (*int32, bool)`

GetDriveTimeWeightOk returns a tuple with the DriveTimeWeight field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDriveTimeWeight

`func (o *Weights) SetDriveTimeWeight(v int32)`

SetDriveTimeWeight sets DriveTimeWeight field to given value.

### HasDriveTimeWeight

`func (o *Weights) HasDriveTimeWeight() bool`

HasDriveTimeWeight returns a boolean if a field has been set.

### SetDriveTimeWeightNil

`func (o *Weights) SetDriveTimeWeightNil(b bool)`

 SetDriveTimeWeightNil sets the value for DriveTimeWeight to be an explicit nil

### UnsetDriveTimeWeight
`func (o *Weights) UnsetDriveTimeWeight()`

UnsetDriveTimeWeight ensures that no value is present for DriveTimeWeight, not even an explicit nil
### GetRankingWeight

`func (o *Weights) GetRankingWeight() int32`

GetRankingWeight returns the RankingWeight field if non-nil, zero value otherwise.

### GetRankingWeightOk

`func (o *Weights) GetRankingWeightOk() (*int32, bool)`

GetRankingWeightOk returns a tuple with the RankingWeight field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRankingWeight

`func (o *Weights) SetRankingWeight(v int32)`

SetRankingWeight sets RankingWeight field to given value.

### HasRankingWeight

`func (o *Weights) HasRankingWeight() bool`

HasRankingWeight returns a boolean if a field has been set.

### SetRankingWeightNil

`func (o *Weights) SetRankingWeightNil(b bool)`

 SetRankingWeightNil sets the value for RankingWeight to be an explicit nil

### UnsetRankingWeight
`func (o *Weights) UnsetRankingWeight()`

UnsetRankingWeight ensures that no value is present for RankingWeight, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


