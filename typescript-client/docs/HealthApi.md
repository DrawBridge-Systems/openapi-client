# HealthApi

All URIs are relative to *https://api.bridge.med*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getHealth**](HealthApi.md#gethealth) | **GET** /health/ | Health check |
| [**getHealthVersion**](HealthApi.md#gethealthversion) | **GET** /health/version | Build version info |
| [**pingHealth**](HealthApi.md#pinghealth) | **GET** /health/ping | Ping |



## getHealth

> HealthResponse getHealth()

Health check

### Example

```ts
import {
  Configuration,
  HealthApi,
} from '';
import type { GetHealthRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const api = new HealthApi();

  try {
    const data = await api.getHealth();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**HealthResponse**](HealthResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Service health |  -  |
| **503** | Service degraded |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getHealthVersion

> BuildInfo getHealthVersion()

Build version info

### Example

```ts
import {
  Configuration,
  HealthApi,
} from '';
import type { GetHealthVersionRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const api = new HealthApi();

  try {
    const data = await api.getHealthVersion();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**BuildInfo**](BuildInfo.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Build metadata |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## pingHealth

> string pingHealth()

Ping

### Example

```ts
import {
  Configuration,
  HealthApi,
} from '';
import type { PingHealthRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const api = new HealthApi();

  try {
    const data = await api.pingHealth();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `text/plain`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Pong text response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

