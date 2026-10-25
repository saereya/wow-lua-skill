# TooltipInfoShared

source `interface/addons/blizzard_apidocumentationgenerated/tooltipinfoshareddocumentation.lua` (FileDataID 4763884)

## Types

### TooltipDataItemBinding

*Enumeration* · 11 values, 0..10

Access values as `Enum.TooltipDataItemBinding.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Quest` | `TooltipDataItemBinding` | = 0 |
| `Account` | `TooltipDataItemBinding` | = 1 |
| `BnetAccount` | `TooltipDataItemBinding` | = 2 |
| `Soulbound` | `TooltipDataItemBinding` | = 3 |
| `BindToAccount` | `TooltipDataItemBinding` | = 4 |
| `BindToBnetAccount` | `TooltipDataItemBinding` | = 5 |
| `BindOnPickup` | `TooltipDataItemBinding` | = 6 |
| `BindOnEquip` | `TooltipDataItemBinding` | = 7 |
| `BindOnUse` | `TooltipDataItemBinding` | = 8 |
| `AccountUntilEquipped` | `TooltipDataItemBinding` | = 9 |
| `BindToAccountUntilEquipped` | `TooltipDataItemBinding` | = 10 |

### TooltipDataLineType

*Enumeration* · 52 values, 0..51

Access values as `Enum.TooltipDataLineType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `TooltipDataLineType` | = 0 |
| `Blank` | `TooltipDataLineType` | = 1 |
| `UnitName` | `TooltipDataLineType` | = 2 |
| `GemSocket` | `TooltipDataLineType` | = 3 |
| `AzeriteEssenceSlot` | `TooltipDataLineType` | = 4 |
| `AzeriteEssencePower` | `TooltipDataLineType` | = 5 |
| `LearnableSpell` | `TooltipDataLineType` | = 6 |
| `UnitThreat` | `TooltipDataLineType` | = 7 |
| `QuestObjective` | `TooltipDataLineType` | = 8 |
| `AzeriteItemPowerDescription` | `TooltipDataLineType` | = 9 |
| `RuneforgeLegendaryPowerDescription` | `TooltipDataLineType` | = 10 |
| `SellPrice` | `TooltipDataLineType` | = 11 |
| `ProfessionCraftingQuality` | `TooltipDataLineType` | = 12 |
| `SpellName` | `TooltipDataLineType` | = 13 |
| `CurrencyTotal` | `TooltipDataLineType` | = 14 |
| `ItemEnchantmentPermanent` | `TooltipDataLineType` | = 15 |
| `UnitOwner` | `TooltipDataLineType` | = 16 |
| `QuestTitle` | `TooltipDataLineType` | = 17 |
| `QuestPlayer` | `TooltipDataLineType` | = 18 |
| `NestedBlock` | `TooltipDataLineType` | = 19 |
| `ItemBinding` | `TooltipDataLineType` | = 20 |
| `EquipSlot` | `TooltipDataLineType` | = 21 |
| `ItemName` | `TooltipDataLineType` | = 22 |
| `Separator` | `TooltipDataLineType` | = 23 |
| `ToyName` | `TooltipDataLineType` | = 24 |
| `ToyText` | `TooltipDataLineType` | = 25 |
| `ToyEffect` | `TooltipDataLineType` | = 26 |
| `ToyDuration` | `TooltipDataLineType` | = 27 |
| `ToyDescription` | `TooltipDataLineType` | = 28 |
| `ToySource` | `TooltipDataLineType` | = 29 |
| `GemSocketEnchantment` | `TooltipDataLineType` | = 30 |
| `ItemLevel` | `TooltipDataLineType` | = 31 |
| `ItemUpgradeLevel` | `TooltipDataLineType` | = 32 |
| `SpellPassive` | `TooltipDataLineType` | = 33 |
| `SpellDescription` | `TooltipDataLineType` | = 34 |
| `ItemQuality` | `TooltipDataLineType` | = 35 |
| `TradeTimeRemaining` | `TooltipDataLineType` | = 36 |
| `FlavorText` | `TooltipDataLineType` | = 37 |
| `ItemSpellTriggerLearn` | `TooltipDataLineType` | = 38 |
| `LearnTransmogSet` | `TooltipDataLineType` | = 39 |
| `LearnTransmogIllusion` | `TooltipDataLineType` | = 40 |
| `ErrorLine` | `TooltipDataLineType` | = 41 |
| `DisabledLine` | `TooltipDataLineType` | = 42 |
| `UsageRequirement` | `TooltipDataLineType` | = 43 |
| `ItemSpellTriggerOnUse` | `TooltipDataLineType` | = 44 |
| `ItemSpellTriggerOnEquip` | `TooltipDataLineType` | = 45 |
| `ItemSpellTriggerOnProc` | `TooltipDataLineType` | = 46 |
| `UnitLevel` | `TooltipDataLineType` | = 47 |
| `UnitType` | `TooltipDataLineType` | = 48 |
| `UnitDead` | `TooltipDataLineType` | = 49 |
| `UnitCriteriaProgress` | `TooltipDataLineType` | = 50 |
| `AuraCaster` | `TooltipDataLineType` | = 51 |

### TooltipDataType

*Enumeration* · 28 values, 0..27

Access values as `Enum.TooltipDataType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Item` | `TooltipDataType` | = 0 |
| `Spell` | `TooltipDataType` | = 1 |
| `Unit` | `TooltipDataType` | = 2 |
| `Corpse` | `TooltipDataType` | = 3 |
| `Object` | `TooltipDataType` | = 4 |
| `Currency` | `TooltipDataType` | = 5 |
| `BattlePet` | `TooltipDataType` | = 6 |
| `UnitAura` | `TooltipDataType` | = 7 |
| `AzeriteEssence` | `TooltipDataType` | = 8 |
| `CompanionPet` | `TooltipDataType` | = 9 |
| `Mount` | `TooltipDataType` | = 10 |
| `PetAction` | `TooltipDataType` | = 11 |
| `Achievement` | `TooltipDataType` | = 12 |
| `EnhancedConduit` | `TooltipDataType` | = 13 |
| `EquipmentSet` | `TooltipDataType` | = 14 |
| `InstanceLock` | `TooltipDataType` | = 15 |
| `PvPBrawl` | `TooltipDataType` | = 16 |
| `RecipeRankInfo` | `TooltipDataType` | = 17 |
| `Totem` | `TooltipDataType` | = 18 |
| `Toy` | `TooltipDataType` | = 19 |
| `CorruptionCleanser` | `TooltipDataType` | = 20 |
| `MinimapMouseover` | `TooltipDataType` | = 21 |
| `Flyout` | `TooltipDataType` | = 22 |
| `Quest` | `TooltipDataType` | = 23 |
| `QuestPartyProgress` | `TooltipDataType` | = 24 |
| `Macro` | `TooltipDataType` | = 25 |
| `Debug` | `TooltipDataType` | = 26 |
| `Outfit` | `TooltipDataType` | = 27 |

### TooltipDataUsageRequirementType

*Enumeration* · 17 values, 0..16

Access values as `Enum.TooltipDataUsageRequirementType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `RaceClass` | `TooltipDataUsageRequirementType` | = 0 |
| `Faction` | `TooltipDataUsageRequirementType` | = 1 |
| `Skill` | `TooltipDataUsageRequirementType` | = 2 |
| `PvPMedal` | `TooltipDataUsageRequirementType` | = 3 |
| `Reputation` | `TooltipDataUsageRequirementType` | = 4 |
| `Level` | `TooltipDataUsageRequirementType` | = 5 |
| `Guild` | `TooltipDataUsageRequirementType` | = 6 |
| `Achievement` | `TooltipDataUsageRequirementType` | = 7 |
| `PvPRank` | `TooltipDataUsageRequirementType` | = 8 |
| `EquippedItem` | `TooltipDataUsageRequirementType` | = 9 |
| `ShapeshiftForm` | `TooltipDataUsageRequirementType` | = 10 |
| `ArenaRating` | `TooltipDataUsageRequirementType` | = 11 |
| `EarnCurrency` | `TooltipDataUsageRequirementType` | = 12 |
| `Specialization` | `TooltipDataUsageRequirementType` | = 13 |
| `NotAlreadyKnown` | `TooltipDataUsageRequirementType` | = 14 |
| `NotInArena` | `TooltipDataUsageRequirementType` | = 15 |
| `NotInRatedBg` | `TooltipDataUsageRequirementType` | = 16 |

### TooltipComparisonLine

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `text` | `string` |  |
| `color` | `colorRGB` | `Mixin=ColorMixin` |

### TooltipDataArg

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `field` | `string` |  |
| `stringVal` | `string?` |  |
| `intVal` | `number?` |  |
| `floatVal` | `number?` |  |
| `boolVal` | `bool?` |  |
| `colorVal` | `colorRGB?` | `Mixin=ColorMixin` |
| `guidVal` | `WOWGUID?` |  |
