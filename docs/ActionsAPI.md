# \ActionsAPI

All URIs are relative to *https://api.solvice.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**EvaluateVRP**](ActionsAPI.md#EvaluateVRP) | **Post** /v2/vrp/evaluate | Evaluate
[**SolveVRP**](ActionsAPI.md#SolveVRP) | **Post** /v2/vrp/solve | Solve
[**SuggestVRP**](ActionsAPI.md#SuggestVRP) | **Post** /v2/vrp/suggest | Suggest
[**SyncEvaluateVRP**](ActionsAPI.md#SyncEvaluateVRP) | **Post** /v2/vrp/sync/evaluate | Synchronous Evaluate
[**SyncSolveVRP**](ActionsAPI.md#SyncSolveVRP) | **Post** /v2/vrp/sync/solve | Synchronous Solve
[**SyncSuggestVRP**](ActionsAPI.md#SyncSuggestVRP) | **Post** /v2/vrp/sync/suggest | Synchronous Suggest



## EvaluateVRP

> SolviceStatusJob EvaluateVRP(ctx).OnRouteRequest(onRouteRequest).Execute()

Evaluate



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	onRouteRequest := *openapiclient.NewOnRouteRequest([]openapiclient.Resource{*openapiclient.NewResource("vehicle_1", []openapiclient.Shift{*openapiclient.NewShift("2023-01-13T08:00:00", "2023-01-13T16:00:00")})}, []openapiclient.Job{*openapiclient.NewJob("Job-1")}) // OnRouteRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ActionsAPI.EvaluateVRP(context.Background()).OnRouteRequest(onRouteRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ActionsAPI.EvaluateVRP``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EvaluateVRP`: SolviceStatusJob
	fmt.Fprintf(os.Stdout, "Response from `ActionsAPI.EvaluateVRP`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiEvaluateVRPRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **onRouteRequest** | [**OnRouteRequest**](OnRouteRequest.md) |  | 

### Return type

[**SolviceStatusJob**](SolviceStatusJob.md)

### Authorization

[apikey](../README.md#apikey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SolveVRP

> SolviceStatusJob SolveVRP(ctx).Millis(millis).Instance(instance).OnRouteRequest(onRouteRequest).Execute()

Solve



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	millis := "millis_example" // string |  (optional)
	instance := "instance_example" // string |  (optional)
	onRouteRequest := *openapiclient.NewOnRouteRequest([]openapiclient.Resource{*openapiclient.NewResource("vehicle_1", []openapiclient.Shift{*openapiclient.NewShift("2023-01-13T08:00:00", "2023-01-13T16:00:00")})}, []openapiclient.Job{*openapiclient.NewJob("Job-1")}) // OnRouteRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ActionsAPI.SolveVRP(context.Background()).Millis(millis).Instance(instance).OnRouteRequest(onRouteRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ActionsAPI.SolveVRP``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SolveVRP`: SolviceStatusJob
	fmt.Fprintf(os.Stdout, "Response from `ActionsAPI.SolveVRP`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSolveVRPRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **millis** | **string** |  | 
 **instance** | **string** |  | 
 **onRouteRequest** | [**OnRouteRequest**](OnRouteRequest.md) |  | 

### Return type

[**SolviceStatusJob**](SolviceStatusJob.md)

### Authorization

[apikey](../README.md#apikey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SuggestVRP

> SolviceStatusJob SuggestVRP(ctx).Millis(millis).OnRouteRequest(onRouteRequest).Execute()

Suggest



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	millis := "millis_example" // string |  (optional)
	onRouteRequest := *openapiclient.NewOnRouteRequest([]openapiclient.Resource{*openapiclient.NewResource("vehicle_1", []openapiclient.Shift{*openapiclient.NewShift("2023-01-13T08:00:00", "2023-01-13T16:00:00")})}, []openapiclient.Job{*openapiclient.NewJob("Job-1")}) // OnRouteRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ActionsAPI.SuggestVRP(context.Background()).Millis(millis).OnRouteRequest(onRouteRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ActionsAPI.SuggestVRP``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SuggestVRP`: SolviceStatusJob
	fmt.Fprintf(os.Stdout, "Response from `ActionsAPI.SuggestVRP`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSuggestVRPRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **millis** | **string** |  | 
 **onRouteRequest** | [**OnRouteRequest**](OnRouteRequest.md) |  | 

### Return type

[**SolviceStatusJob**](SolviceStatusJob.md)

### Authorization

[apikey](../README.md#apikey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SyncEvaluateVRP

> OnRouteResponse SyncEvaluateVRP(ctx).OnRouteRequest(onRouteRequest).Execute()

Synchronous Evaluate



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	onRouteRequest := *openapiclient.NewOnRouteRequest([]openapiclient.Resource{*openapiclient.NewResource("vehicle_1", []openapiclient.Shift{*openapiclient.NewShift("2023-01-13T08:00:00", "2023-01-13T16:00:00")})}, []openapiclient.Job{*openapiclient.NewJob("Job-1")}) // OnRouteRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ActionsAPI.SyncEvaluateVRP(context.Background()).OnRouteRequest(onRouteRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ActionsAPI.SyncEvaluateVRP``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SyncEvaluateVRP`: OnRouteResponse
	fmt.Fprintf(os.Stdout, "Response from `ActionsAPI.SyncEvaluateVRP`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSyncEvaluateVRPRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **onRouteRequest** | [**OnRouteRequest**](OnRouteRequest.md) |  | 

### Return type

[**OnRouteResponse**](OnRouteResponse.md)

### Authorization

[apikey](../README.md#apikey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SyncSolveVRP

> OnRouteResponse SyncSolveVRP(ctx).Millis(millis).OnRouteRequest(onRouteRequest).Execute()

Synchronous Solve



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	millis := "millis_example" // string |  (optional)
	onRouteRequest := *openapiclient.NewOnRouteRequest([]openapiclient.Resource{*openapiclient.NewResource("vehicle_1", []openapiclient.Shift{*openapiclient.NewShift("2023-01-13T08:00:00", "2023-01-13T16:00:00")})}, []openapiclient.Job{*openapiclient.NewJob("Job-1")}) // OnRouteRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ActionsAPI.SyncSolveVRP(context.Background()).Millis(millis).OnRouteRequest(onRouteRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ActionsAPI.SyncSolveVRP``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SyncSolveVRP`: OnRouteResponse
	fmt.Fprintf(os.Stdout, "Response from `ActionsAPI.SyncSolveVRP`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSyncSolveVRPRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **millis** | **string** |  | 
 **onRouteRequest** | [**OnRouteRequest**](OnRouteRequest.md) |  | 

### Return type

[**OnRouteResponse**](OnRouteResponse.md)

### Authorization

[apikey](../README.md#apikey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SyncSuggestVRP

> OnRouteResponse SyncSuggestVRP(ctx).Millis(millis).OnRouteRequest(onRouteRequest).Execute()

Synchronous Suggest



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	millis := "millis_example" // string |  (optional)
	onRouteRequest := *openapiclient.NewOnRouteRequest([]openapiclient.Resource{*openapiclient.NewResource("vehicle_1", []openapiclient.Shift{*openapiclient.NewShift("2023-01-13T08:00:00", "2023-01-13T16:00:00")})}, []openapiclient.Job{*openapiclient.NewJob("Job-1")}) // OnRouteRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ActionsAPI.SyncSuggestVRP(context.Background()).Millis(millis).OnRouteRequest(onRouteRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ActionsAPI.SyncSuggestVRP``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SyncSuggestVRP`: OnRouteResponse
	fmt.Fprintf(os.Stdout, "Response from `ActionsAPI.SyncSuggestVRP`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSyncSuggestVRPRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **millis** | **string** |  | 
 **onRouteRequest** | [**OnRouteRequest**](OnRouteRequest.md) |  | 

### Return type

[**OnRouteResponse**](OnRouteResponse.md)

### Authorization

[apikey](../README.md#apikey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

