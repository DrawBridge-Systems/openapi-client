
# RepAvailabilityProfile


## Properties

Name | Type
------------ | -------------
`rep_user_id` | string
`status` | [RepAvailabilityStatus](RepAvailabilityStatus.md)
`note` | string
`timezone` | string
`date_added` | Date
`date_updated` | Date
`effective_status` | [RepAvailabilityStatus](RepAvailabilityStatus.md)
`effective_note` | string
`effective_source` | string

## Example

```typescript
import type { RepAvailabilityProfile } from ''

// TODO: Update the object below with actual values
const example = {
  "rep_user_id": null,
  "status": null,
  "note": null,
  "timezone": null,
  "date_added": null,
  "date_updated": null,
  "effective_status": null,
  "effective_note": null,
  "effective_source": null,
} satisfies RepAvailabilityProfile

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RepAvailabilityProfile
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


