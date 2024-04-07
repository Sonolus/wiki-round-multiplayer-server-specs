# `UpdateOptionsEvent`

## Message

```ts
type UpdateOptionsEvent = {
    type: 'updateOptions'
    options: ServerOptionsSection[]
    optionValues: string
}
```

## Remarks

Upon receiving, client will:

-   Update options to `options`.
-   Update option values to `optionValues`.
