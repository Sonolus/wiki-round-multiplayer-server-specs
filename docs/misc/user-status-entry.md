# `UserStatusEntry`

Player status.

## Syntax

```ts
type UserStatusEntry = {
    userId: string
    status: UserStatus
}
```

## Remarks

Client will raise a fatal error if:

-   User of `userId` does not exist.
