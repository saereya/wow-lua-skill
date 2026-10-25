# MajorFactionsUI

Namespace `C_MajorFactions` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/majorfactionsdocumentation.lua` (FileDataID 4681097)

## Functions

### GetCurrentRenownLevel

```lua
C_MajorFactions.GetCurrentRenownLevel(majorFactionID: number) -> level: number
```

`SecretArguments=AllowedWhenUntainted`

### GetMajorFactionData

```lua
C_MajorFactions.GetMajorFactionData(majorFactionID: number) -> data: MajorFactionData?
```

`SecretArguments=AllowedWhenUntainted`

### GetMajorFactionIDs

```lua
C_MajorFactions.GetMajorFactionIDs(expansionID: number?) -> majorFactionIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetMajorFactionProgressionInfo

```lua
C_MajorFactions.GetMajorFactionProgressionInfo(majorFactionID: number) -> data: MajorFactionProgressionInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetMajorFactionRenownInfo

```lua
C_MajorFactions.GetMajorFactionRenownInfo(majorFactionID: number) -> data: MajorFactionRenownInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetRenownLevels

```lua
C_MajorFactions.GetRenownLevels(majorFactionID: number) -> levels: MajorFactionRenownLevelInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetRenownNPCFactionID

```lua
C_MajorFactions.GetRenownNPCFactionID() -> renownNPCFactionID: number
```

### GetRenownRewardsForLevel

```lua
C_MajorFactions.GetRenownRewardsForLevel(majorFactionID: number, renownLevel: number) -> rewards: MajorFactionRenownRewardInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetTotalReputationForRenownLevel

```lua
C_MajorFactions.GetTotalReputationForRenownLevel(majorFactionID: number, renownLevel: number) -> totalReputation: number
```

`SecretArguments=AllowedWhenUntainted`

### HasMaximumRenown

```lua
C_MajorFactions.HasMaximumRenown(majorFactionID: number) -> hasMaxRenown: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsMajorFactionHiddenFromExpansionPage

```lua
C_MajorFactions.IsMajorFactionHiddenFromExpansionPage(majorFactionID: number) -> isHidden: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsWeeklyRenownCapped

```lua
C_MajorFactions.IsWeeklyRenownCapped(majorFactionID: number) -> isWeeklyCapped: bool
```

`SecretArguments=AllowedWhenUntainted`

### ShouldDisplayMajorFactionAsJourney

```lua
C_MajorFactions.ShouldDisplayMajorFactionAsJourney(majorFactionID: number) -> shouldDisplayMajorFactionAsJourney: bool
```

`SecretArguments=AllowedWhenUntainted`

### ShouldUseJourneyRewardTrack

```lua
C_MajorFactions.ShouldUseJourneyRewardTrack(majorFactionID: number) -> shouldUseJourneyRewardTrack: bool
```

`SecretArguments=AllowedWhenUntainted`

## Events

### MAJOR_FACTION_INTERACTION_ENDED

```lua
MAJOR_FACTION_INTERACTION_ENDED()
```

`SynchronousEvent`

### MAJOR_FACTION_INTERACTION_STARTED

```lua
MAJOR_FACTION_INTERACTION_STARTED()
```

`SynchronousEvent`

### MAJOR_FACTION_RENOWN_LEVEL_CHANGED

```lua
MAJOR_FACTION_RENOWN_LEVEL_CHANGED(majorFactionID: number, newRenownLevel: number, oldRenownLevel: number)
```

`SynchronousEvent`

### MAJOR_FACTION_UNLOCKED

```lua
MAJOR_FACTION_UNLOCKED(majorFactionID: number)
```

`SynchronousEvent`

## Types

### MajorFactionData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `description` | `cstring` |  |
| `highlights` | `RenownHighlightInfo[]` |  |
| `factionID` | `number` |  |
| `expansionID` | `number` |  |
| `bountySetID` | `number` |  |
| `isUnlocked` | `bool` |  |
| `useJourneyUnlockToast` | `bool` |  |
| `hideRenownLevelUpToast` | `bool` |  |
| `unlockDescription` | `cstring?` |  |
| `uiPriority` | `number` |  |
| `renownLevel` | `number` |  |
| `maxLevel` | `number` |  |
| `renownReputationEarned` | `number` |  |
| `renownLevelThreshold` | `number` |  |
| `textureKit` | `textureKit` |  |
| `celebrationSoundKit` | `number` |  |
| `renownFanfareSoundKitID` | `number` |  |
| `factionFontColor` | `DBColorExport?` |  |
| `renownTrackLevelEffectID` | `number?` |  |
| `playerCompanionID` | `number?` |  |

### MajorFactionProgressionInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `renownLevel` | `number` |  |
| `previousWeekProgressiveMaxLevel` | `number` |  |
| `currentWeekProgressiveMaxLevel` | `number` |  |
| `maxLevel` | `number` |  |
| `renownReputationEarned` | `number` |  |
| `renownLevelThreshold` | `number` |  |
| `weekNumber` | `number` |  |

### MajorFactionRenownInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `renownLevel` | `number` |  |
| `renownReputationEarned` | `number` |  |
| `renownLevelThreshold` | `number` |  |

### MajorFactionRenownLevelInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `factionID` | `number` |  |
| `level` | `number` |  |
| `locked` | `bool` |  |
| `isMilestone` | `bool` |  |
| `isCapstone` | `bool` |  |

### MajorFactionRenownRewardInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `renownRewardID` | `number` |  |
| `uiOrder` | `number` |  |
| `isAccountUnlock` | `bool` |  |
| `itemID` | `number?` |  |
| `spellID` | `number?` |  |
| `mountID` | `number?` |  |
| `transmogID` | `number?` |  |
| `transmogSetID` | `number?` |  |
| `titleMaskID` | `number?` |  |
| `transmogIllusionSourceID` | `number?` |  |
| `icon` | `fileID?` |  |
| `name` | `cstring?` |  |
| `description` | `cstring?` |  |
| `toastDescription` | `cstring?` |  |
| `rewardType` | `number?` |  |
| `isCollected` | `bool?` |  |

### RenownHighlightInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `title` | `cstring` |  |
| `description` | `cstring` |  |
| `level` | `number` |  |
