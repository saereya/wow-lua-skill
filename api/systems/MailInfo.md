# MailInfo

Namespace `C_Mail` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/mailinfodocumentation.lua` (FileDataID 4637133)

## Functions

### CanCheckInbox

```lua
C_Mail.CanCheckInbox() -> canCheckInbox: bool, secondsUntilAllowed: number
```

### GetCraftingOrderMailInfo

```lua
C_Mail.GetCraftingOrderMailInfo(inboxIndex: luaIndex) -> info: CraftingOrderMailInfo?
```

`SecretArguments=AllowedWhenUntainted`

### HasInboxMoney

```lua
C_Mail.HasInboxMoney(inboxIndex: luaIndex) -> inboxItemHasMoneyAttached: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsCommandPending

```lua
C_Mail.IsCommandPending() -> isCommandPending: bool
```

### SetOpeningAll

```lua
C_Mail.SetOpeningAll(openingAll: bool)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### CLOSE_INBOX_ITEM

```lua
CLOSE_INBOX_ITEM(mailIndex: luaIndex)
```

`SynchronousEvent`

### MAIL_CLOSED

```lua
MAIL_CLOSED()
```

`SynchronousEvent`

### MAIL_FAILED

```lua
MAIL_FAILED(itemID: number?)
```

`SynchronousEvent`

### MAIL_INBOX_UPDATE

```lua
MAIL_INBOX_UPDATE()
```

`SynchronousEvent` `UniqueEvent`

### MAIL_LOCK_SEND_ITEMS

```lua
MAIL_LOCK_SEND_ITEMS(attachSlot: luaIndex, itemLink: cstring)
```

`SynchronousEvent`

### MAIL_OPEN_ALL_CANCELED

```lua
MAIL_OPEN_ALL_CANCELED()
```

`SynchronousEvent`

### MAIL_SEND_INFO_UPDATE

```lua
MAIL_SEND_INFO_UPDATE()
```

`SynchronousEvent` `UniqueEvent`

### MAIL_SEND_SUCCESS

```lua
MAIL_SEND_SUCCESS()
```

`SynchronousEvent`

### MAIL_SHOW

```lua
MAIL_SHOW()
```

`SynchronousEvent`

### MAIL_SUCCESS

```lua
MAIL_SUCCESS(itemID: number?)
```

`SynchronousEvent`

### MAIL_UNLOCK_SEND_ITEMS

```lua
MAIL_UNLOCK_SEND_ITEMS()
```

`SynchronousEvent`

### SEND_MAIL_COD_CHANGED

```lua
SEND_MAIL_COD_CHANGED()
```

`SynchronousEvent`

### SEND_MAIL_MONEY_CHANGED

```lua
SEND_MAIL_MONEY_CHANGED()
```

`SynchronousEvent`

### UPDATE_PENDING_MAIL

```lua
UPDATE_PENDING_MAIL()
```

`SynchronousEvent`
