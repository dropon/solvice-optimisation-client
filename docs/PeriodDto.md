# PeriodDto

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**From** | **time.Time** | Start date-time  | 
**End** | **interface{}** | End date-time  | 
**To** | **time.Time** |  | 

## Methods

### NewPeriodDto

`func NewPeriodDto(from time.Time, end interface{}, to time.Time, ) *PeriodDto`

NewPeriodDto instantiates a new PeriodDto object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPeriodDtoWithDefaults

`func NewPeriodDtoWithDefaults() *PeriodDto`

NewPeriodDtoWithDefaults instantiates a new PeriodDto object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFrom

`func (o *PeriodDto) GetFrom() time.Time`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *PeriodDto) GetFromOk() (*time.Time, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *PeriodDto) SetFrom(v time.Time)`

SetFrom sets From field to given value.


### GetEnd

`func (o *PeriodDto) GetEnd() interface{}`

GetEnd returns the End field if non-nil, zero value otherwise.

### GetEndOk

`func (o *PeriodDto) GetEndOk() (*interface{}, bool)`

GetEndOk returns a tuple with the End field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnd

`func (o *PeriodDto) SetEnd(v interface{})`

SetEnd sets End field to given value.


### SetEndNil

`func (o *PeriodDto) SetEndNil(b bool)`

 SetEndNil sets the value for End to be an explicit nil

### UnsetEnd
`func (o *PeriodDto) UnsetEnd()`

UnsetEnd ensures that no value is present for End, not even an explicit nil
### GetTo

`func (o *PeriodDto) GetTo() time.Time`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *PeriodDto) GetToOk() (*time.Time, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *PeriodDto) SetTo(v time.Time)`

SetTo sets To field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


