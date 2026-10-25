# PvpInfo

Namespace `C_PvP` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/pvpinfodocumentation.lua` (FileDataID 4637170)

## Functions

### ArePvpTalentsUnlocked

```lua
C_PvP.ArePvpTalentsUnlocked() -> arePvpTalentsUnlocked: bool
```

### AreTrainingGroundsEnabled

```lua
C_PvP.AreTrainingGroundsEnabled() -> areTrainingGroundsEnabled: bool
```

### CanDisplayDeaths

```lua
C_PvP.CanDisplayDeaths() -> canDisplay: bool
```

### CanDisplayHonorableKills

```lua
C_PvP.CanDisplayHonorableKills() -> canDisplay: bool
```

### CanPlayerUseRatedPVPUI

```lua
C_PvP.CanPlayerUseRatedPVPUI() -> canUse: bool, failureReason: string
```

### CanPlayerUseTrainingGroundsUI

```lua
C_PvP.CanPlayerUseTrainingGroundsUI() -> canUseTrainingGroundsUI: bool, failureReason: string
```

### CanSurrenderArena

```lua
C_PvP.CanSurrenderArena() -> CanSurrenderArena: bool
```

### CanToggleWarMode

```lua
C_PvP.CanToggleWarMode(toggle: bool) -> canTogglePvP: bool
```

`SecretArguments=AllowedWhenUntainted`

### CanToggleWarModeInArea

```lua
C_PvP.CanToggleWarModeInArea() -> canTogglePvPInArea: bool
```

### DoesMatchOutcomeAffectRating

```lua
C_PvP.DoesMatchOutcomeAffectRating() -> doesAffect: bool
```

### GetActiveBrawlInfo

```lua
C_PvP.GetActiveBrawlInfo() -> brawlInfo: PvpBrawlInfo?
```

### GetActiveMatchBracket

```lua
C_PvP.GetActiveMatchBracket() -> bracket: number
```

### GetActiveMatchDuration

```lua
C_PvP.GetActiveMatchDuration() -> seconds: time_t
```

### GetActiveMatchState

```lua
C_PvP.GetActiveMatchState() -> state: PvPMatchState
```

### GetActiveMatchWinner

```lua
C_PvP.GetActiveMatchWinner() -> winner: number
```

### GetArenaCrowdControlDuration

```lua
C_PvP.GetArenaCrowdControlDuration(playerToken: UnitToken) -> duration: LuaDurationObject
```

`SecretArguments=AllowedWhenUntainted`

### GetArenaCrowdControlInfo

```lua
C_PvP.GetArenaCrowdControlInfo(playerToken: UnitToken) -> spellID: number, startTime: number, duration: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretWhenLossOfControlInfoRestricted`

### GetArenaOpponentSpec

```lua
C_PvP.GetArenaOpponentSpec(index: luaIndex) -> specializationID: number, gender: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `Namespace=` `SecretReturns`

### GetArenaRewards

```lua
C_PvP.GetArenaRewards(teamSize: number) -> honor: number, experience: number, itemRewards: BattlefieldItemReward[]?, currencyRewards: BattlefieldCurrencyReward[]?, roleShortageBonus: RoleShortageReward?
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetArenaSkirmishRewards

```lua
C_PvP.GetArenaSkirmishRewards() -> honor: number, experience: number, itemRewards: BattlefieldItemReward[]?, currencyRewards: BattlefieldCurrencyReward[]?, roleShortageBonus: RoleShortageReward?
```

### GetAssignedSpecForBattlefieldQueue

```lua
C_PvP.GetAssignedSpecForBattlefieldQueue(queueID: number) -> specializationID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetAvailableBrawlInfo

```lua
C_PvP.GetAvailableBrawlInfo() -> brawlInfo: PvpBrawlInfo?
```

If nil is returned, PVP_BRAWL_INFO_UPDATED event will be sent when the data is ready.

### GetBattlefieldFlagPosition

```lua
C_PvP.GetBattlefieldFlagPosition(flagIndex: luaIndex, uiMapId: number) -> uiPosx: number?, uiPosy: number?, flagTexture: number
```

`SecretArguments=AllowedWhenUntainted`

### GetBattlefieldVehicleInfo

```lua
C_PvP.GetBattlefieldVehicleInfo(vehicleIndex: luaIndex, uiMapID: number) -> info: BattlefieldVehicleInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetBattlefieldVehicles

```lua
C_PvP.GetBattlefieldVehicles(uiMapID: number) -> vehicles: BattlefieldVehicleInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetBattlegroundInfo

```lua
C_PvP.GetBattlegroundInfo(battlegroundIndex: luaIndex) -> battlegroundInfo: BattlegroundInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetBrawlRewards

```lua
C_PvP.GetBrawlRewards(brawlType: BrawlType) -> honor: number, experience: number, itemRewards: BattlefieldItemReward[]?, currencyRewards: BattlefieldCurrencyReward[]?, roleShortageBonus: RoleShortageReward?, hasWon: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetBrawlSoloRBGMinItemLevel

```lua
C_PvP.GetBrawlSoloRBGMinItemLevel() -> minItemLevel: number
```

### GetCustomVictoryStatID

```lua
C_PvP.GetCustomVictoryStatID() -> statID: number
```

### GetGlobalPvpScalingInfoForSpecID

```lua
C_PvP.GetGlobalPvpScalingInfoForSpecID(specializationID: number) -> pvpScalingData: PvpScalingData[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetHonorRewardInfo

```lua
C_PvP.GetHonorRewardInfo(honorLevel: number) -> info: HonorRewardInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetLevelUpBattlegrounds

```lua
C_PvP.GetLevelUpBattlegrounds(level: number) -> battlefields: LevelUpBattlegroundInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetMatchPVPStatColumn

```lua
C_PvP.GetMatchPVPStatColumn(pvpStatID: number) -> info: MatchPVPStatColumn?
```

`SecretArguments=AllowedWhenUntainted`

### GetMatchPVPStatColumns

```lua
C_PvP.GetMatchPVPStatColumns() -> columns: MatchPVPStatColumn[]
```

### GetNextHonorLevelForReward

```lua
C_PvP.GetNextHonorLevelForReward(honorLevel: number) -> nextHonorLevelWithReward: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetOutdoorPvPWaitTime

```lua
C_PvP.GetOutdoorPvPWaitTime(uiMapID: number) -> pvpWaitTime: time_t
```

`SecretArguments=AllowedWhenUntainted`

### GetPersonalRatedBGBlitzSpecStats

```lua
C_PvP.GetPersonalRatedBGBlitzSpecStats() -> specStats: RatedBGBlitzSpecStats?
```

### GetPersonalRatedSoloShuffleSpecStats

```lua
C_PvP.GetPersonalRatedSoloShuffleSpecStats() -> specStats: RatedSoloShuffleSpecStats?
```

### GetPostMatchCurrencyRewards

```lua
C_PvP.GetPostMatchCurrencyRewards() -> rewards: PVPPostMatchCurrencyReward[]
```

### GetPostMatchItemRewards

```lua
C_PvP.GetPostMatchItemRewards() -> rewards: PVPPostMatchItemReward[]
```

### GetPVPActiveMatchPersonalRatedInfo

```lua
C_PvP.GetPVPActiveMatchPersonalRatedInfo() -> info: PVPPersonalRatedInfo?
```

### GetPVPActiveRatedMatchDeserterPenalty

```lua
C_PvP.GetPVPActiveRatedMatchDeserterPenalty() -> deserterPenalty: RatedMatchDeserterPenalty?
```

### GetPVPSeasonRewardAchievementID

```lua
C_PvP.GetPVPSeasonRewardAchievementID() -> achievementID: number
```

`MayReturnNothing`

### GetPvpTalentsUnlockedLevel

```lua
C_PvP.GetPvpTalentsUnlockedLevel() -> unlockLevel: number
```

### GetPvpTierID

```lua
C_PvP.GetPvpTierID(tierEnum: number, bracketEnum: luaIndex) -> id: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetPvpTierInfo

```lua
C_PvP.GetPvpTierInfo(tierID: number) -> pvpTierInfo: PvpTierInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetRandomBGInfo

```lua
C_PvP.GetRandomBGInfo() -> info: RandomBGInfo
```

### GetRandomBGRewards

```lua
C_PvP.GetRandomBGRewards() -> honor: number, experience: number, itemRewards: BattlefieldItemReward[]?, currencyRewards: BattlefieldCurrencyReward[]?, roleShortageBonus: RoleShortageReward?
```

### GetRandomEpicBGInfo

```lua
C_PvP.GetRandomEpicBGInfo() -> info: RandomBGInfo
```

### GetRandomEpicBGRewards

```lua
C_PvP.GetRandomEpicBGRewards() -> honor: number, experience: number, itemRewards: BattlefieldItemReward[]?, currencyRewards: BattlefieldCurrencyReward[]?, roleShortageBonus: RoleShortageReward?
```

### GetRandomTrainingGroundArenaRewards

```lua
C_PvP.GetRandomTrainingGroundArenaRewards() -> honor: number, experience: number, itemRewards: BattlefieldItemReward[]?, currencyRewards: BattlefieldCurrencyReward[]?, roleShortageBonus: RoleShortageReward?
```

### GetRandomTrainingGroundBGRewards

```lua
C_PvP.GetRandomTrainingGroundBGRewards() -> honor: number, experience: number, itemRewards: BattlefieldItemReward[]?, currencyRewards: BattlefieldCurrencyReward[]?, roleShortageBonus: RoleShortageReward?
```

### GetRatedBGRewards

```lua
C_PvP.GetRatedBGRewards() -> honor: number, experience: number, itemRewards: BattlefieldItemReward[]?, currencyRewards: BattlefieldCurrencyReward[]?, roleShortageBonus: RoleShortageReward?
```

### GetRatedSoloRBGMinItemLevel

```lua
C_PvP.GetRatedSoloRBGMinItemLevel() -> minItemLevel: number
```

### GetRatedSoloRBGRewards

```lua
C_PvP.GetRatedSoloRBGRewards() -> honor: number, experience: number, itemRewards: BattlefieldItemReward[]?, currencyRewards: BattlefieldCurrencyReward[]?, roleShortageBonus: RoleShortageReward?
```

### GetRatedSoloShuffleMinItemLevel

```lua
C_PvP.GetRatedSoloShuffleMinItemLevel() -> minItemLevel: number
```

### GetRatedSoloShuffleRewards

```lua
C_PvP.GetRatedSoloShuffleRewards() -> honor: number, experience: number, itemRewards: BattlefieldItemReward[]?, currencyRewards: BattlefieldCurrencyReward[]?, roleShortageBonus: RoleShortageReward?
```

### GetRewardItemLevelsByTierEnum

```lua
C_PvP.GetRewardItemLevelsByTierEnum(pvpTierEnum: number) -> activityItemLevel: number, weeklyItemLevel: number
```

`SecretArguments=AllowedWhenUntainted`

### GetScoreInfo

```lua
C_PvP.GetScoreInfo(offsetIndex: luaIndex) -> info: PVPScoreInfo?
```

`SecretArguments=AllowedWhenUntainted` `SecretInActivePvPMatch`

### GetScoreInfoByPlayerGuid

```lua
C_PvP.GetScoreInfoByPlayerGuid(guid: WOWGUID) -> info: PVPScoreInfo?
```

`SecretArguments=AllowedWhenUntainted` `SecretInActivePvPMatch`

### GetSeasonBestInfo

```lua
C_PvP.GetSeasonBestInfo() -> tierID: number, nextTierID: number?
```

### GetSkirmishInfo

```lua
C_PvP.GetSkirmishInfo(pvpBracket: number) -> battlemasterListInfo: BattlemasterListInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSpecialEventBrawlInfo

```lua
C_PvP.GetSpecialEventBrawlInfo() -> brawlInfo: PvpBrawlInfo?
```

### GetTeamInfo

```lua
C_PvP.GetTeamInfo(factionIndex: number) -> info: PVPTeamInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetTrainingGrounds

```lua
C_PvP.GetTrainingGrounds() -> trainingGrounds: BattlegroundInfo[]
```

### GetUIDisplaySeason

```lua
C_PvP.GetUIDisplaySeason() -> uiDisplaySeason: number
```

### GetWarModeRewardBonus

```lua
C_PvP.GetWarModeRewardBonus() -> rewardBonus: number
```

### GetWarModeRewardBonusDefault

```lua
C_PvP.GetWarModeRewardBonusDefault() -> defaultBonus: number
```

### GetWeeklyChestInfo

```lua
C_PvP.GetWeeklyChestInfo() -> rewardAchieved: bool, lastWeekRewardAchieved: bool, lastWeekRewardClaimed: bool, pvpTierMaxFromWins: number
```

### GetZonePVPInfo

```lua
C_PvP.GetZonePVPInfo() -> pvpType: cstring, isSubZonePvP: bool, factionName: cstring?
```

`MayReturnNothing`

### HasArenaSkirmishWinToday

```lua
C_PvP.HasArenaSkirmishWinToday() -> hasArenaSkirmishWinToday: bool
```

### HasMatchStarted

```lua
C_PvP.HasMatchStarted() -> hasStarted: bool
```

Returns true if a match is either active or complete.

### HasRandomTrainingGroundArenaWinToday

```lua
C_PvP.HasRandomTrainingGroundArenaWinToday() -> hasRandomTrainingGroundArenaWinToday: bool
```

### HasRandomTrainingGroundBGWinToday

```lua
C_PvP.HasRandomTrainingGroundBGWinToday() -> hasRandomTrainingGroundBGWinToday: bool
```

### IsActiveBattlefield

```lua
C_PvP.IsActiveBattlefield() -> isActiveBattlefield: bool
```

### IsActiveMatchRegistered

```lua
C_PvP.IsActiveMatchRegistered() -> registered: bool
```

### IsArena

```lua
C_PvP.IsArena() -> isArena: bool
```

### IsBattleground

```lua
C_PvP.IsBattleground() -> isBattleground: bool
```

### IsBattlegroundEnlistmentBonusActive

```lua
C_PvP.IsBattlegroundEnlistmentBonusActive() -> battlegroundActive: bool, brawlActive: bool
```

### IsBrawlSoloRBG

```lua
C_PvP.IsBrawlSoloRBG() -> isBrawlSoloRBG: bool
```

### IsBrawlSoloShuffle

```lua
C_PvP.IsBrawlSoloShuffle() -> isBrawlSoloShuffle: bool
```

### IsInBrawl

```lua
C_PvP.IsInBrawl() -> isInBrawl: bool
```

### IsInRatedMatchWithDeserterPenalty

```lua
C_PvP.IsInRatedMatchWithDeserterPenalty() -> isInRatedMatchWithDeserterPenalty: bool
```

### IsMatchActive

```lua
C_PvP.IsMatchActive() -> isActive: bool
```

### IsMatchComplete

```lua
C_PvP.IsMatchComplete() -> isComplete: bool
```

### IsMatchConsideredArena

```lua
C_PvP.IsMatchConsideredArena() -> asArena: bool
```

### IsMatchFactional

```lua
C_PvP.IsMatchFactional() -> isFactional: bool
```

### IsPVPMap

```lua
C_PvP.IsPVPMap() -> isPVPMap: bool
```

### IsRatedArena

```lua
C_PvP.IsRatedArena() -> isRatedArena: bool
```

### IsRatedBattleground

```lua
C_PvP.IsRatedBattleground() -> isRatedBattleground: bool
```

### IsRatedMap

```lua
C_PvP.IsRatedMap() -> isRatedMap: bool
```

### IsRatedSoloRBG

```lua
C_PvP.IsRatedSoloRBG() -> isRatedSoloRBG: bool
```

### IsRatedSoloShuffle

```lua
C_PvP.IsRatedSoloShuffle() -> isRatedSoloShuffle: bool
```

### IsSoloRBG

```lua
C_PvP.IsSoloRBG() -> isSoloRBG: bool
```

### IsSoloShuffle

```lua
C_PvP.IsSoloShuffle() -> isSoloShuffle: bool
```

### IsSubZonePVPPOI

```lua
C_PvP.IsSubZonePVPPOI() -> result: bool
```

### IsTrainingGroundsArena

```lua
C_PvP.IsTrainingGroundsArena(lfgDungeonsID: number) -> isTrainingGroundsArena: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsTrainingGroundsBG

```lua
C_PvP.IsTrainingGroundsBG(lfgDungeonsID: number) -> isTrainingGroundsBG: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsWarModeActive

```lua
C_PvP.IsWarModeActive() -> warModeActive: bool
```

### IsWarModeDesired

```lua
C_PvP.IsWarModeDesired() -> warModeDesired: bool
```

### IsWarModeFeatureEnabled

```lua
C_PvP.IsWarModeFeatureEnabled() -> warModeEnabled: bool
```

### JoinBattlefield

```lua
C_PvP.JoinBattlefield(battlemasterListId: number)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### JoinBrawl

```lua
C_PvP.JoinBrawl(isSpecialBrawl: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `isSpecialBrawl` | `bool` | default `false` |

### JoinRandomTrainingGroundArena

```lua
C_PvP.JoinRandomTrainingGroundArena()
```

### JoinRandomTrainingGroundBG

```lua
C_PvP.JoinRandomTrainingGroundBG()
```

### JoinRatedBGBlitz

```lua
C_PvP.JoinRatedBGBlitz()
```

### JoinTrainingGround

```lua
C_PvP.JoinTrainingGround(trainingGroundID: number)
```

`SecretArguments=AllowedWhenUntainted`

### RequestCrowdControlSpell

```lua
C_PvP.RequestCrowdControlSpell(playerToken: UnitToken)
```

`SecretArguments=AllowedWhenUntainted`

### SetPVP

```lua
C_PvP.SetPVP(enablePVP: bool)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `enablePVP` | `bool` | default `false` |

### SetWarModeDesired

```lua
C_PvP.SetWarModeDesired(warModeDesired: bool)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### StartSoloRBGWarGameByName

```lua
C_PvP.StartSoloRBGWarGameByName(args: cstring) -> success: number
```

`SecretArguments=AllowedWhenUntainted`

### StartSpectatorSoloRBGWarGame

```lua
C_PvP.StartSpectatorSoloRBGWarGame(opaqueID1: number, opaqueID2: number, specifiedMap: cstring, tournamentRules: bool) -> success: number
```

`SecretArguments=AllowedWhenUntainted`

### TogglePVP

```lua
C_PvP.TogglePVP()
```

`HasRestrictions`

### ToggleWarMode

```lua
C_PvP.ToggleWarMode()
```

`HasRestrictions`

## Events

### ARENA_OPPONENT_UPDATE

```lua
ARENA_OPPONENT_UPDATE(unitToken: cstring, updateReason: cstring)
```

`SynchronousEvent`

### ARENA_PREP_OPPONENT_SPECIALIZATIONS

```lua
ARENA_PREP_OPPONENT_SPECIALIZATIONS()
```

`SynchronousEvent`

### ARENA_SEASON_WORLD_STATE

```lua
ARENA_SEASON_WORLD_STATE()
```

`SynchronousEvent`

### BATTLEFIELD_AUTO_QUEUE

```lua
BATTLEFIELD_AUTO_QUEUE()
```

`SynchronousEvent`

### BATTLEFIELD_AUTO_QUEUE_EJECT

```lua
BATTLEFIELD_AUTO_QUEUE_EJECT()
```

`SynchronousEvent`

### BATTLEFIELD_QUEUE_TIMEOUT

```lua
BATTLEFIELD_QUEUE_TIMEOUT()
```

`SynchronousEvent`

### BATTLEFIELDS_CLOSED

```lua
BATTLEFIELDS_CLOSED()
```

`SynchronousEvent`

### BATTLEFIELDS_SHOW

```lua
BATTLEFIELDS_SHOW(isArena: bool?, battleMasterListID: number?)
```

`SynchronousEvent`

### BATTLEGROUND_OBJECTIVES_UPDATE

```lua
BATTLEGROUND_OBJECTIVES_UPDATE()
```

`SynchronousEvent`

### BATTLEGROUND_POINTS_UPDATE

```lua
BATTLEGROUND_POINTS_UPDATE()
```

`SynchronousEvent`

### GDF_SIM_COMPLETE

```lua
GDF_SIM_COMPLETE()
```

`SynchronousEvent`

### HONOR_LEVEL_UPDATE

```lua
HONOR_LEVEL_UPDATE(isHigherLevel: bool)
```

`SynchronousEvent`

### NOTIFY_PVP_AFK_RESULT

```lua
NOTIFY_PVP_AFK_RESULT(offender: cstring, numBlackMarksOnOffender: number, numPlayersIHaveReported: number)
```

`SynchronousEvent`

### PLAYER_ENTERING_BATTLEGROUND

```lua
PLAYER_ENTERING_BATTLEGROUND()
```

`SynchronousEvent`

### PLAYER_JOINED_PVP_MATCH

```lua
PLAYER_JOINED_PVP_MATCH()
```

`SynchronousEvent`

### PLAYER_PVP_FLAG_CHANGED

```lua
PLAYER_PVP_FLAG_CHANGED(isPvpFlagged: bool)
```

`SynchronousEvent`

### POST_MATCH_CURRENCY_REWARD_UPDATE

```lua
POST_MATCH_CURRENCY_REWARD_UPDATE(reward: PVPPostMatchCurrencyReward)
```

`SynchronousEvent`

### POST_MATCH_ITEM_REWARD_UPDATE

```lua
POST_MATCH_ITEM_REWARD_UPDATE()
```

`SynchronousEvent`

### PVP_BRAWL_INFO_UPDATED

```lua
PVP_BRAWL_INFO_UPDATED()
```

`SynchronousEvent`

### PVP_MATCH_ACTIVE

```lua
PVP_MATCH_ACTIVE()
```

`SynchronousEvent`

### PVP_MATCH_COMPLETE

```lua
PVP_MATCH_COMPLETE(winner: number, duration: time_t)
```

`SynchronousEvent`

### PVP_MATCH_INACTIVE

```lua
PVP_MATCH_INACTIVE()
```

`SynchronousEvent`

### PVP_MATCH_STATE_CHANGED

```lua
PVP_MATCH_STATE_CHANGED()
```

`SynchronousEvent`

### PVPQUEUE_ANYWHERE_SHOW

```lua
PVPQUEUE_ANYWHERE_SHOW()
```

`SynchronousEvent`

### PVPQUEUE_ANYWHERE_UPDATE_AVAILABLE

```lua
PVPQUEUE_ANYWHERE_UPDATE_AVAILABLE()
```

`SynchronousEvent`

### PVP_RATED_STATS_UPDATE

```lua
PVP_RATED_STATS_UPDATE()
```

`SynchronousEvent`

### PVP_REWARDS_UPDATE

```lua
PVP_REWARDS_UPDATE()
```

`SynchronousEvent`

### PVP_ROLE_POPUP_HIDE

```lua
PVP_ROLE_POPUP_HIDE(readyCheckInfo: PvpReadyCheckInfo?)
```

`SynchronousEvent`

### PVP_ROLE_POPUP_SHOW

```lua
PVP_ROLE_POPUP_SHOW(readyCheckInfo: PvpReadyCheckInfo)
```

`SynchronousEvent`

### PVP_ROLE_UPDATE

```lua
PVP_ROLE_UPDATE()
```

`SynchronousEvent`

### PVP_SPECIAL_EVENT_INFO_UPDATED

```lua
PVP_SPECIAL_EVENT_INFO_UPDATED()
```

`SynchronousEvent`

### PVP_TYPES_ENABLED

```lua
PVP_TYPES_ENABLED(wargameBattlegrounds: bool, ratedBattlegrounds: bool, ratedArenas: bool, ratedSoloShuffle: bool, ratedBGBlitz: bool)
```

`SynchronousEvent`

### PVP_VEHICLE_INFO_UPDATED

```lua
PVP_VEHICLE_INFO_UPDATED()
```

`UniqueEvent`

### PVP_WORLDSTATE_UPDATE

```lua
PVP_WORLDSTATE_UPDATE()
```

`SynchronousEvent`

### TRAINING_GROUNDS_ENABLED_STATUS_UPDATED

```lua
TRAINING_GROUNDS_ENABLED_STATUS_UPDATED()
```

`SynchronousEvent`

### UPDATE_ACTIVE_BATTLEFIELD

```lua
UPDATE_ACTIVE_BATTLEFIELD()
```

`SynchronousEvent`

### UPDATE_BATTLEFIELD_SCORE

```lua
UPDATE_BATTLEFIELD_SCORE()
```

`SynchronousEvent`

### UPDATE_BATTLEFIELD_STATUS

```lua
UPDATE_BATTLEFIELD_STATUS(battleFieldIndex: number)
```

`SynchronousEvent`

### WARGAME_INVITE_SENT

```lua
WARGAME_INVITE_SENT()
```

`SynchronousEvent`

### WARGAME_REQUESTED

```lua
WARGAME_REQUESTED(opposingPartyMemberName: cstring, battlegroundName: cstring, timeoutSeconds: time_t, tournamentRules: bool)
```

`SynchronousEvent`

### WARGAME_REQUEST_RESPONSE

```lua
WARGAME_REQUEST_RESPONSE(responderGUID: WOWGUID, responderName: cstring?, accepted: bool)
```

`SynchronousEvent`

### WAR_MODE_STATUS_UPDATE

```lua
WAR_MODE_STATUS_UPDATE(warModeEnabled: bool)
```

`SynchronousEvent`

### WORLD_PVP_QUEUE

```lua
WORLD_PVP_QUEUE()
```

`SynchronousEvent`

## Types

### BrawlType

*Enumeration* · 6 values, 0..5

Access values as `Enum.BrawlType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `BrawlType` | = 0 |
| `Battleground` | `BrawlType` | = 1 |
| `Arena` | `BrawlType` | = 2 |
| `LFG` | `BrawlType` | = 3 |
| `SoloShuffle` | `BrawlType` | = 4 |
| `SoloRbg` | `BrawlType` | = 5 |

### PvPMatchState

*Enumeration* · 6 values, 0..5

Access values as `Enum.PvPMatchState.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Inactive` | `PvPMatchState` | = 0 |
| `Waiting` | `PvPMatchState` | = 1 |
| `StartUp` | `PvPMatchState` | = 2 |
| `Engaged` | `PvPMatchState` | = 3 |
| `PostRound` | `PvPMatchState` | = 4 |
| `Complete` | `PvPMatchState` | = 5 |

### BattlefieldCurrencyReward

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `id` | `number` |  |
| `quantity` | `number` |  |

### BattlefieldItemReward

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `id` | `number` |  |
| `name` | `cstring` |  |
| `texture` | `fileID` |  |
| `quantity` | `number` |  |

### BattlefieldRewards

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `honor` | `number` |  |
| `experience` | `number` |  |
| `itemRewards` | `BattlefieldItemReward[]?` |  |
| `currencyRewards` | `BattlefieldCurrencyReward[]?` |  |
| `roleShortageBonus` | `RoleShortageReward?` |  |

### BattlefieldVehicleInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `x` | `number` |  |
| `y` | `number` |  |
| `name` | `cstring` |  |
| `isOccupied` | `bool` |  |
| `atlas` | `textureAtlas` |  |
| `textureWidth` | `number` |  |
| `textureHeight` | `number` |  |
| `facing` | `number` |  |
| `isPlayer` | `bool` |  |
| `isAlive` | `bool` |  |
| `shouldDrawBelowPlayerBlips` | `bool` |  |

### BattlegroundInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `icon` | `fileID?` |  |
| `gameType` | `cstring` |  |
| `shortDescription` | `cstring` |  |
| `longDescription` | `cstring` |  |
| `mapDescription` | `cstring` |  |
| `maxPlayers` | `number` |  |
| `battlegroundID` | `number?` |  |
| `lfgDungeonID` | `number?` |  |
| `mapID` | `number?` |  |
| `isHoliday` | `bool` |  |
| `isRandom` | `bool` |  |
| `canEnter` | `bool` |  |
| `isTrainingGround` | `bool` |  |

### BattlemasterListInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `matchmakingType` | `PvPMatchmakingType` |  |
| `minPlayers` | `number` |  |
| `maxPlayers` | `number` |  |
| `icon` | `fileID` |  |
| `longDescription` | `string` |  |
| `shortDescription` | `string` |  |

### HonorRewardInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `honorLevelName` | `string` |  |
| `badgeFileDataID` | `fileID` |  |
| `achievementRewardedID` | `number` |  |

### LevelUpBattlegroundInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `id` | `number` |  |
| `icon` | `fileID` |  |
| `name` | `string` |  |
| `isEpic` | `bool` |  |

### MatchPVPStatColumn

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `pvpStatID` | `number` |  |
| `columnHeaderID` | `number` |  |
| `orderIndex` | `number` |  |
| `name` | `string` |  |
| `tooltipTitle` | `string` |  |
| `tooltip` | `string` |  |

### PvpBrawlInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `brawlID` | `number` |  |
| `name` | `string` |  |
| `shortDescription` | `string` |  |
| `longDescription` | `string` |  |
| `canQueue` | `bool` |  |
| `minLevel` | `number` |  |
| `maxLevel` | `number` |  |
| `groupsAllowed` | `bool` |  |
| `crossFactionAllowed` | `bool` | default `false` |
| `timeLeftUntilNextChange` | `number?` |  |
| `brawlType` | `BrawlType` |  |
| `mapNames` | `string[]` |  |
| `includesAllArenas` | `bool` | default `false` |
| `minItemLevel` | `number` | default `0` |
| `shouldHideRewardIcon` | `bool` | default `false` |

### PVPPersonalRatedInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `personalRating` | `number` |  |
| `bestSeasonRating` | `number` |  |
| `bestWeeklyRating` | `number` |  |
| `seasonPlayed` | `number` |  |
| `seasonWon` | `number` |  |
| `weeklyPlayed` | `number` |  |
| `weeklyWon` | `number` |  |
| `lastWeeksBestRating` | `number` |  |
| `hasWonBracketToday` | `bool` |  |
| `tier` | `number` |  |
| `ranking` | `number?` |  |
| `roundsSeasonPlayed` | `number` |  |
| `roundsSeasonWon` | `number` |  |
| `roundsWeeklyPlayed` | `number` |  |
| `roundsWeeklyWon` | `number` |  |

### PVPPostMatchCurrencyReward

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `currencyType` | `number` |  |
| `quantityChanged` | `number` |  |

### PVPPostMatchItemReward

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `type` | `string` |  |
| `link` | `string` |  |
| `quantity` | `number` |  |
| `specID` | `number` |  |
| `sex` | `number` |  |
| `isUpgraded` | `bool` |  |

### PvpReadyCheckInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `roles` | `PvpRoleQueueInfo[]` |  |
| `numPlayersAccepted` | `number` |  |
| `numPlayersDeclined` | `number` |  |
| `totalNumPlayers` | `number` |  |

### PvpRoleQueueInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `role` | `cstring` |  |
| `totalRole` | `number` |  |
| `totalAccepted` | `number` |  |
| `totalDeclined` | `number` |  |

### PvpScalingData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `scalingDataID` | `number` |  |
| `specializationID` | `number` |  |
| `name` | `cstring` |  |
| `value` | `number` |  |

### PVPScoreInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `killingBlows` | `number` |  |
| `honorableKills` | `number` |  |
| `deaths` | `number` |  |
| `honorGained` | `number` |  |
| `faction` | `number` | `NeverSecret` |
| `raceName` | `string` | `NeverSecret` |
| `gender` | `number` | `NeverSecret` |
| `className` | `string` | `NeverSecret` |
| `classToken` | `string` | `NeverSecret` |
| `damageDone` | `number` |  |
| `healingDone` | `number` |  |
| `rating` | `number` |  |
| `ratingChange` | `number` |  |
| `prematchMMR` | `number` |  |
| `mmrChange` | `number` |  |
| `postmatchMMR` | `number` |  |
| `talentSpec` | `string` |  |
| `honorLevel` | `number` | `NeverSecret` |
| `roleAssigned` | `number` |  |
| `stats` | `PVPStatInfo[]` |  |

### PVPStatInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `pvpStatID` | `number` | `NeverSecret` |
| `pvpStatValue` | `number` |  |
| `orderIndex` | `number` | `NeverSecret` |
| `name` | `string` | `NeverSecret` |
| `tooltip` | `string` | `NeverSecret` |
| `iconName` | `string` | `NeverSecret` |

### PVPTeamInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `size` | `number` |  |
| `rating` | `number` |  |
| `ratingNew` | `number` |  |
| `ratingMMR` | `number` |  |

### PvpTierInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `descendRating` | `number` |  |
| `ascendRating` | `number` |  |
| `descendTier` | `number` |  |
| `ascendTier` | `number` |  |
| `pvpTierEnum` | `number` |  |
| `tierIconID` | `fileID` |  |

### RandomBGInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `canQueue` | `bool` |  |
| `bgID` | `number` |  |
| `bgIndex` | `luaIndex` |  |
| `hasRandomWinToday` | `bool` |  |
| `minLevel` | `number` |  |
| `maxLevel` | `number` |  |
| `name` | `string` |  |

### RatedBGBlitzSpecStats

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `weeklyMostPlayedSpecID` | `number` |  |
| `weeklyMostPlayedSpecGames` | `number` |  |
| `seasonMostPlayedSpecID` | `number` |  |
| `seasonMostPlayedSpecGames` | `number` |  |

### RatedMatchDeserterPenalty

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `personalRatingChange` | `number` |  |
| `queuePenaltySpellID` | `number` |  |
| `queuePenaltyDuration` | `number` |  |

### RatedSoloShuffleSpecStats

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `weeklyMostPlayedSpecID` | `number` |  |
| `weeklyMostPlayedSpecRounds` | `number` |  |
| `seasonMostPlayedSpecID` | `number` |  |
| `seasonMostPlayedSpecRounds` | `number` |  |

### RoleShortageReward

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `validRoles` | `cstring[]` |  |
| `rewardSpellID` | `number` |  |
| `rewardItemID` | `number` |  |

### WorldPVPBattlegroundInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `bgID` | `number` |  |
| `name` | `string` |  |
| `isActive` | `bool` |  |
| `canQueue` | `bool` |  |
| `canEnter` | `bool` |  |
| `startTime` | `time_t` |  |
| `minLevel` | `number` |  |
| `maxLevel` | `number` |  |
