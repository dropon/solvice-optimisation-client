# Resource

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** | Unique identifier for this resource. Used to reference the resource in job assignments, relations, and results. Must be unique within the request. | 
**Shifts** | [**[]Shift**](Shift.md) | List of work shifts defining when this resource is available for job assignments. Each shift specifies working hours, start/end locations, breaks, and other constraints. Multiple shifts allow for multi-day planning or split-shift schedules. At least one shift is required. | 
**Start** | Pointer to [**NullableLocation**](Location.md) | Default start location for all shifts of this resource. This field is deprecated in favor of specifying start locations individually for each shift in the shifts array, which provides more flexibility for multi-day planning. | [optional] 
**End** | Pointer to [**NullableLocation**](Location.md) | Default end location for all shifts of this resource. This field is deprecated in favor of specifying end locations individually for each shift in the shifts array, which provides more flexibility for multi-day planning. | [optional] 
**MaxDriveTimeInSeconds** | Pointer to **interface{}** | Maximum total driving time allowed for this resource per shift or planning period. This constraint prevents excessive driving and ensures compliance with regulations or operational policies. Measured in seconds and includes all travel between jobs but excludes service time. | [optional] 
**Region** | Pointer to [**NullableLocation**](Location.md) | Preferred geographic region for this resource&#39;s job assignments. The solver will try to assign jobs that are geographically closer to this location, minimizing travel distance and time. This creates a soft constraint that influences job assignment without being mandatory. | [optional] 
**Tags** | Pointer to **[]string** | List of capability tags that define what types of jobs this resource can perform. Tags create matching constraints between jobs and resources - only resources with matching tags can be assigned to jobs that require those capabilities. For example, &#39;plumbing&#39; or &#39;electrical&#39; tags. | [optional] 
**Category** | Pointer to [**NullableCategory**](Category.md) | Transportation mode used by this resource, affecting routing calculations and capabilities. CAR provides standard vehicle routing, BIKE uses bicycle-friendly routes and speeds, TRUCK uses heavy vehicle routing with appropriate restrictions. This is a beta feature. | [optional] 
**Rules** | Pointer to [**[]Rule**](Rule.md) | List of periodic constraints that apply to this resource over specified time periods. Rules can enforce minimum/maximum work time, service time, drive time, or job complexity limits. These constraints ensure compliance with labor regulations, operational policies, or capacity limitations. | [optional] 
**Capacity** | Pointer to **[]int32** | Multi-dimensional capacity limits for this resource, such as weight, volume, or item count. Each dimension corresponds to job load requirements. For example, [500, 200] might represent 500 kg weight capacity and 200 cubic meters volume capacity. Maximum 5 dimensions supported. | [optional] 
**HourlyCost** | Pointer to **NullableInt32** | Hourly cost rate for this resource in your currency units. Used to calculate total labor costs for solutions. Only counts active time (driving, servicing, or waiting), not idle time. This enables cost-based optimization and financial analysis of routing solutions. | [optional] 
**CompatibleResources** | Pointer to **[]string** | List of resource names that this resource is compatible to work with on linked jobs requiring cooperation | [optional] 
**MaxDriveTime** | Pointer to **NullableInt32** |  | [optional] 
**MaxDriveTimeJob** | Pointer to **NullableInt32** |  | [optional] 

## Methods

### NewResource

`func NewResource(name string, shifts []Shift, ) *Resource`

NewResource instantiates a new Resource object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewResourceWithDefaults

`func NewResourceWithDefaults() *Resource`

NewResourceWithDefaults instantiates a new Resource object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *Resource) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Resource) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Resource) SetName(v string)`

SetName sets Name field to given value.


### GetShifts

`func (o *Resource) GetShifts() []Shift`

GetShifts returns the Shifts field if non-nil, zero value otherwise.

### GetShiftsOk

`func (o *Resource) GetShiftsOk() (*[]Shift, bool)`

GetShiftsOk returns a tuple with the Shifts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShifts

`func (o *Resource) SetShifts(v []Shift)`

SetShifts sets Shifts field to given value.


### SetShiftsNil

`func (o *Resource) SetShiftsNil(b bool)`

 SetShiftsNil sets the value for Shifts to be an explicit nil

### UnsetShifts
`func (o *Resource) UnsetShifts()`

UnsetShifts ensures that no value is present for Shifts, not even an explicit nil
### GetStart

`func (o *Resource) GetStart() Location`

GetStart returns the Start field if non-nil, zero value otherwise.

### GetStartOk

`func (o *Resource) GetStartOk() (*Location, bool)`

GetStartOk returns a tuple with the Start field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStart

`func (o *Resource) SetStart(v Location)`

SetStart sets Start field to given value.

### HasStart

`func (o *Resource) HasStart() bool`

HasStart returns a boolean if a field has been set.

### SetStartNil

`func (o *Resource) SetStartNil(b bool)`

 SetStartNil sets the value for Start to be an explicit nil

### UnsetStart
`func (o *Resource) UnsetStart()`

UnsetStart ensures that no value is present for Start, not even an explicit nil
### GetEnd

`func (o *Resource) GetEnd() Location`

GetEnd returns the End field if non-nil, zero value otherwise.

### GetEndOk

`func (o *Resource) GetEndOk() (*Location, bool)`

GetEndOk returns a tuple with the End field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnd

`func (o *Resource) SetEnd(v Location)`

SetEnd sets End field to given value.

### HasEnd

`func (o *Resource) HasEnd() bool`

HasEnd returns a boolean if a field has been set.

### SetEndNil

`func (o *Resource) SetEndNil(b bool)`

 SetEndNil sets the value for End to be an explicit nil

### UnsetEnd
`func (o *Resource) UnsetEnd()`

UnsetEnd ensures that no value is present for End, not even an explicit nil
### GetMaxDriveTimeInSeconds

`func (o *Resource) GetMaxDriveTimeInSeconds() interface{}`

GetMaxDriveTimeInSeconds returns the MaxDriveTimeInSeconds field if non-nil, zero value otherwise.

### GetMaxDriveTimeInSecondsOk

`func (o *Resource) GetMaxDriveTimeInSecondsOk() (*interface{}, bool)`

GetMaxDriveTimeInSecondsOk returns a tuple with the MaxDriveTimeInSeconds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxDriveTimeInSeconds

`func (o *Resource) SetMaxDriveTimeInSeconds(v interface{})`

SetMaxDriveTimeInSeconds sets MaxDriveTimeInSeconds field to given value.

### HasMaxDriveTimeInSeconds

`func (o *Resource) HasMaxDriveTimeInSeconds() bool`

HasMaxDriveTimeInSeconds returns a boolean if a field has been set.

### SetMaxDriveTimeInSecondsNil

`func (o *Resource) SetMaxDriveTimeInSecondsNil(b bool)`

 SetMaxDriveTimeInSecondsNil sets the value for MaxDriveTimeInSeconds to be an explicit nil

### UnsetMaxDriveTimeInSeconds
`func (o *Resource) UnsetMaxDriveTimeInSeconds()`

UnsetMaxDriveTimeInSeconds ensures that no value is present for MaxDriveTimeInSeconds, not even an explicit nil
### GetRegion

`func (o *Resource) GetRegion() Location`

GetRegion returns the Region field if non-nil, zero value otherwise.

### GetRegionOk

`func (o *Resource) GetRegionOk() (*Location, bool)`

GetRegionOk returns a tuple with the Region field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegion

`func (o *Resource) SetRegion(v Location)`

SetRegion sets Region field to given value.

### HasRegion

`func (o *Resource) HasRegion() bool`

HasRegion returns a boolean if a field has been set.

### SetRegionNil

`func (o *Resource) SetRegionNil(b bool)`

 SetRegionNil sets the value for Region to be an explicit nil

### UnsetRegion
`func (o *Resource) UnsetRegion()`

UnsetRegion ensures that no value is present for Region, not even an explicit nil
### GetTags

`func (o *Resource) GetTags() []string`

GetTags returns the Tags field if non-nil, zero value otherwise.

### GetTagsOk

`func (o *Resource) GetTagsOk() (*[]string, bool)`

GetTagsOk returns a tuple with the Tags field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTags

`func (o *Resource) SetTags(v []string)`

SetTags sets Tags field to given value.

### HasTags

`func (o *Resource) HasTags() bool`

HasTags returns a boolean if a field has been set.

### SetTagsNil

`func (o *Resource) SetTagsNil(b bool)`

 SetTagsNil sets the value for Tags to be an explicit nil

### UnsetTags
`func (o *Resource) UnsetTags()`

UnsetTags ensures that no value is present for Tags, not even an explicit nil
### GetCategory

`func (o *Resource) GetCategory() Category`

GetCategory returns the Category field if non-nil, zero value otherwise.

### GetCategoryOk

`func (o *Resource) GetCategoryOk() (*Category, bool)`

GetCategoryOk returns a tuple with the Category field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCategory

`func (o *Resource) SetCategory(v Category)`

SetCategory sets Category field to given value.

### HasCategory

`func (o *Resource) HasCategory() bool`

HasCategory returns a boolean if a field has been set.

### SetCategoryNil

`func (o *Resource) SetCategoryNil(b bool)`

 SetCategoryNil sets the value for Category to be an explicit nil

### UnsetCategory
`func (o *Resource) UnsetCategory()`

UnsetCategory ensures that no value is present for Category, not even an explicit nil
### GetRules

`func (o *Resource) GetRules() []Rule`

GetRules returns the Rules field if non-nil, zero value otherwise.

### GetRulesOk

`func (o *Resource) GetRulesOk() (*[]Rule, bool)`

GetRulesOk returns a tuple with the Rules field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRules

`func (o *Resource) SetRules(v []Rule)`

SetRules sets Rules field to given value.

### HasRules

`func (o *Resource) HasRules() bool`

HasRules returns a boolean if a field has been set.

### SetRulesNil

`func (o *Resource) SetRulesNil(b bool)`

 SetRulesNil sets the value for Rules to be an explicit nil

### UnsetRules
`func (o *Resource) UnsetRules()`

UnsetRules ensures that no value is present for Rules, not even an explicit nil
### GetCapacity

`func (o *Resource) GetCapacity() []int32`

GetCapacity returns the Capacity field if non-nil, zero value otherwise.

### GetCapacityOk

`func (o *Resource) GetCapacityOk() (*[]int32, bool)`

GetCapacityOk returns a tuple with the Capacity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCapacity

`func (o *Resource) SetCapacity(v []int32)`

SetCapacity sets Capacity field to given value.

### HasCapacity

`func (o *Resource) HasCapacity() bool`

HasCapacity returns a boolean if a field has been set.

### SetCapacityNil

`func (o *Resource) SetCapacityNil(b bool)`

 SetCapacityNil sets the value for Capacity to be an explicit nil

### UnsetCapacity
`func (o *Resource) UnsetCapacity()`

UnsetCapacity ensures that no value is present for Capacity, not even an explicit nil
### GetHourlyCost

`func (o *Resource) GetHourlyCost() int32`

GetHourlyCost returns the HourlyCost field if non-nil, zero value otherwise.

### GetHourlyCostOk

`func (o *Resource) GetHourlyCostOk() (*int32, bool)`

GetHourlyCostOk returns a tuple with the HourlyCost field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHourlyCost

`func (o *Resource) SetHourlyCost(v int32)`

SetHourlyCost sets HourlyCost field to given value.

### HasHourlyCost

`func (o *Resource) HasHourlyCost() bool`

HasHourlyCost returns a boolean if a field has been set.

### SetHourlyCostNil

`func (o *Resource) SetHourlyCostNil(b bool)`

 SetHourlyCostNil sets the value for HourlyCost to be an explicit nil

### UnsetHourlyCost
`func (o *Resource) UnsetHourlyCost()`

UnsetHourlyCost ensures that no value is present for HourlyCost, not even an explicit nil
### GetCompatibleResources

`func (o *Resource) GetCompatibleResources() []string`

GetCompatibleResources returns the CompatibleResources field if non-nil, zero value otherwise.

### GetCompatibleResourcesOk

`func (o *Resource) GetCompatibleResourcesOk() (*[]string, bool)`

GetCompatibleResourcesOk returns a tuple with the CompatibleResources field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCompatibleResources

`func (o *Resource) SetCompatibleResources(v []string)`

SetCompatibleResources sets CompatibleResources field to given value.

### HasCompatibleResources

`func (o *Resource) HasCompatibleResources() bool`

HasCompatibleResources returns a boolean if a field has been set.

### SetCompatibleResourcesNil

`func (o *Resource) SetCompatibleResourcesNil(b bool)`

 SetCompatibleResourcesNil sets the value for CompatibleResources to be an explicit nil

### UnsetCompatibleResources
`func (o *Resource) UnsetCompatibleResources()`

UnsetCompatibleResources ensures that no value is present for CompatibleResources, not even an explicit nil
### GetMaxDriveTime

`func (o *Resource) GetMaxDriveTime() int32`

GetMaxDriveTime returns the MaxDriveTime field if non-nil, zero value otherwise.

### GetMaxDriveTimeOk

`func (o *Resource) GetMaxDriveTimeOk() (*int32, bool)`

GetMaxDriveTimeOk returns a tuple with the MaxDriveTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxDriveTime

`func (o *Resource) SetMaxDriveTime(v int32)`

SetMaxDriveTime sets MaxDriveTime field to given value.

### HasMaxDriveTime

`func (o *Resource) HasMaxDriveTime() bool`

HasMaxDriveTime returns a boolean if a field has been set.

### SetMaxDriveTimeNil

`func (o *Resource) SetMaxDriveTimeNil(b bool)`

 SetMaxDriveTimeNil sets the value for MaxDriveTime to be an explicit nil

### UnsetMaxDriveTime
`func (o *Resource) UnsetMaxDriveTime()`

UnsetMaxDriveTime ensures that no value is present for MaxDriveTime, not even an explicit nil
### GetMaxDriveTimeJob

`func (o *Resource) GetMaxDriveTimeJob() int32`

GetMaxDriveTimeJob returns the MaxDriveTimeJob field if non-nil, zero value otherwise.

### GetMaxDriveTimeJobOk

`func (o *Resource) GetMaxDriveTimeJobOk() (*int32, bool)`

GetMaxDriveTimeJobOk returns a tuple with the MaxDriveTimeJob field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxDriveTimeJob

`func (o *Resource) SetMaxDriveTimeJob(v int32)`

SetMaxDriveTimeJob sets MaxDriveTimeJob field to given value.

### HasMaxDriveTimeJob

`func (o *Resource) HasMaxDriveTimeJob() bool`

HasMaxDriveTimeJob returns a boolean if a field has been set.

### SetMaxDriveTimeJobNil

`func (o *Resource) SetMaxDriveTimeJobNil(b bool)`

 SetMaxDriveTimeJobNil sets the value for MaxDriveTimeJob to be an explicit nil

### UnsetMaxDriveTimeJob
`func (o *Resource) UnsetMaxDriveTimeJob()`

UnsetMaxDriveTimeJob ensures that no value is present for MaxDriveTimeJob, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


