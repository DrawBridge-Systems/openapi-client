
# RepAvailabilityWindow


## Properties

Name | Type
------------ | -------------
`id` | string
`rep_user_id` | string
`window_type` | [RepAvailabilityWindowType](RepAvailabilityWindowType.md)
`starts_at` | Date
`ends_at` | Date
`weekday` | number
`start_minute` | number
`end_minute` | number
`effective_from` | Date
`effective_until` | Date
`status` | [RepAvailabilityStatus](RepAvailabilityStatus.md)
`note` | string
`date_added` | Date
`date_updated` | Date

## Example

```typescript
import type { RepAvailabilityWindow } from ''

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "rep_user_id": null,
  "window_type": null,
  "starts_at": null,
  "ends_at": null,
  "weekday": null,
  "start_minute": null,
  "end_minute": null,
  "effective_from": null,
  "effective_until": null,
  "status": null,
  "note": null,
  "date_added": null,
  "date_updated": null,
} satisfies RepAvailabilityWindow

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RepAvailabilityWindow
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


