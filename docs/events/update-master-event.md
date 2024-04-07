# `UpdateMasterEvent`

## Message

```ts
type UpdateMasterEvent = {
    type: 'updateMaster'
    master: 'room' | (string & {})
}
```

## Remarks

Upon receiving, client will:

-   Update master to `master`.
