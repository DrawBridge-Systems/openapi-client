
# PatchTrainingRequestRequest


## Properties

Name | Type
------------ | -------------
`status` | [TrainingRequestStatus](TrainingRequestStatus.md)
`notes` | string

## Example

```typescript
import type { PatchTrainingRequestRequest } from ''

// TODO: Update the object below with actual values
const example = {
  "status": null,
  "notes": null,
} satisfies PatchTrainingRequestRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PatchTrainingRequestRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


