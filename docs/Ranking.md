# Ranking

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** | Name of the resource being ranked for this job. Must exactly match a resource name defined in the request&#39;s resources list. This creates a preference relationship between the job and the specified resource. | 
**Ranking** | Pointer to **NullableInt32** | Preference ranking score for this resource (1-100). Lower values indicate stronger preference - rank 1 is most preferred, rank 100 is least preferred. The solver will try to assign jobs to higher-ranked (lower-numbered) resources when possible, with the preference strength controlled by the rankingWeight in the weights configuration. | [optional] 

## Methods

### NewRanking

`func NewRanking(name string, ) *Ranking`

NewRanking instantiates a new Ranking object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRankingWithDefaults

`func NewRankingWithDefaults() *Ranking`

NewRankingWithDefaults instantiates a new Ranking object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *Ranking) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Ranking) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Ranking) SetName(v string)`

SetName sets Name field to given value.


### GetRanking

`func (o *Ranking) GetRanking() int32`

GetRanking returns the Ranking field if non-nil, zero value otherwise.

### GetRankingOk

`func (o *Ranking) GetRankingOk() (*int32, bool)`

GetRankingOk returns a tuple with the Ranking field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRanking

`func (o *Ranking) SetRanking(v int32)`

SetRanking sets Ranking field to given value.

### HasRanking

`func (o *Ranking) HasRanking() bool`

HasRanking returns a boolean if a field has been set.

### SetRankingNil

`func (o *Ranking) SetRankingNil(b bool)`

 SetRankingNil sets the value for Ranking to be an explicit nil

### UnsetRanking
`func (o *Ranking) UnsetRanking()`

UnsetRanking ensures that no value is present for Ranking, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


