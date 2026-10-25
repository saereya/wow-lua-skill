# CommentatorFrame

Namespace `C_Commentator` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/commentatorframedocumentation.lua` (FileDataID 4637057)

## Functions

### AddPlayerOverrideName

```lua
C_Commentator.AddPlayerOverrideName(playerName: string, overrideName: string)
```

`SecretArguments=AllowedWhenUntainted`

### AddTrackedDefensiveAuras

```lua
C_Commentator.AddTrackedDefensiveAuras(spellIDs: number[])
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### AddTrackedOffensiveAuras

```lua
C_Commentator.AddTrackedOffensiveAuras(spellIDs: number[])
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### AreTeamsSwapped

```lua
C_Commentator.AreTeamsSwapped() -> teamsAreSwapped: bool
```

### AssignPlayersToTeam

```lua
C_Commentator.AssignPlayersToTeam(playerName: string[], teamName: string)
```

`SecretArguments=AllowedWhenUntainted`

### AssignPlayersToTeamInCurrentInstance

```lua
C_Commentator.AssignPlayersToTeamInCurrentInstance(teamIndex: luaIndex, teamName: string)
```

`SecretArguments=AllowedWhenUntainted`

### AssignPlayerToTeam

```lua
C_Commentator.AssignPlayerToTeam(playerName: string, teamName: string)
```

`SecretArguments=AllowedWhenUntainted`

### CanUseCommentatorCheats

```lua
C_Commentator.CanUseCommentatorCheats() -> canUseCommentatorCheats: bool
```

### ClearCameraTarget

```lua
C_Commentator.ClearCameraTarget()
```

`RequiresActiveCommentator`

### ClearFollowTarget

```lua
C_Commentator.ClearFollowTarget()
```

`RequiresActiveCommentator`

### ClearLookAtTarget

```lua
C_Commentator.ClearLookAtTarget(lookAtIndex: luaIndex?)
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### EnterInstance

```lua
C_Commentator.EnterInstance()
```

`RequiresCommentator`

### ExitInstance

```lua
C_Commentator.ExitInstance()
```

`RequiresCommentator`

### FindSpectatedUnit

```lua
C_Commentator.FindSpectatedUnit(unitToken: UnitToken) -> playerIndex: luaIndex, teamIndex: luaIndex, isPet: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresActiveCommentator`

### FindTeamNameInCurrentInstance

```lua
C_Commentator.FindTeamNameInCurrentInstance(teamIndex: luaIndex) -> teamName: string?
```

`SecretArguments=AllowedWhenUntainted`

### FindTeamNameInDirectory

```lua
C_Commentator.FindTeamNameInDirectory(playerNames: string[]) -> teamName: string?
```

`SecretArguments=AllowedWhenUntainted`

### FlushCommentatorHistory

```lua
C_Commentator.FlushCommentatorHistory()
```

### FollowPlayer

```lua
C_Commentator.FollowPlayer(factionIndex: luaIndex, playerIndex: luaIndex, forceInstantTransition: bool?)
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### FollowUnit

```lua
C_Commentator.FollowUnit(token: string)
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### ForceFollowTransition

```lua
C_Commentator.ForceFollowTransition()
```

`RequiresActiveCommentator`

### GetAdditionalCameraWeight

```lua
C_Commentator.GetAdditionalCameraWeight() -> teamIndex: luaIndex, playerIndex: luaIndex
```

`RequiresActiveCommentator`

### GetAdditionalCameraWeightByToken

```lua
C_Commentator.GetAdditionalCameraWeightByToken(unitToken: UnitToken) -> weight: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresActiveCommentator`

### GetAllPlayerOverrideNames

```lua
C_Commentator.GetAllPlayerOverrideNames() -> nameEntries: NameOverrideEntry[]
```

`RequiresActiveCommentator`

### GetCamera

```lua
C_Commentator.GetCamera() -> xPos: number, yPos: number, zPos: number, yaw: number, pitch: number, roll: number, fov: number
```

`MayReturnNothing` `RequiresActiveCommentator`

### GetCameraCollision

```lua
C_Commentator.GetCameraCollision() -> isColliding: bool
```

### GetCameraPosition

```lua
C_Commentator.GetCameraPosition() -> xPos: number, yPos: number, zPos: number
```

`MayReturnNothing` `RequiresActiveCommentator`

### GetCombatEventInfo

```lua
C_Commentator.GetCombatEventInfo()
```

`RequiresActiveCommentator`

### GetCommentatorHistory

```lua
C_Commentator.GetCommentatorHistory() -> history: CommentatorHistory
```

### GetCommentatorMatchDataState

```lua
C_Commentator.GetCommentatorMatchDataState() -> state: CommentatorMatchDataState
```

`RequiresActiveCommentator`

### GetCurrentMapID

```lua
C_Commentator.GetCurrentMapID() -> mapID: number?
```

`RequiresCommentator`

### GetDampeningPercent

```lua
C_Commentator.GetDampeningPercent() -> percentage: number
```

### GetDistanceBeforeForcedHorizontalConvergence

```lua
C_Commentator.GetDistanceBeforeForcedHorizontalConvergence() -> distance: number
```

### GetDurationToForceHorizontalConvergence

```lua
C_Commentator.GetDurationToForceHorizontalConvergence() -> ms: number
```

### GetExcludeDistance

```lua
C_Commentator.GetExcludeDistance() -> excludeDistance: number
```

### GetHardlockWeight

```lua
C_Commentator.GetHardlockWeight() -> weight: number
```

### GetHorizontalAngleThresholdToSmooth

```lua
C_Commentator.GetHorizontalAngleThresholdToSmooth() -> angle: number
```

### GetIndirectSpellID

```lua
C_Commentator.GetIndirectSpellID(trackedSpellID: number) -> indirectSpellID: number
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### GetInstanceInfo

```lua
C_Commentator.GetInstanceInfo(mapIndex: luaIndex, instanceIndex: luaIndex) -> mapID: number, mapName: string?, status: number, instanceIDLow: number, instanceIDHigh: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresCommentator`

### GetLookAtLerpAmount

```lua
C_Commentator.GetLookAtLerpAmount() -> amount: number
```

### GetMapInfo

```lua
C_Commentator.GetMapInfo(mapIndex: luaIndex) -> teamSize: number, minLevel: number, maxLevel: number, numInstances: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresCommentator`

### GetMatchDuration

```lua
C_Commentator.GetMatchDuration() -> seconds: time_t
```

### GetMaxNumPlayersPerTeam

```lua
C_Commentator.GetMaxNumPlayersPerTeam() -> maxNumPlayersPerTeam: number
```

### GetMaxNumTeams

```lua
C_Commentator.GetMaxNumTeams() -> maxNumTeams: number
```

### GetMode

```lua
C_Commentator.GetMode() -> commentatorMode: number
```

### GetMsToHoldForHorizontalMovement

```lua
C_Commentator.GetMsToHoldForHorizontalMovement() -> ms: number
```

### GetMsToHoldForVerticalMovement

```lua
C_Commentator.GetMsToHoldForVerticalMovement() -> ms: number
```

### GetMsToSmoothHorizontalChange

```lua
C_Commentator.GetMsToSmoothHorizontalChange() -> ms: number
```

### GetMsToSmoothVerticalChange

```lua
C_Commentator.GetMsToSmoothVerticalChange() -> ms: number
```

### GetNumMaps

```lua
C_Commentator.GetNumMaps() -> numMaps: number
```

### GetNumPlayers

```lua
C_Commentator.GetNumPlayers(factionIndex: luaIndex) -> numPlayers: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresActiveCommentator`

### GetOrCreateSeries

```lua
C_Commentator.GetOrCreateSeries(teamName1: string, teamName2: string) -> data: CommentatorSeries
```

`SecretArguments=AllowedWhenUntainted`

### GetPlayerAuraInfo

```lua
C_Commentator.GetPlayerAuraInfo(teamIndex: luaIndex, playerIndex: luaIndex, spellID: number) -> startTime: number, duration: number, enable: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresActiveCommentator`

### GetPlayerAuraInfoByUnit

```lua
C_Commentator.GetPlayerAuraInfoByUnit(token: UnitToken, spellID: number) -> startTime: number, duration: number, enable: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresActiveCommentator`

### GetPlayerCooldownInfo

```lua
C_Commentator.GetPlayerCooldownInfo(teamIndex: luaIndex, playerIndex: luaIndex, spellID: number) -> startTime: number, duration: number, enable: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresActiveCommentator`

### GetPlayerCooldownInfoByUnit

```lua
C_Commentator.GetPlayerCooldownInfoByUnit(unitToken: UnitToken, spellID: number) -> startTime: number, duration: number, enable: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresActiveCommentator`

### GetPlayerCrowdControlInfo

```lua
C_Commentator.GetPlayerCrowdControlInfo(teamIndex: luaIndex, playerIndex: luaIndex) -> spellID: number, expiration: number, duration: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresActiveCommentator`

### GetPlayerCrowdControlInfoByUnit

```lua
C_Commentator.GetPlayerCrowdControlInfoByUnit(token: UnitToken) -> spellID: number, expiration: number, duration: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresActiveCommentator`

### GetPlayerData

```lua
C_Commentator.GetPlayerData(teamIndex: luaIndex, playerIndex: luaIndex) -> info: CommentatorPlayerData?
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### GetPlayerFlagInfo

```lua
C_Commentator.GetPlayerFlagInfo(teamIndex: luaIndex, playerIndex: luaIndex) -> hasFlag: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### GetPlayerFlagInfoByUnit

```lua
C_Commentator.GetPlayerFlagInfoByUnit(unitToken: UnitToken) -> hasFlag: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### GetPlayerItemCooldownInfo

```lua
C_Commentator.GetPlayerItemCooldownInfo(teamIndex: luaIndex, playerIndex: luaIndex, itemID: number) -> startTime: number, duration: number, enable: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresActiveCommentator`

### GetPlayerItemCooldownInfoByUnit

```lua
C_Commentator.GetPlayerItemCooldownInfoByUnit(unitToken: UnitToken, itemID: number) -> startTime: number, duration: number, enable: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresActiveCommentator`

### GetPlayerOverrideName

```lua
C_Commentator.GetPlayerOverrideName(originalName: string) -> overrideName: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetPlayerSpellCharges

```lua
C_Commentator.GetPlayerSpellCharges(teamIndex: luaIndex, playerIndex: luaIndex, spellID: number) -> charges: number, maxCharges: number, startTime: number, duration: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresActiveCommentator`

### GetPlayerSpellChargesByUnit

```lua
C_Commentator.GetPlayerSpellChargesByUnit(unitToken: UnitToken, spellID: number) -> charges: number, maxCharges: number, startTime: number, duration: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresActiveCommentator`

### GetPositionLerpAmount

```lua
C_Commentator.GetPositionLerpAmount() -> amount: number
```

### GetSmoothFollowTransitioning

```lua
C_Commentator.GetSmoothFollowTransitioning() -> enabled: bool
```

`RequiresActiveCommentator`

### GetSoftlockWeight

```lua
C_Commentator.GetSoftlockWeight() -> weight: number
```

### GetSpeedFactor

```lua
C_Commentator.GetSpeedFactor() -> factor: number
```

### GetStartLocation

```lua
C_Commentator.GetStartLocation(mapID: number) -> pos: vector3
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `pos` | `vector3` | `Mixin=Vector3DMixin` |

### GetTeamColor

```lua
C_Commentator.GetTeamColor(teamIndex: luaIndex) -> color: colorRGB
```

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `color` | `colorRGB` | `Mixin=ColorMixin` |

### GetTeamColorByUnit

```lua
C_Commentator.GetTeamColorByUnit(unitToken: UnitToken) -> color: colorRGB
```

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `color` | `colorRGB` | `Mixin=ColorMixin` |

### GetTimeLeftInMatch

```lua
C_Commentator.GetTimeLeftInMatch() -> timeLeft: number?
```

### GetTrackedSpellID

```lua
C_Commentator.GetTrackedSpellID(indirectSpellID: number) -> trackedSpellID: number
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### GetTrackedSpells

```lua
C_Commentator.GetTrackedSpells(teamIndex: luaIndex, playerIndex: luaIndex, category: TrackedSpellCategory) -> spells: number[]?, result: TrackedSpellsResult
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### GetTrackedSpellsByUnit

```lua
C_Commentator.GetTrackedSpellsByUnit(unitToken: UnitToken, category: TrackedSpellCategory) -> spells: number[]?, result: TrackedSpellsResult
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### GetUnitData

```lua
C_Commentator.GetUnitData(unitToken: UnitToken) -> data: CommentatorUnitData
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### GetWargameInfo

```lua
C_Commentator.GetWargameInfo(listID: number) -> name: string, minPlayers: number, maxPlayers: number, isArena: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresCommentator`

### HasTrackedAuras

```lua
C_Commentator.HasTrackedAuras(token: UnitToken) -> hasOffensiveAura: bool, hasDefensiveAura: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### IsSmartCameraLocked

```lua
C_Commentator.IsSmartCameraLocked() -> isSmartCameraLocked: bool
```

### IsSpectating

```lua
C_Commentator.IsSpectating() -> isSpectating: bool
```

### IsTrackedDefensiveAura

```lua
C_Commentator.IsTrackedDefensiveAura(spellID: number) -> isDefensiveTrigger: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### IsTrackedOffensiveAura

```lua
C_Commentator.IsTrackedOffensiveAura(spellID: number) -> isOffensiveTrigger: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### IsTrackedSpell

```lua
C_Commentator.IsTrackedSpell(teamIndex: luaIndex, playerIndex: luaIndex, spellID: number, category: TrackedSpellCategory) -> isTracked: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### IsTrackedSpellByUnit

```lua
C_Commentator.IsTrackedSpellByUnit(unitToken: UnitToken, spellID: number, category: TrackedSpellCategory) -> isTracked: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### IsUsingSmartCamera

```lua
C_Commentator.IsUsingSmartCamera() -> isUsingSmartCamera: bool
```

### LookAtPlayer

```lua
C_Commentator.LookAtPlayer(factionIndex: luaIndex, playerIndex: luaIndex, lookAtIndex: luaIndex?)
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### RemoveAllOverrideNames

```lua
C_Commentator.RemoveAllOverrideNames()
```

### RemovePlayerOverrideName

```lua
C_Commentator.RemovePlayerOverrideName(originalPlayerName: string)
```

`SecretArguments=AllowedWhenUntainted`

### RequestPlayerCooldownInfo

```lua
C_Commentator.RequestPlayerCooldownInfo(teamIndex: luaIndex, playerIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### ResetFoVTarget

```lua
C_Commentator.ResetFoVTarget()
```

### ResetSeriesScores

```lua
C_Commentator.ResetSeriesScores(teamName1: string, teamName2: string)
```

`SecretArguments=AllowedWhenUntainted`

### ResetSettings

```lua
C_Commentator.ResetSettings()
```

### ResetTrackedAuras

```lua
C_Commentator.ResetTrackedAuras()
```

`RequiresActiveCommentator`

### SendAddonMessage

```lua
C_Commentator.SendAddonMessage(prefix: cstring, message: cstring, chatType: cstring?, target: cstring?) -> result: SendAddonMessageResult
```

Works the same as C_ChatInfo.SendAddonMessage but accepts secrets and is only allowed when outgoing addon comms are allowed (i.e. on tournament realms)

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `prefix` | `cstring` |  |
| `message` | `cstring` |  |
| `chatType` | `cstring?` | ChatType, defaults to SLASH_CMD_PARTY. |
| `target` | `cstring?` | Only applies for targeted channels |

### SendAddonMessageLogged

```lua
C_Commentator.SendAddonMessageLogged(prefix: cstring, message: cstring, chatType: cstring?, target: cstring?) -> result: SendAddonMessageResult?
```

Works the same as C_ChatInfo.SendAddonMessageLogged but accepts secrets and is only allowed when outgoing addon comms are allowed (i.e. on tournament realms)

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `prefix` | `cstring` |  |
| `message` | `cstring` |  |
| `chatType` | `cstring?` | ChatType, defaults to SLASH_CMD_PARTY. |
| `target` | `cstring?` | Only applies for targeted channels |

### SetAdditionalCameraWeight

```lua
C_Commentator.SetAdditionalCameraWeight(teamIndex: luaIndex, playerIndex: luaIndex, weight: number)
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### SetAdditionalCameraWeightByToken

```lua
C_Commentator.SetAdditionalCameraWeightByToken(unitToken: UnitToken, weight: number)
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### SetBlocklistedAuras

```lua
C_Commentator.SetBlocklistedAuras(spellIDs: number[])
```

`SecretArguments=AllowedWhenUntainted`

### SetBlocklistedCooldowns

```lua
C_Commentator.SetBlocklistedCooldowns(specID: number, spellIDs: number[])
```

`SecretArguments=AllowedWhenUntainted`

### SetBlocklistedItemCooldowns

```lua
C_Commentator.SetBlocklistedItemCooldowns(itemIDs: number[])
```

`SecretArguments=AllowedWhenUntainted`

### SetCamera

```lua
C_Commentator.SetCamera(xPos: number, yPos: number, zPos: number, yaw: number, pitch: number, roll: number, fov: number)
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### SetCameraCollision

```lua
C_Commentator.SetCameraCollision(collide: bool)
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### SetCameraPosition

```lua
C_Commentator.SetCameraPosition(xPos: number, yPos: number, zPos: number, snapToLocation: bool)
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### SetCheatsEnabled

```lua
C_Commentator.SetCheatsEnabled(enableCheats: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetCommentatorHistory

```lua
C_Commentator.SetCommentatorHistory(history: CommentatorHistory)
```

`SecretArguments=AllowedWhenUntainted`

### SetDistanceBeforeForcedHorizontalConvergence

```lua
C_Commentator.SetDistanceBeforeForcedHorizontalConvergence(distance: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetDurationToForceHorizontalConvergence

```lua
C_Commentator.SetDurationToForceHorizontalConvergence(ms: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetExcludeDistance

```lua
C_Commentator.SetExcludeDistance(excludeDistance: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetFollowCameraSpeeds

```lua
C_Commentator.SetFollowCameraSpeeds(elasticSpeed: number, minSpeed: number)
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### SetHardlockWeight

```lua
C_Commentator.SetHardlockWeight(weight: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetHorizontalAngleThresholdToSmooth

```lua
C_Commentator.SetHorizontalAngleThresholdToSmooth(angle: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetLookAtLerpAmount

```lua
C_Commentator.SetLookAtLerpAmount(amount: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetMapAndInstanceIndex

```lua
C_Commentator.SetMapAndInstanceIndex(mapIndex: luaIndex, instanceIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted` `RequiresCommentator`

### SetMouseDisabled

```lua
C_Commentator.SetMouseDisabled(disabled: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetMoveSpeed

```lua
C_Commentator.SetMoveSpeed(newSpeed: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetMsToHoldForHorizontalMovement

```lua
C_Commentator.SetMsToHoldForHorizontalMovement(ms: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetMsToHoldForVerticalMovement

```lua
C_Commentator.SetMsToHoldForVerticalMovement(ms: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetMsToSmoothHorizontalChange

```lua
C_Commentator.SetMsToSmoothHorizontalChange(ms: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetMsToSmoothVerticalChange

```lua
C_Commentator.SetMsToSmoothVerticalChange(ms: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetPositionLerpAmount

```lua
C_Commentator.SetPositionLerpAmount(amount: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetRequestedDebuffCooldowns

```lua
C_Commentator.SetRequestedDebuffCooldowns(specID: number, spellIDs: number[])
```

`SecretArguments=AllowedWhenUntainted`

### SetRequestedDefensiveCooldowns

```lua
C_Commentator.SetRequestedDefensiveCooldowns(specID: number, spellIDs: number[])
```

`SecretArguments=AllowedWhenUntainted`

### SetRequestedItemCooldowns

```lua
C_Commentator.SetRequestedItemCooldowns(itemIDs: number[])
```

`SecretArguments=AllowedWhenUntainted`

### SetRequestedOffensiveCooldowns

```lua
C_Commentator.SetRequestedOffensiveCooldowns(specID: number, spellIDs: number[])
```

`SecretArguments=AllowedWhenUntainted`

### SetSeriesScore

```lua
C_Commentator.SetSeriesScore(teamName1: string, teamName2: string, scoringTeamName: string, score: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetSeriesScores

```lua
C_Commentator.SetSeriesScores(teamName1: string, teamName2: string, score1: number, score2: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetSmartCameraLocked

```lua
C_Commentator.SetSmartCameraLocked(locked: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetSmoothFollowTransitioning

```lua
C_Commentator.SetSmoothFollowTransitioning(enabled: bool)
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### SetSoftlockWeight

```lua
C_Commentator.SetSoftlockWeight(weight: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetSpeedFactor

```lua
C_Commentator.SetSpeedFactor(factor: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetTargetHeightOffset

```lua
C_Commentator.SetTargetHeightOffset(offset: number)
```

`SecretArguments=AllowedWhenUntainted` `RequiresActiveCommentator`

### SetUseSmartCamera

```lua
C_Commentator.SetUseSmartCamera(useSmartCamera: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SnapCameraLookAtPoint

```lua
C_Commentator.SnapCameraLookAtPoint()
```

`RequiresActiveCommentator`

### SpellUsesItemCharges

```lua
C_Commentator.SpellUsesItemCharges(spellID: number) -> spellUsesItemCharges: bool
```

`SecretArguments=AllowedWhenUntainted`

### StartWargame

```lua
C_Commentator.StartWargame(listID: number, teamSize: number, tournamentRules: bool, teamOneCaptain: string, teamTwoCaptain: string)
```

`SecretArguments=AllowedWhenUntainted` `RequiresCommentator`

### SwapTeamSides

```lua
C_Commentator.SwapTeamSides()
```

### ToggleCheats

```lua
C_Commentator.ToggleCheats()
```

### UpdateMapInfo

```lua
C_Commentator.UpdateMapInfo(targetPlayer: string?)
```

`SecretArguments=AllowedWhenUntainted` `RequiresCommentator`

### UpdatePlayerInfo

```lua
C_Commentator.UpdatePlayerInfo()
```

`RequiresCommentator`

### ZoomIn

```lua
C_Commentator.ZoomIn()
```

### ZoomIn_Position

```lua
C_Commentator.ZoomIn_Position(zoomAmount: number?)
```

`SecretArguments=AllowedWhenUntainted`

### ZoomOut

```lua
C_Commentator.ZoomOut()
```

### ZoomOut_Position

```lua
C_Commentator.ZoomOut_Position(zoomAmount: number?)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### COMMENTATOR_COMBAT_EVENT

```lua
COMMENTATOR_COMBAT_EVENT()
```

`SynchronousEvent`

### COMMENTATOR_ENTER_WORLD

```lua
COMMENTATOR_ENTER_WORLD()
```

`SynchronousEvent`

### COMMENTATOR_HISTORY_FLUSHED

```lua
COMMENTATOR_HISTORY_FLUSHED()
```

`SynchronousEvent`

### COMMENTATOR_IMMEDIATE_FOV_UPDATE

```lua
COMMENTATOR_IMMEDIATE_FOV_UPDATE(fov: number)
```

`SynchronousEvent`

### COMMENTATOR_MAP_UPDATE

```lua
COMMENTATOR_MAP_UPDATE()
```

`SynchronousEvent`

### COMMENTATOR_PLAYER_NAME_OVERRIDE_UPDATE

```lua
COMMENTATOR_PLAYER_NAME_OVERRIDE_UPDATE(nameToOverride: cstring, overrideName: cstring?)
```

`SynchronousEvent`

### COMMENTATOR_PLAYER_UPDATE

```lua
COMMENTATOR_PLAYER_UPDATE()
```

`SynchronousEvent` `UniqueEvent`

### COMMENTATOR_RESET_SETTINGS

```lua
COMMENTATOR_RESET_SETTINGS()
```

`SynchronousEvent`

### COMMENTATOR_TEAM_NAME_UPDATE

```lua
COMMENTATOR_TEAM_NAME_UPDATE(teamName: string)
```

`SynchronousEvent`

### COMMENTATOR_TEAMS_SWAPPED

```lua
COMMENTATOR_TEAMS_SWAPPED(swapped: bool)
```

`SynchronousEvent`

## Types

### TrackedSpellsResult

*Enumeration* · 4 values, 0..3

Access values as `Enum.TrackedSpellsResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Success` | `TrackedSpellsResult` | = 0 |
| `PlayerNotFound` | `TrackedSpellsResult` | = 1 |
| `NoCooldownInfo` | `TrackedSpellsResult` | = 2 |
| `MismatchedCooldownInfo` | `TrackedSpellsResult` | = 3 |

### CommentatorHistory

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `series` | `CommentatorSeries[]` |  |
| `teamDirectory` | `CommentatorTeamDirectoryEntry[]` |  |
| `overrideNameDirectory` | `CommentatorOverrideNameEntry[]` |  |

### CommentatorMatchDataState

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `receivedPlayerInfo` | `bool` |  |
| `setInstancePlayers` | `bool` |  |
| `requestedCooldownInfo` | `bool` |  |
| `requestedPlayerCooldowns` | `TeamPlayerRequestedCooldownInfo[]` |  |

### CommentatorOverrideNameEntry

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `originalName` | `string` |  |
| `newName` | `string` |  |

### CommentatorPlayerData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `unitToken` | `string` |  |
| `name` | `string` |  |
| `faction` | `number` |  |
| `specialization` | `number` |  |
| `damageDone` | `number` |  |
| `damageTaken` | `number` |  |
| `healingDone` | `number` |  |
| `healingTaken` | `number` |  |
| `kills` | `number` |  |
| `deaths` | `number` |  |
| `soloShuffleRoundWins` | `number` |  |
| `soloShuffleRoundLosses` | `number` |  |

### CommentatorSeries

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `teams` | `CommentatorSeriesTeam[]` |  |

### CommentatorSeriesTeam

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `score` | `number` |  |

### CommentatorTeamDirectoryEntry

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `playerName` | `string` |  |
| `teamName` | `string` |  |

### CommentatorTrackedItemCooldown

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `number` |  |
| `category` | `TrackedSpellCategory` |  |

### CommentatorUnitData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `healthMax` | `number` |  |
| `health` | `number` |  |
| `absorbTotal` | `number` |  |
| `isDeadOrGhost` | `bool` |  |
| `isFeignDeath` | `bool` |  |
| `powerTypeToken` | `string` |  |
| `power` | `number` |  |
| `powerMax` | `number` |  |

### NameOverrideEntry

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `originalName` | `string` |  |
| `overrideName` | `string` |  |

### TeamPlayerRequestedCooldownInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `teamIndex` | `number` |  |
| `playerIndex` | `number` |  |
| `cooldownsRequested` | `number` |  |
