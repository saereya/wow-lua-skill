# QuestLineUI

Namespace `C_QuestLine` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/questlineinfodocumentation.lua` (FileDataID 4637167)

## Functions

### GetAvailableQuestLines

```lua
C_QuestLine.GetAvailableQuestLines(uiMapID: number) -> questLines: QuestLineInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetForceVisibleQuests

```lua
C_QuestLine.GetForceVisibleQuests(uiMapID: number) -> questIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetQuestLineInfo

```lua
C_QuestLine.GetQuestLineInfo(questID: number, uiMapID: number?, displayableOnly: bool) -> questLineInfo: QuestLineInfo?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `questID` | `number` |  |
| `uiMapID` | `number?` |  |
| `displayableOnly` | `bool` | default `false` |

### GetQuestLineQuests

```lua
C_QuestLine.GetQuestLineQuests(questLineID: number) -> questIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### IsComplete

```lua
C_QuestLine.IsComplete(questLineID: number) -> isComplete: bool
```

`SecretArguments=AllowedWhenUntainted`

### QuestLineIgnoresAccountCompletedFiltering

```lua
C_QuestLine.QuestLineIgnoresAccountCompletedFiltering(uiMapID: number, questLineID: number) -> questLineIgnoresAccountCompletedFiltering: bool
```

`SecretArguments=AllowedWhenUntainted`

### RequestQuestLinesForMap

```lua
C_QuestLine.RequestQuestLinesForMap(uiMapID: number)
```

`SecretArguments=AllowedWhenUntainted`

## Types

### QuestLineFloorLocation

*Enumeration* · 3 values, 0..2

Access values as `Enum.QuestLineFloorLocation.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Above` | `QuestLineFloorLocation` | = 0 |
| `Below` | `QuestLineFloorLocation` | = 1 |
| `Same` | `QuestLineFloorLocation` | = 2 |

### QuestLineInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `questLineName` | `cstring` |  |
| `questName` | `cstring` |  |
| `questLineID` | `number` |  |
| `questID` | `number` |  |
| `x` | `number` |  |
| `y` | `number` |  |
| `isHidden` | `bool` |  |
| `isLegendary` | `bool` |  |
| `isLocalStory` | `bool` |  |
| `isDaily` | `bool` |  |
| `isCampaign` | `bool` |  |
| `isImportant` | `bool` |  |
| `isAccountCompleted` | `bool` |  |
| `isCombatAllyQuest` | `bool` |  |
| `isMeta` | `bool` |  |
| `inProgress` | `bool` |  |
| `isQuestStart` | `bool` |  |
| `floorLocation` | `QuestLineFloorLocation` |  |
| `startMapID` | `number` |  |
