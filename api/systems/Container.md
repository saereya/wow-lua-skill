# Container

Namespace `C_Container` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/containerdocumentation.lua` (FileDataID 4637075)

## Functions

### CalculateTotalNumberOfFreeBagSlots

```lua
C_Container.CalculateTotalNumberOfFreeBagSlots() -> totalFreeSlots: number
```

### ContainerIDToInventoryID

```lua
C_Container.ContainerIDToInventoryID(containerID: BagIndex) -> inventoryID: luaIndex
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### ContainerRefundItemPurchase

```lua
C_Container.ContainerRefundItemPurchase(containerIndex: BagIndex, slotIndex: luaIndex, isEquipped: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `containerIndex` | `BagIndex` |  |
| `slotIndex` | `luaIndex` |  |
| `isEquipped` | `bool` | default `false` |

### GetBackpackAutosortDisabled

```lua
C_Container.GetBackpackAutosortDisabled() -> isDisabled: bool
```

### GetBackpackSellJunkDisabled

```lua
C_Container.GetBackpackSellJunkDisabled() -> isDisabled: bool
```

### GetBagName

```lua
C_Container.GetBagName(bagIndex: BagIndex) -> name: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetBagSlotFlag

```lua
C_Container.GetBagSlotFlag(bagIndex: BagIndex, flag: BagSlotFlags) -> isSet: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetBankAutosortDisabled

```lua
C_Container.GetBankAutosortDisabled() -> isDisabled: bool
```

### GetContainerFreeSlots

```lua
C_Container.GetContainerFreeSlots(containerIndex: BagIndex) -> freeSlots: luaIndex[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetContainerItemCooldown

```lua
C_Container.GetContainerItemCooldown(containerIndex: BagIndex, slotIndex: luaIndex) -> startTime: number, duration: number, enable: number
```

`SecretArguments=AllowedWhenUntainted`

### GetContainerItemDurability

```lua
C_Container.GetContainerItemDurability(containerIndex: BagIndex, slotIndex: luaIndex) -> durability: number, maxDurability: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetContainerItemEquipmentSetInfo

```lua
C_Container.GetContainerItemEquipmentSetInfo(containerIndex: BagIndex, slotIndex: luaIndex) -> inSet: bool, setList: string
```

`SecretArguments=AllowedWhenUntainted`

### GetContainerItemID

```lua
C_Container.GetContainerItemID(containerIndex: BagIndex, slotIndex: luaIndex) -> containerID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetContainerItemInfo

```lua
C_Container.GetContainerItemInfo(containerIndex: BagIndex, slotIndex: luaIndex) -> containerInfo: ContainerItemInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetContainerItemLink

```lua
C_Container.GetContainerItemLink(containerIndex: BagIndex, slotIndex: luaIndex) -> itemLink: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetContainerItemPurchaseCurrency

```lua
C_Container.GetContainerItemPurchaseCurrency(containerIndex: BagIndex, slotIndex: luaIndex, itemIndex: luaIndex, isEquipped: bool) -> currencyInfo: ItemPurchaseCurrency
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetContainerItemPurchaseInfo

```lua
C_Container.GetContainerItemPurchaseInfo(containerIndex: BagIndex, slotIndex: luaIndex, isEquipped: bool) -> info: ItemPurchaseInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetContainerItemPurchaseItem

```lua
C_Container.GetContainerItemPurchaseItem(containerIndex: BagIndex, slotIndex: luaIndex, itemIndex: luaIndex, isEquipped: bool) -> itemInfo: ItemPurchaseItem
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetContainerItemQuestInfo

```lua
C_Container.GetContainerItemQuestInfo(containerIndex: BagIndex, slotIndex: luaIndex) -> questInfo: ItemQuestInfo
```

`SecretArguments=AllowedWhenUntainted`

### GetContainerNumFreeSlots

```lua
C_Container.GetContainerNumFreeSlots(bagIndex: BagIndex) -> numFreeSlots: number, bagFamily: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetContainerNumSlots

```lua
C_Container.GetContainerNumSlots(containerIndex: BagIndex) -> numSlots: number
```

`SecretArguments=AllowedWhenUntainted`

### GetInsertItemsLeftToRight

```lua
C_Container.GetInsertItemsLeftToRight() -> isEnabled: bool
```

### GetItemCooldown

```lua
C_Container.GetItemCooldown(itemID: number) -> startTime: number, duration: number, enable: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetMaxArenaCurrency

```lua
C_Container.GetMaxArenaCurrency() -> maxCurrency: number
```

### GetSortBagsRightToLeft

```lua
C_Container.GetSortBagsRightToLeft() -> isEnabled: bool
```

### HasContainerItem

```lua
C_Container.HasContainerItem(containerIndex: BagIndex, slotIndex: luaIndex) -> hasItem: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsBattlePayItem

```lua
C_Container.IsBattlePayItem(containerIndex: BagIndex, slotIndex: luaIndex) -> isBattlePayItem: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsContainerFiltered

```lua
C_Container.IsContainerFiltered(containerIndex: BagIndex) -> isFiltered: bool
```

`SecretArguments=AllowedWhenUntainted`

### PickupContainerItem

```lua
C_Container.PickupContainerItem(containerIndex: BagIndex, slotIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### PlayerHasHearthstone

```lua
C_Container.PlayerHasHearthstone() -> itemID: number?
```

### SetBackpackAutosortDisabled

```lua
C_Container.SetBackpackAutosortDisabled(disable: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetBackpackSellJunkDisabled

```lua
C_Container.SetBackpackSellJunkDisabled(disable: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetBagPortraitTexture

```lua
C_Container.SetBagPortraitTexture(texture: SimpleTexture, bagIndex: BagIndex)
```

`SecretArguments=AllowedWhenUntainted`

### SetBagSlotFlag

```lua
C_Container.SetBagSlotFlag(bagIndex: BagIndex, flag: BagSlotFlags, isSet: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetBankAutosortDisabled

```lua
C_Container.SetBankAutosortDisabled(disable: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetInsertItemsLeftToRight

```lua
C_Container.SetInsertItemsLeftToRight(enable: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetItemSearch

```lua
C_Container.SetItemSearch(searchString: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### SetSortBagsRightToLeft

```lua
C_Container.SetSortBagsRightToLeft(enable: bool)
```

`SecretArguments=AllowedWhenUntainted`

### ShowContainerSellCursor

```lua
C_Container.ShowContainerSellCursor(containerIndex: BagIndex, slotIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### SocketContainerItem

```lua
C_Container.SocketContainerItem(containerIndex: BagIndex, slotIndex: luaIndex) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### SortAccountBankBags

```lua
C_Container.SortAccountBankBags()
```

### SortBags

```lua
C_Container.SortBags()
```

### SortBank

```lua
C_Container.SortBank(bankType: BankType)
```

`SecretArguments=AllowedWhenUntainted`

### SortBankBags

```lua
C_Container.SortBankBags()
```

### SplitContainerItem

```lua
C_Container.SplitContainerItem(containerIndex: BagIndex, slotIndex: luaIndex, amount: number)
```

`SecretArguments=AllowedWhenUntainted`

### UseContainerItem

```lua
C_Container.UseContainerItem(containerIndex: BagIndex, slotIndex: luaIndex, unitToken: UnitToken?, bankType: BankType?, reagentBankOpen: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `containerIndex` | `BagIndex` |  |
| `slotIndex` | `luaIndex` |  |
| `unitToken` | `UnitToken?` |  |
| `bankType` | `BankType?` |  |
| `reagentBankOpen` | `bool` | default `false` |

### UseHearthstone

```lua
C_Container.UseHearthstone() -> used: bool
```

## Events

### BAG_CLOSED

```lua
BAG_CLOSED(bagID: BagIndex)
```

`SynchronousEvent`

### BAG_CONTAINER_UPDATE

```lua
BAG_CONTAINER_UPDATE()
```

`SynchronousEvent`

### BAG_NEW_ITEMS_UPDATED

```lua
BAG_NEW_ITEMS_UPDATED()
```

`SynchronousEvent`

### BAG_OPEN

```lua
BAG_OPEN(bagID: number)
```

`SynchronousEvent`

### BAG_OVERFLOW_WITH_FULL_INVENTORY

```lua
BAG_OVERFLOW_WITH_FULL_INVENTORY()
```

`SynchronousEvent`

### BAG_SLOT_FLAGS_UPDATED

```lua
BAG_SLOT_FLAGS_UPDATED(slot: number)
```

`SynchronousEvent`

### BAG_UPDATE

```lua
BAG_UPDATE(bagID: BagIndex)
```

`SynchronousEvent`

### BAG_UPDATE_COOLDOWN

```lua
BAG_UPDATE_COOLDOWN()
```

`UniqueEvent`

### BAG_UPDATE_DELAYED

```lua
BAG_UPDATE_DELAYED()
```

`UniqueEvent`

### EQUIP_BIND_REFUNDABLE_CONFIRM

```lua
EQUIP_BIND_REFUNDABLE_CONFIRM(slot: number, itemLocation: ItemLocation)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `slot` | `number` |  |
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### EQUIP_BIND_TRADEABLE_CONFIRM

```lua
EQUIP_BIND_TRADEABLE_CONFIRM(slot: number, itemLocation: ItemLocation)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `slot` | `number` |  |
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### EXPAND_BAG_BAR_CHANGED

```lua
EXPAND_BAG_BAR_CHANGED(expandBagBar: bool)
```

`SynchronousEvent`

### INVENTORY_SEARCH_UPDATE

```lua
INVENTORY_SEARCH_UPDATE()
```

`SynchronousEvent`

### ITEM_LOCK_CHANGED

```lua
ITEM_LOCK_CHANGED(bagOrSlotIndex: BagIndex, slotIndex: luaIndex?)
```

`SynchronousEvent`

### ITEM_LOCKED

```lua
ITEM_LOCKED(bagOrSlotIndex: BagIndex, slotIndex: luaIndex?)
```

`SynchronousEvent`

### ITEM_UNLOCKED

```lua
ITEM_UNLOCKED(bagOrSlotIndex: BagIndex, slotIndex: luaIndex?)
```

`SynchronousEvent`

### USE_COMBINED_BAGS_CHANGED

```lua
USE_COMBINED_BAGS_CHANGED(useCombinedBags: bool)
```

`SynchronousEvent`

## Types

### ContainerItemInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `iconFileID` | `fileID` |  |
| `stackCount` | `number` |  |
| `isLocked` | `bool` |  |
| `quality` | `ItemQuality?` |  |
| `isReadable` | `bool` |  |
| `hasLoot` | `bool` |  |
| `hyperlink` | `string` |  |
| `isFiltered` | `bool` |  |
| `hasNoValue` | `bool` |  |
| `itemID` | `number` |  |
| `isBound` | `bool` |  |
| `itemName` | `string` |  |

### ItemPurchaseCurrency

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `iconFileID` | `number?` |  |
| `currencyCount` | `number` |  |
| `name` | `cstring` |  |

### ItemPurchaseInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `money` | `WOWMONEY` |  |
| `itemCount` | `number` |  |
| `refundSeconds` | `time_t` |  |
| `currencyCount` | `number` |  |
| `hasEnchants` | `bool` |  |

### ItemPurchaseItem

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `iconFileID` | `number?` |  |
| `itemCount` | `number` |  |
| `hyperlink` | `string` |  |

### ItemQuestInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `isQuestItem` | `bool` |  |
| `questID` | `number?` |  |
| `isActive` | `bool` |  |
