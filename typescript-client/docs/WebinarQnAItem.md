
# WebinarQnAItem


## Properties

Name | Type
------------ | -------------
`id` | string
`webinar_id` | string
`asked_by_user_id` | string
`question` | string
`answer` | string
`answered_by_user_id` | string
`status` | [WebinarQnAStatus](WebinarQnAStatus.md)
`answered_at` | Date
`date_added` | Date
`date_updated` | Date

## Example

```typescript
import type { WebinarQnAItem } from ''

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "webinar_id": null,
  "asked_by_user_id": null,
  "question": null,
  "answer": null,
  "answered_by_user_id": null,
  "status": null,
  "answered_at": null,
  "date_added": null,
  "date_updated": null,
} satisfies WebinarQnAItem

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WebinarQnAItem
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


