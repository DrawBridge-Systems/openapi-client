# MembershipsApi

All URIs are relative to *http://localhost:8080*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createOrganizationMembership**](MembershipsApi.md#createorganizationmembership) | **POST** /api/v1/organizations/{organizationId}/memberships | Add organization membership |
| [**listOrganizationMemberships**](MembershipsApi.md#listorganizationmemberships) | **GET** /api/v1/organizations/{organizationId}/memberships | List organization memberships |



## createOrganizationMembership

> Membership createOrganizationMembership(organizationId, createMembershipRequest)

Add organization membership

### Example

```ts
import {
  Configuration,
  MembershipsApi,
} from '';
import type { CreateOrganizationMembershipRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MembershipsApi(config);

  const body = {
    // string
    organizationId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // CreateMembershipRequest
    createMembershipRequest: ...,
  } satisfies CreateOrganizationMembershipRequest;

  try {
    const data = await api.createOrganizationMembership(body);
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
| **organizationId** | `string` |  | [Defaults to `undefined`] |
| **createMembershipRequest** | [CreateMembershipRequest](CreateMembershipRequest.md) |  | |

### Return type

[**Membership**](Membership.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Membership created |  -  |
| **400** | Validation or request shape error |  -  |
| **401** | Missing or invalid authentication |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listOrganizationMemberships

> ListMembershipsResponse listOrganizationMemberships(organizationId, membershipStatus)

List organization memberships

### Example

```ts
import {
  Configuration,
  MembershipsApi,
} from '';
import type { ListOrganizationMembershipsRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MembershipsApi(config);

  const body = {
    // string
    organizationId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // MembershipStatus (optional)
    membershipStatus: ...,
  } satisfies ListOrganizationMembershipsRequest;

  try {
    const data = await api.listOrganizationMemberships(body);
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
| **organizationId** | `string` |  | [Defaults to `undefined`] |
| **membershipStatus** | `MembershipStatus` |  | [Optional] [Defaults to `undefined`] [Enum: active, inactive, invited] |

### Return type

[**ListMembershipsResponse**](ListMembershipsResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Memberships |  -  |
| **401** | Missing or invalid authentication |  -  |
| **404** | Resource not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

