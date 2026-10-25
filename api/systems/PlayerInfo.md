# PlayerInfo

Namespace `C_PlayerInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/playerinfodocumentation.lua` (FileDataID 4637160)

## Functions

### CanPlayerEnterChromieTime

```lua
C_PlayerInfo.CanPlayerEnterChromieTime() -> canEnter: bool
```

### CanPlayerUseAreaLoot

```lua
C_PlayerInfo.CanPlayerUseAreaLoot() -> canUseAreaLoot: bool
```

### CanPlayerUseMountEquipment

```lua
C_PlayerInfo.CanPlayerUseMountEquipment() -> canUseMountEquipment: bool, failureReason: string
```

### CanUseItem

```lua
C_PlayerInfo.CanUseItem(itemID: number) -> isUseable: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetAlternateFormInfo

```lua
C_PlayerInfo.GetAlternateFormInfo() -> hasAlternateForm: bool, inAlternateForm: bool
```

### GetContentDifficultyCreatureForPlayer

```lua
C_PlayerInfo.GetContentDifficultyCreatureForPlayer(unitToken: UnitToken) -> difficulty: RelativeContentDifficulty
```

`SecretArguments=AllowedWhenUntainted`

### GetContentDifficultyQuestForPlayer

```lua
C_PlayerInfo.GetContentDifficultyQuestForPlayer(questID: number) -> difficulty: RelativeContentDifficulty
```

`SecretArguments=AllowedWhenUntainted`

### GetDisplayID

```lua
C_PlayerInfo.GetDisplayID() -> displayID: number
```

### GetGlidingInfo

```lua
C_PlayerInfo.GetGlidingInfo() -> isGliding: bool, canGlide: bool, forwardSpeed: number
```

### GetInstancesUnlockedAtLevel

```lua
C_PlayerInfo.GetInstancesUnlockedAtLevel(level: number, isRaid: bool) -> dungeonID: number[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetNativeDisplayID

```lua
C_PlayerInfo.GetNativeDisplayID() -> nativeDisplayID: number
```

### GetPetStableCreatureDisplayInfoID

```lua
C_PlayerInfo.GetPetStableCreatureDisplayInfoID(index: number) -> creatureDisplayInfoID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetPlayerCharacterData

```lua
C_PlayerInfo.GetPlayerCharacterData() -> characterData: PlayerInfoCharacterData
```

`MayReturnNothing`

### GetPlayerMythicPlusRatingSummary

```lua
C_PlayerInfo.GetPlayerMythicPlusRatingSummary(playerToken: UnitToken) -> ratingSummary: MythicPlusRatingSummary
```

Returns the players mythic+ rating summary which includes the runs they've completed as well as their current season m+ rating

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### HasAccountInventoryLock

```lua
C_PlayerInfo.HasAccountInventoryLock() -> hasAccountInventoryLock: bool
```

### HasVisibleInvSlot

```lua
C_PlayerInfo.HasVisibleInvSlot(slot: luaIndex) -> isVisible: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsAccountBankEnabled

```lua
C_PlayerInfo.IsAccountBankEnabled() -> isAccountBankEnabled: bool
```

### IsCharacterBankEnabled

```lua
C_PlayerInfo.IsCharacterBankEnabled() -> isCharacterBankEnabled: bool
```

### IsDisplayRaceNative

```lua
C_PlayerInfo.IsDisplayRaceNative() -> isDisplayRaceNative: bool
```

### IsExpansionLandingPageUnlockedForPlayer

```lua
C_PlayerInfo.IsExpansionLandingPageUnlockedForPlayer(expansionID: number) -> isUnlocked: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsMirrorImage

```lua
C_PlayerInfo.IsMirrorImage() -> isMirrorImage: bool
```

### IsPlayerEligibleForNPE

```lua
C_PlayerInfo.IsPlayerEligibleForNPE() -> isEligible: bool, failureReason: string
```

### IsPlayerEligibleForNPEv2

```lua
C_PlayerInfo.IsPlayerEligibleForNPEv2() -> isEligible: bool, failureReason: string
```

### IsPlayerInChromieTime

```lua
C_PlayerInfo.IsPlayerInChromieTime() -> inChromieTime: bool
```

### IsPlayerInRPE

```lua
C_PlayerInfo.IsPlayerInRPE() -> isInRPE: bool
```

### IsPlayerInTimerunningHeroicWorldTier

```lua
C_PlayerInfo.IsPlayerInTimerunningHeroicWorldTier() -> inTimerunningHeroicWorldTier: bool
```

### IsPlayerNPERestricted

```lua
C_PlayerInfo.IsPlayerNPERestricted() -> isRestricted: bool
```

### IsReturningCharacter

```lua
C_PlayerInfo.IsReturningCharacter() -> isReturning: bool
```

### IsSelfFoundActive

```lua
C_PlayerInfo.IsSelfFoundActive() -> active: bool
```

### IsTradingPostAvailable

```lua
C_PlayerInfo.IsTradingPostAvailable() -> isAvailable: bool
```

### IsTravelersLogAvailable

```lua
C_PlayerInfo.IsTravelersLogAvailable() -> isAvailable: bool
```

### IsTutorialsTabAvailable

```lua
C_PlayerInfo.IsTutorialsTabAvailable() -> isAvailable: bool
```

### ShouldDisplaySurname

```lua
C_PlayerInfo.ShouldDisplaySurname() -> display: bool
```

## Types

### MythicPlusRatingMapSummary

*Structure*

Specific information about a completed mythic plus run.

Fields:

| Name | Type | Notes |
|---|---|---|
| `challengeModeID` | `number` |  |
| `mapScore` | `number` |  |
| `bestRunLevel` | `number` |  |
| `bestRunDurationMS` | `number` |  |
| `finishedSuccess` | `bool` |  |

### MythicPlusRatingSummary

*Structure*

The current season rating and well as a list of completed mythic plus runs.

Fields:

| Name | Type | Notes |
|---|---|---|
| `currentSeasonScore` | `number` |  |
| `runs` | `MythicPlusRatingMapSummary[]` |  |
