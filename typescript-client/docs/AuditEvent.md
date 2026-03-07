
# AuditEvent


## Properties

Name | Type
------------ | -------------
`id` | string
`actor_user_id` | string
`tenant_id` | string
`organization_id` | string
`action` | string
`entity_type` | string
`entity_id` | string
`metadata` | { [key: string]: any; }
`date_added` | Date

## Example

```typescript
import type { AuditEvent } from ''

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "actor_user_id": null,
  "tenant_id": null,
  "organization_id": null,
  "action": null,
  "entity_type": null,
  "entity_id": null,
  "metadata": null,
  "date_added": null,
} satisfies AuditEvent

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AuditEvent
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


