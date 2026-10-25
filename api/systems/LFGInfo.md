# LFGInfo

Namespace `C_LFGInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/lfginfodocumentation.lua` (FileDataID 4637140)

## Functions

### AreCrossFactionGroupQueuesAllowed

```lua
C_LFGInfo.AreCrossFactionGroupQueuesAllowed(lfgDungeonID: number) -> areCrossFactionGroupQueuesAllowed: bool
```

`SecretArguments=AllowedWhenUntainted`

### CanPlayerUseGroupFinder

```lua
C_LFGInfo.CanPlayerUseGroupFinder() -> canUse: bool, failureReason: string
```

### CanPlayerUseLFD

```lua
C_LFGInfo.CanPlayerUseLFD() -> canUse: bool, failureReason: string
```

### CanPlayerUseLFR

```lua
C_LFGInfo.CanPlayerUseLFR() -> canUse: bool, failureReason: string
```

### CanPlayerUsePremadeGroup

```lua
C_LFGInfo.CanPlayerUsePremadeGroup() -> canUse: bool, failureReason: string
```

### CanPlayerUsePVP

```lua
C_LFGInfo.CanPlayerUsePVP() -> canUse: bool, failureReason: string
```

### CanPlayerUseScenarioFinder

```lua
C_LFGInfo.CanPlayerUseScenarioFinder() -> canUse: bool, failureReason: string
```

### ConfirmLfgExpandSearch

```lua
C_LFGInfo.ConfirmLfgExpandSearch()
```

### DoesActivePartyMeetPremadeLaunchCount

```lua
C_LFGInfo.DoesActivePartyMeetPremadeLaunchCount(lfgDungeonID: number) -> doesActivePartyMeetPremadeLaunchCount: bool
```

`SecretArguments=AllowedWhenUntainted`

### DoesCrossFactionQueueRequireFullPremade

```lua
C_LFGInfo.DoesCrossFactionQueueRequireFullPremade(lfgDungeonID: number) -> doesCrossFactionQueueRequireFullPremade: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetActiveLFGDungeonName

```lua
C_LFGInfo.GetActiveLFGDungeonName() -> name: string
```

### GetAllEntriesForCategory

```lua
C_LFGInfo.GetAllEntriesForCategory(category: luaIndex) -> lfgDungeonIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetDungeonInfo

```lua
C_LFGInfo.GetDungeonInfo(lfgDungeonID: number) -> dungeonInfo: LFGDungeonInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetLevelUpInstances

```lua
C_LFGInfo.GetLevelUpInstances(currPlayerLevel: number, isRaid: bool) -> instances: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetLFDLockStates

```lua
C_LFGInfo.GetLFDLockStates() -> lockInfo: LFGLockInfo[]
```

### GetRoleCheckDifficultyDetails

```lua
C_LFGInfo.GetRoleCheckDifficultyDetails() -> maxLevel: number?, isLevelReduced: bool
```

### HideNameFromUI

```lua
C_LFGInfo.HideNameFromUI(dungeonID: number) -> shouldHide: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsGroupFinderEnabled

```lua
C_LFGInfo.IsGroupFinderEnabled() -> enabled: bool
```

### IsInLFGFollowerDungeon

```lua
C_LFGInfo.IsInLFGFollowerDungeon() -> result: bool
```

### IsInMatchmadeRaidWithoutRoleRequirements

```lua
C_LFGInfo.IsInMatchmadeRaidWithoutRoleRequirements() -> result: bool
```

### IsLFDEnabled

```lua
C_LFGInfo.IsLFDEnabled() -> enabled: bool
```

### IsLFGFollowerDungeon

```lua
C_LFGInfo.IsLFGFollowerDungeon(dungeonID: number) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsLFREnabled

```lua
C_LFGInfo.IsLFREnabled() -> enabled: bool
```

## Events

### ISLAND_COMPLETED

```lua
ISLAND_COMPLETED(mapID: number, winner: number)
```

`SynchronousEvent`

### LFG_BOOT_PROPOSAL_UPDATE

```lua
LFG_BOOT_PROPOSAL_UPDATE()
```

`SynchronousEvent`

### LFG_COMPLETION_REWARD

```lua
LFG_COMPLETION_REWARD()
```

`SynchronousEvent`

### LFG_COOLDOWNS_UPDATED

```lua
LFG_COOLDOWNS_UPDATED()
```

`SynchronousEvent`

### LFG_ENABLED_STATE_CHANGED

```lua
LFG_ENABLED_STATE_CHANGED()
```

`SynchronousEvent`

### LFG_INVALID_ERROR_MESSAGE

```lua
LFG_INVALID_ERROR_MESSAGE(reason: number, subReason1: number, subReason2: number)
```

`SynchronousEvent`

### LFG_LOCK_INFO_RECEIVED

```lua
LFG_LOCK_INFO_RECEIVED()
```

`SynchronousEvent`

### LFG_OFFER_CONTINUE

```lua
LFG_OFFER_CONTINUE(name: cstring, lfgDungeonsID: number, typeID: number)
```

`SynchronousEvent`

### LFG_OPEN_FROM_GOSSIP

```lua
LFG_OPEN_FROM_GOSSIP(dungeonID: number)
```

`SynchronousEvent`

### LFG_PROPOSAL_DONE

```lua
LFG_PROPOSAL_DONE()
```

`SynchronousEvent`

### LFG_PROPOSAL_FAILED

```lua
LFG_PROPOSAL_FAILED()
```

`SynchronousEvent`

### LFG_PROPOSAL_SHOW

```lua
LFG_PROPOSAL_SHOW()
```

`SynchronousEvent`

### LFG_PROPOSAL_SUCCEEDED

```lua
LFG_PROPOSAL_SUCCEEDED()
```

`SynchronousEvent`

### LFG_PROPOSAL_UPDATE

```lua
LFG_PROPOSAL_UPDATE()
```

`SynchronousEvent`

### LFG_QUEUE_STATUS_UPDATE

```lua
LFG_QUEUE_STATUS_UPDATE()
```

`SynchronousEvent`

### LFG_READY_CHECK_DECLINED

```lua
LFG_READY_CHECK_DECLINED(name: cstring)
```

`SynchronousEvent`

### LFG_READY_CHECK_HIDE

```lua
LFG_READY_CHECK_HIDE()
```

`SynchronousEvent`

### LFG_READY_CHECK_PLAYER_IS_READY

```lua
LFG_READY_CHECK_PLAYER_IS_READY(name: cstring)
```

`SynchronousEvent`

### LFG_READY_CHECK_SHOW

```lua
LFG_READY_CHECK_SHOW(isRequeue: bool)
```

`SynchronousEvent`

### LFG_READY_CHECK_UPDATE

```lua
LFG_READY_CHECK_UPDATE()
```

`SynchronousEvent`

### LFG_ROLE_CHECK_DECLINED

```lua
LFG_ROLE_CHECK_DECLINED()
```

`SynchronousEvent`

### LFG_ROLE_CHECK_HIDE

```lua
LFG_ROLE_CHECK_HIDE()
```

`SynchronousEvent`

### LFG_ROLE_CHECK_ROLE_CHOSEN

```lua
LFG_ROLE_CHECK_ROLE_CHOSEN(name: cstring, isTank: bool, isHealer: bool, isDamage: bool)
```

`SynchronousEvent`

### LFG_ROLE_CHECK_SHOW

```lua
LFG_ROLE_CHECK_SHOW(isRequeue: bool)
```

`SynchronousEvent`

### LFG_ROLE_CHECK_UPDATE

```lua
LFG_ROLE_CHECK_UPDATE()
```

`SynchronousEvent`

### LFG_ROLE_UPDATE

```lua
LFG_ROLE_UPDATE()
```

`SynchronousEvent`

### LFG_UPDATE

```lua
LFG_UPDATE()
```

`SynchronousEvent`

### LFG_UPDATE_RANDOM_INFO

```lua
LFG_UPDATE_RANDOM_INFO()
```

`SynchronousEvent`

### SHOW_LFG_EXPAND_SEARCH_PROMPT

```lua
SHOW_LFG_EXPAND_SEARCH_PROMPT()
```

`SynchronousEvent`

### UPDATE_LFG_LIST

```lua
UPDATE_LFG_LIST()
```

`SynchronousEvent`

### WARFRONT_COMPLETED

```lua
WARFRONT_COMPLETED(mapID: number, winner: number)
```

`SynchronousEvent`

## Types

### LFGDungeonInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `iconID` | `fileID` |  |
| `link` | `string?` |  |

### LFGLockInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `lfgID` | `number` |  |
| `reason` | `number` |  |
| `hideEntry` | `bool` |  |
