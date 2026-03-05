# UsersApi

All URIs are relative to *https://api.bridge.med*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**acceptUserInvite**](UsersApi.md#acceptuserinvite) | **POST** /v1/users/invites/accept | Accept invite and create credentials |
| [**createUserInvite**](UsersApi.md#createuserinvite) | **POST** /v1/users/invites | Create user invite |
| [**getUserById**](UsersApi.md#getuserbyid) | **GET** /v1/users/{id} | Get user by id |



## acceptUserInvite

> User acceptUserInvite(acceptInviteRequest)

Accept invite and create credentials

### Example

```ts
import {
  Configuration,
  UsersApi,
} from '';
import type { AcceptUserInviteRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const api = new UsersApi();

  const body = {
    // AcceptInviteRequest
    acceptInviteRequest: ...,
  } satisfies AcceptUserInviteRequest;

  try {
    const data = await api.acceptUserInvite(body);
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
| **acceptInviteRequest** | [AcceptInviteRequest](AcceptInviteRequest.md) |  | |

### Return type

[**User**](User.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | User accepted invite |  -  |
| **400** | Validation or request shape error |  -  |
| **401** | Missing or invalid authentication |  -  |
| **409** | Conflict with existing state |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## createUserInvite

> CreateInviteResponse createUserInvite(createInviteRequest)

Create user invite

### Example

```ts
import {
  Configuration,
  UsersApi,
} from '';
import type { CreateUserInviteRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new UsersApi(config);

  const body = {
    // CreateInviteRequest
    createInviteRequest: ...,
  } satisfies CreateUserInviteRequest;

  try {
    const data = await api.createUserInvite(body);
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
| **createInviteRequest** | [CreateInviteRequest](CreateInviteRequest.md) |  | |

### Return type

[**CreateInviteResponse**](CreateInviteResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Invite created |  -  |
| **400** | Validation or request shape error |  -  |
| **401** | Missing or invalid authentication |  -  |
| **409** | Conflict with existing state |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getUserById

> User getUserById(id)

Get user by id

### Example

```ts
import {
  Configuration,
  UsersApi,
} from '';
import type { GetUserByIdRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new UsersApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies GetUserByIdRequest;

  try {
    const data = await api.getUserById(body);
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

### Return type

[**User**](User.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User |  -  |
| **400** | Validation or request shape error |  -  |
| **401** | Missing or invalid authentication |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

