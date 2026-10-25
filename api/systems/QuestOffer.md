# QuestOffer

Namespace `C_QuestOffer` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/questofferdocumentation.lua` (FileDataID 4637175)

## Functions

### GetHideRequiredItems

```lua
C_QuestOffer.GetHideRequiredItems() -> hideRequiredItems: bool
```

### GetQuestOfferMajorFactionReputationRewards

```lua
C_QuestOffer.GetQuestOfferMajorFactionReputationRewards() -> reputationRewards: QuestRewardReputationInfo[]
```

`MayReturnNothing`

### GetQuestRequiredCurrencyInfo

```lua
C_QuestOffer.GetQuestRequiredCurrencyInfo(questRewardIndex: luaIndex) -> questRequiredCurrencyInfo: QuestRequiredCurrencyInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetQuestRewardCurrencyInfo

```lua
C_QuestOffer.GetQuestRewardCurrencyInfo(questInfoType: cstring, questRewardIndex: luaIndex) -> questRewardCurrencyInfo: QuestRewardCurrencyInfo?
```

`SecretArguments=AllowedWhenUntainted`

## Events

### QUEST_ACCEPT_CONFIRM

```lua
QUEST_ACCEPT_CONFIRM(name: cstring, questTitle: cstring, questID: number)
```

`SynchronousEvent`

### QUEST_FINISHED

```lua
QUEST_FINISHED()
```

`SynchronousEvent`

### QUEST_GREETING

```lua
QUEST_GREETING()
```

`SynchronousEvent`

### QUEST_ITEM_UPDATE

```lua
QUEST_ITEM_UPDATE()
```

`SynchronousEvent`

### QUEST_PROGRESS

```lua
QUEST_PROGRESS()
```

`SynchronousEvent`

## Types

### QuestRequiredCurrencyInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `texture` | `fileID` |  |
| `name` | `cstring` |  |
| `currencyID` | `number` |  |
| `quality` | `number` |  |
| `requiredAmount` | `number` |  |
