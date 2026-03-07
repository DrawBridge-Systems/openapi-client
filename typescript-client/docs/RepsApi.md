# RepsApi

All URIs are relative to *https://api.bridge.med*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**listRepAccounts**](RepsApi.md#listrepaccounts) | **GET** /v1/reps/accounts | List accounts supported by assigned rep products |
| [**listReps**](RepsApi.md#listreps) | **GET** /v1/reps/ | List representative directory entries |



## listRepAccounts

> Array&lt;RepAssignedAccount&gt; listRepAccounts(scope)

List accounts supported by assigned rep products

### Example

```ts
import {
  Configuration,
  RepsApi,
} from '';
import type { ListRepAccountsRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RepsApi(config);

  const body = {
    // 'assigned'
    scope: scope_example,
  } satisfies ListRepAccountsRequest;

  try {
    const data = await api.listRepAccounts(body);
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
| **scope** | `assigned` |  | [Defaults to `undefined`] [Enum: assigned] |

### Return type

[**Array&lt;RepAssignedAccount&gt;**](RepAssignedAccount.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Rep-supported accounts |  -  |
| **400** | Validation or request shape error |  -  |
| **401** | Missing or invalid authentication |  -  |
| **403** | Authenticated caller is not allowed to perform this action |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listReps

> Array&lt;RepDirectoryEntry&gt; listReps()

List representative directory entries

### Example

```ts
import {
  Configuration,
  RepsApi,
} from '';
import type { ListRepsRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RepsApi(config);

  try {
    const data = await api.listReps();
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

[**Array&lt;RepDirectoryEntry&gt;**](RepDirectoryEntry.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Representative directory entries |  -  |
| **400** | Validation or request shape error |  -  |
| **401** | Missing or invalid authentication |  -  |
| **403** | Authenticated caller is not allowed to perform this action |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

