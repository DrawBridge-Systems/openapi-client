# RepCoverageApi

All URIs are relative to *http://localhost:8080*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createRepCoverage**](RepCoverageApi.md#createrepcoverageoperation) | **POST** /api/v1/rep-coverages | Create rep coverage |
| [**listRepCoverages**](RepCoverageApi.md#listrepcoverages) | **GET** /api/v1/rep-coverages | List rep coverages |



## createRepCoverage

> RepCoverage createRepCoverage(createRepCoverageRequest)

Create rep coverage

### Example

```ts
import {
  Configuration,
  RepCoverageApi,
} from '';
import type { CreateRepCoverageOperationRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RepCoverageApi(config);

  const body = {
    // CreateRepCoverageRequest
    createRepCoverageRequest: ...,
  } satisfies CreateRepCoverageOperationRequest;

  try {
    const data = await api.createRepCoverage(body);
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
| **createRepCoverageRequest** | [CreateRepCoverageRequest](CreateRepCoverageRequest.md) |  | |

### Return type

[**RepCoverage**](RepCoverage.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Coverage created |  -  |
| **400** | Validation or request shape error |  -  |
| **401** | Missing or invalid authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listRepCoverages

> ListRepCoveragesResponse listRepCoverages(repUserId, hospitalId, status)

List rep coverages

### Example

```ts
import {
  Configuration,
  RepCoverageApi,
} from '';
import type { ListRepCoveragesRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RepCoverageApi(config);

  const body = {
    // string (optional)
    repUserId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // string (optional)
    hospitalId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // CoverageStatus (optional)
    status: ...,
  } satisfies ListRepCoveragesRequest;

  try {
    const data = await api.listRepCoverages(body);
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
| **repUserId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **hospitalId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **status** | `CoverageStatus` |  | [Optional] [Defaults to `undefined`] [Enum: active, inactive] |

### Return type

[**ListRepCoveragesResponse**](ListRepCoveragesResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Coverage records |  -  |
| **401** | Missing or invalid authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

