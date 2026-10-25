# PerksProgram

Namespace `C_PerksProgram` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/perksprogramdocumentation.lua` (FileDataID 4637818)

## Functions

### ClearFrozenPerksVendorItem

```lua
C_PerksProgram.ClearFrozenPerksVendorItem()
```

### CloseInteraction

```lua
C_PerksProgram.CloseInteraction()
```

### GetAvailableCategoryIDs

```lua
C_PerksProgram.GetAvailableCategoryIDs() -> categoryIDs: number[]
```

### GetAvailableVendorItemIDs

```lua
C_PerksProgram.GetAvailableVendorItemIDs() -> vendorItemIDs: number[]
```

### GetCategoryInfo

```lua
C_PerksProgram.GetCategoryInfo(categoryID: number) -> categoryInfo: PerksVendorCategoryInfo
```

`SecretArguments=AllowedWhenUntainted`

### GetCurrencyAmount

```lua
C_PerksProgram.GetCurrencyAmount() -> currencyAmount: number
```

### GetDraggedPerksVendorItem

```lua
C_PerksProgram.GetDraggedPerksVendorItem() -> perksVendorItemID: number
```

### GetFrozenPerksVendorItemInfo

```lua
C_PerksProgram.GetFrozenPerksVendorItemInfo() -> vendorItemInfo: PerksVendorItemInfo
```

`MayReturnNothing`

### GetPendingChestRewards

```lua
C_PerksProgram.GetPendingChestRewards() -> pendingRewards: PerksProgramPendingChestRewards[]
```

### GetPerksProgramItemDisplayInfo

```lua
C_PerksProgram.GetPerksProgramItemDisplayInfo(id: number) -> item: PerksProgramItemDisplayInfo
```

`SecretArguments=AllowedWhenUntainted`

### GetTimeRemaining

```lua
C_PerksProgram.GetTimeRemaining(vendorItemID: number) -> timeRemaining: time_t
```

`SecretArguments=AllowedWhenUntainted`

### GetVendorItemInfo

```lua
C_PerksProgram.GetVendorItemInfo(vendorItemID: number) -> vendorItemInfo: PerksVendorItemInfo
```

`SecretArguments=AllowedWhenUntainted`

### GetVendorItemInfoRefundTimeLeft

```lua
C_PerksProgram.GetVendorItemInfoRefundTimeLeft(vendorItemID: number) -> refundTimeRemaining: time_t
```

`SecretArguments=AllowedWhenUntainted`

### IsAttackAnimToggleEnabled

```lua
C_PerksProgram.IsAttackAnimToggleEnabled() -> isAttackAnimToggleEnabled: bool
```

### IsFrozenPerksVendorItem

```lua
C_PerksProgram.IsFrozenPerksVendorItem(perksVendorItemID: number) -> isFrozen: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsMountSpecialAnimToggleEnabled

```lua
C_PerksProgram.IsMountSpecialAnimToggleEnabled() -> isMountSpecialAnimToggleEnabled: bool
```

### ItemSelectedTelemetry

```lua
C_PerksProgram.ItemSelectedTelemetry(perksVendorItemID: number)
```

`SecretArguments=AllowedWhenUntainted`

### PickupPerksVendorItem

```lua
C_PerksProgram.PickupPerksVendorItem(perksVendorItemID: number)
```

`SecretArguments=AllowedWhenUntainted`

### RequestCartCheckout

```lua
C_PerksProgram.RequestCartCheckout(perksVendorItemIDs: number[])
```

`SecretArguments=AllowedWhenUntainted`

### RequestPendingChestRewards

```lua
C_PerksProgram.RequestPendingChestRewards()
```

### RequestPurchase

```lua
C_PerksProgram.RequestPurchase(perksVendorItemID: number)
```

`SecretArguments=AllowedWhenUntainted`

### RequestRefund

```lua
C_PerksProgram.RequestRefund(perksVendorItemID: number)
```

`SecretArguments=AllowedWhenUntainted`

### ResetHeldItemDragAndDrop

```lua
C_PerksProgram.ResetHeldItemDragAndDrop()
```

### SetFrozenPerksVendorItem

```lua
C_PerksProgram.SetFrozenPerksVendorItem()
```

## Events

### CHEST_REWARDS_UPDATED_FROM_SERVER

```lua
CHEST_REWARDS_UPDATED_FROM_SERVER()
```

`SynchronousEvent`

### PERKS_PROGRAM_ADD_PENDING_SHOP_ITEM

```lua
PERKS_PROGRAM_ADD_PENDING_SHOP_ITEM(vendorItemID: number)
```

`SynchronousEvent`

### PERKS_PROGRAM_CLOSE

```lua
PERKS_PROGRAM_CLOSE()
```

`SynchronousEvent`

### PERKS_PROGRAM_CURRENCY_AWARDED

```lua
PERKS_PROGRAM_CURRENCY_AWARDED(value: number)
```

`SynchronousEvent`

### PERKS_PROGRAM_CURRENCY_REFRESH

```lua
PERKS_PROGRAM_CURRENCY_REFRESH(oldValue: number, newValue: number)
```

`SynchronousEvent`

### PERKS_PROGRAM_DATA_REFRESH

```lua
PERKS_PROGRAM_DATA_REFRESH()
```

`SynchronousEvent`

### PERKS_PROGRAM_DATA_SPECIFIC_ITEM_REFRESH

```lua
PERKS_PROGRAM_DATA_SPECIFIC_ITEM_REFRESH(vendorItemID: number)
```

`SynchronousEvent`

### PERKS_PROGRAM_DISABLED

```lua
PERKS_PROGRAM_DISABLED()
```

`SynchronousEvent`

### PERKS_PROGRAM_OPEN

```lua
PERKS_PROGRAM_OPEN()
```

`SynchronousEvent`

### PERKS_PROGRAM_PURCHASE_CART_SUCCESS

```lua
PERKS_PROGRAM_PURCHASE_CART_SUCCESS(vendorItemIDs: number[])
```

`SynchronousEvent`

### PERKS_PROGRAM_PURCHASE_SUCCESS

```lua
PERKS_PROGRAM_PURCHASE_SUCCESS(vendorItemID: number)
```

`SynchronousEvent`

### PERKS_PROGRAM_REFUND_SUCCESS

```lua
PERKS_PROGRAM_REFUND_SUCCESS(vendorItemID: number)
```

`SynchronousEvent`

### PERKS_PROGRAM_REMOVE_PENDING_SHOP_ITEM

```lua
PERKS_PROGRAM_REMOVE_PENDING_SHOP_ITEM(vendorItemID: number)
```

`SynchronousEvent`

### PERKS_PROGRAM_RESULT_ERROR

```lua
PERKS_PROGRAM_RESULT_ERROR()
```

`SynchronousEvent`

### PERKS_PROGRAM_SET_FROZEN_ITEM

```lua
PERKS_PROGRAM_SET_FROZEN_ITEM(vendorItemID: number)
```

`SynchronousEvent`

## Types

### PerksProgramItemDisplayInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `overrideModelSceneID` | `number?` |  |
| `creatureDisplayInfoID` | `number?` |  |
| `mainHandItemModifiedAppearanceID` | `number?` |  |
| `offHandItemModifiedAppearanceID` | `number?` |  |

### PerksProgramPendingChestRewards

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `rewardTypeID` | `number` |  |
| `perksVendorItemID` | `number?` |  |
| `rewardAmount` | `number` |  |
| `monthRewarded` | `string?` |  |
| `activityMonthID` | `number` |  |
| `thresholdOrderIndex` | `number` |  |

### PerksVendorCategoryInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ID` | `number` |  |
| `displayName` | `cstring` |  |
| `defaultUIModelSceneID` | `number` |  |

### PerksVendorItemInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `perksVendorCategoryID` | `number` |  |
| `description` | `string` |  |
| `timeRemaining` | `time_t` |  |
| `purchased` | `bool` |  |
| `refundable` | `bool` |  |
| `subItemsLoaded` | `bool` |  |
| `isPurchasePending` | `bool` |  |
| `doesNotExpire` | `bool` |  |
| `price` | `number` |  |
| `originalPrice` | `number?` |  |
| `showSaleBanner` | `bool` |  |
| `perksVendorItemID` | `number` |  |
| `itemID` | `number` |  |
| `iconTexture` | `string` |  |
| `mountID` | `number` |  |
| `mountTypeName` | `string` |  |
| `speciesID` | `number` |  |
| `transmogSetID` | `number` |  |
| `itemModifiedAppearanceID` | `number` |  |
| `subItems` | `PerksVendorSubItemInfo[]` |  |
| `uiGroupInfo` | `PerksVendorItemUIGroupInfo?` |  |
| `invType` | `string` |  |
| `quality` | `ItemQuality` |  |

### PerksVendorItemUIGroupInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ID` | `number` |  |
| `name` | `cstring` |  |
| `priority` | `number` |  |

### PerksVendorSubItemInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `itemID` | `number` |  |
| `itemModifiedAppearanceID` | `number` |  |
| `invType` | `string` |  |
| `quality` | `ItemQuality` |  |
