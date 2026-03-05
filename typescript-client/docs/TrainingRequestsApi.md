# TrainingRequestsApi

All URIs are relative to *http://localhost:8080*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createTrainingRequest**](TrainingRequestsApi.md#createtrainingrequestoperation) | **POST** /api/v1/training-requests | Create training request |
| [**getTrainingRequest**](TrainingRequestsApi.md#gettrainingrequest) | **GET** /api/v1/training-requests/{trainingRequestId} | Get training request |
| [**listTrainingRequests**](TrainingRequestsApi.md#listtrainingrequests) | **GET** /api/v1/training-requests | List training requests |
| [**patchTrainingRequest**](TrainingRequestsApi.md#patchtrainingrequestoperation) | **PATCH** /api/v1/training-requests/{trainingRequestId} | Update training request status |



## createTrainingRequest

> TrainingRequest createTrainingRequest(createTrainingRequestRequest)

Create training request

### Example

```ts
import {
  Configuration,
  TrainingRequestsApi,
} from '';
import type { CreateTrainingRequestOperationRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TrainingRequestsApi(config);

  const body = {
    // CreateTrainingRequestRequest
    createTrainingRequestRequest: ...,
  } satisfies CreateTrainingRequestOperationRequest;

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
| **createTrainingRequestRequest** | [CreateTrainingRequestRequest](CreateTrainingRequestRequest.md) |  | |

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

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTrainingRequest

> TrainingRequest getTrainingRequest(trainingRequestId)

Get training request

### Example

```ts
import {
  Configuration,
  TrainingRequestsApi,
} from '';
import type { GetTrainingRequestRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TrainingRequestsApi(config);

  const body = {
    // string
    trainingRequestId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies GetTrainingRequestRequest;

  try {
    const data = await api.getTrainingRequest(body);
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
| **trainingRequestId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**TrainingRequest**](TrainingRequest.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Training request |  -  |
| **401** | Missing or invalid authentication |  -  |
| **404** | Resource not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listTrainingRequests

> ListTrainingRequestsResponse listTrainingRequests(status, hospitalId, productId, page, pageSize)

List training requests

### Example

```ts
import {
  Configuration,
  TrainingRequestsApi,
} from '';
import type { ListTrainingRequestsRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TrainingRequestsApi(config);

  const body = {
    // TrainingRequestStatus (optional)
    status: ...,
    // string (optional)
    hospitalId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // string (optional)
    productId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // number (optional)
    page: 56,
    // number (optional)
    pageSize: 56,
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
| **status** | `TrainingRequestStatus` |  | [Optional] [Defaults to `undefined`] [Enum: submitted, acknowledged, scheduled, completed, canceled] |
| **hospitalId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **productId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **page** | `number` |  | [Optional] [Defaults to `1`] |
| **pageSize** | `number` |  | [Optional] [Defaults to `25`] |

### Return type

[**ListTrainingRequestsResponse**](ListTrainingRequestsResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Training requests |  -  |
| **401** | Missing or invalid authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## patchTrainingRequest

> TrainingRequest patchTrainingRequest(trainingRequestId, patchTrainingRequestRequest)

Update training request status

### Example

```ts
import {
  Configuration,
  TrainingRequestsApi,
} from '';
import type { PatchTrainingRequestOperationRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TrainingRequestsApi(config);

  const body = {
    // string
    trainingRequestId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // PatchTrainingRequestRequest
    patchTrainingRequestRequest: ...,
  } satisfies PatchTrainingRequestOperationRequest;

  try {
    const data = await api.patchTrainingRequest(body);
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
| **trainingRequestId** | `string` |  | [Defaults to `undefined`] |
| **patchTrainingRequestRequest** | [PatchTrainingRequestRequest](PatchTrainingRequestRequest.md) |  | |

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
| **404** | Resource not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

