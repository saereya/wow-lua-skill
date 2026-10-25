# QuestTaskInfo

Namespace `C_TaskQuest` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/questtaskinfodocumentation.lua` (FileDataID 4637178)

## Functions

### DoesMapShowTaskQuestObjectives

```lua
C_TaskQuest.DoesMapShowTaskQuestObjectives(uiMapID: number) -> showsTaskQuestObjectives: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetQuestInfoByQuestID

```lua
C_TaskQuest.GetQuestInfoByQuestID(questID: number) -> questTitle: cstring, factionID: number?, capped: bool?, displayAsObjective: bool?
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetQuestLocation

```lua
C_TaskQuest.GetQuestLocation(questID: number, uiMapID: number) -> locationX: number, locationY: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetQuestProgressBarInfo

```lua
C_TaskQuest.GetQuestProgressBarInfo(questID: number) -> progress: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetQuestsOnMap

```lua
C_TaskQuest.GetQuestsOnMap(uiMapID: number) -> taskPOIs: QuestPOIMapInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetQuestTimeLeftMinutes

```lua
C_TaskQuest.GetQuestTimeLeftMinutes(questID: number) -> minutesLeft: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetQuestTimeLeftSeconds

```lua
C_TaskQuest.GetQuestTimeLeftSeconds(questID: number) -> secondsLeft: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetQuestUIWidgetSetByType

```lua
C_TaskQuest.GetQuestUIWidgetSetByType(questID: number, type: MapIconUIWidgetSetType) -> widgetSet: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetQuestZoneID

```lua
C_TaskQuest.GetQuestZoneID(questID: number) -> uiMapID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetThreatQuests

```lua
C_TaskQuest.GetThreatQuests() -> quests: number[]
```

### IsActive

```lua
C_TaskQuest.IsActive(questID: number) -> active: bool
```

`SecretArguments=AllowedWhenUntainted`

### RequestPreloadRewardData

```lua
C_TaskQuest.RequestPreloadRewardData(questID: number)
```

`SecretArguments=AllowedWhenUntainted`
