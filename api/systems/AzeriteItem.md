# AzeriteItem

Namespace `C_AzeriteItem` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/azeriteitemdocumentation.lua` (FileDataID 4637029)

## Functions

### FindActiveAzeriteItem

```lua
C_AzeriteItem.FindActiveAzeriteItem() -> activeAzeriteItemLocation: AzeriteItemLocation
```

`MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `activeAzeriteItemLocation` | `AzeriteItemLocation` | `Mixin=ItemLocationMixin` |

### GetAzeriteItemXPInfo

```lua
C_AzeriteItem.GetAzeriteItemXPInfo(azeriteItemLocation: AzeriteItemLocation) -> xp: number, totalLevelXP: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `azeriteItemLocation` | `AzeriteItemLocation` | `Mixin=ItemLocationMixin` |

### GetPowerLevel

```lua
C_AzeriteItem.GetPowerLevel(azeriteItemLocation: AzeriteItemLocation) -> powerLevel: number
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `azeriteItemLocation` | `AzeriteItemLocation` | `Mixin=ItemLocationMixin` |

### GetUnlimitedPowerLevel

```lua
C_AzeriteItem.GetUnlimitedPowerLevel(azeriteItemLocation: AzeriteItemLocation) -> powerLevel: number
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `azeriteItemLocation` | `AzeriteItemLocation` | `Mixin=ItemLocationMixin` |

### HasActiveAzeriteItem

```lua
C_AzeriteItem.HasActiveAzeriteItem() -> hasActiveAzeriteItem: bool
```

### IsAzeriteItem

```lua
C_AzeriteItem.IsAzeriteItem(itemLocation: ItemLocation) -> isAzeriteItem: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### IsAzeriteItemAtMaxLevel

```lua
C_AzeriteItem.IsAzeriteItemAtMaxLevel() -> isAtMax: bool
```

### IsAzeriteItemByID

```lua
C_AzeriteItem.IsAzeriteItemByID(itemInfo: ItemInfo) -> isAzeriteItem: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsAzeriteItemEnabled

```lua
C_AzeriteItem.IsAzeriteItemEnabled(azeriteItemLocation: AzeriteItemLocation) -> isEnabled: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `azeriteItemLocation` | `AzeriteItemLocation` | `Mixin=ItemLocationMixin` |

### IsUnlimitedLevelingUnlocked

```lua
C_AzeriteItem.IsUnlimitedLevelingUnlocked() -> isUnlimitedLevelingUnlocked: bool
```

## Events

### AZERITE_ITEM_ENABLED_STATE_CHANGED

```lua
AZERITE_ITEM_ENABLED_STATE_CHANGED(enabled: bool)
```

`SynchronousEvent`

### AZERITE_ITEM_EXPERIENCE_CHANGED

```lua
AZERITE_ITEM_EXPERIENCE_CHANGED(azeriteItemLocation: AzeriteItemLocation, oldExperienceAmount: number, newExperienceAmount: number)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `azeriteItemLocation` | `AzeriteItemLocation` | `Mixin=ItemLocationMixin` |
| `oldExperienceAmount` | `number` |  |
| `newExperienceAmount` | `number` |  |

### AZERITE_ITEM_POWER_LEVEL_CHANGED

```lua
AZERITE_ITEM_POWER_LEVEL_CHANGED(azeriteItemLocation: AzeriteItemLocation, oldPowerLevel: number, newPowerLevel: number, unlockedEmpoweredItemsInfo: UnlockedAzeriteEmpoweredItems[], azeriteItemID: number)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `azeriteItemLocation` | `AzeriteItemLocation` | `Mixin=ItemLocationMixin` |
| `oldPowerLevel` | `number` |  |
| `newPowerLevel` | `number` |  |
| `unlockedEmpoweredItemsInfo` | `UnlockedAzeriteEmpoweredItems[]` |  |
| `azeriteItemID` | `number` |  |

## Types

### UnlockedAzeriteEmpoweredItems

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `unlockedItem` | `AzeriteEmpoweredItemLocation` | `Mixin=ItemLocationMixin` |
| `tierIndex` | `luaIndex` |  |
