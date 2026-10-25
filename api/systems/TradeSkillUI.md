# TradeSkillUI

Namespace `C_TradeSkillUI` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/tradeskilluidocumentation.lua` (FileDataID 4637267)

## Functions

### CancelProfessionRespec

```lua
C_TradeSkillUI.CancelProfessionRespec()
```

### CanStoreEnchantInItem

```lua
C_TradeSkillUI.CanStoreEnchantInItem(itemGUID: WOWGUID) -> canStore: bool
```

`SecretArguments=AllowedWhenUntainted`

### CanTradeSkillShowCraftingUI

```lua
C_TradeSkillUI.CanTradeSkillShowCraftingUI(tradeSkillSpellID: number) -> canShow: bool
```

`SecretArguments=AllowedWhenUntainted`

### CheckRespecNPC

```lua
C_TradeSkillUI.CheckRespecNPC() -> canInteract: bool
```

### CloseTradeSkill

```lua
C_TradeSkillUI.CloseTradeSkill()
```

### ConfirmProfessionRespec

```lua
C_TradeSkillUI.ConfirmProfessionRespec()
```

### CraftEnchant

```lua
C_TradeSkillUI.CraftEnchant(recipeSpellID: number, numCasts: number, craftingReagents: CraftingReagentInfo[]?, itemTarget: ItemLocation?, applyConcentration: bool?)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `recipeSpellID` | `number` |  |
| `numCasts` | `number` | default `1` |
| `craftingReagents` | `CraftingReagentInfo[]?` |  |
| `itemTarget` | `ItemLocation?` | `Mixin=ItemLocationMixin` |
| `applyConcentration` | `bool?` |  |

### CraftRecipe

```lua
C_TradeSkillUI.CraftRecipe(recipeSpellID: number, numCasts: number, craftingReagents: CraftingReagentInfo[]?, recipeLevel: luaIndex?, orderID: BigUInteger?, applyConcentration: bool?)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `recipeSpellID` | `number` |  |
| `numCasts` | `number` | default `1` |
| `craftingReagents` | `CraftingReagentInfo[]?` |  |
| `recipeLevel` | `luaIndex?` |  |
| `orderID` | `BigUInteger?` |  |
| `applyConcentration` | `bool?` |  |

### CraftSalvage

```lua
C_TradeSkillUI.CraftSalvage(recipeSpellID: number, numCasts: number, itemTarget: ItemLocation, craftingReagents: CraftingReagentInfo[]?, applyConcentration: bool?)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `recipeSpellID` | `number` |  |
| `numCasts` | `number` | default `1` |
| `itemTarget` | `ItemLocation` | `Mixin=ItemLocationMixin` |
| `craftingReagents` | `CraftingReagentInfo[]?` |  |
| `applyConcentration` | `bool?` |  |

### DoesRecraftingRecipeAcceptItem

```lua
C_TradeSkillUI.DoesRecraftingRecipeAcceptItem(itemLocation: ItemLocation, recipeID: number) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |
| `recipeID` | `number` |  |

### GetAllProfessionTradeSkillLines

```lua
C_TradeSkillUI.GetAllProfessionTradeSkillLines() -> skillLineID: number[]
```

### GetBaseProfessionInfo

```lua
C_TradeSkillUI.GetBaseProfessionInfo() -> info: ProfessionInfo
```

### GetChildProfessionInfo

```lua
C_TradeSkillUI.GetChildProfessionInfo() -> info: ProfessionInfo
```

### GetChildProfessionInfos

```lua
C_TradeSkillUI.GetChildProfessionInfos() -> infos: ProfessionInfo[]
```

### GetConcentrationCurrencyID

```lua
C_TradeSkillUI.GetConcentrationCurrencyID(skillLineID: number) -> currencyType: number
```

`SecretArguments=AllowedWhenUntainted`

### GetCraftableCount

```lua
C_TradeSkillUI.GetCraftableCount(recipeSpellID: number, recipeLevel: luaIndex?) -> numAvailable: number
```

`SecretArguments=AllowedWhenUntainted`

### GetCraftingOperationInfo

```lua
C_TradeSkillUI.GetCraftingOperationInfo(recipeID: number, craftingReagents: CraftingReagentInfo[], allocationItemGUID: WOWGUID?, applyConcentration: bool) -> info: CraftingOperationInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetCraftingOperationInfoForOrder

```lua
C_TradeSkillUI.GetCraftingOperationInfoForOrder(recipeID: number, craftingReagents: CraftingReagentInfo[], orderID: BigUInteger, applyConcentration: bool) -> info: CraftingOperationInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetCraftingReagentBonusText

```lua
C_TradeSkillUI.GetCraftingReagentBonusText(recipeSpellID: number, craftingReagentIndex: luaIndex, craftingReagents: CraftingReagentInfo[], allocationItemGUID: WOWGUID?) -> bonusText: string[]
```

`SecretArguments=AllowedWhenUntainted`

### GetCraftingTargetItems

```lua
C_TradeSkillUI.GetCraftingTargetItems(itemIDs: number[]) -> items: CraftingTargetItem[]
```

`SecretArguments=AllowedWhenUntainted`

### GetDependentReagents

```lua
C_TradeSkillUI.GetDependentReagents(reagent: CraftingReagent) -> reagents: CraftingReagent[]
```

`SecretArguments=AllowedWhenUntainted`

### GetEnchantItems

```lua
C_TradeSkillUI.GetEnchantItems(recipeID: number, craftingReagents: CraftingReagentInfo[]?) -> items: WOWGUID[]
```

`SecretArguments=AllowedWhenUntainted`

### GetFactionSpecificOutputItem

```lua
C_TradeSkillUI.GetFactionSpecificOutputItem(recipeSpellID: number) -> itemID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetGatheringOperationInfo

```lua
C_TradeSkillUI.GetGatheringOperationInfo(recipeID: number) -> info: GatheringOperationInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetHideUnownedFlags

```lua
C_TradeSkillUI.GetHideUnownedFlags(recipeID: number) -> cannotModifyHideUnowned: bool, alwaysShowUnowned: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetItemCraftedQualityByItemInfo

```lua
C_TradeSkillUI.GetItemCraftedQualityByItemInfo(itemInfo: ItemInfo) -> quality: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetItemCraftedQualityInfo

```lua
C_TradeSkillUI.GetItemCraftedQualityInfo(itemInfo: ItemInfo) -> info: CraftingQualityInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetItemReagentQualityByItemInfo

```lua
C_TradeSkillUI.GetItemReagentQualityByItemInfo(itemInfo: ItemInfo) -> quality: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetItemReagentQualityInfo

```lua
C_TradeSkillUI.GetItemReagentQualityInfo(itemInfo: ItemInfo) -> info: CraftingQualityInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetItemSlotModifications

```lua
C_TradeSkillUI.GetItemSlotModifications(itemGUID: WOWGUID) -> slotMods: CraftingItemSlotModification[]
```

`SecretArguments=AllowedWhenUntainted`

### GetItemSlotModificationsForOrder

```lua
C_TradeSkillUI.GetItemSlotModificationsForOrder(orderID: BigUInteger) -> slotMods: CraftingItemSlotModification[]
```

`SecretArguments=AllowedWhenUntainted`

### GetOriginalCraftRecipeID

```lua
C_TradeSkillUI.GetOriginalCraftRecipeID(itemGUID: WOWGUID) -> recipeID: number?, skillLineAbilityID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetProfessionByInventorySlot

```lua
C_TradeSkillUI.GetProfessionByInventorySlot(slot: luaIndex) -> profession: Profession?
```

`SecretArguments=AllowedWhenUntainted`

### GetProfessionChildSkillLineID

```lua
C_TradeSkillUI.GetProfessionChildSkillLineID() -> skillLineID: number
```

### GetProfessionForCursorItem

```lua
C_TradeSkillUI.GetProfessionForCursorItem() -> profession: Profession?
```

### GetProfessionInfoByRecipeID

```lua
C_TradeSkillUI.GetProfessionInfoByRecipeID(recipeID: number) -> info: ProfessionInfo
```

`SecretArguments=AllowedWhenUntainted`

### GetProfessionInfoBySkillLineID

```lua
C_TradeSkillUI.GetProfessionInfoBySkillLineID(skillLineID: number) -> info: ProfessionInfo
```

`SecretArguments=AllowedWhenUntainted`

### GetProfessionInventorySlots

```lua
C_TradeSkillUI.GetProfessionInventorySlots() -> invSlots: InventorySlots[]
```

### GetProfessionNameForSkillLineAbility

```lua
C_TradeSkillUI.GetProfessionNameForSkillLineAbility(skillLineAbilityID: number) -> professionNmae: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetProfessionSkillLineID

```lua
C_TradeSkillUI.GetProfessionSkillLineID(profession: Profession) -> skillLineID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetProfessionSlots

```lua
C_TradeSkillUI.GetProfessionSlots(profession: Profession) -> slots: luaIndex[]
```

`SecretArguments=AllowedWhenUntainted`

### GetProfessionSpells

```lua
C_TradeSkillUI.GetProfessionSpells(professionID: number, skillLineID: number?) -> knownSpells: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetQualitiesForRecipe

```lua
C_TradeSkillUI.GetQualitiesForRecipe(recipeID: number) -> qualityIDs: number[]?
```

`SecretArguments=AllowedWhenUntainted`

### GetReagentDifficultyText

```lua
C_TradeSkillUI.GetReagentDifficultyText(craftingReagentIndex: luaIndex, craftingReagents: CraftingReagentInfo[]) -> bonusText: string
```

`SecretArguments=AllowedWhenUntainted`

### GetReagentSlotStatus

```lua
C_TradeSkillUI.GetReagentSlotStatus(mcrSlotID: number, recipeSpellID: number, skillLineAbilityID: number) -> locked: bool, lockedReason: string
```

`SecretArguments=AllowedWhenUntainted`

### GetRecipeDescription

```lua
C_TradeSkillUI.GetRecipeDescription(recipeID: number, craftingReagents: CraftingReagentInfo[], allocationItemGUID: WOWGUID?) -> description: string
```

`SecretArguments=AllowedWhenUntainted`

### GetRecipeInfo

```lua
C_TradeSkillUI.GetRecipeInfo(recipeSpellID: number, recipeLevel: luaIndex?) -> recipeInfo: TradeSkillRecipeInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetRecipeInfoForSkillLineAbility

```lua
C_TradeSkillUI.GetRecipeInfoForSkillLineAbility(skillLineAbilityID: number, recipeLevel: luaIndex?) -> recipeInfo: TradeSkillRecipeInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetRecipeItemQualityInfo

```lua
C_TradeSkillUI.GetRecipeItemQualityInfo(recipeID: number, quality: number) -> info: CraftingQualityInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetRecipeOutputItemData

```lua
C_TradeSkillUI.GetRecipeOutputItemData(recipeSpellID: number, reagents: CraftingReagentInfo[]?, allocationItemGUID: WOWGUID?, overrideQualityID: number?, recraftOrderID: BigUInteger?) -> outputInfo: CraftingRecipeOutputInfo
```

`SecretArguments=AllowedWhenUntainted`

### GetRecipeQualityItemIDs

```lua
C_TradeSkillUI.GetRecipeQualityItemIDs(recipeSpellID: number) -> qualityItemIDs: number[]?
```

`SecretArguments=AllowedWhenUntainted`

### GetRecipeQualityReagentLink

```lua
C_TradeSkillUI.GetRecipeQualityReagentLink(recipeID: number, dataSlotIndex: luaIndex, qualityIndex: luaIndex) -> link: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetRecipeRequirements

```lua
C_TradeSkillUI.GetRecipeRequirements(recipeID: number) -> requirements: CraftingRecipeRequirement[]
```

`SecretArguments=AllowedWhenUntainted`

### GetRecipeSchematic

```lua
C_TradeSkillUI.GetRecipeSchematic(recipeSpellID: number, isRecraft: bool, recipeLevel: luaIndex?) -> schematic: CraftingRecipeSchematic
```

`SecretArguments=AllowedWhenUntainted`

### GetRecipesTracked

```lua
C_TradeSkillUI.GetRecipesTracked(isRecraft: bool) -> recipeIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetRecraftItems

```lua
C_TradeSkillUI.GetRecraftItems(recipeID: number?) -> items: WOWGUID[]
```

`SecretArguments=AllowedWhenUntainted`

### GetRecraftRemovalWarnings

```lua
C_TradeSkillUI.GetRecraftRemovalWarnings(itemGUID: WOWGUID, replacedReagents: CraftingReagent[]) -> warnings: cstring[]
```

`SecretArguments=AllowedWhenUntainted`

### GetRemainingRecasts

```lua
C_TradeSkillUI.GetRemainingRecasts() -> remaining: number
```

### GetSalvagableItemIDs

```lua
C_TradeSkillUI.GetSalvagableItemIDs(recipeID: number) -> itemIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetShowLearned

```lua
C_TradeSkillUI.GetShowLearned() -> flag: bool
```

### GetShowUnlearned

```lua
C_TradeSkillUI.GetShowUnlearned() -> flag: bool
```

### GetSkillLineForGear

```lua
C_TradeSkillUI.GetSkillLineForGear(itemInfo: ItemInfo) -> skillLineID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetSourceTypeFilter

```lua
C_TradeSkillUI.GetSourceTypeFilter() -> sourceTypeFilter: number
```

### GetTradeSkillDisplayName

```lua
C_TradeSkillUI.GetTradeSkillDisplayName(skillLineID: number) -> professionDisplayName: cstring
```

`SecretArguments=AllowedWhenUntainted`

### HasFavoriteOrderRecipes

```lua
C_TradeSkillUI.HasFavoriteOrderRecipes() -> hasFavorites: bool
```

### IsEnchantTargetValid

```lua
C_TradeSkillUI.IsEnchantTargetValid(recipeID: number, itemGUID: WOWGUID, craftingReagents: CraftingReagentInfo[]?) -> valid: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsGuildTradeSkillsEnabled

```lua
C_TradeSkillUI.IsGuildTradeSkillsEnabled() -> enabled: bool
```

### IsNearProfessionSpellFocus

```lua
C_TradeSkillUI.IsNearProfessionSpellFocus(profession: Profession) -> nearFocus: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsNPCCrafting

```lua
C_TradeSkillUI.IsNPCCrafting() -> result: bool
```

### IsOriginalCraftRecipeLearned

```lua
C_TradeSkillUI.IsOriginalCraftRecipeLearned(itemGUID: WOWGUID) -> learned: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsRecipeFirstCraft

```lua
C_TradeSkillUI.IsRecipeFirstCraft(recipeID: number) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsRecipeInBaseSkillLine

```lua
C_TradeSkillUI.IsRecipeInBaseSkillLine(recipeID: number) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsRecipeInSkillLine

```lua
C_TradeSkillUI.IsRecipeInSkillLine(recipeID: number, skillLineID: number) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsRecipeProfessionLearned

```lua
C_TradeSkillUI.IsRecipeProfessionLearned(recipeID: number) -> recipeProfessionLearned: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsRecipeTracked

```lua
C_TradeSkillUI.IsRecipeTracked(recipeID: number, isRecraft: bool) -> tracked: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsRecraftItemEquipped

```lua
C_TradeSkillUI.IsRecraftItemEquipped(recraftItemGUID: WOWGUID) -> isEquipped: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsRecraftReagentValid

```lua
C_TradeSkillUI.IsRecraftReagentValid(itemGUID: WOWGUID, reagent: CraftingReagent) -> valid: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsRuneforging

```lua
C_TradeSkillUI.IsRuneforging() -> result: bool
```

### OpenRecipe

```lua
C_TradeSkillUI.OpenRecipe(recipeID: number)
```

`SecretArguments=AllowedWhenUntainted`

### OpenTradeSkill

```lua
C_TradeSkillUI.OpenTradeSkill(skillLineID: number) -> opened: bool
```

`SecretArguments=AllowedWhenUntainted`

### RecraftLimitCategoryValid

```lua
C_TradeSkillUI.RecraftLimitCategoryValid(reagent: CraftingReagent) -> recraftValid: bool
```

`SecretArguments=AllowedWhenUntainted`

### RecraftRecipe

```lua
C_TradeSkillUI.RecraftRecipe(itemGUID: WOWGUID, craftingReagents: CraftingReagentInfo[]?, removedModifications: CraftingItemSlotModification[]?, applyConcentration: bool?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### RecraftRecipeForOrder

```lua
C_TradeSkillUI.RecraftRecipeForOrder(orderID: BigUInteger, itemGUID: WOWGUID, craftingReagents: CraftingReagentInfo[]?, removedModifications: CraftingItemSlotModification[]?, applyConcentration: bool?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetOnlyShowAvailableForOrders

```lua
C_TradeSkillUI.SetOnlyShowAvailableForOrders(flag: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetProfessionChildSkillLineID

```lua
C_TradeSkillUI.SetProfessionChildSkillLineID(skillLineID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetRecipeTracked

```lua
C_TradeSkillUI.SetRecipeTracked(recipeID: number, tracked: bool, isRecraft: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetShowLearned

```lua
C_TradeSkillUI.SetShowLearned(flag: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetShowUnlearned

```lua
C_TradeSkillUI.SetShowUnlearned(flag: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetSourceTypeFilter

```lua
C_TradeSkillUI.SetSourceTypeFilter(sourceTypeFilter: number)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### CRAFTING_DETAILS_UPDATE

```lua
CRAFTING_DETAILS_UPDATE()
```

`SynchronousEvent`

### NEW_RECIPE_LEARNED

```lua
NEW_RECIPE_LEARNED(recipeID: number, recipeLevel: luaIndex?, baseRecipeID: number?)
```

`SynchronousEvent`

### OBLITERUM_FORGE_PENDING_ITEM_CHANGED

```lua
OBLITERUM_FORGE_PENDING_ITEM_CHANGED()
```

`SynchronousEvent`

### OPEN_RECIPE_RESPONSE

```lua
OPEN_RECIPE_RESPONSE(recipeID: number, skillLineID: number, expansionSkillLineID: number)
```

`SynchronousEvent`

### PROFESSION_RESPEC_CONFIRMATION

```lua
PROFESSION_RESPEC_CONFIRMATION(skillName: cstring)
```

`SynchronousEvent`

### TRACKED_RECIPE_UPDATE

```lua
TRACKED_RECIPE_UPDATE(recipeID: number, tracked: bool)
```

`SynchronousEvent`

### TRADE_SKILL_CLOSE

```lua
TRADE_SKILL_CLOSE()
```

`SynchronousEvent`

### TRADE_SKILL_CRAFT_BEGIN

```lua
TRADE_SKILL_CRAFT_BEGIN(recipeSpellID: number)
```

`SynchronousEvent`

### TRADE_SKILL_CRAFTING_REAGENT_BONUS_TEXT_UPDATED

```lua
TRADE_SKILL_CRAFTING_REAGENT_BONUS_TEXT_UPDATED(itemID: number)
```

`SynchronousEvent`

### TRADE_SKILL_CURRENCY_REWARD_RESULT

```lua
TRADE_SKILL_CURRENCY_REWARD_RESULT(data: CraftingCurrencyResultData)
```

`SynchronousEvent`

### TRADE_SKILL_DATA_SOURCE_CHANGED

```lua
TRADE_SKILL_DATA_SOURCE_CHANGED()
```

`UniqueEvent`

### TRADE_SKILL_DATA_SOURCE_CHANGING

```lua
TRADE_SKILL_DATA_SOURCE_CHANGING()
```

`UniqueEvent`

### TRADE_SKILL_DETAILS_UPDATE

```lua
TRADE_SKILL_DETAILS_UPDATE()
```

`UniqueEvent`

### TRADE_SKILL_FAVORITES_CHANGED

```lua
TRADE_SKILL_FAVORITES_CHANGED(isFavorite: bool, recipeSpellID: number)
```

`UniqueEvent`

### TRADE_SKILL_ITEM_CRAFTED_RESULT

```lua
TRADE_SKILL_ITEM_CRAFTED_RESULT(data: CraftingItemResultData)
```

`SynchronousEvent`

### TRADE_SKILL_ITEM_UPDATE

```lua
TRADE_SKILL_ITEM_UPDATE(itemGUID: WOWGUID)
```

`SynchronousEvent`

### TRADE_SKILL_LIST_UPDATE

```lua
TRADE_SKILL_LIST_UPDATE()
```

`UniqueEvent`

### TRADE_SKILL_NAME_UPDATE

```lua
TRADE_SKILL_NAME_UPDATE()
```

`SynchronousEvent`

### TRADE_SKILL_SHOW

```lua
TRADE_SKILL_SHOW()
```

`SynchronousEvent`

### UPDATE_TRADESKILL_CAST_STOPPED

```lua
UPDATE_TRADESKILL_CAST_STOPPED(isScrapping: bool)
```

`UniqueEvent`
