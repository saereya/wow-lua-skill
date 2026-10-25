# ChallengeModeInfo

Namespace `C_ChallengeMode` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/challengemodeinfodocumentation.lua` (FileDataID 4637053)

## Functions

### CanUseKeystoneInCurrentMap

```lua
C_ChallengeMode.CanUseKeystoneInCurrentMap(itemLocation: ItemLocation) -> canUse: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### ClearKeystone

```lua
C_ChallengeMode.ClearKeystone()
```

### CloseKeystoneFrame

```lua
C_ChallengeMode.CloseKeystoneFrame()
```

### GetActiveChallengeMapID

```lua
C_ChallengeMode.GetActiveChallengeMapID() -> mapChallengeModeID: number?
```

### GetActiveKeystoneInfo

```lua
C_ChallengeMode.GetActiveKeystoneInfo() -> activeKeystoneLevel: number, activeAffixIDs: number[], wasActiveKeystoneCharged: bool
```

### GetAffixInfo

```lua
C_ChallengeMode.GetAffixInfo(affixID: number) -> name: cstring, description: cstring, filedataid: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetChallengeCompletionInfo

```lua
C_ChallengeMode.GetChallengeCompletionInfo() -> info: ChallengeCompletionInfo
```

### GetDeathCount

```lua
C_ChallengeMode.GetDeathCount() -> numDeaths: number, timeLost: number
```

`MayReturnNothing`

### GetDungeonScoreRarityColor

```lua
C_ChallengeMode.GetDungeonScoreRarityColor(dungeonScore: number) -> scoreColor: colorRGB
```

Returns a color value from the passed in overall season M+ rating.

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `scoreColor` | `colorRGB` | `Mixin=ColorMixin` |

### GetGuildLeaders

```lua
C_ChallengeMode.GetGuildLeaders() -> topAttempt: ChallengeModeGuildTopAttempt[]
```

`MayReturnNothing`

### GetKeystoneLevelRarityColor

```lua
C_ChallengeMode.GetKeystoneLevelRarityColor(level: number) -> levelScore: colorRGB
```

Returns a color value from the passed in keystone level.

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `levelScore` | `colorRGB` | `Mixin=ColorMixin` |

### GetLeaverPenaltyWarningTimeLeft

```lua
C_ChallengeMode.GetLeaverPenaltyWarningTimeLeft() -> timeLeftSeconds: number
```

Returns how much time is left before player is automatically flagged as a leaver (and removed from the group) for exiting a restricted challenge mode instance

Returns:

| Name | Type | Notes |
|---|---|---|
| `timeLeftSeconds` | `number` | default `0` |

### GetMapScoreInfo

```lua
C_ChallengeMode.GetMapScoreInfo() -> displayScores: MythicPlusRatingLinkInfo[]
```

`MayReturnNothing`

### GetMapTable

```lua
C_ChallengeMode.GetMapTable() -> mapChallengeModeIDs: number[]
```

### GetMapUIInfo

```lua
C_ChallengeMode.GetMapUIInfo(mapChallengeModeID: number) -> name: cstring, id: number, timeLimit: number, texture: number?, backgroundTexture: number, mapID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetOverallDungeonScore

```lua
C_ChallengeMode.GetOverallDungeonScore() -> overallDungeonScore: number
```

Gets the overall season mythic+ rating for the player.

### GetPowerLevelDamageHealthMod

```lua
C_ChallengeMode.GetPowerLevelDamageHealthMod(powerLevel: number) -> damageMod: number, healthMod: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSlottedKeystoneInfo

```lua
C_ChallengeMode.GetSlottedKeystoneInfo() -> mapChallengeModeID: number, affixIDs: number[], keystoneLevel: number
```

`MayReturnNothing`

### GetSpecificDungeonOverallScoreRarityColor

```lua
C_ChallengeMode.GetSpecificDungeonOverallScoreRarityColor(specificDungeonOverallScore: number) -> specificDungeonOverallScoreColor: colorRGB
```

Returns a color value from the passed in mythic+ rating from the combined affix scores for a specific dungeon

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `specificDungeonOverallScoreColor` | `colorRGB` | `Mixin=ColorMixin` |

### GetSpecificDungeonScoreRarityColor

```lua
C_ChallengeMode.GetSpecificDungeonScoreRarityColor(specificDungeonScore: number) -> specificDungeonScoreColor: colorRGB
```

Returns a color value from the passed in mythic+ rating for a specific dungeon.

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `specificDungeonScoreColor` | `colorRGB` | `Mixin=ColorMixin` |

### GetStartTime

```lua
C_ChallengeMode.GetStartTime() -> startTime: number
```

### HasSlottedKeystone

```lua
C_ChallengeMode.HasSlottedKeystone() -> hasSlottedKeystone: bool
```

### IsChallengeModeActive

```lua
C_ChallengeMode.IsChallengeModeActive() -> challengeModeActive: bool
```

### IsChallengeModeResettable

```lua
C_ChallengeMode.IsChallengeModeResettable() -> canReset: bool
```

### RemoveKeystone

```lua
C_ChallengeMode.RemoveKeystone() -> removalSuccessful: bool
```

### RequestLeaders

```lua
C_ChallengeMode.RequestLeaders(mapChallengeModeID: number)
```

`SecretArguments=AllowedWhenUntainted`

### Reset

```lua
C_ChallengeMode.Reset()
```

### SlotKeystone

```lua
C_ChallengeMode.SlotKeystone()
```

### StartChallengeMode

```lua
C_ChallengeMode.StartChallengeMode() -> success: bool
```

## Events

### CHALLENGE_MODE_COMPLETED

```lua
CHALLENGE_MODE_COMPLETED()
```

`SynchronousEvent`

### CHALLENGE_MODE_COMPLETED_REWARDS

```lua
CHALLENGE_MODE_COMPLETED_REWARDS(mapID: number, medal: number, timeMS: number, money: number, rewards: ChallengeModeReward[])
```

`SynchronousEvent`

### CHALLENGE_MODE_DEATH_COUNT_UPDATED

```lua
CHALLENGE_MODE_DEATH_COUNT_UPDATED()
```

`SynchronousEvent`

### CHALLENGE_MODE_KEYSTONE_RECEPTABLE_OPEN

```lua
CHALLENGE_MODE_KEYSTONE_RECEPTABLE_OPEN()
```

`SynchronousEvent`

### CHALLENGE_MODE_KEYSTONE_SLOTTED

```lua
CHALLENGE_MODE_KEYSTONE_SLOTTED(keystoneID: number)
```

`SynchronousEvent`

### CHALLENGE_MODE_LEADERBOARD_RESULT

```lua
CHALLENGE_MODE_LEADERBOARD_RESULT(mapID: number, challengeModeID: number, page: number, results: MythicPlusLeaderboardResult[])
```

`SynchronousEvent`

### CHALLENGE_MODE_LEADERS_UPDATE

```lua
CHALLENGE_MODE_LEADERS_UPDATE()
```

`SynchronousEvent`

### CHALLENGE_MODE_LEAVER_TIMER_ENDED

```lua
CHALLENGE_MODE_LEAVER_TIMER_ENDED()
```

`SynchronousEvent`

### CHALLENGE_MODE_LEAVER_TIMER_STARTED

```lua
CHALLENGE_MODE_LEAVER_TIMER_STARTED()
```

`SynchronousEvent`

### CHALLENGE_MODE_MAPS_UPDATE

```lua
CHALLENGE_MODE_MAPS_UPDATE()
```

`SynchronousEvent`

### CHALLENGE_MODE_MEMBER_INFO_UPDATED

```lua
CHALLENGE_MODE_MEMBER_INFO_UPDATED()
```

`SynchronousEvent`

### CHALLENGE_MODE_NEW_RECORD

```lua
CHALLENGE_MODE_NEW_RECORD(mapID: number, timeMS: number, medal: number)
```

`SynchronousEvent`

### CHALLENGE_MODE_RESET

```lua
CHALLENGE_MODE_RESET(mapID: number)
```

`SynchronousEvent`

### CHALLENGE_MODE_START

```lua
CHALLENGE_MODE_START(mapID: number)
```

`SynchronousEvent`

## Types

### ChallengeCompletionInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `mapChallengeModeID` | `number` | default `0` |
| `level` | `number` | default `0` |
| `time` | `number` | default `0` |
| `onTime` | `bool` | default `false` |
| `keystoneUpgradeLevels` | `number` | default `0` |
| `practiceRun` | `bool` | default `false` |
| `oldOverallDungeonScore` | `number?` |  |
| `newOverallDungeonScore` | `number?` |  |
| `isMapRecord` | `bool` | default `false` |
| `isAffixRecord` | `bool` | default `false` |
| `isEligibleForScore` | `bool` | default `false` |
| `members` | `ChallengeModeCompletionMemberInfo[]` |  |

### ChallengeModeBestTime

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `mapChallengeModeID` | `number` |  |
| `durationMs` | `number` |  |
| `members` | `ChallengeModeBestTimeMember[]` |  |

### ChallengeModeBestTimeMember

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `classFileName` | `cstring` |  |
| `className` | `cstring` |  |
| `specializationID` | `number` |  |

### ChallengeModeCompletionMemberInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `memberGUID` | `WOWGUID` |  |
| `name` | `string` |  |

### ChallengeModeGuildAttemptMember

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `classFileName` | `cstring` |  |

### ChallengeModeGuildTopAttempt

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `classFileName` | `cstring` |  |
| `keystoneLevel` | `number` |  |
| `mapChallengeModeID` | `number` |  |
| `isYou` | `bool` |  |
| `members` | `ChallengeModeGuildAttemptMember[]` |  |

### ChallengeModeReward

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `rewardID` | `number` |  |
| `displayInfoID` | `number` |  |
| `quantity` | `number` |  |
| `isCurrency` | `bool` |  |
