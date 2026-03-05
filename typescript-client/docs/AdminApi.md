# AdminApi

All URIs are relative to *https://api.bridge.med*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createAdminUser**](AdminApi.md#createadminuseroperation) | **POST** /v1/admin/users | Create admin user |



## createAdminUser

> User createAdminUser(createAdminUserRequest)

Create admin user

### Example

```ts
import {
  Configuration,
  AdminApi,
} from '';
import type { CreateAdminUserOperationRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AdminApi(config);

  const body = {
    // CreateAdminUserRequest
    createAdminUserRequest: ...,
  } satisfies CreateAdminUserOperationRequest;

  try {
    const data = await api.createAdminUser(body);
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
| **createAdminUserRequest** | [CreateAdminUserRequest](CreateAdminUserRequest.md) |  | |

### Return type

[**User**](User.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Admin user created |  -  |
| **400** | Validation or request shape error |  -  |
| **401** | Missing or invalid authentication |  -  |
| **403** | Authenticated caller is not allowed to perform this action |  -  |
| **409** | Conflict with existing state |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

