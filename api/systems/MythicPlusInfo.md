# MythicPlusInfo

Namespace `C_MythicPlus` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/mythicplusinfodocumentation.lua` (FileDataID 4637148)

## Functions

### GetCurrentAffixes

```lua
C_MythicPlus.GetCurrentAffixes() -> affixIDs: MythicPlusKeystoneAffix[]
```

`MayReturnNothing`

### GetCurrentSeason

```lua
C_MythicPlus.GetCurrentSeason() -> seasonID: number
```

### GetCurrentSeasonValues

```lua
C_MythicPlus.GetCurrentSeasonValues() -> displaySeasonID: number, milestoneSeasonID: number, rewardSeasonID: number
```

### GetCurrentUIDisplaySeason

```lua
C_MythicPlus.GetCurrentUIDisplaySeason() -> seasonID: number?
```

### GetEndOfRunGearSequenceLevel

```lua
C_MythicPlus.GetEndOfRunGearSequenceLevel(keystoneLevel: number) -> sequenceLevel: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetLastWeeklyBestInformation

```lua
C_MythicPlus.GetLastWeeklyBestInformation() -> challengeMapId: number, level: number
```

`MayReturnNothing`

### GetOwnedKeystoneChallengeMapID

```lua
C_MythicPlus.GetOwnedKeystoneChallengeMapID() -> challengeMapID: number
```

`MayReturnNothing`

### GetOwnedKeystoneLevel

```lua
C_MythicPlus.GetOwnedKeystoneLevel() -> keyStoneLevel: number
```

`MayReturnNothing`

### GetOwnedKeystoneMapID

```lua
C_MythicPlus.GetOwnedKeystoneMapID() -> mapID: number
```

`MayReturnNothing`

### GetRewardLevelForDifficultyLevel

```lua
C_MythicPlus.GetRewardLevelForDifficultyLevel(difficultyLevel: number) -> weeklyRewardLevel: number, endOfRunRewardLevel: number
```

`SecretArguments=AllowedWhenUntainted`

### GetRewardLevelFromKeystoneLevel

```lua
C_MythicPlus.GetRewardLevelFromKeystoneLevel(keystoneLevel: number) -> rewardLevel: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetRunHistory

```lua
C_MythicPlus.GetRunHistory(includePreviousWeeks: bool, includeIncompleteRuns: bool, currentSeasonOnly: bool) -> runs: MythicPlusRunInfo[]
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `includePreviousWeeks` | `bool` | default `false` |
| `includeIncompleteRuns` | `bool` | default `false` |
| `currentSeasonOnly` | `bool` | default `false` |

### GetSeasonBestAffixScoreInfoForMap

```lua
C_MythicPlus.GetSeasonBestAffixScoreInfoForMap(mapChallengeModeID: number) -> affixScores: MythicPlusAffixScoreInfo[], bestOverAllScore: number
```

Gets the active players best runs by the seasonal tracked affixes as well as their overall score for the current season.

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSeasonBestForMap

```lua
C_MythicPlus.GetSeasonBestForMap(mapChallengeModeID: number) -> intimeInfo: MapSeasonBestInfo?, overtimeInfo: MapSeasonBestInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetSeasonBestMythicRatingFromThisExpansion

```lua
C_MythicPlus.GetSeasonBestMythicRatingFromThisExpansion() -> bestSeasonScore: number, bestSeason: number
```

`MayReturnNothing`

### GetWeeklyBestForMap

```lua
C_MythicPlus.GetWeeklyBestForMap(mapChallengeModeID: number) -> durationSec: number, level: number, completionDate: CalendarTime, affixIDs: number[], members: MythicPlusMember[], dungeonScore: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetWeeklyChestRewardLevel

```lua
C_MythicPlus.GetWeeklyChestRewardLevel() -> currentWeekBestLevel: number, weeklyRewardLevel: number, nextDifficultyWeeklyRewardLevel: number, nextBestLevel: number
```

### IsMythicPlusActive

```lua
C_MythicPlus.IsMythicPlusActive() -> isMythicPlusActive: bool
```

### RequestCurrentAffixes

```lua
C_MythicPlus.RequestCurrentAffixes()
```

### RequestMapInfo

```lua
C_MythicPlus.RequestMapInfo()
```

### RequestRewards

```lua
C_MythicPlus.RequestRewards()
```

## Events

### MYTHIC_PLUS_CURRENT_AFFIX_UPDATE

```lua
MYTHIC_PLUS_CURRENT_AFFIX_UPDATE()
```

`SynchronousEvent`

### MYTHIC_PLUS_NEW_WEEKLY_RECORD

```lua
MYTHIC_PLUS_NEW_WEEKLY_RECORD(mapChallengeModeID: number, completionMilliseconds: number, level: number)
```

`SynchronousEvent`

## Types

### MapSeasonBestInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `durationSec` | `number` |  |
| `level` | `number` |  |
| `completionDate` | `CalendarTime` |  |
| `affixIDs` | `number[]` |  |
| `members` | `MythicPlusMember[]` |  |
| `dungeonScore` | `number` |  |

### MythicPlusDate

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `year` | `number` |  |
| `month` | `number` |  |
| `day` | `number` |  |
| `hour` | `number` |  |
| `minute` | `number` |  |
| `weekday` | `luaIndex` |  |

### MythicPlusKeystoneAffix

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `id` | `number` |  |
| `seasonID` | `number` |  |

### MythicPlusMember

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string?` |  |
| `specID` | `number` |  |
| `classID` | `number` |  |

### MythicPlusRunInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `mapChallengeModeID` | `number` |  |
| `level` | `number` |  |
| `thisWeek` | `bool` |  |
| `completed` | `bool` |  |
| `runScore` | `number` |  |
| `durationSec` | `number` |  |
| `completionDate` | `CalendarTime` |  |
| `season` | `number` |  |

### SeasonTimeInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `bestTime` | `number` |  |
| `lastTime` | `number` |  |
| `medal` | `number` |  |
