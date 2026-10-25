# QuestLog

Namespace `C_QuestLog` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/questlogdocumentation.lua` (FileDataID 4637174)

## Functions

### AbandonQuest

```lua
C_QuestLog.AbandonQuest()
```

### AddQuestWatch

```lua
C_QuestLog.AddQuestWatch(questID: number) -> wasWatched: bool
```

`SecretArguments=AllowedWhenUntainted`

### AddWorldQuestWatch

```lua
C_QuestLog.AddWorldQuestWatch(questID: number, watchType: QuestWatchType?) -> wasWatched: bool
```

`SecretArguments=AllowedWhenUntainted`

### CanAbandonQuest

```lua
C_QuestLog.CanAbandonQuest(questID: number) -> canAbandon: bool
```

`SecretArguments=AllowedWhenUntainted`

### DoesQuestAwardReputationWithFaction

```lua
C_QuestLog.DoesQuestAwardReputationWithFaction(questID: number, targetFactionID: number) -> awardsReputation: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetAbandonQuest

```lua
C_QuestLog.GetAbandonQuest() -> questID: number
```

### GetAbandonQuestItems

```lua
C_QuestLog.GetAbandonQuestItems() -> itemIDs: number[]
```

`MayReturnNothing`

### GetActivePreyQuest

```lua
C_QuestLog.GetActivePreyQuest() -> questID: number
```

`MayReturnNothing`

### GetActiveThreatMaps

```lua
C_QuestLog.GetActiveThreatMaps() -> uiMapIDs: number[]
```

`MayReturnNothing`

### GetAllCompletedQuestIDs

```lua
C_QuestLog.GetAllCompletedQuestIDs() -> quests: number[]
```

### GetBountiesForMapID

```lua
C_QuestLog.GetBountiesForMapID(uiMapID: number) -> bounties: BountyInfo[]?
```

`SecretArguments=AllowedWhenUntainted`

### GetBountySetInfoForMapID

```lua
C_QuestLog.GetBountySetInfoForMapID(uiMapID: number) -> displayLocation: MapOverlayDisplayLocation, lockQuestID: number, bountySetID: number, isActivitySet: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetDistanceSqToQuest

```lua
C_QuestLog.GetDistanceSqToQuest(questID: number) -> distanceSq: number, onContinent: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetHeaderIndexForQuest

```lua
C_QuestLog.GetHeaderIndexForQuest(questID: number) -> index: luaIndex?
```

`SecretArguments=AllowedWhenUntainted`

### GetInfo

```lua
C_QuestLog.GetInfo(questLogIndex: luaIndex) -> info: QuestInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetLogIndexForQuestID

```lua
C_QuestLog.GetLogIndexForQuestID(questID: number) -> questLogIndex: luaIndex?
```

Only returns a log index for actual quests, not headers

`SecretArguments=AllowedWhenUntainted`

### GetMapForQuestPOIs

```lua
C_QuestLog.GetMapForQuestPOIs() -> uiMapID: number
```

### GetMaxNumQuests

```lua
C_QuestLog.GetMaxNumQuests() -> maxNumQuests: number
```

This is the maximum number of quests a player can be on, including hidden quests, world quests, emissaries etc

### GetMaxNumQuestsCanAccept

```lua
C_QuestLog.GetMaxNumQuestsCanAccept() -> maxNumQuestsCanAccept: number
```

This is the maximum number of standard quests a player can accept. These are quests that are normally visible in the quest log.

### GetNextWaypoint

```lua
C_QuestLog.GetNextWaypoint(questID: number) -> mapID: number, x: number, y: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetNextWaypointForMap

```lua
C_QuestLog.GetNextWaypointForMap(questID: number, uiMapID: number) -> x: number, y: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetNextWaypointText

```lua
C_QuestLog.GetNextWaypointText(questID: number) -> waypointText: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetNumQuestLogEntries

```lua
C_QuestLog.GetNumQuestLogEntries() -> numShownEntries: number, numQuests: number
```

### GetNumQuestObjectives

```lua
C_QuestLog.GetNumQuestObjectives(questID: number) -> leaderboardCount: number
```

`SecretArguments=AllowedWhenUntainted`

### GetNumQuestWatches

```lua
C_QuestLog.GetNumQuestWatches() -> numQuestWatches: number
```

### GetNumWorldQuestWatches

```lua
C_QuestLog.GetNumWorldQuestWatches() -> numQuestWatches: number
```

### GetQuestAdditionalHighlights

```lua
C_QuestLog.GetQuestAdditionalHighlights(questID: number) -> uiMapID: number, worldQuests: bool, worldQuestsElite: bool, dungeons: bool, treasures: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetQuestDetailsTheme

```lua
C_QuestLog.GetQuestDetailsTheme(questID: number) -> theme: QuestTheme?
```

`SecretArguments=AllowedWhenUntainted`

### GetQuestDifficultyLevel

```lua
C_QuestLog.GetQuestDifficultyLevel(questID: number) -> level: number
```

`SecretArguments=AllowedWhenUntainted`

### GetQuestIDForLogIndex

```lua
C_QuestLog.GetQuestIDForLogIndex(questLogIndex: luaIndex) -> questID: number?
```

Only returns a questID for actual quests, not headers

`SecretArguments=AllowedWhenUntainted`

### GetQuestIDForQuestWatchIndex

```lua
C_QuestLog.GetQuestIDForQuestWatchIndex(questWatchIndex: luaIndex) -> questID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetQuestIDForWorldQuestWatchIndex

```lua
C_QuestLog.GetQuestIDForWorldQuestWatchIndex(questWatchIndex: luaIndex) -> questID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetQuestLogMajorFactionReputationRewards

```lua
C_QuestLog.GetQuestLogMajorFactionReputationRewards(questID: number) -> reputationRewards: QuestRewardReputationInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetQuestLogPortraitGiver

```lua
C_QuestLog.GetQuestLogPortraitGiver(questLogIndex: luaIndex?) -> portraitGiver: number, portraitGiverText: cstring, portraitGiverName: cstring, portraitGiverMount: number, portraitGiverModelSceneID: number?
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetQuestObjectives

```lua
C_QuestLog.GetQuestObjectives(questID: number) -> objectives: QuestObjectiveInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetQuestRewardCurrencies

```lua
C_QuestLog.GetQuestRewardCurrencies(questID: number) -> questRewardCurrencies: QuestRewardCurrencyInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetQuestRewardCurrencyInfo

```lua
C_QuestLog.GetQuestRewardCurrencyInfo(questID: number, currencyIndex: luaIndex, isChoice: bool) -> questRewardCurrencyInfo: QuestRewardCurrencyInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetQuestsOnMap

```lua
C_QuestLog.GetQuestsOnMap(uiMapID: number) -> quests: QuestPOIMapInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetQuestTagInfo

```lua
C_QuestLog.GetQuestTagInfo(questID: number) -> info: QuestTagInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetQuestTimers

```lua
C_QuestLog.GetQuestTimers() -> questTimers: QuestTimerInfo[]
```

### GetQuestType

```lua
C_QuestLog.GetQuestType(questID: number) -> questType: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetQuestWatchType

```lua
C_QuestLog.GetQuestWatchType(questID: number) -> watchType: QuestWatchType?
```

`SecretArguments=AllowedWhenUntainted`

### GetRequiredMoney

```lua
C_QuestLog.GetRequiredMoney(questID: number?) -> requiredMoney: number
```

Uses the selected quest if no questID is provided

`SecretArguments=AllowedWhenUntainted`

### GetSelectedQuest

```lua
C_QuestLog.GetSelectedQuest() -> questID: number
```

### GetSuggestedGroupSize

```lua
C_QuestLog.GetSuggestedGroupSize(questID: number) -> suggestedGroupSize: number
```

`SecretArguments=AllowedWhenUntainted`

### GetTimeAllowed

```lua
C_QuestLog.GetTimeAllowed(questID: number) -> totalTime: number, elapsedTime: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetTitleForLogIndex

```lua
C_QuestLog.GetTitleForLogIndex(questLogIndex: luaIndex) -> title: cstring?
```

Returns a valid title for anything that is in the quest log.

`SecretArguments=AllowedWhenUntainted`

### GetTitleForQuestID

```lua
C_QuestLog.GetTitleForQuestID(questID: number) -> title: cstring?
```

Only returns a valid title for quests, header titles cannot be discovered using this.

`SecretArguments=AllowedWhenUntainted`

### GetTrivialRange

```lua
C_QuestLog.GetTrivialRange() -> range: number
```

### GetZoneStoryInfo

```lua
C_QuestLog.GetZoneStoryInfo(uiMapID: number) -> achievementID: number, storyMapID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### HasActiveThreats

```lua
C_QuestLog.HasActiveThreats() -> hasActiveThreats: bool
```

### IsAccountQuest

```lua
C_QuestLog.IsAccountQuest(questID: number) -> isAccountQuest: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsComplete

```lua
C_QuestLog.IsComplete(questID: number) -> isComplete: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsEliteQuest

```lua
C_QuestLog.IsEliteQuest(questID: number) -> isEliteQuest: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsFailed

```lua
C_QuestLog.IsFailed(questID: number) -> isFailed: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsImportantQuest

```lua
C_QuestLog.IsImportantQuest(questID: number) -> isImportant: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsMetaQuest

```lua
C_QuestLog.IsMetaQuest(questID: number) -> isMeta: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsOnMap

```lua
C_QuestLog.IsOnMap(questID: number) -> onMap: bool, hasLocalPOI: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsOnQuest

```lua
C_QuestLog.IsOnQuest(questID: number) -> isOnQuest: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsPushableQuest

```lua
C_QuestLog.IsPushableQuest(questID: number) -> isPushable: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsQuestBounty

```lua
C_QuestLog.IsQuestBounty(questID: number) -> isBounty: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsQuestCalling

```lua
C_QuestLog.IsQuestCalling(questID: number) -> isCalling: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsQuestCriteriaForBounty

```lua
C_QuestLog.IsQuestCriteriaForBounty(questID: number, bountyQuestID: number) -> isCriteriaForBounty: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsQuestDisabledForSession

```lua
C_QuestLog.IsQuestDisabledForSession(questID: number) -> isDisabled: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsQuestFlaggedCompleted

```lua
C_QuestLog.IsQuestFlaggedCompleted(questID: number) -> isCompleted: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsQuestFlaggedCompletedOnAccount

```lua
C_QuestLog.IsQuestFlaggedCompletedOnAccount(questID: number) -> isCompletedOnAccount: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsQuestFromContentPush

```lua
C_QuestLog.IsQuestFromContentPush(questID: number) -> isFromContentPush: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsQuestInvasion

```lua
C_QuestLog.IsQuestInvasion(questID: number) -> isInvasion: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsQuestReplayable

```lua
C_QuestLog.IsQuestReplayable(questID: number) -> isReplayable: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsQuestReplayedRecently

```lua
C_QuestLog.IsQuestReplayedRecently(questID: number) -> recentlyReplayed: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsQuestTask

```lua
C_QuestLog.IsQuestTask(questID: number) -> isTask: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsQuestTrivial

```lua
C_QuestLog.IsQuestTrivial(questID: number) -> isTrivial: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsRepeatableQuest

```lua
C_QuestLog.IsRepeatableQuest(questID: number) -> isRepeatable: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsThreatQuest

```lua
C_QuestLog.IsThreatQuest(questID: number) -> isThreat: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsUnitOnQuest

```lua
C_QuestLog.IsUnitOnQuest(unit: UnitToken, questID: number) -> isOnQuest: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsWorldQuest

```lua
C_QuestLog.IsWorldQuest(questID: number) -> isWorldQuest: bool
```

`SecretArguments=AllowedWhenUntainted`

### QuestCanHaveWarModeBonus

```lua
C_QuestLog.QuestCanHaveWarModeBonus(questID: number) -> hasBonus: bool
```

Tests whether a quest is eligible for warmode bonuses (e.g. most world quests, some daily quests

`SecretArguments=AllowedWhenUntainted`

### QuestContainsFirstTimeRepBonusForPlayer

```lua
C_QuestLog.QuestContainsFirstTimeRepBonusForPlayer(questID: number) -> questContainsFirstTimeRepBonusForPlayer: bool
```

`SecretArguments=AllowedWhenUntainted`

### QuestHasQuestSessionBonus

```lua
C_QuestLog.QuestHasQuestSessionBonus(questID: number) -> hasBonus: bool
```

`SecretArguments=AllowedWhenUntainted`

### QuestHasWarModeBonus

```lua
C_QuestLog.QuestHasWarModeBonus(questID: number) -> hasBonus: bool
```

Tests whether a quest in the player's quest log that is eligible for warmode bonuses (see 'QuestCanHaveWarModeBOnus') has been completed in warmode (including accepting it)

`SecretArguments=AllowedWhenUntainted`

### QuestIgnoresAccountCompletedFiltering

```lua
C_QuestLog.QuestIgnoresAccountCompletedFiltering(questID: number) -> questIgnoresAccountCompletedFiltering: bool
```

`SecretArguments=AllowedWhenUntainted`

### ReadyForTurnIn

```lua
C_QuestLog.ReadyForTurnIn(questID: number) -> readyForTurnIn: bool?
```

`SecretArguments=AllowedWhenUntainted`

### RemoveQuestWatch

```lua
C_QuestLog.RemoveQuestWatch(questID: number) -> wasRemoved: bool
```

`SecretArguments=AllowedWhenUntainted`

### RemoveWorldQuestWatch

```lua
C_QuestLog.RemoveWorldQuestWatch(questID: number) -> wasRemoved: bool
```

`SecretArguments=AllowedWhenUntainted`

### RequestLoadQuestByID

```lua
C_QuestLog.RequestLoadQuestByID(questID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetAbandonQuest

```lua
C_QuestLog.SetAbandonQuest()
```

### SetMapForQuestPOIs

```lua
C_QuestLog.SetMapForQuestPOIs(uiMapID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetSelectedQuest

```lua
C_QuestLog.SetSelectedQuest(questID: number)
```

`SecretArguments=AllowedWhenUntainted`

### ShouldDisplayTimeRemaining

```lua
C_QuestLog.ShouldDisplayTimeRemaining(questID: number) -> displayTimeRemaining: bool
```

`SecretArguments=AllowedWhenUntainted`

### ShouldShowQuestRewards

```lua
C_QuestLog.ShouldShowQuestRewards(questID: number) -> shouldShow: bool
```

`SecretArguments=AllowedWhenUntainted`

### SortQuestWatches

```lua
C_QuestLog.SortQuestWatches()
```

### UnitIsRelatedToActiveQuest

```lua
C_QuestLog.UnitIsRelatedToActiveQuest(unit: UnitToken) -> isRelatedToActiveQuest: bool
```

`SecretArguments=AllowedWhenUntainted`

### UpdateCampaignHeaders

```lua
C_QuestLog.UpdateCampaignHeaders()
```

## Events

### QUEST_ACCEPTED

```lua
QUEST_ACCEPTED(questId: number)
```

`SynchronousEvent`

### QUEST_AUTOCOMPLETE

```lua
QUEST_AUTOCOMPLETE(questId: number)
```

`SynchronousEvent`

### QUEST_COMPLETE

```lua
QUEST_COMPLETE()
```

`SynchronousEvent`

### QUEST_DATA_LOAD_RESULT

```lua
QUEST_DATA_LOAD_RESULT(questID: number, success: bool)
```

`SynchronousEvent`

### QUEST_DETAIL

```lua
QUEST_DETAIL(questStartItemID: number?)
```

`SynchronousEvent`

### QUESTLINE_UPDATE

```lua
QUESTLINE_UPDATE(requestRequired: bool)
```

`SynchronousEvent`

### QUEST_LOG_CRITERIA_UPDATE

```lua
QUEST_LOG_CRITERIA_UPDATE(questID: number, specificTreeID: number, description: cstring, numFulfilled: number, numRequired: number)
```

`SynchronousEvent`

### QUEST_LOG_UPDATE

```lua
QUEST_LOG_UPDATE()
```

`UniqueEvent`

### QUEST_POI_UPDATE

```lua
QUEST_POI_UPDATE()
```

`UniqueEvent`

### QUEST_REMOVED

```lua
QUEST_REMOVED(questID: number, wasReplayQuest: bool)
```

`SynchronousEvent`

### QUEST_TURNED_IN

```lua
QUEST_TURNED_IN(questID: number, xpReward: number, moneyReward: number)
```

`SynchronousEvent`

### QUEST_WATCH_LIST_CHANGED

```lua
QUEST_WATCH_LIST_CHANGED(questID: number?, added: bool?)
```

`SynchronousEvent` `UniqueEvent`

### QUEST_WATCH_UPDATE

```lua
QUEST_WATCH_UPDATE(questID: number)
```

`SynchronousEvent`

### TASK_PROGRESS_UPDATE

```lua
TASK_PROGRESS_UPDATE()
```

`SynchronousEvent`

### TREASURE_PICKER_CACHE_FLUSH

```lua
TREASURE_PICKER_CACHE_FLUSH()
```

`SynchronousEvent`

### WAYPOINT_UPDATE

```lua
WAYPOINT_UPDATE()
```

`SynchronousEvent`

### WORLD_QUEST_COMPLETED_BY_SPELL

```lua
WORLD_QUEST_COMPLETED_BY_SPELL(questID: number)
```

`SynchronousEvent`

## Types

### MapOverlayDisplayLocation

*Enumeration* · 6 values, 0..5

Access values as `Enum.MapOverlayDisplayLocation.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Default` | `MapOverlayDisplayLocation` | = 0 |
| `BottomLeft` | `MapOverlayDisplayLocation` | = 1 |
| `TopLeft` | `MapOverlayDisplayLocation` | = 2 |
| `BottomRight` | `MapOverlayDisplayLocation` | = 3 |
| `TopRight` | `MapOverlayDisplayLocation` | = 4 |
| `Hidden` | `MapOverlayDisplayLocation` | = 5 |

### QuestFrequency

*Enumeration* · 4 values, 0..3

Access values as `Enum.QuestFrequency.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Default` | `QuestFrequency` | = 0 |
| `Daily` | `QuestFrequency` | = 1 |
| `Weekly` | `QuestFrequency` | = 2 |
| `ResetByScheduler` | `QuestFrequency` | = 3 |

### QuestTag

*Enumeration* · 12 values, 1..288

Access values as `Enum.QuestTag.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Group` | `QuestTag` | = 1 |
| `PvP` | `QuestTag` | = 41 |
| `Raid` | `QuestTag` | = 62 |
| `Dungeon` | `QuestTag` | = 81 |
| `Legendary` | `QuestTag` | = 83 |
| `Heroic` | `QuestTag` | = 85 |
| `Raid10` | `QuestTag` | = 88 |
| `Raid25` | `QuestTag` | = 89 |
| `Scenario` | `QuestTag` | = 98 |
| `Account` | `QuestTag` | = 102 |
| `CombatAlly` | `QuestTag` | = 266 |
| `Delve` | `QuestTag` | = 288 |

### QuestWatchType

*Enumeration* · 2 values, 0..1

Access values as `Enum.QuestWatchType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Automatic` | `QuestWatchType` | = 0 |
| `Manual` | `QuestWatchType` | = 1 |

### WorldQuestQuality

*Enumeration* · 3 values, 0..2

Access values as `Enum.WorldQuestQuality.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Common` | `WorldQuestQuality` | = 0 |
| `Rare` | `WorldQuestQuality` | = 1 |
| `Epic` | `WorldQuestQuality` | = 2 |

### QuestInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `title` | `string` |  |
| `questLogIndex` | `luaIndex` |  |
| `questID` | `number` |  |
| `campaignID` | `number?` |  |
| `level` | `number` |  |
| `difficultyLevel` | `number` |  |
| `suggestedGroup` | `number` |  |
| `frequency` | `QuestFrequency?` |  |
| `isHeader` | `bool` |  |
| `useMinimalHeader` | `bool` |  |
| `sortAsNormalQuest` | `bool` |  |
| `isCollapsed` | `bool` |  |
| `startEvent` | `bool` |  |
| `isTask` | `bool` |  |
| `isBounty` | `bool` |  |
| `isStory` | `bool` |  |
| `isScaling` | `bool` |  |
| `isOnMap` | `bool` |  |
| `hasLocalPOI` | `bool` |  |
| `isHidden` | `bool` |  |
| `isAutoComplete` | `bool` |  |
| `overridesSortOrder` | `bool` |  |
| `readyForTranslation` | `bool` | default `true` |
| `isInternalOnly` | `bool` |  |
| `isAbandonOnDisable` | `bool` |  |
| `headerSortKey` | `number?` |  |
| `questClassification` | `QuestClassification` |  |

### QuestObjectiveInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `text` | `string` |  |
| `type` | `string` |  |
| `finished` | `bool` |  |
| `numFulfilled` | `number` |  |
| `numRequired` | `number` |  |
| `objectiveType` | `QuestObjectiveType?` |  |

### QuestTagInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `tagName` | `cstring` |  |
| `tagID` | `number` |  |
| `worldQuestType` | `number?` |  |
| `quality` | `WorldQuestQuality?` |  |
| `tradeskillLineID` | `number?` |  |
| `isElite` | `bool?` |  |
| `displayExpiration` | `bool?` |  |

### QuestTheme

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `background` | `textureAtlas` |  |
| `seal` | `textureAtlas` |  |
| `signature` | `cstring` |  |
| `poiIcon` | `textureAtlas` |  |
| `mapPinInfo` | `UIMapPinInfo?` |  |

### QuestTimerInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `questID` | `number` |  |
| `questTimer` | `number` |  |
