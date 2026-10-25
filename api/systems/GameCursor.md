# GameCursor

Global functions · environment All · source `interface/addons/blizzard_apidocumentationgenerated/gamecursordocumentation.lua` (FileDataID 5555479)

## Functions

### ClearCursor

```lua
ClearCursor()
```

### ClearCursorHoveredItem

```lua
ClearCursorHoveredItem()
```

### CursorHasItem

```lua
CursorHasItem() -> result: bool
```

### CursorHasMacro

```lua
CursorHasMacro() -> result: bool
```

### CursorHasMoney

```lua
CursorHasMoney() -> result: bool
```

### CursorHasSpell

```lua
CursorHasSpell() -> result: bool
```

### DeleteCursorItem

```lua
DeleteCursorItem()
```

`HasRestrictions`

### DropCursorMoney

```lua
DropCursorMoney()
```

`HasRestrictions`

### EquipCursorItem

```lua
EquipCursorItem(slot: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### GetCursorInfo

```lua
GetCursorInfo()
```

### GetCursorMoney

```lua
GetCursorMoney() -> amount: number
```

### PickupPlayerMoney

```lua
PickupPlayerMoney(amount: WOWMONEY)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### ResetCursor

```lua
ResetCursor()
```

### SellCursorItem

```lua
SellCursorItem()
```

### SetCursor

```lua
SetCursor(name: cstring?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetCursorByMode

```lua
SetCursorByMode(mode: Cursormode) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetCursorHoveredItem

```lua
SetCursorHoveredItem(item: ItemLocation)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `item` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### SetCursorHoveredItemTradeItem

```lua
SetCursorHoveredItemTradeItem(enabled: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetCursorVirtualItem

```lua
SetCursorVirtualItem(itemInfo: ItemInfo, cursorType: UICursorType)
```

`SecretArguments=AllowedWhenUntainted`
