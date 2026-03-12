
# UpdateCatalogContentRequest


## Properties

Name | Type
------------ | -------------
`title` | string
`description` | string
`content_type` | [CatalogContentType](CatalogContentType.md)
`external_url` | string
`tags` | Array&lt;string&gt;
`product_id` | string

## Example

```typescript
import type { UpdateCatalogContentRequest } from ''

// TODO: Update the object below with actual values
const example = {
  "title": null,
  "description": null,
  "content_type": null,
  "external_url": null,
  "tags": null,
  "product_id": null,
} satisfies UpdateCatalogContentRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UpdateCatalogContentRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


