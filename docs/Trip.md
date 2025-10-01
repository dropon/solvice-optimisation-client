# Trip

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Visits** | [**[]Visit**](Visit.md) | List of visits for a resource and a date. | 
**Resource** | Pointer to **NullableString** | Resource | [optional] 
**Date** | Pointer to **NullableString** | Date | [optional] 
**DepartureTime** | Pointer to **NullableString** | Departure date-time | [optional] 
**WaitTime** | Pointer to **NullableInt64** | Wait time in seconds | [optional] 
**TravelTime** | Pointer to **NullableInt64** | Travel time in seconds | [optional] 
**WorkTime** | Pointer to **NullableInt64** | Work time in seconds | [optional] 
**ServiceTime** | Pointer to **NullableInt64** | Service time in seconds | [optional] 
**Polyline** | Pointer to **NullableString** | Polyline of the trip | [optional] 
**Occupancy** | Pointer to **NullableFloat64** | How full this trip is in terms of work time over capacity. Eg 80% | [optional] 
**Start** | Pointer to [**NullableVisit**](Visit.md) |  | [optional] 
**End** | Pointer to [**NullableVisit**](Visit.md) |  | [optional] 
**Distance** | Pointer to **NullableInt64** |  | [optional] 

## Methods

### NewTrip

`func NewTrip(visits []Visit, ) *Trip`

NewTrip instantiates a new Trip object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTripWithDefaults

`func NewTripWithDefaults() *Trip`

NewTripWithDefaults instantiates a new Trip object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetVisits

`func (o *Trip) GetVisits() []Visit`

GetVisits returns the Visits field if non-nil, zero value otherwise.

### GetVisitsOk

`func (o *Trip) GetVisitsOk() (*[]Visit, bool)`

GetVisitsOk returns a tuple with the Visits field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVisits

`func (o *Trip) SetVisits(v []Visit)`

SetVisits sets Visits field to given value.


### GetResource

`func (o *Trip) GetResource() string`

GetResource returns the Resource field if non-nil, zero value otherwise.

### GetResourceOk

`func (o *Trip) GetResourceOk() (*string, bool)`

GetResourceOk returns a tuple with the Resource field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResource

`func (o *Trip) SetResource(v string)`

SetResource sets Resource field to given value.

### HasResource

`func (o *Trip) HasResource() bool`

HasResource returns a boolean if a field has been set.

### SetResourceNil

`func (o *Trip) SetResourceNil(b bool)`

 SetResourceNil sets the value for Resource to be an explicit nil

### UnsetResource
`func (o *Trip) UnsetResource()`

UnsetResource ensures that no value is present for Resource, not even an explicit nil
### GetDate

`func (o *Trip) GetDate() string`

GetDate returns the Date field if non-nil, zero value otherwise.

### GetDateOk

`func (o *Trip) GetDateOk() (*string, bool)`

GetDateOk returns a tuple with the Date field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDate

`func (o *Trip) SetDate(v string)`

SetDate sets Date field to given value.

### HasDate

`func (o *Trip) HasDate() bool`

HasDate returns a boolean if a field has been set.

### SetDateNil

`func (o *Trip) SetDateNil(b bool)`

 SetDateNil sets the value for Date to be an explicit nil

### UnsetDate
`func (o *Trip) UnsetDate()`

UnsetDate ensures that no value is present for Date, not even an explicit nil
### GetDepartureTime

`func (o *Trip) GetDepartureTime() string`

GetDepartureTime returns the DepartureTime field if non-nil, zero value otherwise.

### GetDepartureTimeOk

`func (o *Trip) GetDepartureTimeOk() (*string, bool)`

GetDepartureTimeOk returns a tuple with the DepartureTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDepartureTime

`func (o *Trip) SetDepartureTime(v string)`

SetDepartureTime sets DepartureTime field to given value.

### HasDepartureTime

`func (o *Trip) HasDepartureTime() bool`

HasDepartureTime returns a boolean if a field has been set.

### SetDepartureTimeNil

`func (o *Trip) SetDepartureTimeNil(b bool)`

 SetDepartureTimeNil sets the value for DepartureTime to be an explicit nil

### UnsetDepartureTime
`func (o *Trip) UnsetDepartureTime()`

UnsetDepartureTime ensures that no value is present for DepartureTime, not even an explicit nil
### GetWaitTime

`func (o *Trip) GetWaitTime() int64`

GetWaitTime returns the WaitTime field if non-nil, zero value otherwise.

### GetWaitTimeOk

`func (o *Trip) GetWaitTimeOk() (*int64, bool)`

GetWaitTimeOk returns a tuple with the WaitTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWaitTime

`func (o *Trip) SetWaitTime(v int64)`

SetWaitTime sets WaitTime field to given value.

### HasWaitTime

`func (o *Trip) HasWaitTime() bool`

HasWaitTime returns a boolean if a field has been set.

### SetWaitTimeNil

`func (o *Trip) SetWaitTimeNil(b bool)`

 SetWaitTimeNil sets the value for WaitTime to be an explicit nil

### UnsetWaitTime
`func (o *Trip) UnsetWaitTime()`

UnsetWaitTime ensures that no value is present for WaitTime, not even an explicit nil
### GetTravelTime

`func (o *Trip) GetTravelTime() int64`

GetTravelTime returns the TravelTime field if non-nil, zero value otherwise.

### GetTravelTimeOk

`func (o *Trip) GetTravelTimeOk() (*int64, bool)`

GetTravelTimeOk returns a tuple with the TravelTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTravelTime

`func (o *Trip) SetTravelTime(v int64)`

SetTravelTime sets TravelTime field to given value.

### HasTravelTime

`func (o *Trip) HasTravelTime() bool`

HasTravelTime returns a boolean if a field has been set.

### SetTravelTimeNil

`func (o *Trip) SetTravelTimeNil(b bool)`

 SetTravelTimeNil sets the value for TravelTime to be an explicit nil

### UnsetTravelTime
`func (o *Trip) UnsetTravelTime()`

UnsetTravelTime ensures that no value is present for TravelTime, not even an explicit nil
### GetWorkTime

`func (o *Trip) GetWorkTime() int64`

GetWorkTime returns the WorkTime field if non-nil, zero value otherwise.

### GetWorkTimeOk

`func (o *Trip) GetWorkTimeOk() (*int64, bool)`

GetWorkTimeOk returns a tuple with the WorkTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkTime

`func (o *Trip) SetWorkTime(v int64)`

SetWorkTime sets WorkTime field to given value.

### HasWorkTime

`func (o *Trip) HasWorkTime() bool`

HasWorkTime returns a boolean if a field has been set.

### SetWorkTimeNil

`func (o *Trip) SetWorkTimeNil(b bool)`

 SetWorkTimeNil sets the value for WorkTime to be an explicit nil

### UnsetWorkTime
`func (o *Trip) UnsetWorkTime()`

UnsetWorkTime ensures that no value is present for WorkTime, not even an explicit nil
### GetServiceTime

`func (o *Trip) GetServiceTime() int64`

GetServiceTime returns the ServiceTime field if non-nil, zero value otherwise.

### GetServiceTimeOk

`func (o *Trip) GetServiceTimeOk() (*int64, bool)`

GetServiceTimeOk returns a tuple with the ServiceTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetServiceTime

`func (o *Trip) SetServiceTime(v int64)`

SetServiceTime sets ServiceTime field to given value.

### HasServiceTime

`func (o *Trip) HasServiceTime() bool`

HasServiceTime returns a boolean if a field has been set.

### SetServiceTimeNil

`func (o *Trip) SetServiceTimeNil(b bool)`

 SetServiceTimeNil sets the value for ServiceTime to be an explicit nil

### UnsetServiceTime
`func (o *Trip) UnsetServiceTime()`

UnsetServiceTime ensures that no value is present for ServiceTime, not even an explicit nil
### GetPolyline

`func (o *Trip) GetPolyline() string`

GetPolyline returns the Polyline field if non-nil, zero value otherwise.

### GetPolylineOk

`func (o *Trip) GetPolylineOk() (*string, bool)`

GetPolylineOk returns a tuple with the Polyline field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolyline

`func (o *Trip) SetPolyline(v string)`

SetPolyline sets Polyline field to given value.

### HasPolyline

`func (o *Trip) HasPolyline() bool`

HasPolyline returns a boolean if a field has been set.

### SetPolylineNil

`func (o *Trip) SetPolylineNil(b bool)`

 SetPolylineNil sets the value for Polyline to be an explicit nil

### UnsetPolyline
`func (o *Trip) UnsetPolyline()`

UnsetPolyline ensures that no value is present for Polyline, not even an explicit nil
### GetOccupancy

`func (o *Trip) GetOccupancy() float64`

GetOccupancy returns the Occupancy field if non-nil, zero value otherwise.

### GetOccupancyOk

`func (o *Trip) GetOccupancyOk() (*float64, bool)`

GetOccupancyOk returns a tuple with the Occupancy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOccupancy

`func (o *Trip) SetOccupancy(v float64)`

SetOccupancy sets Occupancy field to given value.

### HasOccupancy

`func (o *Trip) HasOccupancy() bool`

HasOccupancy returns a boolean if a field has been set.

### SetOccupancyNil

`func (o *Trip) SetOccupancyNil(b bool)`

 SetOccupancyNil sets the value for Occupancy to be an explicit nil

### UnsetOccupancy
`func (o *Trip) UnsetOccupancy()`

UnsetOccupancy ensures that no value is present for Occupancy, not even an explicit nil
### GetStart

`func (o *Trip) GetStart() Visit`

GetStart returns the Start field if non-nil, zero value otherwise.

### GetStartOk

`func (o *Trip) GetStartOk() (*Visit, bool)`

GetStartOk returns a tuple with the Start field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStart

`func (o *Trip) SetStart(v Visit)`

SetStart sets Start field to given value.

### HasStart

`func (o *Trip) HasStart() bool`

HasStart returns a boolean if a field has been set.

### SetStartNil

`func (o *Trip) SetStartNil(b bool)`

 SetStartNil sets the value for Start to be an explicit nil

### UnsetStart
`func (o *Trip) UnsetStart()`

UnsetStart ensures that no value is present for Start, not even an explicit nil
### GetEnd

`func (o *Trip) GetEnd() Visit`

GetEnd returns the End field if non-nil, zero value otherwise.

### GetEndOk

`func (o *Trip) GetEndOk() (*Visit, bool)`

GetEndOk returns a tuple with the End field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnd

`func (o *Trip) SetEnd(v Visit)`

SetEnd sets End field to given value.

### HasEnd

`func (o *Trip) HasEnd() bool`

HasEnd returns a boolean if a field has been set.

### SetEndNil

`func (o *Trip) SetEndNil(b bool)`

 SetEndNil sets the value for End to be an explicit nil

### UnsetEnd
`func (o *Trip) UnsetEnd()`

UnsetEnd ensures that no value is present for End, not even an explicit nil
### GetDistance

`func (o *Trip) GetDistance() int64`

GetDistance returns the Distance field if non-nil, zero value otherwise.

### GetDistanceOk

`func (o *Trip) GetDistanceOk() (*int64, bool)`

GetDistanceOk returns a tuple with the Distance field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDistance

`func (o *Trip) SetDistance(v int64)`

SetDistance sets Distance field to given value.

### HasDistance

`func (o *Trip) HasDistance() bool`

HasDistance returns a boolean if a field has been set.

### SetDistanceNil

`func (o *Trip) SetDistanceNil(b bool)`

 SetDistanceNil sets the value for Distance to be an explicit nil

### UnsetDistance
`func (o *Trip) UnsetDistance()`

UnsetDistance ensures that no value is present for Distance, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


