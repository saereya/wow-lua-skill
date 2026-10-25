# RecruitAFriend

Namespace `C_RecruitAFriend` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/recruitafrienddocumentation.lua` (FileDataID 4637194)

## Functions

### CanSummonFriend

```lua
C_RecruitAFriend.CanSummonFriend(guid: WOWGUID) -> canSummon: bool, reason: RecruitAFriendFailure
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### ClaimActivityReward

```lua
C_RecruitAFriend.ClaimActivityReward(activityID: number, acceptanceID: RecruitAcceptanceID) -> success: bool
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### ClaimNextReward

```lua
C_RecruitAFriend.ClaimNextReward(rafVersion: RecruitAFriendRewardsVersion?) -> success: bool
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### GenerateRecruitmentLink

```lua
C_RecruitAFriend.GenerateRecruitmentLink() -> success: bool
```

`HasRestrictions`

### GetRAFInfo

```lua
C_RecruitAFriend.GetRAFInfo() -> info: RafInfo
```

### GetRAFSystemInfo

```lua
C_RecruitAFriend.GetRAFSystemInfo() -> systemInfo: RafSystemInfo
```

### GetRecruitActivityRequirementsText

```lua
C_RecruitAFriend.GetRecruitActivityRequirementsText(activityID: number, acceptanceID: RecruitAcceptanceID) -> requirementsText: string[]
```

`SecretArguments=AllowedWhenUntainted`

### GetRecruitInfo

```lua
C_RecruitAFriend.GetRecruitInfo() -> active: bool, faction: number
```

### GetSummonFriendCooldown

```lua
C_RecruitAFriend.GetSummonFriendCooldown() -> startTimeSeconds: number, durationSeconds: number, enableCooldownTimer: bool
```

### IsRecruitAFriendLinked

```lua
C_RecruitAFriend.IsRecruitAFriendLinked(guid: WOWGUID) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsRecruitingEnabled

```lua
C_RecruitAFriend.IsRecruitingEnabled() -> enabled: bool
```

### IsSystemEnabled

```lua
C_RecruitAFriend.IsSystemEnabled() -> isSystemEnabled: bool
```

### IsSystemSupported

```lua
C_RecruitAFriend.IsSystemSupported() -> isSystemSupported: bool
```

### RemoveRAFRecruit

```lua
C_RecruitAFriend.RemoveRAFRecruit(wowAccountGUID: WOWGUID) -> success: bool
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### RequestUpdatedRecruitmentInfo

```lua
C_RecruitAFriend.RequestUpdatedRecruitmentInfo() -> success: bool
```

`HasRestrictions`

### SummonFriend

```lua
C_RecruitAFriend.SummonFriend(target: WOWGUID, name: cstring)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### RAF_INFO_UPDATED

```lua
RAF_INFO_UPDATED(info: RafInfo)
```

`SynchronousEvent`

### RAF_RECRUITING_ENABLED_STATUS

```lua
RAF_RECRUITING_ENABLED_STATUS(enabled: bool)
```

`SynchronousEvent`

### RAF_REWARD_CLAIM_FAILED

```lua
RAF_REWARD_CLAIM_FAILED()
```

`SynchronousEvent`

### RAF_SYSTEM_ENABLED_STATUS

```lua
RAF_SYSTEM_ENABLED_STATUS(enabled: bool)
```

`SynchronousEvent`

### RAF_SYSTEM_INFO_UPDATED

```lua
RAF_SYSTEM_INFO_UPDATED(systemInfo: RafSystemInfo)
```

`SynchronousEvent`

## Types

### RafRecruitActivityState

*Enumeration* · 3 values, 0..2

Access values as `Enum.RafRecruitActivityState.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Incomplete` | `RafRecruitActivityState` | = 0 |
| `Complete` | `RafRecruitActivityState` | = 1 |
| `RewardClaimed` | `RafRecruitActivityState` | = 2 |

### RafRecruitSubStatus

*Enumeration* · 3 values, 0..2

Access values as `Enum.RafRecruitSubStatus.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Trial` | `RafRecruitSubStatus` | = 0 |
| `Active` | `RafRecruitSubStatus` | = 1 |
| `Inactive` | `RafRecruitSubStatus` | = 2 |

### RafRewardType

*Enumeration* · 8 values, 0..7

Access values as `Enum.RafRewardType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Pet` | `RafRewardType` | = 0 |
| `Mount` | `RafRewardType` | = 1 |
| `Appearance` | `RafRewardType` | = 2 |
| `Title` | `RafRewardType` | = 3 |
| `GameTime` | `RafRewardType` | = 4 |
| `AppearanceSet` | `RafRewardType` | = 5 |
| `Illusion` | `RafRewardType` | = 6 |
| `Invalid` | `RafRewardType` | = 7 |

### RafAppearanceInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `appearanceID` | `number` |  |

### RafAppearanceSetInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `setID` | `number` |  |
| `setName` | `string` |  |
| `appearanceIDs` | `number[]` |  |

### RafIllusionInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `spellItemEnchantmentID` | `number` |  |

### RafInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `versions` | `RafVersionInfo[]` |  |
| `recruitmentInfo` | `RafRecruitmentinfo?` |  |
| `recruits` | `RafRecruit[]` |  |
| `claimInProgress` | `bool` |  |

### RafMonthCount

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `lifetimeMonths` | `number` |  |
| `spentMonths` | `number` |  |
| `availableMonths` | `number` |  |

### RafMountInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `number` |  |
| `mountID` | `number` |  |

### RafPetInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `creatureID` | `number` |  |
| `speciesID` | `number` |  |
| `displayID` | `number` |  |
| `speciesName` | `string` |  |
| `description` | `string` |  |

### RafRecruit

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `bnetAccountID` | `number` |  |
| `wowAccountGUID` | `WOWGUID` |  |
| `battleTag` | `string` |  |
| `monthsRemaining` | `number` |  |
| `subStatus` | `RafRecruitSubStatus` |  |
| `acceptanceID` | `RecruitAcceptanceID` |  |
| `versionRecruited` | `RecruitAFriendRewardsVersion` |  |
| `activities` | `RafRecruitActivity[]` |  |

### RafRecruitActivity

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `activityID` | `number` |  |
| `rewardQuestID` | `number` |  |
| `state` | `RafRecruitActivityState` |  |

### RafRecruitmentinfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `recruitmentCode` | `string` |  |
| `recruitmentURL` | `string` |  |
| `expireTime` | `number` |  |
| `remainingTimeSeconds` | `number` |  |
| `totalUses` | `number` |  |
| `remainingUses` | `number` |  |
| `sourceRealm` | `string` |  |
| `sourceFaction` | `string` |  |

### RafReward

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `rewardID` | `number` |  |
| `rafVersion` | `RecruitAFriendRewardsVersion` |  |
| `itemID` | `number` |  |
| `rewardType` | `RafRewardType` |  |
| `petInfo` | `RafPetInfo?` |  |
| `mountInfo` | `RafMountInfo?` |  |
| `appearanceInfo` | `RafAppearanceInfo?` |  |
| `titleInfo` | `RafTitleInfo?` |  |
| `appearanceSetInfo` | `RafAppearanceSetInfo?` |  |
| `illusionInfo` | `RafIllusionInfo?` |  |
| `canClaim` | `bool` |  |
| `claimed` | `bool` |  |
| `canAfford` | `bool` |  |
| `repeatable` | `bool` |  |
| `repeatableClaimCount` | `number` |  |
| `monthsRequired` | `number` |  |
| `monthCost` | `number` |  |
| `availableInMonths` | `number` |  |
| `iconID` | `fileID` |  |

### RafSystemInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `maxRecruits` | `number` |  |
| `maxRecruitMonths` | `number` |  |
| `maxRecruitmentUses` | `number` |  |
| `daysInCycle` | `number` |  |

### RafTitleInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `titleMaskID` | `number` |  |

### RafVersionInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `rafVersion` | `RecruitAFriendRewardsVersion` |  |
| `monthCount` | `RafMonthCount` |  |
| `rewards` | `RafReward[]` |  |
| `nextReward` | `RafReward?` |  |
| `numAffordableRewards` | `number` |  |
| `numRecruits` | `number` |  |
