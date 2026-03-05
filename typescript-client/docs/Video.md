
# Video


## Properties

Name | Type
------------ | -------------
`id` | string
`organization_id` | string
`title` | string
`description` | string
`status` | [VideoStatus](VideoStatus.md)
`duration_seconds` | number
`created_at` | Date
`updated_at` | Date

## Example

```typescript
import type { Video } from ''

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "organization_id": null,
  "title": null,
  "description": null,
  "status": null,
  "duration_seconds": null,
  "created_at": null,
  "updated_at": null,
} satisfies Video

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Video
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


