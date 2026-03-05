# VideosApi

All URIs are relative to *http://localhost:8080*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**completeVideoUpload**](VideosApi.md#completevideoupload) | **POST** /api/v1/videos/{videoId}/upload-complete | Mark upload complete |
| [**createVideo**](VideosApi.md#createvideooperation) | **POST** /api/v1/videos | Create video upload record |
| [**getVideo**](VideosApi.md#getvideo) | **GET** /api/v1/videos/{videoId} | Get video |
| [**getVideoPlay**](VideosApi.md#getvideoplay) | **GET** /api/v1/videos/{videoId}/play | Get short-lived playback authorization |



## completeVideoUpload

> completeVideoUpload(videoId)

Mark upload complete

### Example

```ts
import {
  Configuration,
  VideosApi,
} from '';
import type { CompleteVideoUploadRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new VideosApi(config);

  const body = {
    // string
    videoId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies CompleteVideoUploadRequest;

  try {
    const data = await api.completeVideoUpload(body);
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
| **videoId** | `string` |  | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **202** | Upload accepted for processing |  -  |
| **401** | Missing or invalid authentication |  -  |
| **404** | Resource not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## createVideo

> Video createVideo(createVideoRequest)

Create video upload record

### Example

```ts
import {
  Configuration,
  VideosApi,
} from '';
import type { CreateVideoOperationRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new VideosApi(config);

  const body = {
    // CreateVideoRequest
    createVideoRequest: ...,
  } satisfies CreateVideoOperationRequest;

  try {
    const data = await api.createVideo(body);
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
| **createVideoRequest** | [CreateVideoRequest](CreateVideoRequest.md) |  | |

### Return type

[**Video**](Video.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Video created |  -  |
| **400** | Validation or request shape error |  -  |
| **401** | Missing or invalid authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getVideo

> Video getVideo(videoId)

Get video

### Example

```ts
import {
  Configuration,
  VideosApi,
} from '';
import type { GetVideoRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new VideosApi(config);

  const body = {
    // string
    videoId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies GetVideoRequest;

  try {
    const data = await api.getVideo(body);
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
| **videoId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**Video**](Video.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Video |  -  |
| **401** | Missing or invalid authentication |  -  |
| **404** | Resource not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getVideoPlay

> VideoPlayResponse getVideoPlay(videoId)

Get short-lived playback authorization

### Example

```ts
import {
  Configuration,
  VideosApi,
} from '';
import type { GetVideoPlayRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new VideosApi(config);

  const body = {
    // string
    videoId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies GetVideoPlayRequest;

  try {
    const data = await api.getVideoPlay(body);
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
| **videoId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**VideoPlayResponse**](VideoPlayResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Playback authorization payload |  -  |
| **401** | Missing or invalid authentication |  -  |
| **404** | Resource not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

