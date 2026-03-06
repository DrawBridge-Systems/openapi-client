# EventsApi

All URIs are relative to *https://api.bridge.med*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**listCalendarEvents**](EventsApi.md#listcalendarevents) | **GET** /v1/events/calendar | Unified calendar events |



## listCalendarEvents

> Array&lt;CalendarItem&gt; listCalendarEvents(start, end, scope, types)

Unified calendar events

### Example

```ts
import {
  Configuration,
  EventsApi,
} from '';
import type { ListCalendarEventsRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EventsApi(config);

  const body = {
    // Date (optional)
    start: 2013-10-20T19:20:30+01:00,
    // Date (optional)
    end: 2013-10-20T19:20:30+01:00,
    // CalendarScope (optional)
    scope: ...,
    // string | Comma-separated event source types (optional)
    types: types_example,
  } satisfies ListCalendarEventsRequest;

  try {
    const data = await api.listCalendarEvents(body);
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
| **start** | `Date` |  | [Optional] [Defaults to `undefined`] |
| **end** | `Date` |  | [Optional] [Defaults to `undefined`] |
| **scope** | `CalendarScope` |  | [Optional] [Defaults to `undefined`] [Enum: personal, org, hybrid] |
| **types** | `string` | Comma-separated event source types | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;CalendarItem&gt;**](CalendarItem.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Calendar events |  -  |
| **400** | Validation or request shape error |  -  |
| **401** | Missing or invalid authentication |  -  |
| **403** | Authenticated caller is not allowed to perform this action |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

