# QuestInfoSystem

Namespace `C_QuestInfoSystem` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/questinfosystemdocumentation.lua` (FileDataID 5142699)

## Functions

### GetQuestClassification

```lua
C_QuestInfoSystem.GetQuestClassification(questID: number?, questInfoID: number?) -> classification: QuestClassification
```

`SecretArguments=AllowedWhenUntainted`

### GetQuestHasShortExpirationWarning

```lua
C_QuestInfoSystem.GetQuestHasShortExpirationWarning(questID: number?) -> hasShortExpirationWarning: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetQuestLogRewardFavor

```lua
C_QuestInfoSystem.GetQuestLogRewardFavor(questID: number?, clampFavorToCycleCap: bool?) -> amount: number
```

`SecretArguments=AllowedWhenUntainted`

### GetQuestRewardCurrencies

```lua
C_QuestInfoSystem.GetQuestRewardCurrencies(questID: number?) -> questRewardCurrencyInfo: QuestRewardCurrencyInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetQuestRewardSpellInfo

```lua
C_QuestInfoSystem.GetQuestRewardSpellInfo(questID: number?, spellID: number) -> info: QuestRewardSpellInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetQuestRewardSpells

```lua
C_QuestInfoSystem.GetQuestRewardSpells(questID: number?) -> spellIDs: number[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetQuestShouldToastCompletion

```lua
C_QuestInfoSystem.GetQuestShouldToastCompletion(questID: number?) -> shouldToast: bool
```

`SecretArguments=AllowedWhenUntainted`

### HasQuestRewardCurrencies

```lua
C_QuestInfoSystem.HasQuestRewardCurrencies(questID: number?) -> hasQuestRewardCurrencies: bool
```

`SecretArguments=AllowedWhenUntainted`

### HasQuestRewardSpells

```lua
C_QuestInfoSystem.HasQuestRewardSpells(questID: number?) -> hasRewardSpells: bool
```

`SecretArguments=AllowedWhenUntainted`
