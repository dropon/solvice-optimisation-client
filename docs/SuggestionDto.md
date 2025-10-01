# SuggestionDto

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Score** | [**Score**](Score.md) |  | 
**Assignments** | [**[]JobAssignment**](JobAssignment.md) |  | 

## Methods

### NewSuggestionDto

`func NewSuggestionDto(score Score, assignments []JobAssignment, ) *SuggestionDto`

NewSuggestionDto instantiates a new SuggestionDto object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSuggestionDtoWithDefaults

`func NewSuggestionDtoWithDefaults() *SuggestionDto`

NewSuggestionDtoWithDefaults instantiates a new SuggestionDto object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetScore

`func (o *SuggestionDto) GetScore() Score`

GetScore returns the Score field if non-nil, zero value otherwise.

### GetScoreOk

`func (o *SuggestionDto) GetScoreOk() (*Score, bool)`

GetScoreOk returns a tuple with the Score field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScore

`func (o *SuggestionDto) SetScore(v Score)`

SetScore sets Score field to given value.


### GetAssignments

`func (o *SuggestionDto) GetAssignments() []JobAssignment`

GetAssignments returns the Assignments field if non-nil, zero value otherwise.

### GetAssignmentsOk

`func (o *SuggestionDto) GetAssignmentsOk() (*[]JobAssignment, bool)`

GetAssignmentsOk returns a tuple with the Assignments field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAssignments

`func (o *SuggestionDto) SetAssignments(v []JobAssignment)`

SetAssignments sets Assignments field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


