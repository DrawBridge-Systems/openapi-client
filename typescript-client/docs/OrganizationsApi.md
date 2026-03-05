# OrganizationsApi

All URIs are relative to *https://api.bridge.med*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createOrganization**](OrganizationsApi.md#createorganizationoperation) | **POST** /v1/organizations | Create organization |
| [**createOrganizationRelation**](OrganizationsApi.md#createorganizationrelationoperation) | **POST** /v1/organizations/{id}/relations | Create organization relation |
| [**createOrganizationUser**](OrganizationsApi.md#createorganizationuseroperation) | **POST** /v1/organizations/{id}/users | Add user to organization |
| [**deleteOrganizationRelation**](OrganizationsApi.md#deleteorganizationrelation) | **DELETE** /v1/organizations/{id}/relations/{childOrganizationID} | Delete organization relation |
| [**deleteOrganizationUser**](OrganizationsApi.md#deleteorganizationuser) | **DELETE** /v1/organizations/{id}/users/{userID} | Remove user from organization |
| [**getOrganization**](OrganizationsApi.md#getorganization) | **GET** /v1/organizations/{id} | Get organization |
| [**listOrganizationRelations**](OrganizationsApi.md#listorganizationrelations) | **GET** /v1/organizations/{id}/relations | List organization relations |
| [**listOrganizationUsers**](OrganizationsApi.md#listorganizationusers) | **GET** /v1/organizations/{id}/users | List organization users |



## createOrganization

> Organization createOrganization(createOrganizationRequest)

Create organization

### Example

```ts
import {
  Configuration,
  OrganizationsApi,
} from '';
import type { CreateOrganizationOperationRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrganizationsApi(config);

  const body = {
    // CreateOrganizationRequest
    createOrganizationRequest: ...,
  } satisfies CreateOrganizationOperationRequest;

  try {
    const data = await api.createOrganization(body);
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
| **createOrganizationRequest** | [CreateOrganizationRequest](CreateOrganizationRequest.md) |  | |

### Return type

[**Organization**](Organization.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Organization created |  -  |
| **400** | Validation or request shape error |  -  |
| **401** | Missing or invalid authentication |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## createOrganizationRelation

> OrganizationRelation createOrganizationRelation(id, createOrganizationRelationRequest)

Create organization relation

### Example

```ts
import {
  Configuration,
  OrganizationsApi,
} from '';
import type { CreateOrganizationRelationOperationRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrganizationsApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // CreateOrganizationRelationRequest
    createOrganizationRelationRequest: ...,
  } satisfies CreateOrganizationRelationOperationRequest;

  try {
    const data = await api.createOrganizationRelation(body);
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
| **createOrganizationRelationRequest** | [CreateOrganizationRelationRequest](CreateOrganizationRelationRequest.md) |  | |

### Return type

[**OrganizationRelation**](OrganizationRelation.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Organization relation created |  -  |
| **400** | Validation or request shape error |  -  |
| **401** | Missing or invalid authentication |  -  |
| **404** | Resource not found |  -  |
| **409** | Conflict with existing state |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## createOrganizationUser

> OrganizationUser createOrganizationUser(id, createOrganizationUserRequest)

Add user to organization

### Example

```ts
import {
  Configuration,
  OrganizationsApi,
} from '';
import type { CreateOrganizationUserOperationRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrganizationsApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // CreateOrganizationUserRequest
    createOrganizationUserRequest: ...,
  } satisfies CreateOrganizationUserOperationRequest;

  try {
    const data = await api.createOrganizationUser(body);
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
| **createOrganizationUserRequest** | [CreateOrganizationUserRequest](CreateOrganizationUserRequest.md) |  | |

### Return type

[**OrganizationUser**](OrganizationUser.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Organization user created |  -  |
| **400** | Validation or request shape error |  -  |
| **401** | Missing or invalid authentication |  -  |
| **404** | Resource not found |  -  |
| **409** | Conflict with existing state |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteOrganizationRelation

> deleteOrganizationRelation(id, childOrganizationID)

Delete organization relation

### Example

```ts
import {
  Configuration,
  OrganizationsApi,
} from '';
import type { DeleteOrganizationRelationRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrganizationsApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // string
    childOrganizationID: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies DeleteOrganizationRelationRequest;

  try {
    const data = await api.deleteOrganizationRelation(body);
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
| **childOrganizationID** | `string` |  | [Defaults to `undefined`] |

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
| **204** | Organization relation removed |  -  |
| **400** | Validation or request shape error |  -  |
| **401** | Missing or invalid authentication |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteOrganizationUser

> deleteOrganizationUser(id, userID)

Remove user from organization

### Example

```ts
import {
  Configuration,
  OrganizationsApi,
} from '';
import type { DeleteOrganizationUserRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrganizationsApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // string
    userID: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies DeleteOrganizationUserRequest;

  try {
    const data = await api.deleteOrganizationUser(body);
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
| **userID** | `string` |  | [Defaults to `undefined`] |

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
| **204** | Organization user removed |  -  |
| **400** | Validation or request shape error |  -  |
| **401** | Missing or invalid authentication |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getOrganization

> Organization getOrganization(id)

Get organization

### Example

```ts
import {
  Configuration,
  OrganizationsApi,
} from '';
import type { GetOrganizationRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrganizationsApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies GetOrganizationRequest;

  try {
    const data = await api.getOrganization(body);
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

[**Organization**](Organization.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Organization |  -  |
| **400** | Validation or request shape error |  -  |
| **401** | Missing or invalid authentication |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listOrganizationRelations

> Array&lt;OrganizationRelation&gt; listOrganizationRelations(id)

List organization relations

### Example

```ts
import {
  Configuration,
  OrganizationsApi,
} from '';
import type { ListOrganizationRelationsRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrganizationsApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies ListOrganizationRelationsRequest;

  try {
    const data = await api.listOrganizationRelations(body);
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

[**Array&lt;OrganizationRelation&gt;**](OrganizationRelation.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Organization relations |  -  |
| **400** | Validation or request shape error |  -  |
| **401** | Missing or invalid authentication |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listOrganizationUsers

> Array&lt;OrganizationUser&gt; listOrganizationUsers(id)

List organization users

### Example

```ts
import {
  Configuration,
  OrganizationsApi,
} from '';
import type { ListOrganizationUsersRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new OrganizationsApi(config);

  const body = {
    // string
    id: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies ListOrganizationUsersRequest;

  try {
    const data = await api.listOrganizationUsers(body);
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

[**Array&lt;OrganizationUser&gt;**](OrganizationUser.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Organization users |  -  |
| **400** | Validation or request shape error |  -  |
| **401** | Missing or invalid authentication |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

