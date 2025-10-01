# Visit

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Arrival** | Pointer to **NullableTime** | Actual arrival date-time | [optional] 
**ServiceTime** | Pointer to **NullableInt64** | Total service time of that job in seconds | [optional] 
**TravelTime** | Pointer to **NullableInt64** | Total travel time to that job in seconds | [optional] 
**Distance** | Pointer to **NullableInt64** | Total travel distance to that job in meters | [optional] 
**Job** | Pointer to **NullableString** | Job | [optional] 
**Activity** | Pointer to **NullableString** | The activity to  | [optional] 
**Location** | Pointer to [**NullableLocation**](Location.md) | Location with lat/lon | [optional] 
**Latlon** | Pointer to **[]float64** | Snapped Latlng. When we get your lat/lon in input, we snap it on our map to a valid point in the graph. We return all snapped points. | [optional] 
**SnappedLocation** | Pointer to [**NullableLocation**](Location.md) | Snapped location. When we get your lat/lon in input, we snap it on our map to a valid point in the graph. We return all snapped points. | [optional] 
**BreakTime** | Pointer to **NullableInt32** | Break time in seconds | [optional] 
**WaitTime** | Pointer to **NullableInt64** | Wait time in seconds | [optional] 

## Methods

### NewVisit

`func NewVisit() *Visit`

NewVisit instantiates a new Visit object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewVisitWithDefaults

`func NewVisitWithDefaults() *Visit`

NewVisitWithDefaults instantiates a new Visit object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetArrival

`func (o *Visit) GetArrival() time.Time`

GetArrival returns the Arrival field if non-nil, zero value otherwise.

### GetArrivalOk

`func (o *Visit) GetArrivalOk() (*time.Time, bool)`

GetArrivalOk returns a tuple with the Arrival field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArrival

`func (o *Visit) SetArrival(v time.Time)`

SetArrival sets Arrival field to given value.

### HasArrival

`func (o *Visit) HasArrival() bool`

HasArrival returns a boolean if a field has been set.

### SetArrivalNil

`func (o *Visit) SetArrivalNil(b bool)`

 SetArrivalNil sets the value for Arrival to be an explicit nil

### UnsetArrival
`func (o *Visit) UnsetArrival()`

UnsetArrival ensures that no value is present for Arrival, not even an explicit nil
### GetServiceTime

`func (o *Visit) GetServiceTime() int64`

GetServiceTime returns the ServiceTime field if non-nil, zero value otherwise.

### GetServiceTimeOk

`func (o *Visit) GetServiceTimeOk() (*int64, bool)`

GetServiceTimeOk returns a tuple with the ServiceTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetServiceTime

`func (o *Visit) SetServiceTime(v int64)`

SetServiceTime sets ServiceTime field to given value.

### HasServiceTime

`func (o *Visit) HasServiceTime() bool`

HasServiceTime returns a boolean if a field has been set.

### SetServiceTimeNil

`func (o *Visit) SetServiceTimeNil(b bool)`

 SetServiceTimeNil sets the value for ServiceTime to be an explicit nil

### UnsetServiceTime
`func (o *Visit) UnsetServiceTime()`

UnsetServiceTime ensures that no value is present for ServiceTime, not even an explicit nil
### GetTravelTime

`func (o *Visit) GetTravelTime() int64`

GetTravelTime returns the TravelTime field if non-nil, zero value otherwise.

### GetTravelTimeOk

`func (o *Visit) GetTravelTimeOk() (*int64, bool)`

GetTravelTimeOk returns a tuple with the TravelTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTravelTime

`func (o *Visit) SetTravelTime(v int64)`

SetTravelTime sets TravelTime field to given value.

### HasTravelTime

`func (o *Visit) HasTravelTime() bool`

HasTravelTime returns a boolean if a field has been set.

### SetTravelTimeNil

`func (o *Visit) SetTravelTimeNil(b bool)`

 SetTravelTimeNil sets the value for TravelTime to be an explicit nil

### UnsetTravelTime
`func (o *Visit) UnsetTravelTime()`

UnsetTravelTime ensures that no value is present for TravelTime, not even an explicit nil
### GetDistance

`func (o *Visit) GetDistance() int64`

GetDistance returns the Distance field if non-nil, zero value otherwise.

### GetDistanceOk

`func (o *Visit) GetDistanceOk() (*int64, bool)`

GetDistanceOk returns a tuple with the Distance field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDistance

`func (o *Visit) SetDistance(v int64)`

SetDistance sets Distance field to given value.

### HasDistance

`func (o *Visit) HasDistance() bool`

HasDistance returns a boolean if a field has been set.

### SetDistanceNil

`func (o *Visit) SetDistanceNil(b bool)`

 SetDistanceNil sets the value for Distance to be an explicit nil

### UnsetDistance
`func (o *Visit) UnsetDistance()`

UnsetDistance ensures that no value is present for Distance, not even an explicit nil
### GetJob

`func (o *Visit) GetJob() string`

GetJob returns the Job field if non-nil, zero value otherwise.

### GetJobOk

`func (o *Visit) GetJobOk() (*string, bool)`

GetJobOk returns a tuple with the Job field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJob

`func (o *Visit) SetJob(v string)`

SetJob sets Job field to given value.

### HasJob

`func (o *Visit) HasJob() bool`

HasJob returns a boolean if a field has been set.

### SetJobNil

`func (o *Visit) SetJobNil(b bool)`

 SetJobNil sets the value for Job to be an explicit nil

### UnsetJob
`func (o *Visit) UnsetJob()`

UnsetJob ensures that no value is present for Job, not even an explicit nil
### GetActivity

`func (o *Visit) GetActivity() string`

GetActivity returns the Activity field if non-nil, zero value otherwise.

### GetActivityOk

`func (o *Visit) GetActivityOk() (*string, bool)`

GetActivityOk returns a tuple with the Activity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActivity

`func (o *Visit) SetActivity(v string)`

SetActivity sets Activity field to given value.

### HasActivity

`func (o *Visit) HasActivity() bool`

HasActivity returns a boolean if a field has been set.

### SetActivityNil

`func (o *Visit) SetActivityNil(b bool)`

 SetActivityNil sets the value for Activity to be an explicit nil

### UnsetActivity
`func (o *Visit) UnsetActivity()`

UnsetActivity ensures that no value is present for Activity, not even an explicit nil
### GetLocation

`func (o *Visit) GetLocation() Location`

GetLocation returns the Location field if non-nil, zero value otherwise.

### GetLocationOk

`func (o *Visit) GetLocationOk() (*Location, bool)`

GetLocationOk returns a tuple with the Location field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLocation

`func (o *Visit) SetLocation(v Location)`

SetLocation sets Location field to given value.

### HasLocation

`func (o *Visit) HasLocation() bool`

HasLocation returns a boolean if a field has been set.

### SetLocationNil

`func (o *Visit) SetLocationNil(b bool)`

 SetLocationNil sets the value for Location to be an explicit nil

### UnsetLocation
`func (o *Visit) UnsetLocation()`

UnsetLocation ensures that no value is present for Location, not even an explicit nil
### GetLatlon

`func (o *Visit) GetLatlon() []float64`

GetLatlon returns the Latlon field if non-nil, zero value otherwise.

### GetLatlonOk

`func (o *Visit) GetLatlonOk() (*[]float64, bool)`

GetLatlonOk returns a tuple with the Latlon field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLatlon

`func (o *Visit) SetLatlon(v []float64)`

SetLatlon sets Latlon field to given value.

### HasLatlon

`func (o *Visit) HasLatlon() bool`

HasLatlon returns a boolean if a field has been set.

### SetLatlonNil

`func (o *Visit) SetLatlonNil(b bool)`

 SetLatlonNil sets the value for Latlon to be an explicit nil

### UnsetLatlon
`func (o *Visit) UnsetLatlon()`

UnsetLatlon ensures that no value is present for Latlon, not even an explicit nil
### GetSnappedLocation

`func (o *Visit) GetSnappedLocation() Location`

GetSnappedLocation returns the SnappedLocation field if non-nil, zero value otherwise.

### GetSnappedLocationOk

`func (o *Visit) GetSnappedLocationOk() (*Location, bool)`

GetSnappedLocationOk returns a tuple with the SnappedLocation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSnappedLocation

`func (o *Visit) SetSnappedLocation(v Location)`

SetSnappedLocation sets SnappedLocation field to given value.

### HasSnappedLocation

`func (o *Visit) HasSnappedLocation() bool`

HasSnappedLocation returns a boolean if a field has been set.

### SetSnappedLocationNil

`func (o *Visit) SetSnappedLocationNil(b bool)`

 SetSnappedLocationNil sets the value for SnappedLocation to be an explicit nil

### UnsetSnappedLocation
`func (o *Visit) UnsetSnappedLocation()`

UnsetSnappedLocation ensures that no value is present for SnappedLocation, not even an explicit nil
### GetBreakTime

`func (o *Visit) GetBreakTime() int32`

GetBreakTime returns the BreakTime field if non-nil, zero value otherwise.

### GetBreakTimeOk

`func (o *Visit) GetBreakTimeOk() (*int32, bool)`

GetBreakTimeOk returns a tuple with the BreakTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBreakTime

`func (o *Visit) SetBreakTime(v int32)`

SetBreakTime sets BreakTime field to given value.

### HasBreakTime

`func (o *Visit) HasBreakTime() bool`

HasBreakTime returns a boolean if a field has been set.

### SetBreakTimeNil

`func (o *Visit) SetBreakTimeNil(b bool)`

 SetBreakTimeNil sets the value for BreakTime to be an explicit nil

### UnsetBreakTime
`func (o *Visit) UnsetBreakTime()`

UnsetBreakTime ensures that no value is present for BreakTime, not even an explicit nil
### GetWaitTime

`func (o *Visit) GetWaitTime() int64`

GetWaitTime returns the WaitTime field if non-nil, zero value otherwise.

### GetWaitTimeOk

`func (o *Visit) GetWaitTimeOk() (*int64, bool)`

GetWaitTimeOk returns a tuple with the WaitTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWaitTime

`func (o *Visit) SetWaitTime(v int64)`

SetWaitTime sets WaitTime field to given value.

### HasWaitTime

`func (o *Visit) HasWaitTime() bool`

HasWaitTime returns a boolean if a field has been set.

### SetWaitTimeNil

`func (o *Visit) SetWaitTimeNil(b bool)`

 SetWaitTimeNil sets the value for WaitTime to be an explicit nil

### UnsetWaitTime
`func (o *Visit) UnsetWaitTime()`

UnsetWaitTime ensures that no value is present for WaitTime, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


