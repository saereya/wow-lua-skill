# GarrisonShared

source `interface/addons/blizzard_apidocumentationgenerated/garrisonshareddocumentation.lua` (FileDataID 4637101)

## Types

### GarrisonAbilityEffect

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `description` | `cstring` |  |
| `icon` | `number` |  |
| `factor` | `number` |  |

### GarrisonFollowerAbilityInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `id` | `number` |  |
| `name` | `cstring` |  |
| `description` | `string` |  |
| `icon` | `number` |  |
| `isTrait` | `bool` |  |
| `isSpecialization` | `bool` |  |
| `temporary` | `bool` |  |
| `category` | `cstring?` |  |
| `counters` | `GarrisonAbilityEffect[]` |  |
| `isEmptySlot` | `bool` |  |

### GarrisonTalentCurrencyCostInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `currencyType` | `number` |  |
| `currencyQuantity` | `number` |  |

### GarrisonTalentInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `id` | `number` |  |
| `ability` | `GarrisonFollowerAbilityInfo` |  |
| `name` | `string` |  |
| `icon` | `number` |  |
| `tier` | `number` |  |
| `uiOrder` | `number` |  |
| `type` | `number` |  |
| `prerequisiteTalentID` | `number?` |  |
| `selected` | `bool` |  |
| `researched` | `bool` |  |
| `ignoreTalent` | `bool` |  |
| `researchDuration` | `time_t` |  |
| `startTime` | `time_t` |  |
| `timeRemaining` | `time_t` |  |
| `researchGoldCost` | `number` |  |
| `researchCurrencyCosts` | `GarrisonTalentCurrencyCostInfo[]` |  |
| `talentAvailability` | `GarrisonTalentAvailability` |  |
| `talentRank` | `number` |  |
| `talentMaxRank` | `number` |  |
| `isBeingResearched` | `bool` |  |
| `description` | `string` |  |
| `perkSpellID` | `number` |  |
| `researchDescription` | `string?` |  |
| `playerConditionReason` | `string?` |  |
| `socketInfo` | `GarrisonTalentSocketInfo` |  |
| `treeID` | `number` |  |

### GarrisonTalentSocketInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `socketType` | `number` |  |
| `socketSubtype` | `number` |  |
| `misc0` | `number` |  |
| `misc1` | `number` |  |

### GarrisonTalentTreeInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `treeID` | `number` |  |
| `title` | `cstring` |  |
| `textureKit` | `textureKit` |  |
| `talents` | `GarrisonTalentInfo[]` |  |
| `isClassAgnostic` | `bool` |  |
| `isThemed` | `bool` |  |
| `featureType` | `number` |  |
| `featureSubtype` | `number` |  |
