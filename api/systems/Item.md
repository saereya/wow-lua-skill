# Item

Namespace `C_Item` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/itemdocumentation.lua` (FileDataID 4637136)

## Functions

### ActionBindsItem

```lua
C_Item.ActionBindsItem()
```

### BindEnchant

```lua
C_Item.BindEnchant()
```

### CanBeRefunded

```lua
C_Item.CanBeRefunded(itemLocation: ItemLocation) -> canBeRefunded: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### CanItemTransmogAppearance

```lua
C_Item.CanItemTransmogAppearance(itemLoc: ItemLocation) -> canTransmog: bool, errorCode: TransmogOutfitSlotError
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLoc` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### CanScrapItem

```lua
C_Item.CanScrapItem(itemLoc: ItemLocation) -> canBeScrapped: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLoc` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### CanViewItemPowers

```lua
C_Item.CanViewItemPowers(itemLoc: ItemLocation) -> isItemViewable: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLoc` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### ConfirmBindOnUse

```lua
C_Item.ConfirmBindOnUse()
```

### ConfirmDeleteItem

```lua
C_Item.ConfirmDeleteItem(itemGUID: WOWGUID)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### ConfirmNoRefundOnUse

```lua
C_Item.ConfirmNoRefundOnUse()
```

### ConfirmOnUse

```lua
C_Item.ConfirmOnUse()
```

### DeleteItem

```lua
C_Item.DeleteItem(itemGUID: WOWGUID)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### DoesItemContainSpec

```lua
C_Item.DoesItemContainSpec(itemInfo: ItemInfo, classID: number, specID: number) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemInfo` | `ItemInfo` |  |
| `classID` | `number` |  |
| `specID` | `number` | default `0` |

### DoesItemExist

```lua
C_Item.DoesItemExist(emptiableItemLocation: EmptiableItemLocation) -> itemExists: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `emptiableItemLocation` | `EmptiableItemLocation` | `Mixin=ItemLocationMixin` |

### DoesItemExistByID

```lua
C_Item.DoesItemExistByID(itemInfo: ItemInfo) -> itemExists: bool
```

`SecretArguments=AllowedWhenUntainted`

### DoesItemMatchBonusTreeReplacement

```lua
C_Item.DoesItemMatchBonusTreeReplacement(itemLoc: ItemLocation) -> matchesBonusTree: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLoc` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### DoesItemMatchSpellItemCondition

```lua
C_Item.DoesItemMatchSpellItemCondition(itemLoc: ItemLocation) -> matches: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLoc` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### DoesItemMatchTargetEnchantingSpell

```lua
C_Item.DoesItemMatchTargetEnchantingSpell(itemLoc: ItemLocation) -> matchesTargetEnchantingSpell: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLoc` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### DoesItemMatchTrackJump

```lua
C_Item.DoesItemMatchTrackJump(itemLoc: ItemLocation) -> matchesTrackJump: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLoc` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### DropItemOnUnit

```lua
C_Item.DropItemOnUnit(unitGUID: UnitToken)
```

`SecretArguments=AllowedWhenUntainted`

### EndBoundTradeable

```lua
C_Item.EndBoundTradeable(type: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### EndRefund

```lua
C_Item.EndRefund(type: number)
```

`SecretArguments=AllowedWhenUntainted`

### EquipItemByName

```lua
C_Item.EquipItemByName(itemInfo: ItemInfo, dstSlot: luaIndex?)
```

`SecretArguments=AllowedWhenUntainted`

### GetAppliedItemTransmogInfo

```lua
C_Item.GetAppliedItemTransmogInfo(itemLoc: ItemLocation) -> info: ItemTransmogInfo?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLoc` | `ItemLocation` | `Mixin=ItemLocationMixin` |

Returns:

| Name | Type | Notes |
|---|---|---|
| `info` | `ItemTransmogInfo?` | `Mixin=ItemTransmogInfoMixin` |

### GetBaseItemTransmogInfo

```lua
C_Item.GetBaseItemTransmogInfo(itemLoc: ItemLocation) -> info: ItemTransmogInfo?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLoc` | `ItemLocation` | `Mixin=ItemLocationMixin` |

Returns:

| Name | Type | Notes |
|---|---|---|
| `info` | `ItemTransmogInfo?` | `Mixin=ItemTransmogInfoMixin` |

### GetCurrentItemLevel

```lua
C_Item.GetCurrentItemLevel(itemLocation: ItemLocation) -> currentItemLevel: number?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### GetCurrentItemTransmogInfo

```lua
C_Item.GetCurrentItemTransmogInfo(itemLoc: ItemLocation) -> info: ItemTransmogInfo?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLoc` | `ItemLocation` | `Mixin=ItemLocationMixin` |

Returns:

| Name | Type | Notes |
|---|---|---|
| `info` | `ItemTransmogInfo?` | `Mixin=ItemTransmogInfoMixin` |

### GetDelvePreviewItemLink

```lua
C_Item.GetDelvePreviewItemLink(itemID: number, context: ItemCreationContext) -> itemLink: string?
```

`SecretArguments=AllowedWhenUntainted`

### GetDelvePreviewItemQuality

```lua
C_Item.GetDelvePreviewItemQuality(itemID: number, context: ItemCreationContext) -> itemQuality: ItemQuality
```

`SecretArguments=AllowedWhenUntainted`

### GetDetailedItemLevelInfo

```lua
C_Item.GetDetailedItemLevelInfo(itemInfo: ItemInfo) -> actualItemLevel: number, previewLevel: bool, sparseItemLevel: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetFirstTriggeredSpellForItem

```lua
C_Item.GetFirstTriggeredSpellForItem(itemID: number, itemQuality: number) -> spellID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetItemChildInfo

```lua
C_Item.GetItemChildInfo(itemInfo: ItemInfo, slotID: luaIndex?) -> result: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetItemClassInfo

```lua
C_Item.GetItemClassInfo(itemClassID: number) -> result: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetItemConversionOutputIcon

```lua
C_Item.GetItemConversionOutputIcon(itemLoc: ItemLocation) -> icon: fileID?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLoc` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### GetItemCooldown

```lua
C_Item.GetItemCooldown(itemInfo: ItemInfo) -> startTimeSeconds: number, durationSeconds: number, enableCooldownTimer: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetItemCount

```lua
C_Item.GetItemCount(itemInfo: ItemInfo, includeBank: bool, includeUses: bool, includeReagentBank: bool, includeAccountBank: bool) -> count: number
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemInfo` | `ItemInfo` |  |
| `includeBank` | `bool` | default `false` |
| `includeUses` | `bool` | default `false` |
| `includeReagentBank` | `bool` | default `false` |
| `includeAccountBank` | `bool` | default `false` |

### GetItemCreationContext

```lua
C_Item.GetItemCreationContext(itemInfo: ItemInfo) -> itemID: number, creationContext: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetItemFamily

```lua
C_Item.GetItemFamily(itemInfo: ItemInfo) -> result: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetItemGem

```lua
C_Item.GetItemGem(hyperlink: cstring, index: luaIndex) -> gemName: string, gemLink: cstring
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetItemGemID

```lua
C_Item.GetItemGemID(itemInfo: ItemInfo, index: luaIndex) -> gemID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetItemGUID

```lua
C_Item.GetItemGUID(itemLocation: ItemLocation) -> itemGUID: WOWGUID
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### GetItemIcon

```lua
C_Item.GetItemIcon(itemLocation: ItemLocation) -> icon: fileID?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### GetItemIconByID

```lua
C_Item.GetItemIconByID(itemInfo: ItemInfo) -> icon: fileID?
```

`SecretArguments=AllowedWhenUntainted`

### GetItemID

```lua
C_Item.GetItemID(itemLocation: ItemLocation) -> itemID: number
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### GetItemIDByGUID

```lua
C_Item.GetItemIDByGUID(itemGUID: WOWGUID) -> itemID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetItemIDForItemInfo

```lua
C_Item.GetItemIDForItemInfo(itemInfo: ItemInfo) -> itemID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetItemInfo

```lua
C_Item.GetItemInfo(itemInfo: ItemInfo) -> itemName: cstring, itemLink: cstring, itemQuality: ItemQuality, itemLevel: number, itemMinLevel: number, itemType: cstring, itemSubType: cstring, itemStackCount: number, itemEquipLoc: cstring, itemTexture: fileID, sellPrice: number, classID: number, subclassID: number, bindType: number, expansionID: number, setID: number?, isCraftingReagent: bool, itemDescription: cstring
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetItemInfoInstant

```lua
C_Item.GetItemInfoInstant(itemInfo: ItemInfo) -> itemID: number, itemType: cstring, itemSubType: cstring, itemEquipLoc: cstring, icon: fileID, classID: number, subClassID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetItemInventorySlotInfo

```lua
C_Item.GetItemInventorySlotInfo(inventorySlot: InventoryType) -> result: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetItemInventorySlotKey

```lua
C_Item.GetItemInventorySlotKey(inventorySlot: InventoryType) -> result: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetItemInventoryType

```lua
C_Item.GetItemInventoryType(itemLocation: ItemLocation) -> inventoryType: InventoryType?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### GetItemInventoryTypeByID

```lua
C_Item.GetItemInventoryTypeByID(itemInfo: ItemInfo) -> inventoryType: InventoryType?
```

`SecretArguments=AllowedWhenUntainted`

### GetItemLearnTransmogSet

```lua
C_Item.GetItemLearnTransmogSet(itemInfo: ItemInfo) -> setID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetItemLink

```lua
C_Item.GetItemLink(itemLocation: ItemLocation) -> itemLink: string?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### GetItemLinkByGUID

```lua
C_Item.GetItemLinkByGUID(itemGUID: WOWGUID) -> itemLink: string?
```

`SecretArguments=AllowedWhenUntainted`

### GetItemLocation

```lua
C_Item.GetItemLocation(itemGUID: WOWGUID) -> itemLocation: ItemLocation?
```

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation?` | `Mixin=ItemLocationMixin` |

### GetItemMaxStackSize

```lua
C_Item.GetItemMaxStackSize(itemLocation: ItemLocation) -> stackSize: number?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### GetItemMaxStackSizeByID

```lua
C_Item.GetItemMaxStackSizeByID(itemInfo: ItemInfo) -> stackSize: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetItemName

```lua
C_Item.GetItemName(itemLocation: ItemLocation) -> itemName: string?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### GetItemNameByID

```lua
C_Item.GetItemNameByID(itemInfo: ItemInfo) -> itemName: string?
```

`SecretArguments=AllowedWhenUntainted`

### GetItemNumAddedSockets

```lua
C_Item.GetItemNumAddedSockets(itemInfo: ItemInfo) -> socketCount: number
```

`SecretArguments=AllowedWhenUntainted`

### GetItemNumSockets

```lua
C_Item.GetItemNumSockets(itemInfo: ItemInfo) -> socketCount: number
```

`SecretArguments=AllowedWhenUntainted`

### GetItemQuality

```lua
C_Item.GetItemQuality(itemLocation: ItemLocation) -> itemQuality: ItemQuality?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### GetItemQualityByID

```lua
C_Item.GetItemQualityByID(itemInfo: ItemInfo) -> itemQuality: ItemQuality?
```

`SecretArguments=AllowedWhenUntainted`

### GetItemQualityColor

```lua
C_Item.GetItemQualityColor(quality: ItemQuality) -> colorRGBR: number, colorRGBG: number, colorRGBB: number, qualityString: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetItemSetInfo

```lua
C_Item.GetItemSetInfo(setID: number) -> result: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetItemSpecInfo

```lua
C_Item.GetItemSpecInfo(itemInfo: ItemInfo) -> specTable: number[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetItemSpell

```lua
C_Item.GetItemSpell(itemInfo: ItemInfo) -> spellName: cstring, spellID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetItemStatDelta

```lua
C_Item.GetItemStatDelta(itemLink1: cstring, itemLink2: cstring) -> statTable: LuaValueVariant
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetItemStats

```lua
C_Item.GetItemStats(itemLink: cstring) -> statTable: LuaValueVariant
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetItemSubClassInfo

```lua
C_Item.GetItemSubClassInfo(itemClassID: number, itemSubClassID: number) -> subClassName: cstring, subClassUsesInvType: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetItemUniqueness

```lua
C_Item.GetItemUniqueness(itemInfo: ItemInfo) -> limitCategory: number, limitMax: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetItemUniquenessByID

```lua
C_Item.GetItemUniquenessByID(itemInfo: ItemInfo) -> isUnique: bool, limitCategoryName: cstring?, limitCategoryCount: number?, limitCategoryID: number?
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetItemUpgradeInfo

```lua
C_Item.GetItemUpgradeInfo(itemInfo: ItemInfo) -> itemUpgradeInfo: ItemUpgradeInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetLimitedCurrencyItemInfo

```lua
C_Item.GetLimitedCurrencyItemInfo(itemInfo: ItemInfo) -> name: cstring, icon: fileID, quantity: number, maxQuantity: number, totalEarned: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSetBonusesForSpecializationByItemID

```lua
C_Item.GetSetBonusesForSpecializationByItemID(specID: number, itemID: number) -> itemSetSpellIDs: number[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetStackCount

```lua
C_Item.GetStackCount(itemLocation: ItemLocation) -> stackCount: number
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### GetWeaponEnchantInfo

```lua
C_Item.GetWeaponEnchantInfo(weaponSlot: WeaponSlot) -> enchants: WeaponEnchantInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### IsAnimaItemByID

```lua
C_Item.IsAnimaItemByID(itemInfo: ItemInfo) -> isAnimaItem: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsArtifactPowerItem

```lua
C_Item.IsArtifactPowerItem(itemInfo: ItemInfo) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsBound

```lua
C_Item.IsBound(itemLocation: ItemLocation) -> isBound: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### IsBoundToAccountUntilEquip

```lua
C_Item.IsBoundToAccountUntilEquip(itemLocation: ItemLocation) -> isBoundToAccountUntilEquip: bool
```

You can use IsItemBindToAccountUntilEquip instead if the item is not in your inventory

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### IsConsumableItem

```lua
C_Item.IsConsumableItem(itemInfo: ItemInfo) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsCorruptedItem

```lua
C_Item.IsCorruptedItem(itemInfo: ItemInfo) -> result: bool?
```

`SecretArguments=AllowedWhenUntainted`

### IsCosmeticItem

```lua
C_Item.IsCosmeticItem(itemInfo: ItemInfo) -> result: bool?
```

`SecretArguments=AllowedWhenUntainted`

### IsCurioItem

```lua
C_Item.IsCurioItem(itemInfo: ItemInfo) -> result: bool?
```

Returns whether the item is a consumable curio that can be applied to a delves companion.

`SecretArguments=AllowedWhenUntainted`

### IsCurrentItem

```lua
C_Item.IsCurrentItem(itemInfo: ItemInfo) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsDecorItem

```lua
C_Item.IsDecorItem(itemInfo: ItemInfo) -> isDecor: bool?
```

Returns whether the item is a consumable decor item.

`SecretArguments=AllowedWhenUntainted`

### IsDressableItemByID

```lua
C_Item.IsDressableItemByID(itemInfo: ItemInfo) -> isDressableItem: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsEquippableItem

```lua
C_Item.IsEquippableItem(itemInfo: ItemInfo) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsEquippedItem

```lua
C_Item.IsEquippedItem(itemInfo: ItemInfo) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsEquippedItemType

```lua
C_Item.IsEquippedItemType(type: cstring) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsHarmfulItem

```lua
C_Item.IsHarmfulItem(itemInfo: ItemInfo) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsHelpfulItem

```lua
C_Item.IsHelpfulItem(itemInfo: ItemInfo) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsItemBindToAccount

```lua
C_Item.IsItemBindToAccount(itemInfo: ItemInfo) -> isItemBindToAccount: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsItemBindToAccountUntilEquip

```lua
C_Item.IsItemBindToAccountUntilEquip(itemInfo: ItemInfo) -> isItemBindToAccountUntilEquip: bool
```

You can use IsBoundToAccountUntilEquip instead if the item exists in your inventory

`SecretArguments=AllowedWhenUntainted`

### IsItemConduit

```lua
C_Item.IsItemConduit(itemLoc: ItemLocation) -> isConduit: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLoc` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### IsItemConvertibleAndValidForPlayer

```lua
C_Item.IsItemConvertibleAndValidForPlayer(itemLoc: ItemLocation) -> isItemConvertibleAndValidForPlayer: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLoc` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### IsItemCorrupted

```lua
C_Item.IsItemCorrupted(itemLoc: ItemLocation) -> isCorrupted: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLoc` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### IsItemCorruptionRelated

```lua
C_Item.IsItemCorruptionRelated(itemLoc: ItemLocation) -> isCorruptionRelated: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLoc` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### IsItemCorruptionResistant

```lua
C_Item.IsItemCorruptionResistant(itemLoc: ItemLocation) -> isCorruptionResistant: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLoc` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### IsItemDataCached

```lua
C_Item.IsItemDataCached(itemLocation: ItemLocation) -> isCached: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### IsItemDataCachedByID

```lua
C_Item.IsItemDataCachedByID(itemInfo: ItemInfo) -> isCached: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsItemGUIDInInventory

```lua
C_Item.IsItemGUIDInInventory(itemGUID: WOWGUID) -> valid: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsItemInRange

```lua
C_Item.IsItemInRange(itemInfo: ItemInfo, targetToken: cstring) -> result: bool?
```

`SecretArguments=AllowedWhenUntainted`

### IsItemKeystoneByID

```lua
C_Item.IsItemKeystoneByID(itemInfo: ItemInfo) -> isKeystone: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsItemSpecificToPlayerClass

```lua
C_Item.IsItemSpecificToPlayerClass(itemInfo: ItemInfo) -> isItemSpecificToPlayerClass: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsLocked

```lua
C_Item.IsLocked(itemLocation: ItemLocation) -> isLocked: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### IsRelicItem

```lua
C_Item.IsRelicItem(itemInfo: ItemInfo) -> result: bool?
```

Returns whether the item is a consumable relic  that can be applied to an artifact weapon.

`SecretArguments=AllowedWhenUntainted`

### IsUsableItem

```lua
C_Item.IsUsableItem(itemInfo: ItemInfo) -> usable: bool, noMana: bool
```

`SecretArguments=AllowedWhenUntainted`

### ItemHasRange

```lua
C_Item.ItemHasRange(itemInfo: ItemInfo) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### LockItem

```lua
C_Item.LockItem(itemLocation: ItemLocation)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### LockItemByGUID

```lua
C_Item.LockItemByGUID(itemGUID: WOWGUID)
```

`SecretArguments=AllowedWhenUntainted`

### PickupItem

```lua
C_Item.PickupItem(itemInfo: ItemInfo)
```

`SecretArguments=AllowedWhenUntainted`

### ReplaceEnchant

```lua
C_Item.ReplaceEnchant()
```

### ReplaceTradeEnchant

```lua
C_Item.ReplaceTradeEnchant()
```

### ReplaceTradeskillEnchant

```lua
C_Item.ReplaceTradeskillEnchant()
```

### RequestLoadItemData

```lua
C_Item.RequestLoadItemData(itemLocation: ItemLocation)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### RequestLoadItemDataByID

```lua
C_Item.RequestLoadItemDataByID(itemInfo: ItemInfo)
```

`SecretArguments=AllowedWhenUntainted`

### UnlockItem

```lua
C_Item.UnlockItem(itemLocation: ItemLocation)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### UnlockItemByGUID

```lua
C_Item.UnlockItemByGUID(itemGUID: WOWGUID)
```

`SecretArguments=AllowedWhenUntainted`

### UseItemByName

```lua
C_Item.UseItemByName(itemInfo: ItemInfo, target: cstring?)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### ACTION_WILL_BIND_ITEM

```lua
ACTION_WILL_BIND_ITEM()
```

`SynchronousEvent`

### BIND_ENCHANT

```lua
BIND_ENCHANT()
```

`SynchronousEvent`

### CHARACTER_ITEM_FIXUP_NOTIFICATION

```lua
CHARACTER_ITEM_FIXUP_NOTIFICATION(fixupVersion: number)
```

`SynchronousEvent`

### CONFIRM_BEFORE_USE

```lua
CONFIRM_BEFORE_USE()
```

`SynchronousEvent`

### CONVERT_TO_BIND_TO_ACCOUNT_CONFIRM

```lua
CONVERT_TO_BIND_TO_ACCOUNT_CONFIRM()
```

`SynchronousEvent`

### DELETE_ITEM_CONFIRM

```lua
DELETE_ITEM_CONFIRM(itemName: cstring, qualityID: number, bonding: number, questWarn: number, itemGUID: WOWGUID?)
```

`SynchronousEvent`

### END_BOUND_TRADEABLE

```lua
END_BOUND_TRADEABLE(reason: cstring)
```

`SynchronousEvent`

### GET_ITEM_INFO_RECEIVED

```lua
GET_ITEM_INFO_RECEIVED(itemID: number, success: bool)
```

`SynchronousEvent`

### ITEM_CHANGED

```lua
ITEM_CHANGED(previousHyperlink: string, newHyperlink: string)
```

`SynchronousEvent`

### ITEM_CONVERSION_DATA_READY

```lua
ITEM_CONVERSION_DATA_READY(itemGUID: WOWGUID)
```

`SynchronousEvent`

### ITEM_COUNT_CHANGED

```lua
ITEM_COUNT_CHANGED(itemID: number)
```

`UniqueEvent`

### ITEM_DATA_LOAD_RESULT

```lua
ITEM_DATA_LOAD_RESULT(itemID: number, success: bool)
```

`SynchronousEvent`

### MERCHANT_CONFIRM_TRADE_TIMER_REMOVAL

```lua
MERCHANT_CONFIRM_TRADE_TIMER_REMOVAL(itemLink: cstring)
```

`SynchronousEvent`

### REPLACE_ENCHANT

```lua
REPLACE_ENCHANT(existingStr: cstring, replacementStr: cstring)
```

`SynchronousEvent`

### REPLACE_TRADESKILL_ENCHANT

```lua
REPLACE_TRADESKILL_ENCHANT(existing: cstring, replacement: cstring)
```

`SynchronousEvent`

### TRADE_REPLACE_ENCHANT

```lua
TRADE_REPLACE_ENCHANT(existing: cstring, replacement: cstring)
```

`SynchronousEvent`

### USE_BIND_CONFIRM

```lua
USE_BIND_CONFIRM()
```

`SynchronousEvent`

### USE_NO_REFUND_CONFIRM

```lua
USE_NO_REFUND_CONFIRM()
```

`SynchronousEvent`

### WEAPON_ENCHANT_CHANGED

```lua
WEAPON_ENCHANT_CHANGED()
```

`UniqueEvent`

## Types

### ItemInfoResult

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `itemName` | `cstring` |  |
| `itemLink` | `cstring` |  |
| `itemQuality` | `ItemQuality` |  |
| `itemLevel` | `number` |  |
| `itemMinLevel` | `number` |  |
| `itemType` | `cstring` |  |
| `itemSubType` | `cstring` |  |
| `itemStackCount` | `number` |  |
| `itemEquipLoc` | `cstring` |  |
| `itemTexture` | `fileID` |  |
| `sellPrice` | `number` |  |
| `classID` | `number` |  |
| `subclassID` | `number` |  |
| `bindType` | `number` |  |
| `expansionID` | `number` |  |
| `setID` | `number?` |  |
| `isCraftingReagent` | `bool` |  |
| `itemDescription` | `cstring` |  |

### ItemUpgradeInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `currentLevel` | `number` |  |
| `maxLevel` | `number` |  |
| `maxItemLevel` | `number` |  |
| `trackString` | `cstring?` |  |
| `trackStringID` | `number?` |  |

### WeaponEnchantInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `hasEnchant` | `bool` |  |
| `enchantType` | `ItemEnchantType` |  |
| `timeLeft` | `number` |  |
| `charges` | `number` |  |
| `enchantID` | `number` |  |
| `enchantIconID` | `number` |  |
