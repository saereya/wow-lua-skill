# Flyout

Namespace `C_Flyout` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/flyoutdocumentation.lua` (FileDataID 8474100)

## Functions

### FlyoutHasSpell

```lua
C_Flyout.FlyoutHasSpell(flyoutID: number, spellID: number) -> hasSpell: bool
```

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

### GetFlyoutID

```lua
C_Flyout.GetFlyoutID(index: luaIndex) -> flyoutID: number
```

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

### GetFlyoutInfo

```lua
C_Flyout.GetFlyoutInfo(flyoutID: number) -> info: FlyoutInfo
```

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

### GetFlyoutSlotInfo

```lua
C_Flyout.GetFlyoutSlotInfo(flyoutID: number, slotIndex: luaIndex) -> slotInfo: FlyoutSlotInfo
```

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

### GetFlyoutTexture

```lua
C_Flyout.GetFlyoutTexture(flyoutID: number) -> textureID: fileID
```

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

### GetNumFlyouts

```lua
C_Flyout.GetNumFlyouts() -> numFlyouts: number
```

## Types

### FlyoutInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `description` | `string` |  |
| `numSlots` | `number` |  |
| `isKnown` | `bool` |  |

### FlyoutSlotInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `number` |  |
| `overrideSpellID` | `number` |  |
| `isKnown` | `bool` |  |
| `name` | `string?` |  |
| `specID` | `number?` |  |
