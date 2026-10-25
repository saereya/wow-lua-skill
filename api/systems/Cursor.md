# Cursor

Namespace `C_Cursor` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/cursordocumentation.lua` (FileDataID 4637079)

## Functions

### GetCursorItem

```lua
C_Cursor.GetCursorItem() -> item: ItemLocation
```

`MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `item` | `ItemLocation` | `Mixin=ItemLocationMixin` |

## Events

### BATTLE_PET_CURSOR_CLEAR

```lua
BATTLE_PET_CURSOR_CLEAR()
```

`SynchronousEvent`

### CURSOR_CHANGED

```lua
CURSOR_CHANGED(isDefault: bool, newCursorType: UICursorType, oldCursorType: UICursorType, oldCursorVirtualID: number)
```

`SynchronousEvent`

### MOUNT_CURSOR_CLEAR

```lua
MOUNT_CURSOR_CLEAR()
```

`SynchronousEvent`

### WORLD_CURSOR_TOOLTIP_UPDATE

```lua
WORLD_CURSOR_TOOLTIP_UPDATE(anchorType: WorldCursorAnchorType)
```

Sends an update when the mouse enters or leaves something in-world (object, unit, etc) that should display a tooltip

`SynchronousEvent`
