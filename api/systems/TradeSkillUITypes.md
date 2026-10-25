# TradeSkillUITypes

source `interface/addons/blizzard_apidocumentationgenerated/tradeskilluitypesdocumentation.lua` (FileDataID 4637269)

## Types

### CraftingReagentItemFlag

*Enumeration* · 1 values, 1..1

Access values as `Enum.CraftingReagentItemFlag.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `TooltipShowsAsStatModifications` | `CraftingReagentItemFlag` | = 1 |

### RecipeRequirementType

*Enumeration* · 3 values, 0..2

Access values as `Enum.RecipeRequirementType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `SpellFocus` | `RecipeRequirementType` | = 0 |
| `Totem` | `RecipeRequirementType` | = 1 |
| `Area` | `RecipeRequirementType` | = 2 |

### TradeskillOrderDuration

*Enumeration* · 3 values, 1..3

Access values as `Enum.TradeskillOrderDuration.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Short` | `TradeskillOrderDuration` | = 1 |
| `Medium` | `TradeskillOrderDuration` | = 2 |
| `Long` | `TradeskillOrderDuration` | = 3 |

### TradeskillOrderRecipient

*Enumeration* · 3 values, 1..3

Access values as `Enum.TradeskillOrderRecipient.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Public` | `TradeskillOrderRecipient` | = 1 |
| `Guild` | `TradeskillOrderRecipient` | = 2 |
| `Private` | `TradeskillOrderRecipient` | = 3 |

### TradeskillOrderStatus

*Enumeration* · 4 values, 1..4

Access values as `Enum.TradeskillOrderStatus.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Unclaimed` | `TradeskillOrderStatus` | = 1 |
| `Started` | `TradeskillOrderStatus` | = 2 |
| `Completed` | `TradeskillOrderStatus` | = 3 |
| `Expired` | `TradeskillOrderStatus` | = 4 |

### TradeskillRecipeType

*Enumeration* · 4 values, 1..4

Access values as `Enum.TradeskillRecipeType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Item` | `TradeskillRecipeType` | = 1 |
| `Salvage` | `TradeskillRecipeType` | = 2 |
| `Enchant` | `TradeskillRecipeType` | = 3 |
| `Gathering` | `TradeskillRecipeType` | = 4 |

### TradeskillRelativeDifficulty

*Enumeration* · 4 values, 0..3

Access values as `Enum.TradeskillRelativeDifficulty.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Optimal` | `TradeskillRelativeDifficulty` | = 0 |
| `Medium` | `TradeskillRelativeDifficulty` | = 1 |
| `Easy` | `TradeskillRelativeDifficulty` | = 2 |
| `Trivial` | `TradeskillRelativeDifficulty` | = 3 |

### TradeskillSlotDataType

*Enumeration* · 3 values, 1..3

Access values as `Enum.TradeskillSlotDataType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Reagent` | `TradeskillSlotDataType` | = 1 |
| `ModifiedReagent` | `TradeskillSlotDataType` | = 2 |
| `Currency` | `TradeskillSlotDataType` | = 3 |

### CraftingCurrencyResultData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `currencyID` | `number` | default `0` |
| `quantity` | `number` | default `0` |
| `operationID` | `number` | default `0` |
| `firstCraftReward` | `bool` | default `false` |
| `showCurrencyText` | `bool` | default `true` |

### CraftingItemResultData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `resourcesReturned` | `CraftingResourceReturnInfo[]?` |  |
| `craftingQuality` | `number?` |  |
| `qualityProgress` | `number` | default `0` |
| `itemID` | `number` | default `0` |
| `itemGUID` | `WOWGUID` |  |
| `quantity` | `number` | default `0` |
| `hyperlink` | `string` |  |
| `isCrit` | `bool` | default `false` |
| `critBonusSkill` | `number` | default `0` |
| `recraftable` | `bool` | default `false` |
| `bonusCraft` | `bool` | default `false` |
| `multicraft` | `number` | default `0` |
| `operationID` | `number` | default `0` |
| `firstCraftReward` | `bool` | default `false` |
| `isEnchant` | `bool` | default `false` |
| `hasIngenuityProc` | `bool` | default `false` |
| `concentrationCurrencyID` | `number` | default `0` |
| `concentrationSpent` | `number` | default `0` |
| `ingenuityRefund` | `number` | default `0` |

### CraftingItemSlotModification

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `dataSlotIndex` | `luaIndex` |  |
| `reagent` | `CraftingReagent` |  |

### CraftingOperationBonusStatInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `bonusStatName` | `string` |  |
| `bonusStatValue` | `number` |  |
| `ratingDescription` | `string` |  |
| `ratingPct` | `number` |  |
| `bonusRatingPct` | `number` |  |

### CraftingOperationInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `recipeID` | `number` |  |
| `baseDifficulty` | `number` |  |
| `bonusDifficulty` | `number` |  |
| `baseSkill` | `number` |  |
| `bonusSkill` | `number` |  |
| `isQualityCraft` | `bool` |  |
| `quality` | `number` |  |
| `craftingQuality` | `number` |  |
| `craftingQualityID` | `number` |  |
| `craftingDataID` | `number` |  |
| `lowerSkillThreshold` | `number` |  |
| `upperSkillTreshold` | `number` |  |
| `guaranteedCraftingQualityID` | `number` |  |
| `bonusStats` | `CraftingOperationBonusStatInfo[]` |  |
| `concentrationCurrencyID` | `number` |  |
| `concentrationCost` | `number` |  |
| `ingenuityRefund` | `number` |  |

### CraftingQualityInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `quality` | `number` |  |
| `icon` | `textureAtlas` |  |
| `iconSmall` | `textureAtlas` |  |
| `iconInventory` | `textureAtlas` |  |
| `iconMixed` | `textureAtlas` |  |
| `iconAppear` | `textureAtlas` |  |
| `iconDissolve` | `textureAtlas` |  |
| `barFill` | `textureAtlas` |  |
| `barBackground` | `textureAtlas` |  |
| `barBackgroundCap` | `textureAtlas` |  |
| `barHighlight` | `textureAtlas` |  |
| `iconChat` | `textureAtlas` |  |
| `iconQuestObjective` | `textureAtlas` |  |

### CraftingReagent

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `itemID` | `number?` |  |
| `currencyID` | `number?` |  |

### CraftingReagentInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `reagent` | `CraftingReagent` |  |
| `dataSlotIndex` | `luaIndex` |  |
| `quantity` | `number` |  |

### CraftingReagentSlotInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `mcrSlotID` | `number` |  |
| `requiredSkillRank` | `number` |  |
| `slotText` | `cstring?` |  |

### CraftingReagentSlotSchematic

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `reagents` | `CraftingReagent[]` |  |
| `reagentType` | `CraftingReagentType` |  |
| `variableQuantities` | `CraftingVariableQuantities[]` |  |
| `quantityRequired` | `number` |  |
| `slotInfo` | `CraftingReagentSlotInfo?` |  |
| `dataSlotType` | `TradeskillSlotDataType` | default `"Reagent"` |
| `dataSlotIndex` | `luaIndex` |  |
| `slotIndex` | `luaIndex` |  |
| `orderSource` | `CraftingOrderReagentSource?` |  |
| `required` | `bool` |  |
| `hiddenInCraftingForm` | `bool` |  |

### CraftingRecipeOutputInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `icon` | `number` |  |
| `hyperlink` | `cstring?` |  |
| `itemID` | `number?` |  |

### CraftingRecipeRequirement

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `met` | `bool` |  |
| `type` | `RecipeRequirementType` |  |

### CraftingRecipeSchematic

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `recipeID` | `number` |  |
| `icon` | `number` |  |
| `quantityMin` | `number` |  |
| `quantityMax` | `number` |  |
| `name` | `cstring` |  |
| `recipeType` | `TradeskillRecipeType` | default `"Item"` |
| `productQuality` | `number?` |  |
| `outputItemID` | `number?` |  |
| `reagentSlotSchematics` | `CraftingReagentSlotSchematic[]` |  |
| `isRecraft` | `bool` |  |
| `hasCraftingOperationInfo` | `bool` |  |

### CraftingRecipeSkillLineInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `professionSkillLineID` | `number` |  |
| `expansionSkillLineID` | `number` |  |

### CraftingResourceReturnInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `reagent` | `CraftingReagent` |  |
| `quantity` | `number` |  |

### CraftingTargetItem

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `itemID` | `number` |  |
| `itemGUID` | `WOWGUID` |  |
| `hyperlink` | `string?` |  |
| `quantity` | `number` |  |

### CraftingVariableQuantities

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `reagent` | `CraftingReagent` |  |
| `quantity` | `number` |  |

### GatheringOperationBonusStatInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `bonusStatName` | `string` |  |
| `bonusStatValue` | `number` |  |
| `ratingDescription` | `string` |  |
| `ratingPct` | `number` |  |
| `bonusRatingPct` | `number` |  |

### GatheringOperationInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `number` |  |
| `maxDifficulty` | `number` |  |
| `baseSkill` | `number` |  |
| `bonusSkill` | `number` |  |
| `bonusStats` | `GatheringOperationBonusStatInfo[]` |  |

### ProfessionInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `profession` | `Profession?` |  |
| `professionID` | `number` |  |
| `sourceCounter` | `number` |  |
| `professionName` | `cstring` |  |
| `expansionName` | `cstring` |  |
| `skillLevel` | `number` |  |
| `maxSkillLevel` | `number` |  |
| `skillModifier` | `number` |  |
| `isPrimaryProfession` | `bool` |  |
| `parentProfessionID` | `number?` |  |
| `parentProfessionName` | `cstring?` |  |

### RegularReagentInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `reagent` | `CraftingReagent` |  |
| `quantity` | `number` |  |

### TradeSkillRecipeInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `categoryID` | `number` |  |
| `name` | `cstring` |  |
| `relativeDifficulty` | `TradeskillRelativeDifficulty?` |  |
| `maxTrivialLevel` | `number` |  |
| `itemLevel` | `number` |  |
| `alternateVerb` | `cstring?` |  |
| `numSkillUps` | `number` |  |
| `canSkillUp` | `bool` |  |
| `firstCraft` | `bool` |  |
| `sourceType` | `number?` |  |
| `learned` | `bool` |  |
| `disabled` | `bool` |  |
| `favorite` | `bool` |  |
| `supportsQualities` | `bool` |  |
| `craftable` | `bool` | default `true` |
| `disabledReason` | `cstring?` |  |
| `recipeID` | `number` |  |
| `skillLineAbilityID` | `number` |  |
| `previousRecipeID` | `number?` |  |
| `nextRecipeID` | `number?` |  |
| `icon` | `number?` |  |
| `hyperlink` | `cstring?` |  |
| `currentRecipeExperience` | `number?` |  |
| `nextLevelRecipeExperience` | `number?` |  |
| `unlockedRecipeLevel` | `number?` |  |
| `earnedExperience` | `number?` |  |
| `supportsCraftingStats` | `bool` | default `false` |
| `hasSingleItemOutput` | `bool` | default `false` |
| `qualityItemIDs` | `number[]?` |  |
| `qualityIlvlBonuses` | `number[]?` |  |
| `alwaysUsesLowestQuality` | `bool` | default `false` |
| `maxQuality` | `number?` |  |
| `qualityIDs` | `number[]?` |  |
| `canCreateMultiple` | `bool` | default `true` |
| `abilityVerb` | `cstring?` |  |
| `abilityAllVerb` | `cstring?` |  |
| `isRecraft` | `bool` | default `false` |
| `isDummyRecipe` | `bool` | default `false` |
| `isGatheringRecipe` | `bool` | default `false` |
| `isEnchantingRecipe` | `bool` | default `false` |
| `isSalvageRecipe` | `bool` | default `false` |
