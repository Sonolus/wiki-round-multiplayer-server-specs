# `UpdateLeadEvent`

## Message

```ts
type UpdateLeadEvent = {
    type: 'updateLead'
    lead: 'room' | (string & {})
}
```

## Remarks

Upon receiving, client will:

-   Update lead to `lead`.
