# QuestRewards

source `interface/addons/blizzard_apidocumentationgenerated/questrewardsdocumentation.lua` (FileDataID 4737046)

## Types

### QuestRewardCurrencyInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `texture` | `fileID` |  |
| `name` | `cstring` |  |
| `currencyID` | `number` |  |
| `quality` | `number` |  |
| `baseRewardAmount` | `number` |  |
| `bonusRewardAmount` | `number` |  |
| `totalRewardAmount` | `number` |  |
| `questRewardContextFlags` | `QuestRewardContextFlags?` |  |

### QuestRewardReputationInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `factionID` | `number` |  |
| `rewardAmount` | `number` |  |

### QuestRewardSpellInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `texture` | `fileID` |  |
| `name` | `cstring` |  |
| `garrFollowerID` | `number?` |  |
| `isTradeskill` | `bool` |  |
| `isSpellLearned` | `bool` |  |
| `hideSpellLearnText` | `bool` |  |
| `isBoostSpell` | `bool` |  |
| `genericUnlock` | `bool` |  |
| `type` | `QuestCompleteSpellType` |  |
