# GarrisonInfo

Namespace `C_Garrison` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/garrisoninfodocumentation.lua` (FileDataID 4637102)

## Functions

### AddFollowerToMission

```lua
C_Garrison.AddFollowerToMission(missionID: number, followerID: GarrisonFollower, boardIndex: number?) -> followerAdded: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetAutoCombatDamageClassValues

```lua
C_Garrison.GetAutoCombatDamageClassValues() -> damageClassStrings: AutoCombatDamageClassString[]
```

### GetAutoMissionBoardState

```lua
C_Garrison.GetAutoMissionBoardState(missionID: number) -> targetInfo: AutoMissionTargetingInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetAutoMissionEnvironmentEffect

```lua
C_Garrison.GetAutoMissionEnvironmentEffect(missionID: number) -> autoMissionEnvEffect: AutoMissionEnvironmentEffect?
```

`SecretArguments=AllowedWhenUntainted`

### GetAutoMissionTargetingInfo

```lua
C_Garrison.GetAutoMissionTargetingInfo(missionID: number, followerID: GarrisonFollower, casterBoardIndex: number) -> targetInfo: AutoMissionTargetingInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetAutoMissionTargetingInfoForSpell

```lua
C_Garrison.GetAutoMissionTargetingInfoForSpell(missionID: number, autoCombatSpellID: number, casterBoardIndex: number) -> targetInfo: AutoMissionTargetingInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetAutoTroops

```lua
C_Garrison.GetAutoTroops(followerType: number) -> autoTroopInfo: AutoCombatTroopInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetCombatLogSpellInfo

```lua
C_Garrison.GetCombatLogSpellInfo(autoCombatSpellID: number) -> spellInfo: AutoCombatSpellInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetCurrentCypherEquipmentLevel

```lua
C_Garrison.GetCurrentCypherEquipmentLevel() -> equipmentLevel: number
```

### GetCurrentGarrTalentTreeFriendshipFactionID

```lua
C_Garrison.GetCurrentGarrTalentTreeFriendshipFactionID() -> currentGarrTalentTreeFriendshipFactionID: number?
```

### GetCurrentGarrTalentTreeID

```lua
C_Garrison.GetCurrentGarrTalentTreeID() -> currentGarrTalentTreeID: number?
```

### GetCyphersToNextEquipmentLevel

```lua
C_Garrison.GetCyphersToNextEquipmentLevel() -> cyphersToNext: number?
```

### GetFollowerAutoCombatSpells

```lua
C_Garrison.GetFollowerAutoCombatSpells(garrFollowerID: GarrisonFollower, followerLevel: number) -> autoCombatSpells: AutoCombatSpellInfo[], autoCombatAutoAttack: AutoCombatSpellInfo?
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetFollowerAutoCombatStats

```lua
C_Garrison.GetFollowerAutoCombatStats(garrFollowerID: GarrisonFollower) -> autoCombatInfo: FollowerAutoCombatStatsInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetFollowerMissionCompleteInfo

```lua
C_Garrison.GetFollowerMissionCompleteInfo(followerID: GarrisonFollower) -> followerMissionCompleteInfo: FollowerMissionCompleteInfo
```

`SecretArguments=AllowedWhenUntainted`

### GetGarrisonPlotsInstancesForMap

```lua
C_Garrison.GetGarrisonPlotsInstancesForMap(uiMapID: number) -> garrisonPlotInstances: GarrisonPlotInstanceMapInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetGarrisonTalentTreeCurrencyTypes

```lua
C_Garrison.GetGarrisonTalentTreeCurrencyTypes(garrTalentTreeID: number) -> garrTalentTreeCurrencyType: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetGarrisonTalentTreeType

```lua
C_Garrison.GetGarrisonTalentTreeType(garrTalentTreeID: number) -> garrTalentTreeType: number
```

`SecretArguments=AllowedWhenUntainted`

### GetMaxCypherEquipmentLevel

```lua
C_Garrison.GetMaxCypherEquipmentLevel() -> maxEquipmentLevel: number
```

### GetMissionCompleteEncounters

```lua
C_Garrison.GetMissionCompleteEncounters(missionID: number) -> encounters: GarrisonEnemyEncounterInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetMissionDeploymentInfo

```lua
C_Garrison.GetMissionDeploymentInfo(missionID: number) -> missionDeploymentInfo: MissionDeploymentInfo
```

`SecretArguments=AllowedWhenUntainted`

### GetMissionEncounterIconInfo

```lua
C_Garrison.GetMissionEncounterIconInfo(missionID: number) -> missionEncounterIconInfo: MissionEncounterIconInfo
```

`SecretArguments=AllowedWhenUntainted`

### GetTalentInfo

```lua
C_Garrison.GetTalentInfo(talentID: number) -> info: GarrisonTalentInfo
```

`SecretArguments=AllowedWhenUntainted`

### GetTalentPointsSpentInTalentTree

```lua
C_Garrison.GetTalentPointsSpentInTalentTree(garrTalentTreeID: number) -> talentPoints: number
```

`SecretArguments=AllowedWhenUntainted`

### GetTalentTreeIDsByClassID

```lua
C_Garrison.GetTalentTreeIDsByClassID(garrType: number, classID: number) -> treeIDs: number[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetTalentTreeInfo

```lua
C_Garrison.GetTalentTreeInfo(treeID: number) -> info: GarrisonTalentTreeInfo
```

`SecretArguments=AllowedWhenUntainted`

### GetTalentTreeResetInfo

```lua
C_Garrison.GetTalentTreeResetInfo(garrTalentTreeID: number) -> goldCost: number, currencyCosts: GarrisonTalentCurrencyCostInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetTalentTreeTalentPointResearchInfo

```lua
C_Garrison.GetTalentTreeTalentPointResearchInfo(garrTalentID: number, researchRank: number, garrTalentTreeID: number, talentPointIndex: number, isRespec: bool) -> goldCost: number, currencyCosts: GarrisonTalentCurrencyCostInfo[], durationSecs: number
```

`SecretArguments=AllowedWhenUntainted`

### GetTalentUnlockWorldQuest

```lua
C_Garrison.GetTalentUnlockWorldQuest(talentID: number) -> worldQuestID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### HasAdventures

```lua
C_Garrison.HasAdventures() -> hasAdventures: bool
```

### IsAtGarrisonMissionNPC

```lua
C_Garrison.IsAtGarrisonMissionNPC() -> atGarrisonMissionNPC: bool
```

### IsEnvironmentCountered

```lua
C_Garrison.IsEnvironmentCountered(missionID: number) -> environmentCountered: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsFollowerOnCompletedMission

```lua
C_Garrison.IsFollowerOnCompletedMission(followerID: GarrisonFollower) -> followerOnCompletedMission: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsLandingPageMinimapButtonVisible

```lua
C_Garrison.IsLandingPageMinimapButtonVisible(garrType: number) -> isLandingPageMinimapButtonVisible: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsTalentConditionMet

```lua
C_Garrison.IsTalentConditionMet(talentID: number) -> isMet: bool, failureString: cstring?
```

`SecretArguments=AllowedWhenUntainted`

### RegenerateCombatLog

```lua
C_Garrison.RegenerateCombatLog(missionID: number) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### RemoveFollowerFromMission

```lua
C_Garrison.RemoveFollowerFromMission(missionID: number, followerID: GarrisonFollower, boardIndex: number?)
```

`SecretArguments=AllowedWhenUntainted`

### RushHealAllFollowers

```lua
C_Garrison.RushHealAllFollowers(followerType: number)
```

`SecretArguments=AllowedWhenUntainted`

### RushHealFollower

```lua
C_Garrison.RushHealFollower(garrFollowerID: GarrisonFollower)
```

`SecretArguments=AllowedWhenUntainted`

### SetAutoCombatSpellFastForward

```lua
C_Garrison.SetAutoCombatSpellFastForward(state: bool)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### GARRISON_ARCHITECT_CLOSED

```lua
GARRISON_ARCHITECT_CLOSED()
```

`SynchronousEvent`

### GARRISON_ARCHITECT_OPENED

```lua
GARRISON_ARCHITECT_OPENED(followerTypeID: number)
```

`SynchronousEvent`

### GARRISON_BUILDING_ACTIVATABLE

```lua
GARRISON_BUILDING_ACTIVATABLE(buildingName: cstring, garrisonType: number)
```

`SynchronousEvent`

### GARRISON_BUILDING_ACTIVATED

```lua
GARRISON_BUILDING_ACTIVATED(garrisonPlotInstanceID: number, garrisonBuildingID: number)
```

`SynchronousEvent`

### GARRISON_BUILDING_ERROR

```lua
GARRISON_BUILDING_ERROR()
```

`SynchronousEvent`

### GARRISON_BUILDING_LIST_UPDATE

```lua
GARRISON_BUILDING_LIST_UPDATE(categoryID: number)
```

`SynchronousEvent`

### GARRISON_BUILDING_PLACED

```lua
GARRISON_BUILDING_PLACED(garrisonPlotInstanceID: number, newPlacement: bool)
```

`SynchronousEvent`

### GARRISON_BUILDING_REMOVED

```lua
GARRISON_BUILDING_REMOVED(garrPlotInstanceID: number, garrBuildingID: number)
```

`SynchronousEvent`

### GARRISON_BUILDING_UPDATE

```lua
GARRISON_BUILDING_UPDATE(garrisonBuildingID: number, garrPlotInstanceID: number?)
```

`SynchronousEvent`

### GARRISON_FOLLOWER_ADDED

```lua
GARRISON_FOLLOWER_ADDED(followerDbID: GarrisonFollower, followerName: cstring, followerClassName: cstring, followerLevel: number, followerQuality: number, isUpgraded: bool, textureKit: textureKit, followerTypeID: number)
```

`SynchronousEvent`

### GARRISON_FOLLOWER_CATEGORIES_UPDATED

```lua
GARRISON_FOLLOWER_CATEGORIES_UPDATED()
```

`SynchronousEvent`

### GARRISON_FOLLOWER_DURABILITY_CHANGED

```lua
GARRISON_FOLLOWER_DURABILITY_CHANGED(garrFollowerTypeID: number, followerDbID: GarrisonFollower, followerDurability: number)
```

`SynchronousEvent`

### GARRISON_FOLLOWER_HEALED

```lua
GARRISON_FOLLOWER_HEALED(followerID: GarrisonFollower)
```

`SynchronousEvent`

### GARRISON_FOLLOWER_LIST_UPDATE

```lua
GARRISON_FOLLOWER_LIST_UPDATE(followerTypeID: number)
```

`SynchronousEvent`

### GARRISON_FOLLOWER_REMOVED

```lua
GARRISON_FOLLOWER_REMOVED(followerTypeID: number)
```

`SynchronousEvent`

### GARRISON_FOLLOWER_UPGRADED

```lua
GARRISON_FOLLOWER_UPGRADED(followerDbID: GarrisonFollower)
```

`SynchronousEvent`

### GARRISON_FOLLOWER_XP_CHANGED

```lua
GARRISON_FOLLOWER_XP_CHANGED(garrFollowerTypeID: number, followerDbID: GarrisonFollower, xpChange: number, oldFollowerXp: number, oldFollowerLevel: number, oldFollowerQuality: number)
```

`SynchronousEvent`

### GARRISON_HIDE_LANDING_PAGE

```lua
GARRISON_HIDE_LANDING_PAGE()
```

`SynchronousEvent`

### GARRISON_INVASION_AVAILABLE

```lua
GARRISON_INVASION_AVAILABLE()
```

`SynchronousEvent`

### GARRISON_INVASION_UNAVAILABLE

```lua
GARRISON_INVASION_UNAVAILABLE()
```

`SynchronousEvent`

### GARRISON_LANDINGPAGE_SHIPMENTS

```lua
GARRISON_LANDINGPAGE_SHIPMENTS()
```

`SynchronousEvent` `UniqueEvent`

### GARRISON_MISSION_AREA_BONUS_ADDED

```lua
GARRISON_MISSION_AREA_BONUS_ADDED(garrisonMissonBonusAbilityID: number)
```

`SynchronousEvent`

### GARRISON_MISSION_BONUS_ROLL_COMPLETE

```lua
GARRISON_MISSION_BONUS_ROLL_COMPLETE(missionID: number, success: bool)
```

`SynchronousEvent`

### GARRISON_MISSION_COMPLETE_RESPONSE

```lua
GARRISON_MISSION_COMPLETE_RESPONSE(missionID: number, canComplete: bool, success: bool, bonusRollSuccess: bool, followerDeaths: GarrisonFollowerDeathInfo[], autoCombatResult: AutoCombatResult?)
```

`SynchronousEvent`

### GARRISON_MISSION_FINISHED

```lua
GARRISON_MISSION_FINISHED(followerTypeID: number, missionID: number)
```

`SynchronousEvent`

### GARRISON_MISSION_LIST_UPDATE

```lua
GARRISON_MISSION_LIST_UPDATE(garrFollowerTypeID: number)
```

`SynchronousEvent`

### GARRISON_MISSION_NPC_CLOSED

```lua
GARRISON_MISSION_NPC_CLOSED()
```

`SynchronousEvent`

### GARRISON_MISSION_NPC_OPENED

```lua
GARRISON_MISSION_NPC_OPENED(followerTypeID: number)
```

`SynchronousEvent`

### GARRISON_MISSION_REWARD_INFO

```lua
GARRISON_MISSION_REWARD_INFO(missionID: number, followerDbID: GarrisonFollower)
```

`SynchronousEvent`

### GARRISON_MISSION_STARTED

```lua
GARRISON_MISSION_STARTED(garrFollowerTypeID: number, missionID: number)
```

`SynchronousEvent`

### GARRISON_MONUMENT_CLOSE_UI

```lua
GARRISON_MONUMENT_CLOSE_UI()
```

`SynchronousEvent`

### GARRISON_MONUMENT_LIST_LOADED

```lua
GARRISON_MONUMENT_LIST_LOADED(success: bool)
```

`SynchronousEvent`

### GARRISON_MONUMENT_REPLACED

```lua
GARRISON_MONUMENT_REPLACED(success: bool)
```

`SynchronousEvent`

### GARRISON_MONUMENT_SELECTED_TROPHY_ID_LOADED

```lua
GARRISON_MONUMENT_SELECTED_TROPHY_ID_LOADED(success: bool)
```

`SynchronousEvent`

### GARRISON_MONUMENT_SHOW_UI

```lua
GARRISON_MONUMENT_SHOW_UI()
```

`SynchronousEvent`

### GARRISON_RANDOM_MISSION_ADDED

```lua
GARRISON_RANDOM_MISSION_ADDED(followerTypeID: number, missionID: number)
```

`SynchronousEvent`

### GARRISON_RECALL_PORTAL_LAST_USED_TIME

```lua
GARRISON_RECALL_PORTAL_LAST_USED_TIME(success: bool, recallPortalLastUsedTime: number)
```

`SynchronousEvent`

### GARRISON_RECALL_PORTAL_USED

```lua
GARRISON_RECALL_PORTAL_USED(success: bool)
```

`SynchronousEvent`

### GARRISON_RECRUIT_FOLLOWER_RESULT

```lua
GARRISON_RECRUIT_FOLLOWER_RESULT()
```

`SynchronousEvent`

### GARRISON_RECRUITMENT_FOLLOWERS_GENERATED

```lua
GARRISON_RECRUITMENT_FOLLOWERS_GENERATED()
```

`SynchronousEvent`

### GARRISON_RECRUITMENT_NPC_CLOSED

```lua
GARRISON_RECRUITMENT_NPC_CLOSED()
```

`SynchronousEvent`

### GARRISON_RECRUITMENT_NPC_OPENED

```lua
GARRISON_RECRUITMENT_NPC_OPENED(followerTypeID: number)
```

`SynchronousEvent`

### GARRISON_RECRUITMENT_READY

```lua
GARRISON_RECRUITMENT_READY()
```

`SynchronousEvent`

### GARRISON_SHIPMENT_RECEIVED

```lua
GARRISON_SHIPMENT_RECEIVED()
```

`UniqueEvent`

### GARRISON_SHIPYARD_NPC_CLOSED

```lua
GARRISON_SHIPYARD_NPC_CLOSED()
```

`SynchronousEvent`

### GARRISON_SHIPYARD_NPC_OPENED

```lua
GARRISON_SHIPYARD_NPC_OPENED(followerTypeID: number)
```

`SynchronousEvent`

### GARRISON_SHOW_LANDING_PAGE

```lua
GARRISON_SHOW_LANDING_PAGE()
```

`SynchronousEvent`

### GARRISON_SPEC_GROUPS_CLEARED

```lua
GARRISON_SPEC_GROUPS_CLEARED(garrTypeID: number)
```

`SynchronousEvent`

### GARRISON_SPEC_GROUP_UPDATED

```lua
GARRISON_SPEC_GROUP_UPDATED(garrTypeID: number, specID: number)
```

`SynchronousEvent`

### GARRISON_TALENT_COMPLETE

```lua
GARRISON_TALENT_COMPLETE(garrTypeID: number, doAlert: bool)
```

`SynchronousEvent`

### GARRISON_TALENT_EVENT_UPDATE

```lua
GARRISON_TALENT_EVENT_UPDATE(eventType: number, eventID: number)
```

`SynchronousEvent`

### GARRISON_TALENT_NPC_CLOSED

```lua
GARRISON_TALENT_NPC_CLOSED()
```

`SynchronousEvent`

### GARRISON_TALENT_NPC_OPENED

```lua
GARRISON_TALENT_NPC_OPENED(garrisonTypeID: number, garrisonTalentTreeID: number)
```

`SynchronousEvent`

### GARRISON_TALENT_RESEARCH_STARTED

```lua
GARRISON_TALENT_RESEARCH_STARTED(garrTypeID: number, garrisonTalentTreeID: number, garrTalentID: number)
```

`SynchronousEvent`

### GARRISON_TALENT_UNLOCKS_RESULT

```lua
GARRISON_TALENT_UNLOCKS_RESULT()
```

`SynchronousEvent`

### GARRISON_TALENT_UPDATE

```lua
GARRISON_TALENT_UPDATE(garrTypeID: number)
```

`SynchronousEvent`

### GARRISON_TRADESKILL_NPC_CLOSED

```lua
GARRISON_TRADESKILL_NPC_CLOSED()
```

`SynchronousEvent`

### GARRISON_UPDATE

```lua
GARRISON_UPDATE()
```

`SynchronousEvent`

### GARRISON_UPGRADEABLE_RESULT

```lua
GARRISON_UPGRADEABLE_RESULT(garrisonUpgradeable: bool)
```

`SynchronousEvent`

### GARRISON_USE_PARTY_GARRISON_CHANGED

```lua
GARRISON_USE_PARTY_GARRISON_CHANGED()
```

`SynchronousEvent`

### SHIPMENT_CRAFTER_CLOSED

```lua
SHIPMENT_CRAFTER_CLOSED()
```

`SynchronousEvent`

### SHIPMENT_CRAFTER_INFO

```lua
SHIPMENT_CRAFTER_INFO(success: number, shipmentCount: number, maxShipments: number, ownedShipments: number, plotInstanceID: number)
```

`SynchronousEvent`

### SHIPMENT_CRAFTER_OPENED

```lua
SHIPMENT_CRAFTER_OPENED(charShipmentContainerID: number)
```

`SynchronousEvent`

### SHIPMENT_CRAFTER_REAGENT_UPDATE

```lua
SHIPMENT_CRAFTER_REAGENT_UPDATE()
```

`SynchronousEvent`

### SHIPMENT_UPDATE

```lua
SHIPMENT_UPDATE(shipmentStarted: bool?, hasAttachedFollower: bool?)
```

`SynchronousEvent`

## Types

### AutoCombatDamageClassString

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `damageClassValue` | `number` |  |
| `locString` | `cstring` |  |

### AutoCombatResult

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `winner` | `bool` |  |
| `combatLog` | `AutoMissionRound[]` |  |

### AutoCombatSpellInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `autoCombatSpellID` | `number` |  |
| `name` | `cstring` |  |
| `description` | `string` |  |
| `cooldown` | `number` |  |
| `duration` | `number` |  |
| `schoolMask` | `number` |  |
| `previewMask` | `number` |  |
| `icon` | `fileID` |  |
| `spellTutorialFlag` | `number` |  |
| `hasThornsEffect` | `bool` |  |

### AutoCombatTroopInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `followerID` | `GarrisonFollower` |  |
| `garrFollowerID` | `GarrisonFollower` |  |
| `followerTypeID` | `number` |  |
| `displayIDs` | `FollowerDisplayID[]` |  |
| `level` | `number` |  |
| `quality` | `number` |  |
| `levelXP` | `number` |  |
| `maxXP` | `number` |  |
| `height` | `number` |  |
| `scale` | `number` |  |
| `displayScale` | `number?` |  |
| `displayHeight` | `number?` |  |
| `classSpec` | `number?` |  |
| `className` | `string?` |  |
| `flavorText` | `string?` |  |
| `classAtlas` | `textureAtlas` |  |
| `portraitIconID` | `fileID` |  |
| `textureKit` | `textureKit` |  |
| `isTroop` | `bool` |  |
| `raceID` | `number` |  |
| `health` | `number` |  |
| `maxHealth` | `number` |  |
| `role` | `number` |  |
| `isAutoTroop` | `bool` |  |
| `isSoulbind` | `bool` |  |
| `isCollected` | `bool` |  |
| `autoCombatStats` | `FollowerAutoCombatStatsInfo` |  |

### AutoMissionCombatEventInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `boardIndex` | `number` |  |
| `oldHealth` | `number` |  |
| `newHealth` | `number` |  |
| `maxHealth` | `number` |  |
| `points` | `number?` |  |

### AutoMissionEnvironmentEffect

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `autoCombatSpellInfo` | `AutoCombatSpellInfo` |  |

### AutoMissionEvent

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `type` | `number` |  |
| `spellID` | `number` |  |
| `schoolMask` | `number` |  |
| `effectIndex` | `number` |  |
| `casterBoardIndex` | `number` |  |
| `auraType` | `number` |  |
| `targetInfo` | `AutoMissionCombatEventInfo[]` |  |

### AutoMissionRound

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `events` | `AutoMissionEvent[]` |  |

### AutoMissionTargetingInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `targetIndex` | `number` |  |
| `previewType` | `number` |  |
| `spellID` | `number` |  |
| `effectIndex` | `number` |  |

### FollowerAutoCombatStatsInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `currentHealth` | `number` |  |
| `maxHealth` | `number` |  |
| `attack` | `number` |  |
| `healingTimestamp` | `time_t` |  |
| `healCost` | `number` |  |
| `minutesHealingRemaining` | `number` |  |

### FollowerDisplayID

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `id` | `number` |  |
| `followerPageScale` | `number` |  |
| `showWeapon` | `bool` |  |

### FollowerMissionCompleteInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `displayIDs` | `FollowerDisplayID[]` |  |
| `level` | `number` |  |
| `quality` | `number` |  |
| `currentXP` | `number` |  |
| `maxXP` | `number` |  |
| `height` | `number` |  |
| `scale` | `number` |  |
| `movementType` | `number?` |  |
| `impactDelay` | `number?` |  |
| `castID` | `number?` |  |
| `castSoundID` | `number?` |  |
| `impactID` | `number?` |  |
| `impactSoundID` | `number?` |  |
| `targetImpactID` | `number?` |  |
| `targetImpactSoundID` | `number?` |  |
| `className` | `string?` |  |
| `classAtlas` | `textureAtlas` |  |
| `portraitIconID` | `fileID` |  |
| `textureKit` | `textureKit` |  |
| `isTroop` | `bool` |  |
| `boardIndex` | `number` |  |
| `health` | `number` |  |
| `maxHealth` | `number` |  |
| `role` | `number` |  |

### GarrisonAbilityCounterInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `id` | `number` |  |
| `icon` | `fileID` |  |
| `name` | `cstring` |  |
| `factor` | `number` |  |
| `description` | `cstring` |  |

### GarrisonAbilityInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `id` | `number` |  |
| `name` | `cstring` |  |
| `description` | `string` |  |
| `icon` | `fileID` |  |
| `isTrait` | `bool` |  |
| `isSpecialization` | `bool` |  |
| `temporary` | `bool` |  |
| `category` | `string?` |  |
| `counters` | `GarrisonAbilityCounterInfo[]` |  |
| `isEmptySlot` | `bool` |  |

### GarrisonEnemyEncounterInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `displayID` | `fileID` |  |
| `portraitFileDataID` | `fileID` |  |
| `textureKit` | `textureKit` |  |
| `scale` | `number` |  |
| `height` | `number` |  |
| `mechanics` | `GarrisonMechanicInfo[]` |  |
| `autoCombatSpells` | `AutoCombatSpellInfo[]` |  |
| `autoCombatAutoAttack` | `AutoCombatSpellInfo?` |  |
| `role` | `number` |  |
| `health` | `number` |  |
| `maxHealth` | `number` |  |
| `attack` | `number` |  |
| `boardIndex` | `number` |  |
| `isElite` | `bool` |  |

### GarrisonFollowerDeathInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `followerID` | `GarrisonFollower` |  |
| `state` | `luaIndex` |  |

### GarrisonMechanicInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `mechanicTypeID` | `number` |  |
| `icon` | `fileID` |  |
| `name` | `cstring` |  |
| `factor` | `number` |  |
| `description` | `cstring` |  |
| `ability` | `GarrisonAbilityInfo?` |  |

### GarrisonPlotInstanceMapInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `buildingPlotInstanceID` | `number` |  |
| `position` | `vector2` | `Mixin=Vector2DMixin` |
| `name` | `cstring` |  |
| `atlasName` | `textureAtlas` |  |

### MissionDeploymentInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `location` | `cstring` |  |
| `xp` | `number` |  |
| `environment` | `string?` |  |
| `environmentDesc` | `string?` |  |
| `environmentTexture` | `fileID` |  |
| `locTextureKit` | `textureKit` |  |
| `isExhausting` | `bool` |  |
| `enemies` | `GarrisonEnemyEncounterInfo[]` |  |

### MissionEncounterIconInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `portraitFileDataID` | `fileID` |  |
| `missionScalar` | `number` |  |
| `isElite` | `bool` |  |
| `isRare` | `bool` |  |
