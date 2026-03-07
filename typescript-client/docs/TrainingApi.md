# TrainingApi

All URIs are relative to *https://api.bridge.med*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createTrainingRequest**](TrainingApi.md#createtrainingrequest) | **POST** /v1/training/requests/ | Create training request |
| [**listTrainingRequests**](TrainingApi.md#listtrainingrequests) | **GET** /v1/training/requests/ | List training requests |
| [**updateTrainingRequestStatus**](TrainingApi.md#updatetrainingrequeststatusoperation) | **PATCH** /v1/training/requests/{id} | Update training request status |



## createTrainingRequest

> TrainingRequest createTrainingRequest(createTrainingRequest)

Create training request

### Example

```ts
import {
  Configuration,
  TrainingApi,
} from '';
import type { CreateTrainingRequestRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TrainingApi(config);

  const body = {
    // CreateTrainingRequest
    createTrainingRequest: ...,
  } satisfies CreateTrainingRequestRequest;

  try {
    const data = await api.createTrainingRequest(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **createTrainingRequest** | [CreateTrainingRequest](CreateTrainingRequest.md) |  | |

### Return type

[**TrainingRequest**](TrainingRequest.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Training request created |  -  |
| **400** | Validation or request shape error |  -  |
| **401** | Missing or invalid authentication |  -  |
| **403** | Authenticated caller is not allowed to perform this action |  -  |
| **409** | Conflict with existing state |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listTrainingRequests

> Array&lt;TrainingRequest&gt; listTrainingRequests(organizationId, submittedByUserId, assignedUserId, statuses, scope)

List training requests

### Example

```ts
import {
  Configuration,
  TrainingApi,
} from '';
import type { ListTrainingRequestsRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TrainingApi(config);

  const body = {
    // string (optional)
    organizationId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // string (optional)
    submittedByUserId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // string (optional)
    assignedUserId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // string | Comma-separated training request statuses (optional)
    statuses: statuses_example,
    // 'assigned_products' (optional)
    scope: scope_example,
  } satisfies ListTrainingRequestsRequest;

  try {
    const data = await api.listTrainingRequests(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **organizationId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **submittedByUserId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **assignedUserId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **statuses** | `string` | Comma-separated training request statuses | [Optional] [Defaults to `undefined`] |
| **scope** | `assigned_products` |  | [Optional] [Defaults to `undefined`] [Enum: assigned_products] |

### Return type

[**Array&lt;TrainingRequest&gt;**](TrainingRequest.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Training requests |  -  |
| **400** | Validation or request shape error |  -  |
| **401** | Missing or invalid authentication |  -  |
| **403** | Authenticated caller is not allowed to perform this action |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateTrainingRequestStatus

> TrainingRequest updateTrainingRequestStatus(id, updateTrainingRequestStatusRequest)

Update training request status

### Example

```ts
import {
  Configuration,
  TrainingApi,
} from '';
import type { UpdateTrainingRequestStatusOperationRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TrainingApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // UpdateTrainingRequestStatusRequest
    updateTrainingRequestStatusRequest: ...,
  } satisfies UpdateTrainingRequestStatusOperationRequest;

  try {
    const data = await api.updateTrainingRequestStatus(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | `string` |  | [Defaults to `undefined`] |
| **updateTrainingRequestStatusRequest** | [UpdateTrainingRequestStatusRequest](UpdateTrainingRequestStatusRequest.md) |  | |

### Return type

[**TrainingRequest**](TrainingRequest.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Training request updated |  -  |
| **400** | Validation or request shape error |  -  |
| **401** | Missing or invalid authentication |  -  |
| **403** | Authenticated caller is not allowed to perform this action |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

