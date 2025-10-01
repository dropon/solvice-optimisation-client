# OnRouteResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **NullableString** | Id of the solve job | [optional] 
**Status** | Pointer to [**NullableSolviceStatus**](SolviceStatus.md) | Status of the Response | [optional] 
**Score** | Pointer to [**NullableOnRouteResponseScore**](OnRouteResponseScore.md) |  | [optional] 
**Unresolved** | Pointer to **interface{}** | Constraints that are violated | [optional] 
**Trips** | [**[]Trip**](Trip.md) | Actual solution: trips per shift/day and per resource | 
**TotalWaitTimeInSeconds** | Pointer to **NullableInt64** | Wait time for all resources | [optional] 
**Occupancy** | Pointer to **NullableFloat64** | How full this schedule is in terms of work time (incl travel) over capacity. Eg 80% | [optional] 
**TotalTravelDistanceInMeters** | Pointer to **NullableInt64** | Travel distance for all resources in meters | [optional] 
**TotalTravelTimeInSeconds** | Pointer to **NullableInt64** | Travel time for all resources | [optional] 
**TotalServiceTimeInSeconds** | Pointer to **NullableInt64** | Service time for all resources | [optional] 
**Unserved** | Pointer to **[]string** | Unserved jobs | [optional] 
**UnservedReasons** | Pointer to **map[string]map[string]interface{}** | Reasons why jobs could not be served, mapped by job name | [optional] 
**Suggestions** | Pointer to [**[]SuggestionDto**](SuggestionDto.md) | List of suggested assignments returned by suggest api call | [optional] 
**Messages** | Pointer to **[]string** | Events and warnings generated during the solver execution | [optional] 
**Violations** | Pointer to [**[]ViolatedConstraint**](ViolatedConstraint.md) |  | [optional] 
**WorkloadFairness** | Pointer to **NullableFloat64** |  | [optional] 

## Methods

### NewOnRouteResponse

`func NewOnRouteResponse(trips []Trip, ) *OnRouteResponse`

NewOnRouteResponse instantiates a new OnRouteResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewOnRouteResponseWithDefaults

`func NewOnRouteResponseWithDefaults() *OnRouteResponse`

NewOnRouteResponseWithDefaults instantiates a new OnRouteResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *OnRouteResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *OnRouteResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *OnRouteResponse) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *OnRouteResponse) HasId() bool`

HasId returns a boolean if a field has been set.

### SetIdNil

`func (o *OnRouteResponse) SetIdNil(b bool)`

 SetIdNil sets the value for Id to be an explicit nil

### UnsetId
`func (o *OnRouteResponse) UnsetId()`

UnsetId ensures that no value is present for Id, not even an explicit nil
### GetStatus

`func (o *OnRouteResponse) GetStatus() SolviceStatus`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *OnRouteResponse) GetStatusOk() (*SolviceStatus, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *OnRouteResponse) SetStatus(v SolviceStatus)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *OnRouteResponse) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### SetStatusNil

`func (o *OnRouteResponse) SetStatusNil(b bool)`

 SetStatusNil sets the value for Status to be an explicit nil

### UnsetStatus
`func (o *OnRouteResponse) UnsetStatus()`

UnsetStatus ensures that no value is present for Status, not even an explicit nil
### GetScore

`func (o *OnRouteResponse) GetScore() OnRouteResponseScore`

GetScore returns the Score field if non-nil, zero value otherwise.

### GetScoreOk

`func (o *OnRouteResponse) GetScoreOk() (*OnRouteResponseScore, bool)`

GetScoreOk returns a tuple with the Score field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScore

`func (o *OnRouteResponse) SetScore(v OnRouteResponseScore)`

SetScore sets Score field to given value.

### HasScore

`func (o *OnRouteResponse) HasScore() bool`

HasScore returns a boolean if a field has been set.

### SetScoreNil

`func (o *OnRouteResponse) SetScoreNil(b bool)`

 SetScoreNil sets the value for Score to be an explicit nil

### UnsetScore
`func (o *OnRouteResponse) UnsetScore()`

UnsetScore ensures that no value is present for Score, not even an explicit nil
### GetUnresolved

`func (o *OnRouteResponse) GetUnresolved() interface{}`

GetUnresolved returns the Unresolved field if non-nil, zero value otherwise.

### GetUnresolvedOk

`func (o *OnRouteResponse) GetUnresolvedOk() (*interface{}, bool)`

GetUnresolvedOk returns a tuple with the Unresolved field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnresolved

`func (o *OnRouteResponse) SetUnresolved(v interface{})`

SetUnresolved sets Unresolved field to given value.

### HasUnresolved

`func (o *OnRouteResponse) HasUnresolved() bool`

HasUnresolved returns a boolean if a field has been set.

### SetUnresolvedNil

`func (o *OnRouteResponse) SetUnresolvedNil(b bool)`

 SetUnresolvedNil sets the value for Unresolved to be an explicit nil

### UnsetUnresolved
`func (o *OnRouteResponse) UnsetUnresolved()`

UnsetUnresolved ensures that no value is present for Unresolved, not even an explicit nil
### GetTrips

`func (o *OnRouteResponse) GetTrips() []Trip`

GetTrips returns the Trips field if non-nil, zero value otherwise.

### GetTripsOk

`func (o *OnRouteResponse) GetTripsOk() (*[]Trip, bool)`

GetTripsOk returns a tuple with the Trips field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTrips

`func (o *OnRouteResponse) SetTrips(v []Trip)`

SetTrips sets Trips field to given value.


### GetTotalWaitTimeInSeconds

`func (o *OnRouteResponse) GetTotalWaitTimeInSeconds() int64`

GetTotalWaitTimeInSeconds returns the TotalWaitTimeInSeconds field if non-nil, zero value otherwise.

### GetTotalWaitTimeInSecondsOk

`func (o *OnRouteResponse) GetTotalWaitTimeInSecondsOk() (*int64, bool)`

GetTotalWaitTimeInSecondsOk returns a tuple with the TotalWaitTimeInSeconds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalWaitTimeInSeconds

`func (o *OnRouteResponse) SetTotalWaitTimeInSeconds(v int64)`

SetTotalWaitTimeInSeconds sets TotalWaitTimeInSeconds field to given value.

### HasTotalWaitTimeInSeconds

`func (o *OnRouteResponse) HasTotalWaitTimeInSeconds() bool`

HasTotalWaitTimeInSeconds returns a boolean if a field has been set.

### SetTotalWaitTimeInSecondsNil

`func (o *OnRouteResponse) SetTotalWaitTimeInSecondsNil(b bool)`

 SetTotalWaitTimeInSecondsNil sets the value for TotalWaitTimeInSeconds to be an explicit nil

### UnsetTotalWaitTimeInSeconds
`func (o *OnRouteResponse) UnsetTotalWaitTimeInSeconds()`

UnsetTotalWaitTimeInSeconds ensures that no value is present for TotalWaitTimeInSeconds, not even an explicit nil
### GetOccupancy

`func (o *OnRouteResponse) GetOccupancy() float64`

GetOccupancy returns the Occupancy field if non-nil, zero value otherwise.

### GetOccupancyOk

`func (o *OnRouteResponse) GetOccupancyOk() (*float64, bool)`

GetOccupancyOk returns a tuple with the Occupancy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOccupancy

`func (o *OnRouteResponse) SetOccupancy(v float64)`

SetOccupancy sets Occupancy field to given value.

### HasOccupancy

`func (o *OnRouteResponse) HasOccupancy() bool`

HasOccupancy returns a boolean if a field has been set.

### SetOccupancyNil

`func (o *OnRouteResponse) SetOccupancyNil(b bool)`

 SetOccupancyNil sets the value for Occupancy to be an explicit nil

### UnsetOccupancy
`func (o *OnRouteResponse) UnsetOccupancy()`

UnsetOccupancy ensures that no value is present for Occupancy, not even an explicit nil
### GetTotalTravelDistanceInMeters

`func (o *OnRouteResponse) GetTotalTravelDistanceInMeters() int64`

GetTotalTravelDistanceInMeters returns the TotalTravelDistanceInMeters field if non-nil, zero value otherwise.

### GetTotalTravelDistanceInMetersOk

`func (o *OnRouteResponse) GetTotalTravelDistanceInMetersOk() (*int64, bool)`

GetTotalTravelDistanceInMetersOk returns a tuple with the TotalTravelDistanceInMeters field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalTravelDistanceInMeters

`func (o *OnRouteResponse) SetTotalTravelDistanceInMeters(v int64)`

SetTotalTravelDistanceInMeters sets TotalTravelDistanceInMeters field to given value.

### HasTotalTravelDistanceInMeters

`func (o *OnRouteResponse) HasTotalTravelDistanceInMeters() bool`

HasTotalTravelDistanceInMeters returns a boolean if a field has been set.

### SetTotalTravelDistanceInMetersNil

`func (o *OnRouteResponse) SetTotalTravelDistanceInMetersNil(b bool)`

 SetTotalTravelDistanceInMetersNil sets the value for TotalTravelDistanceInMeters to be an explicit nil

### UnsetTotalTravelDistanceInMeters
`func (o *OnRouteResponse) UnsetTotalTravelDistanceInMeters()`

UnsetTotalTravelDistanceInMeters ensures that no value is present for TotalTravelDistanceInMeters, not even an explicit nil
### GetTotalTravelTimeInSeconds

`func (o *OnRouteResponse) GetTotalTravelTimeInSeconds() int64`

GetTotalTravelTimeInSeconds returns the TotalTravelTimeInSeconds field if non-nil, zero value otherwise.

### GetTotalTravelTimeInSecondsOk

`func (o *OnRouteResponse) GetTotalTravelTimeInSecondsOk() (*int64, bool)`

GetTotalTravelTimeInSecondsOk returns a tuple with the TotalTravelTimeInSeconds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalTravelTimeInSeconds

`func (o *OnRouteResponse) SetTotalTravelTimeInSeconds(v int64)`

SetTotalTravelTimeInSeconds sets TotalTravelTimeInSeconds field to given value.

### HasTotalTravelTimeInSeconds

`func (o *OnRouteResponse) HasTotalTravelTimeInSeconds() bool`

HasTotalTravelTimeInSeconds returns a boolean if a field has been set.

### SetTotalTravelTimeInSecondsNil

`func (o *OnRouteResponse) SetTotalTravelTimeInSecondsNil(b bool)`

 SetTotalTravelTimeInSecondsNil sets the value for TotalTravelTimeInSeconds to be an explicit nil

### UnsetTotalTravelTimeInSeconds
`func (o *OnRouteResponse) UnsetTotalTravelTimeInSeconds()`

UnsetTotalTravelTimeInSeconds ensures that no value is present for TotalTravelTimeInSeconds, not even an explicit nil
### GetTotalServiceTimeInSeconds

`func (o *OnRouteResponse) GetTotalServiceTimeInSeconds() int64`

GetTotalServiceTimeInSeconds returns the TotalServiceTimeInSeconds field if non-nil, zero value otherwise.

### GetTotalServiceTimeInSecondsOk

`func (o *OnRouteResponse) GetTotalServiceTimeInSecondsOk() (*int64, bool)`

GetTotalServiceTimeInSecondsOk returns a tuple with the TotalServiceTimeInSeconds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalServiceTimeInSeconds

`func (o *OnRouteResponse) SetTotalServiceTimeInSeconds(v int64)`

SetTotalServiceTimeInSeconds sets TotalServiceTimeInSeconds field to given value.

### HasTotalServiceTimeInSeconds

`func (o *OnRouteResponse) HasTotalServiceTimeInSeconds() bool`

HasTotalServiceTimeInSeconds returns a boolean if a field has been set.

### SetTotalServiceTimeInSecondsNil

`func (o *OnRouteResponse) SetTotalServiceTimeInSecondsNil(b bool)`

 SetTotalServiceTimeInSecondsNil sets the value for TotalServiceTimeInSeconds to be an explicit nil

### UnsetTotalServiceTimeInSeconds
`func (o *OnRouteResponse) UnsetTotalServiceTimeInSeconds()`

UnsetTotalServiceTimeInSeconds ensures that no value is present for TotalServiceTimeInSeconds, not even an explicit nil
### GetUnserved

`func (o *OnRouteResponse) GetUnserved() []string`

GetUnserved returns the Unserved field if non-nil, zero value otherwise.

### GetUnservedOk

`func (o *OnRouteResponse) GetUnservedOk() (*[]string, bool)`

GetUnservedOk returns a tuple with the Unserved field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnserved

`func (o *OnRouteResponse) SetUnserved(v []string)`

SetUnserved sets Unserved field to given value.

### HasUnserved

`func (o *OnRouteResponse) HasUnserved() bool`

HasUnserved returns a boolean if a field has been set.

### SetUnservedNil

`func (o *OnRouteResponse) SetUnservedNil(b bool)`

 SetUnservedNil sets the value for Unserved to be an explicit nil

### UnsetUnserved
`func (o *OnRouteResponse) UnsetUnserved()`

UnsetUnserved ensures that no value is present for Unserved, not even an explicit nil
### GetUnservedReasons

`func (o *OnRouteResponse) GetUnservedReasons() map[string]map[string]interface{}`

GetUnservedReasons returns the UnservedReasons field if non-nil, zero value otherwise.

### GetUnservedReasonsOk

`func (o *OnRouteResponse) GetUnservedReasonsOk() (*map[string]map[string]interface{}, bool)`

GetUnservedReasonsOk returns a tuple with the UnservedReasons field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnservedReasons

`func (o *OnRouteResponse) SetUnservedReasons(v map[string]map[string]interface{})`

SetUnservedReasons sets UnservedReasons field to given value.

### HasUnservedReasons

`func (o *OnRouteResponse) HasUnservedReasons() bool`

HasUnservedReasons returns a boolean if a field has been set.

### SetUnservedReasonsNil

`func (o *OnRouteResponse) SetUnservedReasonsNil(b bool)`

 SetUnservedReasonsNil sets the value for UnservedReasons to be an explicit nil

### UnsetUnservedReasons
`func (o *OnRouteResponse) UnsetUnservedReasons()`

UnsetUnservedReasons ensures that no value is present for UnservedReasons, not even an explicit nil
### GetSuggestions

`func (o *OnRouteResponse) GetSuggestions() []SuggestionDto`

GetSuggestions returns the Suggestions field if non-nil, zero value otherwise.

### GetSuggestionsOk

`func (o *OnRouteResponse) GetSuggestionsOk() (*[]SuggestionDto, bool)`

GetSuggestionsOk returns a tuple with the Suggestions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuggestions

`func (o *OnRouteResponse) SetSuggestions(v []SuggestionDto)`

SetSuggestions sets Suggestions field to given value.

### HasSuggestions

`func (o *OnRouteResponse) HasSuggestions() bool`

HasSuggestions returns a boolean if a field has been set.

### SetSuggestionsNil

`func (o *OnRouteResponse) SetSuggestionsNil(b bool)`

 SetSuggestionsNil sets the value for Suggestions to be an explicit nil

### UnsetSuggestions
`func (o *OnRouteResponse) UnsetSuggestions()`

UnsetSuggestions ensures that no value is present for Suggestions, not even an explicit nil
### GetMessages

`func (o *OnRouteResponse) GetMessages() []string`

GetMessages returns the Messages field if non-nil, zero value otherwise.

### GetMessagesOk

`func (o *OnRouteResponse) GetMessagesOk() (*[]string, bool)`

GetMessagesOk returns a tuple with the Messages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessages

`func (o *OnRouteResponse) SetMessages(v []string)`

SetMessages sets Messages field to given value.

### HasMessages

`func (o *OnRouteResponse) HasMessages() bool`

HasMessages returns a boolean if a field has been set.

### SetMessagesNil

`func (o *OnRouteResponse) SetMessagesNil(b bool)`

 SetMessagesNil sets the value for Messages to be an explicit nil

### UnsetMessages
`func (o *OnRouteResponse) UnsetMessages()`

UnsetMessages ensures that no value is present for Messages, not even an explicit nil
### GetViolations

`func (o *OnRouteResponse) GetViolations() []ViolatedConstraint`

GetViolations returns the Violations field if non-nil, zero value otherwise.

### GetViolationsOk

`func (o *OnRouteResponse) GetViolationsOk() (*[]ViolatedConstraint, bool)`

GetViolationsOk returns a tuple with the Violations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetViolations

`func (o *OnRouteResponse) SetViolations(v []ViolatedConstraint)`

SetViolations sets Violations field to given value.

### HasViolations

`func (o *OnRouteResponse) HasViolations() bool`

HasViolations returns a boolean if a field has been set.

### SetViolationsNil

`func (o *OnRouteResponse) SetViolationsNil(b bool)`

 SetViolationsNil sets the value for Violations to be an explicit nil

### UnsetViolations
`func (o *OnRouteResponse) UnsetViolations()`

UnsetViolations ensures that no value is present for Violations, not even an explicit nil
### GetWorkloadFairness

`func (o *OnRouteResponse) GetWorkloadFairness() float64`

GetWorkloadFairness returns the WorkloadFairness field if non-nil, zero value otherwise.

### GetWorkloadFairnessOk

`func (o *OnRouteResponse) GetWorkloadFairnessOk() (*float64, bool)`

GetWorkloadFairnessOk returns a tuple with the WorkloadFairness field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkloadFairness

`func (o *OnRouteResponse) SetWorkloadFairness(v float64)`

SetWorkloadFairness sets WorkloadFairness field to given value.

### HasWorkloadFairness

`func (o *OnRouteResponse) HasWorkloadFairness() bool`

HasWorkloadFairness returns a boolean if a field has been set.

### SetWorkloadFairnessNil

`func (o *OnRouteResponse) SetWorkloadFairnessNil(b bool)`

 SetWorkloadFairnessNil sets the value for WorkloadFairness to be an explicit nil

### UnsetWorkloadFairness
`func (o *OnRouteResponse) UnsetWorkloadFairness()`

UnsetWorkloadFairness ensures that no value is present for WorkloadFairness, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


