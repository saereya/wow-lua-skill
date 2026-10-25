# WeeklyRewards

Namespace `C_WeeklyRewards` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/weeklyrewardsdocumentation.lua` (FileDataID 4637303)

## Functions

### AreRewardsForCurrentRewardPeriod

```lua
C_WeeklyRewards.AreRewardsForCurrentRewardPeriod() -> isCurrentPeriod: bool
```

### CanClaimRewards

```lua
C_WeeklyRewards.CanClaimRewards() -> canClaimRewards: bool
```

### ClaimReward

```lua
C_WeeklyRewards.ClaimReward(id: number)
```

`SecretArguments=AllowedWhenUntainted`

### CloseInteraction

```lua
C_WeeklyRewards.CloseInteraction()
```

### GetActivities

```lua
C_WeeklyRewards.GetActivities(type: WeeklyRewardChestThresholdType?) -> activities: WeeklyRewardActivityInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetActivityEncounterInfo

```lua
C_WeeklyRewards.GetActivityEncounterInfo(type: WeeklyRewardChestThresholdType, index: luaIndex) -> info: WeeklyRewardActivityEncounterInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetConquestWeeklyProgress

```lua
C_WeeklyRewards.GetConquestWeeklyProgress() -> weeklyProgress: ConquestWeeklyProgress
```

### GetDifficultyIDForActivityTier

```lua
C_WeeklyRewards.GetDifficultyIDForActivityTier(activityTierID: number) -> difficultyID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetExampleRewardItemHyperlinks

```lua
C_WeeklyRewards.GetExampleRewardItemHyperlinks(id: number) -> hyperlink: string, upgradeHyperlink: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetItemHyperlink

```lua
C_WeeklyRewards.GetItemHyperlink(itemDBID: WeeklyRewardItemDBID) -> hyperlink: cstring
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetNextActivitiesIncrease

```lua
C_WeeklyRewards.GetNextActivitiesIncrease(activityTierID: number, level: number) -> hasSeasonData: bool, nextActivityTierID: number?, nextLevel: number?, itemLevel: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetNextMythicPlusIncrease

```lua
C_WeeklyRewards.GetNextMythicPlusIncrease(mythicPlusLevel: number) -> hasSeasonData: bool, nextMythicPlusLevel: number?, itemLevel: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetNumCompletedDungeonRuns

```lua
C_WeeklyRewards.GetNumCompletedDungeonRuns() -> numHeroic: number, numMythic: number, numMythicPlus: number
```

### GetSortedProgressForActivity

```lua
C_WeeklyRewards.GetSortedProgressForActivity(type: WeeklyRewardChestThresholdType, combineSharedDifficulty: bool) -> progress: WeeklyRewardActivityTierProgress[]
```

`SecretArguments=AllowedWhenUntainted`

### HasAvailableRewards

```lua
C_WeeklyRewards.HasAvailableRewards() -> hasAvailableRewards: bool
```

### HasGeneratedRewards

```lua
C_WeeklyRewards.HasGeneratedRewards() -> hasGeneratedRewards: bool
```

### HasInteraction

```lua
C_WeeklyRewards.HasInteraction() -> isInteracting: bool
```

### IsWeeklyChestRetired

```lua
C_WeeklyRewards.IsWeeklyChestRetired() -> isRetired: bool
```

### OnUIInteract

```lua
C_WeeklyRewards.OnUIInteract()
```

### ShouldShowFinalRetirementMessage

```lua
C_WeeklyRewards.ShouldShowFinalRetirementMessage() -> showRetirementMessage: bool
```

### ShouldShowRetirementMessage

```lua
C_WeeklyRewards.ShouldShowRetirementMessage() -> showRetirementMessage: bool
```

## Events

### WEEKLY_REWARDS_ITEM_CHANGED

```lua
WEEKLY_REWARDS_ITEM_CHANGED()
```

`SynchronousEvent`

### WEEKLY_REWARDS_UPDATE

```lua
WEEKLY_REWARDS_UPDATE()
```

`SynchronousEvent`

## Types

### ConquestProgressBarDisplayType

*Enumeration* · 3 values, 0..2

Access values as `Enum.ConquestProgressBarDisplayType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `FirstChest` | `ConquestProgressBarDisplayType` | = 0 |
| `AdditionalChest` | `ConquestProgressBarDisplayType` | = 1 |
| `Seasonal` | `ConquestProgressBarDisplayType` | = 2 |

### ConquestWeeklyProgress

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `progress` | `number` |  |
| `maxProgress` | `number` |  |
| `displayType` | `ConquestProgressBarDisplayType` |  |
| `unlocksCompleted` | `number` |  |
| `maxUnlocks` | `number` |  |
| `sampleItemHyperlink` | `string` |  |

### WeeklyRewardActivityEncounterInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `encounterID` | `number` |  |
| `bestDifficulty` | `number` |  |
| `uiOrder` | `number` |  |
| `instanceID` | `number` |  |

### WeeklyRewardActivityInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `type` | `WeeklyRewardChestThresholdType` |  |
| `index` | `luaIndex` |  |
| `threshold` | `number` |  |
| `progress` | `number` |  |
| `id` | `number` |  |
| `activityTierID` | `number` |  |
| `level` | `number` |  |
| `claimID` | `number?` |  |
| `raidString` | `cstring?` |  |
| `rewards` | `WeeklyRewardActivityRewardInfo[]` |  |

### WeeklyRewardActivityRewardInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `type` | `CachedRewardType` |  |
| `id` | `number` |  |
| `quantity` | `number` |  |
| `itemDBID` | `WeeklyRewardItemDBID?` |  |

### WeeklyRewardActivityTierProgress

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `activityTierID` | `number` |  |
| `difficulty` | `number` |  |
| `numPoints` | `number` |  |
