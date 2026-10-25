# DelvesConstants

source `interface/addons/blizzard_apidocumentationgenerated/delvesconstantsdocumentation.lua` (FileDataID 5910530)

## Types

### CompanionConfigSlotTypes

*Enumeration* · 4 values, 0..3

Access values as `Enum.CompanionConfigSlotTypes.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Role` | `CompanionConfigSlotTypes` | = 0 |
| `Utility` | `CompanionConfigSlotTypes` | = 1 |
| `Combat` | `CompanionConfigSlotTypes` | = 2 |
| `Flavor` | `CompanionConfigSlotTypes` | = 3 |

### CurioRarity

*Enumeration* · 5 values, 1..5

Access values as `Enum.CurioRarity.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Common` | `CurioRarity` | = 1 |
| `Uncommon` | `CurioRarity` | = 2 |
| `Rare` | `CurioRarity` | = 3 |
| `Epic` | `CurioRarity` | = 4 |
| `EpicTier2` | `CurioRarity` | = 5 |

### PlayerCompanionInfoFlags

*Enumeration* · 1 values, 1..1

Access values as `Enum.PlayerCompanionInfoFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `IgnoreSeasonInScenarios` | `PlayerCompanionInfoFlags` | = 1 |

### TieredEntranceTierFlag

*Enumeration* · 3 values, 0..2

Access values as `Enum.TieredEntranceTierFlag.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `TieredEntranceTierFlag` | = 0 |
| `IsLFG` | `TieredEntranceTierFlag` | = 1 |
| `DisableTraitSystem` | `TieredEntranceTierFlag` | = 2 |

### TieredEntranceType

*Enumeration* · 7 values, 0..6

Access values as `Enum.TieredEntranceType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Invalid` | `TieredEntranceType` | = 0 |
| `Delve` | `TieredEntranceType` | = 1 |
| `Sites` | `TieredEntranceType` | = 2 |
| `WorldTier` | `TieredEntranceType` | = 3 |
| `Lairs` | `TieredEntranceType` | = 4 |
| `Placeholder_5` | `TieredEntranceType` | = 5 |
| `Placeholder_6` | `TieredEntranceType` | = 6 |

### WorldTierDifficulty

*Enumeration* · 3 values, 1..3

Access values as `Enum.WorldTierDifficulty.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Normal` | `WorldTierDifficulty` | = 1 |
| `Heroic` | `WorldTierDifficulty` | = 2 |
| `Mythic` | `WorldTierDifficulty` | = 3 |

### DelveAssistActionData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `assistedPlayer` | `string` |  |
| `mapName` | `cstring?` |  |
| `creatureName` | `cstring?` |  |
| `receivedSpellID` | `number?` |  |
| `assistAction` | `AssistActionType` |  |

### DelvesConsts

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `DELVES_MIN_PLAYER_LEVEL_CONTENT_TUNING_ID` | `number` | = `2677` |
| `DELVES_NORMAL_KEY_CURRENCY_ID` | `number` | = `3028` |
| `DELVES_COMPANION_INFO_SELECTION_CHARACTER_DATA_ELEMENT_ID` | `number` | = `13` |
| `DELVES_COMPANION_TOOLTIP_WIDGET_SET_ID` | `number` | = `1331` |
| `DELVES_COMPANION_BRANN_CREATURE_ID` | `number` | = `210759` |
| `DELVES_COMPANION_VALEERA_CREATURE_ID` | `number` | = `248567` |

### TieredEntranceConsts

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `TIERED_ENTRANCE_TIER_SCORE_VALUE_TIER_LEVEL` | `number` | = `1` |
| `TIERED_ENTRANCE_TIER_SCORE_VALUE_MAP_ID` | `number` | = `3` |
| `TIERED_ENTRANCE_TIER_SCORE_VALUE_PLAYER_CONDITION_ID` | `number` | = `6` |
| `TIERED_ENTRANCE_INFO_WORLD_TIER_DIFFICULTY_CHARACTER_ELEMENT_ID` | `number` | = `522` |
