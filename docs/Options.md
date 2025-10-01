# Options

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Euclidian** | Pointer to **NullableBool** | Use euclidean distance calculations for travel time and distance instead of real road networks. When true, straight-line distances are used which is faster but less accurate. When false (default), routing engines like OSM, TomTom, or Google provide real road distances and travel times. | [optional] 
**RoutingEngine** | Pointer to [**NullableRoutingEngine**](RoutingEngine.md) | The routing engine used for calculating real-world distances and travel times. OSM (OpenStreetMaps) is free but basic, TomTom and Google provide more accurate traffic data and routing but require API keys. Only effective when euclidean is false. | [optional] 
**PartialPlanning** | Pointer to **NullableBool** | Allow the solver to create solutions where not all jobs are assigned to resources. When true (default), the solver will assign as many jobs as possible while respecting constraints. When false, the solver will only accept solutions where all jobs are assigned, which may result in infeasible solutions. | [optional] 
**MinimizeResources** | Pointer to **NullableBool** | Primary optimization objective. When true, the solver prioritizes using fewer resources (vehicles/drivers) even if it increases total travel time. When false, the solver prioritizes minimizing total travel time even if it requires more resources. This fundamentally changes the optimization strategy. | [optional] 
**Traffic** | Pointer to **NullableFloat64** | Global traffic multiplier applied to all travel times. A value of 1.1 increases travel times by 10% to account for traffic congestion. For real-time traffic data, use TomTom or Google routing engines. This is a simple approximation for scenarios where precise traffic data is unavailable. | [optional] 
**Polylines** | Pointer to **NullableBool** | Generate detailed route polylines (encoded route geometries) for each trip segment. When true, the response includes polyline data that can be used to draw routes on maps. This increases processing time and response size but provides visual route information for mapping applications. | [optional] 
**FairWorkloadPerTrip** | Pointer to **NullableBool** | Enable workload balancing across all resources and all days/trips. When true, the solver attempts to distribute service time evenly across all resources and time periods, preventing overloading of specific resources or days. The effectiveness is controlled by &#x60;Weights.workloadSpreadWeight&#x60; and &#x60;options.workloadSensitivity&#x60;. | [optional] 
**FairWorkloadPerResource** | Pointer to **NullableBool** | Enable workload balancing across different days for each individual resource. When true, the solver ensures that each resource&#39;s workload is distributed evenly across their available days, preventing some days from being overloaded while others are underutilized. Works in conjunction with &#x60;Weights.workloadSpreadWeight&#x60; and &#x60;options.workloadSensitivity&#x60;. | [optional] 
**SnapUnit** | Pointer to **NullableInt32** | Time granularity in seconds for arrival time snapping. All calculated arrival times are rounded up to the nearest multiple of this value. For example, with snapUnit&#x3D;300 (5 minutes), an arrival time of 08:32 becomes 08:35. This helps create more practical schedules by avoiding precise timings that are difficult to follow in real operations. The snapping affects score calculation during optimization. | [optional] 
**MaxSuggestions** | Pointer to **NullableInt32** | Maximum number of alternative assignment suggestions to return when using the suggestion endpoint. The solver generates multiple assignment options for unassigned jobs, ranked by quality. A value of 0 (default) returns all possible suggestions, while values 1-5 limit the results to the best alternatives. Higher values increase response time but provide more options. | [optional] 
**OnlyFeasibleSuggestions** | Pointer to **NullableBool** | Filter suggestions based on feasibility. When true (default), only suggestions that don&#39;t violate hard constraints are returned if the initial plan is feasible. If the initial plan is infeasible, only suggestions that don&#39;t worsen the infeasibility are returned. When false, all suggestions are returned regardless of feasibility, which may include constraint violations. | [optional] 
**WorkloadSensitivity** | Pointer to **NullableFloat64** |  | [optional] 
**Explanation** | Pointer to [**NullableExplanationOptions**](ExplanationOptions.md) |  | [optional] 
**FairComplexityPerTrip** | Pointer to **NullableBool** |  | [optional] 
**FairComplexityPerResource** | Pointer to **NullableBool** |  | [optional] 

## Methods

### NewOptions

`func NewOptions() *Options`

NewOptions instantiates a new Options object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewOptionsWithDefaults

`func NewOptionsWithDefaults() *Options`

NewOptionsWithDefaults instantiates a new Options object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEuclidian

`func (o *Options) GetEuclidian() bool`

GetEuclidian returns the Euclidian field if non-nil, zero value otherwise.

### GetEuclidianOk

`func (o *Options) GetEuclidianOk() (*bool, bool)`

GetEuclidianOk returns a tuple with the Euclidian field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEuclidian

`func (o *Options) SetEuclidian(v bool)`

SetEuclidian sets Euclidian field to given value.

### HasEuclidian

`func (o *Options) HasEuclidian() bool`

HasEuclidian returns a boolean if a field has been set.

### SetEuclidianNil

`func (o *Options) SetEuclidianNil(b bool)`

 SetEuclidianNil sets the value for Euclidian to be an explicit nil

### UnsetEuclidian
`func (o *Options) UnsetEuclidian()`

UnsetEuclidian ensures that no value is present for Euclidian, not even an explicit nil
### GetRoutingEngine

`func (o *Options) GetRoutingEngine() RoutingEngine`

GetRoutingEngine returns the RoutingEngine field if non-nil, zero value otherwise.

### GetRoutingEngineOk

`func (o *Options) GetRoutingEngineOk() (*RoutingEngine, bool)`

GetRoutingEngineOk returns a tuple with the RoutingEngine field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRoutingEngine

`func (o *Options) SetRoutingEngine(v RoutingEngine)`

SetRoutingEngine sets RoutingEngine field to given value.

### HasRoutingEngine

`func (o *Options) HasRoutingEngine() bool`

HasRoutingEngine returns a boolean if a field has been set.

### SetRoutingEngineNil

`func (o *Options) SetRoutingEngineNil(b bool)`

 SetRoutingEngineNil sets the value for RoutingEngine to be an explicit nil

### UnsetRoutingEngine
`func (o *Options) UnsetRoutingEngine()`

UnsetRoutingEngine ensures that no value is present for RoutingEngine, not even an explicit nil
### GetPartialPlanning

`func (o *Options) GetPartialPlanning() bool`

GetPartialPlanning returns the PartialPlanning field if non-nil, zero value otherwise.

### GetPartialPlanningOk

`func (o *Options) GetPartialPlanningOk() (*bool, bool)`

GetPartialPlanningOk returns a tuple with the PartialPlanning field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPartialPlanning

`func (o *Options) SetPartialPlanning(v bool)`

SetPartialPlanning sets PartialPlanning field to given value.

### HasPartialPlanning

`func (o *Options) HasPartialPlanning() bool`

HasPartialPlanning returns a boolean if a field has been set.

### SetPartialPlanningNil

`func (o *Options) SetPartialPlanningNil(b bool)`

 SetPartialPlanningNil sets the value for PartialPlanning to be an explicit nil

### UnsetPartialPlanning
`func (o *Options) UnsetPartialPlanning()`

UnsetPartialPlanning ensures that no value is present for PartialPlanning, not even an explicit nil
### GetMinimizeResources

`func (o *Options) GetMinimizeResources() bool`

GetMinimizeResources returns the MinimizeResources field if non-nil, zero value otherwise.

### GetMinimizeResourcesOk

`func (o *Options) GetMinimizeResourcesOk() (*bool, bool)`

GetMinimizeResourcesOk returns a tuple with the MinimizeResources field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMinimizeResources

`func (o *Options) SetMinimizeResources(v bool)`

SetMinimizeResources sets MinimizeResources field to given value.

### HasMinimizeResources

`func (o *Options) HasMinimizeResources() bool`

HasMinimizeResources returns a boolean if a field has been set.

### SetMinimizeResourcesNil

`func (o *Options) SetMinimizeResourcesNil(b bool)`

 SetMinimizeResourcesNil sets the value for MinimizeResources to be an explicit nil

### UnsetMinimizeResources
`func (o *Options) UnsetMinimizeResources()`

UnsetMinimizeResources ensures that no value is present for MinimizeResources, not even an explicit nil
### GetTraffic

`func (o *Options) GetTraffic() float64`

GetTraffic returns the Traffic field if non-nil, zero value otherwise.

### GetTrafficOk

`func (o *Options) GetTrafficOk() (*float64, bool)`

GetTrafficOk returns a tuple with the Traffic field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTraffic

`func (o *Options) SetTraffic(v float64)`

SetTraffic sets Traffic field to given value.

### HasTraffic

`func (o *Options) HasTraffic() bool`

HasTraffic returns a boolean if a field has been set.

### SetTrafficNil

`func (o *Options) SetTrafficNil(b bool)`

 SetTrafficNil sets the value for Traffic to be an explicit nil

### UnsetTraffic
`func (o *Options) UnsetTraffic()`

UnsetTraffic ensures that no value is present for Traffic, not even an explicit nil
### GetPolylines

`func (o *Options) GetPolylines() bool`

GetPolylines returns the Polylines field if non-nil, zero value otherwise.

### GetPolylinesOk

`func (o *Options) GetPolylinesOk() (*bool, bool)`

GetPolylinesOk returns a tuple with the Polylines field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolylines

`func (o *Options) SetPolylines(v bool)`

SetPolylines sets Polylines field to given value.

### HasPolylines

`func (o *Options) HasPolylines() bool`

HasPolylines returns a boolean if a field has been set.

### SetPolylinesNil

`func (o *Options) SetPolylinesNil(b bool)`

 SetPolylinesNil sets the value for Polylines to be an explicit nil

### UnsetPolylines
`func (o *Options) UnsetPolylines()`

UnsetPolylines ensures that no value is present for Polylines, not even an explicit nil
### GetFairWorkloadPerTrip

`func (o *Options) GetFairWorkloadPerTrip() bool`

GetFairWorkloadPerTrip returns the FairWorkloadPerTrip field if non-nil, zero value otherwise.

### GetFairWorkloadPerTripOk

`func (o *Options) GetFairWorkloadPerTripOk() (*bool, bool)`

GetFairWorkloadPerTripOk returns a tuple with the FairWorkloadPerTrip field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFairWorkloadPerTrip

`func (o *Options) SetFairWorkloadPerTrip(v bool)`

SetFairWorkloadPerTrip sets FairWorkloadPerTrip field to given value.

### HasFairWorkloadPerTrip

`func (o *Options) HasFairWorkloadPerTrip() bool`

HasFairWorkloadPerTrip returns a boolean if a field has been set.

### SetFairWorkloadPerTripNil

`func (o *Options) SetFairWorkloadPerTripNil(b bool)`

 SetFairWorkloadPerTripNil sets the value for FairWorkloadPerTrip to be an explicit nil

### UnsetFairWorkloadPerTrip
`func (o *Options) UnsetFairWorkloadPerTrip()`

UnsetFairWorkloadPerTrip ensures that no value is present for FairWorkloadPerTrip, not even an explicit nil
### GetFairWorkloadPerResource

`func (o *Options) GetFairWorkloadPerResource() bool`

GetFairWorkloadPerResource returns the FairWorkloadPerResource field if non-nil, zero value otherwise.

### GetFairWorkloadPerResourceOk

`func (o *Options) GetFairWorkloadPerResourceOk() (*bool, bool)`

GetFairWorkloadPerResourceOk returns a tuple with the FairWorkloadPerResource field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFairWorkloadPerResource

`func (o *Options) SetFairWorkloadPerResource(v bool)`

SetFairWorkloadPerResource sets FairWorkloadPerResource field to given value.

### HasFairWorkloadPerResource

`func (o *Options) HasFairWorkloadPerResource() bool`

HasFairWorkloadPerResource returns a boolean if a field has been set.

### SetFairWorkloadPerResourceNil

`func (o *Options) SetFairWorkloadPerResourceNil(b bool)`

 SetFairWorkloadPerResourceNil sets the value for FairWorkloadPerResource to be an explicit nil

### UnsetFairWorkloadPerResource
`func (o *Options) UnsetFairWorkloadPerResource()`

UnsetFairWorkloadPerResource ensures that no value is present for FairWorkloadPerResource, not even an explicit nil
### GetSnapUnit

`func (o *Options) GetSnapUnit() int32`

GetSnapUnit returns the SnapUnit field if non-nil, zero value otherwise.

### GetSnapUnitOk

`func (o *Options) GetSnapUnitOk() (*int32, bool)`

GetSnapUnitOk returns a tuple with the SnapUnit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSnapUnit

`func (o *Options) SetSnapUnit(v int32)`

SetSnapUnit sets SnapUnit field to given value.

### HasSnapUnit

`func (o *Options) HasSnapUnit() bool`

HasSnapUnit returns a boolean if a field has been set.

### SetSnapUnitNil

`func (o *Options) SetSnapUnitNil(b bool)`

 SetSnapUnitNil sets the value for SnapUnit to be an explicit nil

### UnsetSnapUnit
`func (o *Options) UnsetSnapUnit()`

UnsetSnapUnit ensures that no value is present for SnapUnit, not even an explicit nil
### GetMaxSuggestions

`func (o *Options) GetMaxSuggestions() int32`

GetMaxSuggestions returns the MaxSuggestions field if non-nil, zero value otherwise.

### GetMaxSuggestionsOk

`func (o *Options) GetMaxSuggestionsOk() (*int32, bool)`

GetMaxSuggestionsOk returns a tuple with the MaxSuggestions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxSuggestions

`func (o *Options) SetMaxSuggestions(v int32)`

SetMaxSuggestions sets MaxSuggestions field to given value.

### HasMaxSuggestions

`func (o *Options) HasMaxSuggestions() bool`

HasMaxSuggestions returns a boolean if a field has been set.

### SetMaxSuggestionsNil

`func (o *Options) SetMaxSuggestionsNil(b bool)`

 SetMaxSuggestionsNil sets the value for MaxSuggestions to be an explicit nil

### UnsetMaxSuggestions
`func (o *Options) UnsetMaxSuggestions()`

UnsetMaxSuggestions ensures that no value is present for MaxSuggestions, not even an explicit nil
### GetOnlyFeasibleSuggestions

`func (o *Options) GetOnlyFeasibleSuggestions() bool`

GetOnlyFeasibleSuggestions returns the OnlyFeasibleSuggestions field if non-nil, zero value otherwise.

### GetOnlyFeasibleSuggestionsOk

`func (o *Options) GetOnlyFeasibleSuggestionsOk() (*bool, bool)`

GetOnlyFeasibleSuggestionsOk returns a tuple with the OnlyFeasibleSuggestions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOnlyFeasibleSuggestions

`func (o *Options) SetOnlyFeasibleSuggestions(v bool)`

SetOnlyFeasibleSuggestions sets OnlyFeasibleSuggestions field to given value.

### HasOnlyFeasibleSuggestions

`func (o *Options) HasOnlyFeasibleSuggestions() bool`

HasOnlyFeasibleSuggestions returns a boolean if a field has been set.

### SetOnlyFeasibleSuggestionsNil

`func (o *Options) SetOnlyFeasibleSuggestionsNil(b bool)`

 SetOnlyFeasibleSuggestionsNil sets the value for OnlyFeasibleSuggestions to be an explicit nil

### UnsetOnlyFeasibleSuggestions
`func (o *Options) UnsetOnlyFeasibleSuggestions()`

UnsetOnlyFeasibleSuggestions ensures that no value is present for OnlyFeasibleSuggestions, not even an explicit nil
### GetWorkloadSensitivity

`func (o *Options) GetWorkloadSensitivity() float64`

GetWorkloadSensitivity returns the WorkloadSensitivity field if non-nil, zero value otherwise.

### GetWorkloadSensitivityOk

`func (o *Options) GetWorkloadSensitivityOk() (*float64, bool)`

GetWorkloadSensitivityOk returns a tuple with the WorkloadSensitivity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkloadSensitivity

`func (o *Options) SetWorkloadSensitivity(v float64)`

SetWorkloadSensitivity sets WorkloadSensitivity field to given value.

### HasWorkloadSensitivity

`func (o *Options) HasWorkloadSensitivity() bool`

HasWorkloadSensitivity returns a boolean if a field has been set.

### SetWorkloadSensitivityNil

`func (o *Options) SetWorkloadSensitivityNil(b bool)`

 SetWorkloadSensitivityNil sets the value for WorkloadSensitivity to be an explicit nil

### UnsetWorkloadSensitivity
`func (o *Options) UnsetWorkloadSensitivity()`

UnsetWorkloadSensitivity ensures that no value is present for WorkloadSensitivity, not even an explicit nil
### GetExplanation

`func (o *Options) GetExplanation() ExplanationOptions`

GetExplanation returns the Explanation field if non-nil, zero value otherwise.

### GetExplanationOk

`func (o *Options) GetExplanationOk() (*ExplanationOptions, bool)`

GetExplanationOk returns a tuple with the Explanation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExplanation

`func (o *Options) SetExplanation(v ExplanationOptions)`

SetExplanation sets Explanation field to given value.

### HasExplanation

`func (o *Options) HasExplanation() bool`

HasExplanation returns a boolean if a field has been set.

### SetExplanationNil

`func (o *Options) SetExplanationNil(b bool)`

 SetExplanationNil sets the value for Explanation to be an explicit nil

### UnsetExplanation
`func (o *Options) UnsetExplanation()`

UnsetExplanation ensures that no value is present for Explanation, not even an explicit nil
### GetFairComplexityPerTrip

`func (o *Options) GetFairComplexityPerTrip() bool`

GetFairComplexityPerTrip returns the FairComplexityPerTrip field if non-nil, zero value otherwise.

### GetFairComplexityPerTripOk

`func (o *Options) GetFairComplexityPerTripOk() (*bool, bool)`

GetFairComplexityPerTripOk returns a tuple with the FairComplexityPerTrip field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFairComplexityPerTrip

`func (o *Options) SetFairComplexityPerTrip(v bool)`

SetFairComplexityPerTrip sets FairComplexityPerTrip field to given value.

### HasFairComplexityPerTrip

`func (o *Options) HasFairComplexityPerTrip() bool`

HasFairComplexityPerTrip returns a boolean if a field has been set.

### SetFairComplexityPerTripNil

`func (o *Options) SetFairComplexityPerTripNil(b bool)`

 SetFairComplexityPerTripNil sets the value for FairComplexityPerTrip to be an explicit nil

### UnsetFairComplexityPerTrip
`func (o *Options) UnsetFairComplexityPerTrip()`

UnsetFairComplexityPerTrip ensures that no value is present for FairComplexityPerTrip, not even an explicit nil
### GetFairComplexityPerResource

`func (o *Options) GetFairComplexityPerResource() bool`

GetFairComplexityPerResource returns the FairComplexityPerResource field if non-nil, zero value otherwise.

### GetFairComplexityPerResourceOk

`func (o *Options) GetFairComplexityPerResourceOk() (*bool, bool)`

GetFairComplexityPerResourceOk returns a tuple with the FairComplexityPerResource field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFairComplexityPerResource

`func (o *Options) SetFairComplexityPerResource(v bool)`

SetFairComplexityPerResource sets FairComplexityPerResource field to given value.

### HasFairComplexityPerResource

`func (o *Options) HasFairComplexityPerResource() bool`

HasFairComplexityPerResource returns a boolean if a field has been set.

### SetFairComplexityPerResourceNil

`func (o *Options) SetFairComplexityPerResourceNil(b bool)`

 SetFairComplexityPerResourceNil sets the value for FairComplexityPerResource to be an explicit nil

### UnsetFairComplexityPerResource
`func (o *Options) UnsetFairComplexityPerResource()`

UnsetFairComplexityPerResource ensures that no value is present for FairComplexityPerResource, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


