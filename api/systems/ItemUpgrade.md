# ItemUpgrade

Namespace `C_ItemUpgrade` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/itemupgradedocumentation.lua` (FileDataID 4637120)

## Functions

### CanUpgradeItem

```lua
C_ItemUpgrade.CanUpgradeItem(baseItem: ItemLocation) -> isValid: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `baseItem` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### ClearItemUpgrade

```lua
C_ItemUpgrade.ClearItemUpgrade()
```

### CloseItemUpgrade

```lua
C_ItemUpgrade.CloseItemUpgrade()
```

### GetHighWatermarkForItem

```lua
C_ItemUpgrade.GetHighWatermarkForItem(itemInfo: ItemInfo) -> characterHighWatermark: number, accountHighWatermark: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemInfo` | `ItemInfo` | Item ID, Link, or Name |

### GetHighWatermarkForSlot

```lua
C_ItemUpgrade.GetHighWatermarkForSlot(itemRedundancySlot: number) -> characterHighWatermark: number, accountHighWatermark: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemRedundancySlot` | `number` | Must be an Enum.ItemRedundancySlot value |

### GetHighWatermarkSlotForItem

```lua
C_ItemUpgrade.GetHighWatermarkSlotForItem(itemInfo: ItemInfo) -> itemRedundancySlot: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemInfo` | `ItemInfo` | Item ID, Link, or Name |

Returns:

| Name | Type | Notes |
|---|---|---|
| `itemRedundancySlot` | `number` | Enum.ItemRedundancySlot value |

### GetItemHyperlink

```lua
C_ItemUpgrade.GetItemHyperlink() -> link: cstring
```

`MayReturnNothing`

### GetItemUpgradeCurrentLevel

```lua
C_ItemUpgrade.GetItemUpgradeCurrentLevel() -> itemLevel: number, isPvpItemLevel: bool
```

`MayReturnNothing`

### GetItemUpgradeEffect

```lua
C_ItemUpgrade.GetItemUpgradeEffect(effectIndex: number, numUpgradeLevels: number?) -> outBaseEffect: string, outUpgradedEffect: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetItemUpgradeItemInfo

```lua
C_ItemUpgrade.GetItemUpgradeItemInfo() -> itemInfo: ItemUpgradeItemInfo
```

`MayReturnNothing`

### GetItemUpgradePvpItemLevelDeltaValues

```lua
C_ItemUpgrade.GetItemUpgradePvpItemLevelDeltaValues(numUpgradeLevels: number) -> currentPvPItemLevel: number, upgradedPvPItemLevel: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetNumItemUpgradeEffects

```lua
C_ItemUpgrade.GetNumItemUpgradeEffects() -> numItemUpgradeEffects: number
```

### IsItemBound

```lua
C_ItemUpgrade.IsItemBound() -> isBound: bool
```

### SetItemUpgradeFromCursorItem

```lua
C_ItemUpgrade.SetItemUpgradeFromCursorItem()
```

### SetItemUpgradeFromLocation

```lua
C_ItemUpgrade.SetItemUpgradeFromLocation(itemToSet: ItemLocation)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemToSet` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### UpgradeItem

```lua
C_ItemUpgrade.UpgradeItem(numUpgrades: number)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `numUpgrades` | `number` | default `1` |

## Events

### ITEM_UPGRADE_FAILED

```lua
ITEM_UPGRADE_FAILED()
```

`SynchronousEvent`

### ITEM_UPGRADE_MASTER_SET_ITEM

```lua
ITEM_UPGRADE_MASTER_SET_ITEM()
```

`SynchronousEvent`

### ITEM_UPGRADE_MASTER_UPDATE

```lua
ITEM_UPGRADE_MASTER_UPDATE()
```

`SynchronousEvent`

## Types

### ItemUpgradeCostDiscountInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `isDiscounted` | `bool` |  |
| `discountHighWatermark` | `number` |  |
| `isPartialTwoHandDiscount` | `bool` |  |
| `isAccountWideDiscount` | `bool` |  |
| `doesCurrentCharacterMeetHighWatermark` | `bool` | Reflects whether current character meets discount's high watermark, even if discount itself is account-wide |

### ItemUpgradeCurrencyCost

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `cost` | `number` |  |
| `currencyID` | `number` |  |
| `discountInfo` | `ItemUpgradeCostDiscountInfo` |  |

### ItemUpgradeItemCost

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `cost` | `number` |  |
| `itemID` | `number` |  |
| `discountInfo` | `ItemUpgradeCostDiscountInfo` |  |

### ItemUpgradeItemInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `iconID` | `number` |  |
| `name` | `string` |  |
| `itemUpgradeable` | `bool` |  |
| `displayQuality` | `number` |  |
| `highWatermarkSlot` | `number` |  |
| `currUpgrade` | `number` |  |
| `maxUpgrade` | `number` |  |
| `minItemLevel` | `number` |  |
| `maxItemLevel` | `number` |  |
| `upgradeLevelInfos` | `ItemUpgradeLevelInfo[]` |  |
| `customUpgradeString` | `string?` |  |
| `upgradeCostTypesForSeason` | `ItemUpgradeSeasonalCostType[]` |  |

### ItemUpgradeLevelInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `upgradeLevel` | `number` |  |
| `displayQuality` | `number` |  |
| `itemLevelIncrement` | `number` |  |
| `levelStats` | `ItemUpgradeStat[]` |  |
| `currencyCostsToUpgrade` | `ItemUpgradeCurrencyCost[]` |  |
| `itemCostsToUpgrade` | `ItemUpgradeItemCost[]` |  |
| `moneyCost` | `WOWMONEY?` |  |
| `failureMessage` | `string?` |  |

### ItemUpgradeSeasonalCostType

*Structure*

Costs are made up of either an Item OR a Currency, so either itemID or currencyID will be nil

Fields:

| Name | Type | Notes |
|---|---|---|
| `itemID` | `number?` |  |
| `currencyID` | `number?` |  |
| `orderIndex` | `number` |  |
| `sourceString` | `string?` |  |

### ItemUpgradeStat

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `displayString` | `string` |  |
| `statValue` | `number` |  |
| `active` | `bool` |  |
