# AzeriteEmpoweredItem

Namespace `C_AzeriteEmpoweredItem` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/azeriteempowereditemdocumentation.lua` (FileDataID 4637025)

## Functions

### CanSelectPower

```lua
C_AzeriteEmpoweredItem.CanSelectPower(azeriteEmpoweredItemLocation: AzeriteEmpoweredItemLocation, powerID: number) -> canSelect: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `azeriteEmpoweredItemLocation` | `AzeriteEmpoweredItemLocation` | `Mixin=ItemLocationMixin` |
| `powerID` | `number` |  |

### ConfirmAzeriteEmpoweredItemRespec

```lua
C_AzeriteEmpoweredItem.ConfirmAzeriteEmpoweredItemRespec(azeriteEmpoweredItemLocation: AzeriteEmpoweredItemLocation)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `azeriteEmpoweredItemLocation` | `AzeriteEmpoweredItemLocation` | `Mixin=ItemLocationMixin` |

### GetAllTierInfo

```lua
C_AzeriteEmpoweredItem.GetAllTierInfo(azeriteEmpoweredItemLocation: AzeriteEmpoweredItemLocation) -> tierInfo: AzeriteEmpoweredItemTierInfo[]
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `azeriteEmpoweredItemLocation` | `AzeriteEmpoweredItemLocation` | `Mixin=ItemLocationMixin` |

### GetAllTierInfoByItemID

```lua
C_AzeriteEmpoweredItem.GetAllTierInfoByItemID(itemInfo: ItemInfo, classID: number?) -> tierInfo: AzeriteEmpoweredItemTierInfo[]
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemInfo` | `ItemInfo` |  |
| `classID` | `number?` | Specify a class ID to get tier information about that class, otherwise uses the player's class if left nil |

### GetAzeriteEmpoweredItemRespecCost

```lua
C_AzeriteEmpoweredItem.GetAzeriteEmpoweredItemRespecCost() -> cost: number
```

### GetPowerInfo

```lua
C_AzeriteEmpoweredItem.GetPowerInfo(powerID: number) -> powerInfo: AzeriteEmpoweredItemPowerInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetPowerText

```lua
C_AzeriteEmpoweredItem.GetPowerText(azeriteEmpoweredItemLocation: AzeriteEmpoweredItemLocation, powerID: number, level: AzeritePowerLevel) -> powerText: AzeriteEmpoweredItemPowerText
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `azeriteEmpoweredItemLocation` | `AzeriteEmpoweredItemLocation` | `Mixin=ItemLocationMixin` |
| `powerID` | `number` |  |
| `level` | `AzeritePowerLevel` |  |

### GetSpecsForPower

```lua
C_AzeriteEmpoweredItem.GetSpecsForPower(powerID: number) -> specInfo: AzeriteSpecInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### HasAnyUnselectedPowers

```lua
C_AzeriteEmpoweredItem.HasAnyUnselectedPowers(azeriteEmpoweredItemLocation: AzeriteEmpoweredItemLocation) -> hasAnyUnselectedPowers: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `azeriteEmpoweredItemLocation` | `AzeriteEmpoweredItemLocation` | `Mixin=ItemLocationMixin` |

### HasBeenViewed

```lua
C_AzeriteEmpoweredItem.HasBeenViewed(azeriteEmpoweredItemLocation: AzeriteEmpoweredItemLocation) -> hasBeenViewed: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `azeriteEmpoweredItemLocation` | `AzeriteEmpoweredItemLocation` | `Mixin=ItemLocationMixin` |

### IsAzeriteEmpoweredItem

```lua
C_AzeriteEmpoweredItem.IsAzeriteEmpoweredItem(itemLocation: ItemLocation) -> isAzeriteEmpoweredItem: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### IsAzeriteEmpoweredItemByID

```lua
C_AzeriteEmpoweredItem.IsAzeriteEmpoweredItemByID(itemInfo: ItemInfo) -> isAzeriteEmpoweredItem: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsAzeritePreviewSourceDisplayable

```lua
C_AzeriteEmpoweredItem.IsAzeritePreviewSourceDisplayable(itemInfo: ItemInfo, classID: number?) -> isAzeritePreviewSourceDisplayable: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemInfo` | `ItemInfo` |  |
| `classID` | `number?` | Specify a class ID to determine if its displayable for that class, otherwise uses the player's class if left nil |

### IsHeartOfAzerothEquipped

```lua
C_AzeriteEmpoweredItem.IsHeartOfAzerothEquipped() -> isHeartOfAzerothEquipped: bool
```

### IsPowerAvailableForSpec

```lua
C_AzeriteEmpoweredItem.IsPowerAvailableForSpec(powerID: number, specID: number) -> isPowerAvailableForSpec: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsPowerSelected

```lua
C_AzeriteEmpoweredItem.IsPowerSelected(azeriteEmpoweredItemLocation: AzeriteEmpoweredItemLocation, powerID: number) -> isSelected: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `azeriteEmpoweredItemLocation` | `AzeriteEmpoweredItemLocation` | `Mixin=ItemLocationMixin` |
| `powerID` | `number` |  |

### SelectPower

```lua
C_AzeriteEmpoweredItem.SelectPower(azeriteEmpoweredItemLocation: AzeriteEmpoweredItemLocation, powerID: number) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `azeriteEmpoweredItemLocation` | `AzeriteEmpoweredItemLocation` | `Mixin=ItemLocationMixin` |
| `powerID` | `number` |  |

### SetHasBeenViewed

```lua
C_AzeriteEmpoweredItem.SetHasBeenViewed(azeriteEmpoweredItemLocation: AzeriteEmpoweredItemLocation)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `azeriteEmpoweredItemLocation` | `AzeriteEmpoweredItemLocation` | `Mixin=ItemLocationMixin` |

## Events

### AZERITE_EMPOWERED_ITEM_EQUIPPED_STATUS_CHANGED

```lua
AZERITE_EMPOWERED_ITEM_EQUIPPED_STATUS_CHANGED(isHeartEquipped: bool)
```

`SynchronousEvent`

### AZERITE_EMPOWERED_ITEM_SELECTION_UPDATED

```lua
AZERITE_EMPOWERED_ITEM_SELECTION_UPDATED(azeriteEmpoweredItemLocation: AzeriteEmpoweredItemLocation)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `azeriteEmpoweredItemLocation` | `AzeriteEmpoweredItemLocation` | `Mixin=ItemLocationMixin` |

## Types

### AzeritePowerLevel

*Enumeration* · 3 values, 0..2

Access values as `Enum.AzeritePowerLevel.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Base` | `AzeritePowerLevel` | = 0 |
| `Upgraded` | `AzeritePowerLevel` | = 1 |
| `Downgraded` | `AzeritePowerLevel` | = 2 |

### AzeriteEmpoweredItemPowerInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `azeritePowerID` | `number` |  |
| `spellID` | `number` |  |

### AzeriteEmpoweredItemPowerText

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `description` | `string` |  |

### AzeriteEmpoweredItemTierInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `azeritePowerIDs` | `number[]` |  |
| `unlockLevel` | `number` |  |

### AzeriteSpecInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `classID` | `number` |  |
| `specID` | `number` |  |
