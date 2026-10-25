# ItemInteractionUI

Namespace `C_ItemInteraction` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/iteminteractionuidocumentation.lua` (FileDataID 4637115)

## Functions

### ClearPendingItem

```lua
C_ItemInteraction.ClearPendingItem()
```

### CloseUI

```lua
C_ItemInteraction.CloseUI()
```

### GetChargeInfo

```lua
C_ItemInteraction.GetChargeInfo() -> chargeInfo: ItemInteractionChargeInfo
```

### GetItemConversionCurrencyCost

```lua
C_ItemInteraction.GetItemConversionCurrencyCost(item: ItemLocation) -> conversionCost: ConversionCurrencyCost
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `item` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### GetItemInteractionInfo

```lua
C_ItemInteraction.GetItemInteractionInfo() -> info: ItemInteractionFrameInfo?
```

### GetItemInteractionSpellId

```lua
C_ItemInteraction.GetItemInteractionSpellId() -> spellId: number
```

### InitializeFrame

```lua
C_ItemInteraction.InitializeFrame()
```

### PerformItemInteraction

```lua
C_ItemInteraction.PerformItemInteraction()
```

`HasRestrictions`

### Reset

```lua
C_ItemInteraction.Reset()
```

### SetPendingItem

```lua
C_ItemInteraction.SetPendingItem(item: ItemLocation?) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `item` | `ItemLocation?` | `Mixin=ItemLocationMixin` |

## Events

### ITEM_INTERACTION_CHARGE_INFO_UPDATED

```lua
ITEM_INTERACTION_CHARGE_INFO_UPDATED()
```

`SynchronousEvent`

### ITEM_INTERACTION_ITEM_SELECTION_UPDATED

```lua
ITEM_INTERACTION_ITEM_SELECTION_UPDATED(itemLocation: ItemLocation?)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation?` | `Mixin=ItemLocationMixin` |

## Types

### ConversionCurrencyCost

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `currencyID` | `number` |  |
| `amount` | `number` |  |

### ItemInteractionChargeInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `newChargeAmount` | `number` |  |
| `rechargeRate` | `number` |  |
| `timeToNextCharge` | `number` |  |

### ItemInteractionFrameInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `textureKit` | `textureKit` |  |
| `openSoundKitID` | `number` |  |
| `closeSoundKitID` | `number` |  |
| `titleText` | `string` |  |
| `tutorialText` | `string` |  |
| `buttonText` | `string` |  |
| `interactionType` | `UIItemInteractionType` |  |
| `flags` | `UIItemInteractionFlags` |  |
| `description` | `string?` |  |
| `buttonTooltip` | `string?` |  |
| `confirmationDescription` | `string?` |  |
| `slotTooltip` | `string?` |  |
| `cost` | `number?` |  |
| `currencyTypeId` | `number?` |  |
| `dropInSlotSoundKitId` | `number?` |  |
