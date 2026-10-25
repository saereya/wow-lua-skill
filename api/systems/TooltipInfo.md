# TooltipInfo

Namespace `C_TooltipInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/tooltipinfodocumentation.lua` (FileDataID 4763883)

## Functions

### GetAchievementByID

```lua
C_TooltipInfo.GetAchievementByID(achievementID: number) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetAction

```lua
C_TooltipInfo.GetAction(actionID: luaIndex) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetArtifactItem

```lua
C_TooltipInfo.GetArtifactItem() -> data: TooltipData
```

`MayReturnNothing`

### GetArtifactPowerByID

```lua
C_TooltipInfo.GetArtifactPowerByID(powerID: number) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetAzeriteEssence

```lua
C_TooltipInfo.GetAzeriteEssence(essenceID: number, rank: number?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetAzeriteEssenceSlot

```lua
C_TooltipInfo.GetAzeriteEssenceSlot(slot: AzeriteEssenceSlot) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetAzeritePower

```lua
C_TooltipInfo.GetAzeritePower(itemID: number, itemLevel: number, powerID: number, owningItemLink: cstring?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetBackpackToken

```lua
C_TooltipInfo.GetBackpackToken(index: luaIndex) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetBagItem

```lua
C_TooltipInfo.GetBagItem(bagIndex: BagIndex, slotIndex: luaIndex) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetBagItemChild

```lua
C_TooltipInfo.GetBagItemChild(bagIndex: BagIndex, slotIndex: luaIndex, equipSlotIndex: luaIndex) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetBuybackItem

```lua
C_TooltipInfo.GetBuybackItem(index: luaIndex) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetCompanionPet

```lua
C_TooltipInfo.GetCompanionPet(petGUID: WOWGUID) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetConduit

```lua
C_TooltipInfo.GetConduit(conduitID: number, conduitRank: number) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetCurrencyByID

```lua
C_TooltipInfo.GetCurrencyByID(currencyID: number, amount: number?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetCurrencyToken

```lua
C_TooltipInfo.GetCurrencyToken(tokenIndex: luaIndex) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetEnhancedConduit

```lua
C_TooltipInfo.GetEnhancedConduit(conduitID: number, rank: number) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetEquipmentSet

```lua
C_TooltipInfo.GetEquipmentSet(setID: number) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetExistingSocketGem

```lua
C_TooltipInfo.GetExistingSocketGem(index: luaIndex, toDestroy: bool?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetGuildBankItem

```lua
C_TooltipInfo.GetGuildBankItem(tab: luaIndex, slot: luaIndex) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetHeirloomByItemID

```lua
C_TooltipInfo.GetHeirloomByItemID(itemID: number) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetHyperlink

```lua
C_TooltipInfo.GetHyperlink(hyperlink: cstring, optionalArg1: number?, optionalArg2: number?, hideVendorPrice: bool?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetInboxItem

```lua
C_TooltipInfo.GetInboxItem(messageIndex: luaIndex, attachmentIndex: luaIndex?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetInstanceLockEncountersComplete

```lua
C_TooltipInfo.GetInstanceLockEncountersComplete(index: luaIndex) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetInventoryItem

```lua
C_TooltipInfo.GetInventoryItem(unit: UnitToken, slot: luaIndex, hideUselessStats: bool?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetInventoryItemByID

```lua
C_TooltipInfo.GetInventoryItemByID(itemID: number) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetItemByGUID

```lua
C_TooltipInfo.GetItemByGUID(guid: WOWGUID) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetItemByID

```lua
C_TooltipInfo.GetItemByID(itemID: number, quality: number?, itemContext: number?, treasureContextLevel: number?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetItemByItemModifiedAppearanceID

```lua
C_TooltipInfo.GetItemByItemModifiedAppearanceID(itemModifiedAppearanceID: number) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetItemInteractionItem

```lua
C_TooltipInfo.GetItemInteractionItem() -> data: TooltipData
```

`MayReturnNothing`

### GetItemKey

```lua
C_TooltipInfo.GetItemKey(itemID: number, itemLevel: number, itemSuffix: number, requiredLevel: number?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetLFGDungeonReward

```lua
C_TooltipInfo.GetLFGDungeonReward(dungeonID: number, lootIndex: luaIndex) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetLFGDungeonShortageReward

```lua
C_TooltipInfo.GetLFGDungeonShortageReward(dungeonID: number, shortageSeverity: luaIndex, lootIndex: luaIndex) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetLootCurrency

```lua
C_TooltipInfo.GetLootCurrency(slot: luaIndex) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetLootItem

```lua
C_TooltipInfo.GetLootItem(slot: luaIndex) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetLootRollItem

```lua
C_TooltipInfo.GetLootRollItem(id: number) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetMerchantCostItem

```lua
C_TooltipInfo.GetMerchantCostItem(slot: luaIndex, costIndex: luaIndex) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetMerchantItem

```lua
C_TooltipInfo.GetMerchantItem(slot: luaIndex) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetMinimapMouseover

```lua
C_TooltipInfo.GetMinimapMouseover() -> data: TooltipData
```

`MayReturnNothing`

### GetMountBySpellID

```lua
C_TooltipInfo.GetMountBySpellID(spellID: SpellIdentifier, checkIndoors: bool?) -> data: TooltipData
```

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `SpellIdentifier` |  |
| `checkIndoors` | `bool?` | `NeverSecret` |

### GetOutfit

```lua
C_TooltipInfo.GetOutfit(outfitID: number) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetOwnedItemByID

```lua
C_TooltipInfo.GetOwnedItemByID(itemID: number) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetPetAction

```lua
C_TooltipInfo.GetPetAction(slot: luaIndex) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetPossession

```lua
C_TooltipInfo.GetPossession(slot: luaIndex) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetPvpBrawl

```lua
C_TooltipInfo.GetPvpBrawl(isSpecial: bool?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetPvpTalent

```lua
C_TooltipInfo.GetPvpTalent(talentID: number, isInspect: bool?, groupIndex: luaIndex?, talentIndex: number?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetQuestCurrency

```lua
C_TooltipInfo.GetQuestCurrency(type: cstring, currencyIndex: luaIndex) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetQuestItem

```lua
C_TooltipInfo.GetQuestItem(type: cstring, itemIndex: luaIndex, allowCollectionText: bool?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetQuestLogCurrency

```lua
C_TooltipInfo.GetQuestLogCurrency(type: cstring, currencyIndex: luaIndex, questID: number?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetQuestLogItem

```lua
C_TooltipInfo.GetQuestLogItem(type: cstring, itemIndex: luaIndex, questID: number?, allowCollectionText: bool?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetQuestLogSpecialItem

```lua
C_TooltipInfo.GetQuestLogSpecialItem(questIndex: luaIndex) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetQuestPartyProgress

```lua
C_TooltipInfo.GetQuestPartyProgress(questID: number, omitTitle: bool?, ignoreActivePlayer: bool?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetRecipeRankInfo

```lua
C_TooltipInfo.GetRecipeRankInfo(recipeID: number, rank: number) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetRecipeReagentItem

```lua
C_TooltipInfo.GetRecipeReagentItem(recipeSpellID: number, dataSlotIndex: luaIndex) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetRecipeResultItem

```lua
C_TooltipInfo.GetRecipeResultItem(recipeID: number, reagentInfos: CraftingReagentInfo[]?, recraftItemGUID: WOWGUID?, recipeLevel: luaIndex?, overrideQualityID: number?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetRecipeResultItemForOrder

```lua
C_TooltipInfo.GetRecipeResultItemForOrder(recipeID: number, reagentInfos: CraftingReagentInfo[]?, orderID: BigUInteger?, recipeLevel: luaIndex?, overrideQualityID: number?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetRuneforgeResultItem

```lua
C_TooltipInfo.GetRuneforgeResultItem(itemGUID: WOWGUID, itemLevel: number, powerID: number?, modifiers: number[]?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSendMailItem

```lua
C_TooltipInfo.GetSendMailItem(attachmentIndex: luaIndex?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetShapeshift

```lua
C_TooltipInfo.GetShapeshift(slot: luaIndex) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSlottedKeystone

```lua
C_TooltipInfo.GetSlottedKeystone() -> data: TooltipData
```

`MayReturnNothing`

### GetSocketedItem

```lua
C_TooltipInfo.GetSocketedItem() -> data: TooltipData
```

`MayReturnNothing`

### GetSocketedRelic

```lua
C_TooltipInfo.GetSocketedRelic(slotIndex: luaIndex) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSocketGem

```lua
C_TooltipInfo.GetSocketGem(index: luaIndex) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSpellBookItem

```lua
C_TooltipInfo.GetSpellBookItem(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSpellByID

```lua
C_TooltipInfo.GetSpellByID(spellID: SpellIdentifier, isPet: bool?, showSubtext: bool?, dontOverride: bool?, difficultyID: number?, isLink: bool?) -> data: TooltipData
```

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `SpellIdentifier` |  |
| `isPet` | `bool?` | `NeverSecret` |
| `showSubtext` | `bool?` | `NeverSecret` |
| `dontOverride` | `bool?` | `NeverSecret` |
| `difficultyID` | `number?` | `NeverSecret` |
| `isLink` | `bool?` | `NeverSecret` |

### GetTalent

```lua
C_TooltipInfo.GetTalent(talentID: number, isInspect: bool?, groupIndex: luaIndex?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetTotem

```lua
C_TooltipInfo.GetTotem(slot: luaIndex) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetToyByItemID

```lua
C_TooltipInfo.GetToyByItemID(itemID: number) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetTradePlayerItem

```lua
C_TooltipInfo.GetTradePlayerItem(slot: luaIndex) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetTradeTargetItem

```lua
C_TooltipInfo.GetTradeTargetItem(slot: luaIndex) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetTrainerService

```lua
C_TooltipInfo.GetTrainerService(serviceIndex: luaIndex) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetTraitEntry

```lua
C_TooltipInfo.GetTraitEntry(entryID: number, rank: number?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetUnit

```lua
C_TooltipInfo.GetUnit(unit: UnitTokenPvPRestrictedForAddOns, hideStatus: bool?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetUnitAura

```lua
C_TooltipInfo.GetUnitAura(unitToken: UnitTokenRestrictedForAddOns, index: luaIndex, filter: AuraFilters?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresUnitAuraAccess` `SecretWhenUnitAuraRestricted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unitToken` | `UnitTokenRestrictedForAddOns` | `NeverSecret` |
| `index` | `luaIndex` |  |
| `filter` | `AuraFilters?` |  |

### GetUnitAuraByAuraInstanceID

```lua
C_TooltipInfo.GetUnitAuraByAuraInstanceID(unitToken: UnitTokenRestrictedForAddOns, auraInstanceID: number, filter: AuraFilters?) -> data: TooltipData
```

Obtains aura info like other functions with the caveat that the filters will always at least include the typically mutually exclusive HELPFUL|HARMFUL regardless of what the argument value is set to

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresUnitAuraAccess` `SecretWhenUnitAuraRestricted`

### GetUnitBuff

```lua
C_TooltipInfo.GetUnitBuff(unitToken: UnitTokenRestrictedForAddOns, index: luaIndex, filter: AuraFilters?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresUnitAuraAccess` `SecretWhenUnitAuraRestricted`

### GetUnitBuffByAuraInstanceID

```lua
C_TooltipInfo.GetUnitBuffByAuraInstanceID(unitToken: UnitTokenRestrictedForAddOns, auraInstanceID: number, filter: AuraFilters?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresUnitAuraAccess` `SecretWhenUnitAuraRestricted`

### GetUnitDebuff

```lua
C_TooltipInfo.GetUnitDebuff(unitToken: UnitTokenRestrictedForAddOns, index: luaIndex, filter: AuraFilters?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresUnitAuraAccess` `SecretWhenUnitAuraRestricted`

### GetUnitDebuffByAuraInstanceID

```lua
C_TooltipInfo.GetUnitDebuffByAuraInstanceID(unitToken: UnitTokenRestrictedForAddOns, auraInstanceID: number, filter: AuraFilters?) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresUnitAuraAccess` `SecretWhenUnitAuraRestricted`

### GetUpgradeItem

```lua
C_TooltipInfo.GetUpgradeItem() -> data: TooltipData
```

`MayReturnNothing`

### GetWeeklyReward

```lua
C_TooltipInfo.GetWeeklyReward(itemDBID: WeeklyRewardItemDBID) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetWorldCursor

```lua
C_TooltipInfo.GetWorldCursor() -> data: TooltipData
```

`MayReturnNothing`

### GetWorldLootObject

```lua
C_TooltipInfo.GetWorldLootObject(unitTokenString: cstring) -> data: TooltipData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

## Events

### HIDE_HYPERLINK_TOOLTIP

```lua
HIDE_HYPERLINK_TOOLTIP()
```

`SynchronousEvent`

### SHOW_HYPERLINK_TOOLTIP

```lua
SHOW_HYPERLINK_TOOLTIP(hyperlink: string)
```

`SynchronousEvent`

### TOOLTIP_DATA_UPDATE

```lua
TOOLTIP_DATA_UPDATE(dataInstanceID: number?)
```

Sends an update to the UI that a sparse or cache lookup has resolved

`UniqueEvent`
