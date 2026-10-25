# QuestInfoShared

source `interface/addons/blizzard_apidocumentationgenerated/questinfoshareddocumentation.lua` (FileDataID 6029104)

## Types

### QuestClassification

*Enumeration* · 11 values, 0..10

Access values as `Enum.QuestClassification.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Important` | `QuestClassification` | = 0 |
| `Legendary` | `QuestClassification` | = 1 |
| `Campaign` | `QuestClassification` | = 2 |
| `Calling` | `QuestClassification` | = 3 |
| `Meta` | `QuestClassification` | = 4 |
| `Recurring` | `QuestClassification` | = 5 |
| `Questline` | `QuestClassification` | = 6 |
| `Normal` | `QuestClassification` | = 7 |
| `BonusObjective` | `QuestClassification` | = 8 |
| `Threat` | `QuestClassification` | = 9 |
| `WorldQuest` | `QuestClassification` | = 10 |

### QuestPOIMapInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `childDepth` | `number?` |  |
| `questTagType` | `QuestTagType?` |  |
| `questID` | `number` |  |
| `numObjectives` | `number` |  |
| `mapID` | `number` |  |
| `x` | `number` |  |
| `y` | `number` |  |
| `isQuestStart` | `bool` |  |
| `isDaily` | `bool` |  |
| `isCombatAllyQuest` | `bool` |  |
| `isMeta` | `bool` |  |
| `inProgress` | `bool` |  |
| `isMapIndicatorQuest` | `bool` |  |
