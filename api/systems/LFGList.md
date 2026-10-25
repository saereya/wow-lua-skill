# LFGList

Namespace `C_LFGList` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/lfglistinfodocumentation.lua` (FileDataID 4637130)

## Functions

### CanActiveEntryUseAutoAccept

```lua
C_LFGList.CanActiveEntryUseAutoAccept() -> canUseAutoAccept: bool
```

### CanCreateQuestGroup

```lua
C_LFGList.CanCreateQuestGroup(questID: number) -> canCreate: bool
```

`SecretArguments=AllowedWhenUntainted`

### CanCreateScenarioGroup

```lua
C_LFGList.CanCreateScenarioGroup(scenarioID: number) -> canCreate: bool
```

`SecretArguments=AllowedWhenUntainted`

### ClearApplicationTextFields

```lua
C_LFGList.ClearApplicationTextFields()
```

### ClearCreationTextFields

```lua
C_LFGList.ClearCreationTextFields()
```

### ClearSearchTextFields

```lua
C_LFGList.ClearSearchTextFields()
```

### ConfirmCensoredActiveEntry

```lua
C_LFGList.ConfirmCensoredActiveEntry()
```

### CopyActiveEntryInfoToCreationFields

```lua
C_LFGList.CopyActiveEntryInfoToCreationFields()
```

### CreateListing

```lua
C_LFGList.CreateListing(createData: LfgListingCreateData) -> success: bool
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### CreateScenarioListing

```lua
C_LFGList.CreateScenarioListing(activityID: number, itemLevel: number, autoAccept: bool, privateGroup: bool, scenarioID: number) -> canCreate: bool
```

`SecretArguments=AllowedWhenUntainted`

### DoesCensoredTextMatch

```lua
C_LFGList.DoesCensoredTextMatch(name: cstring, comment: cstring) -> isMatch: bool
```

`SecretArguments=AllowedWhenUntainted`

### DoesEntryTitleMatchPrebuiltTitle

```lua
C_LFGList.DoesEntryTitleMatchPrebuiltTitle(activityID: number, groupID: number, playstyle: LFGEntryPlaystyle?, generalPlaystyle: LFGEntryGeneralPlaystyle?) -> matches: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetActiveEntryInfo

```lua
C_LFGList.GetActiveEntryInfo() -> entryData: LfgEntryData
```

`MayReturnNothing` `SecretInChatMessagingLockdown`

### GetActivityFullName

```lua
C_LFGList.GetActivityFullName(activityID: number, questID: number?, showWarmode: bool?) -> fullName: string
```

`SecretArguments=AllowedWhenUntainted`

### GetActivityGroupInfo

```lua
C_LFGList.GetActivityGroupInfo(groupID: number) -> name: string, orderIndex: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetActivityInfoTable

```lua
C_LFGList.GetActivityInfoTable(activityID: number, questID: number?, showWarmode: bool?) -> activityInfo: GroupFinderActivityInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetAdvancedFilter

```lua
C_LFGList.GetAdvancedFilter() -> options: AdvancedFilterOptions
```

### GetApplicantBestDungeonScore

```lua
C_LFGList.GetApplicantBestDungeonScore(localID: number, applicantIndex: luaIndex) -> bestDungeonScoreForListing: BestDungeonScoreMapInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetApplicantDungeonScoreForListing

```lua
C_LFGList.GetApplicantDungeonScoreForListing(localID: number, applicantIndex: luaIndex, activityID: number) -> bestDungeonScoreForListing: BestDungeonScoreMapInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetApplicantInfo

```lua
C_LFGList.GetApplicantInfo(applicantID: number) -> applicantData: LfgApplicantData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretInChatMessagingLockdown`

### GetApplicantPvpRatingInfoForListing

```lua
C_LFGList.GetApplicantPvpRatingInfoForListing(localID: number, applicantIndex: luaIndex, activityID: number) -> pvpRatingInfo: PvpRatingInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetAvailableActivityGroups

```lua
C_LFGList.GetAvailableActivityGroups(categoryID: number, filter: number) -> activityIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `categoryID` | `number` |  |
| `filter` | `number` | default `0` |

### GetFilteredSearchResults

```lua
C_LFGList.GetFilteredSearchResults() -> totalResultsFound: number, filteredResults: number[]
```

Returns:

| Name | Type | Notes |
|---|---|---|
| `totalResultsFound` | `number` | default `0` |
| `filteredResults` | `number[]` |  |

### GetGroupLeaverCountsByRole

```lua
C_LFGList.GetGroupLeaverCountsByRole() -> tankLeavers: number, healerLeavers: number, damageLeavers: number
```

### GetKeystoneForActivity

```lua
C_LFGList.GetKeystoneForActivity(activityID: number) -> level: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetLfgCategoryInfo

```lua
C_LFGList.GetLfgCategoryInfo(categoryID: number) -> categoryData: LfgCategoryData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetOwnedKeystoneActivityAndGroupAndLevel

```lua
C_LFGList.GetOwnedKeystoneActivityAndGroupAndLevel(getTimewalking: bool) -> activityID: number, groupID: number, keystoneLevel: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `getTimewalking` | `bool` | default `false` |

### GetPlaystyleString

```lua
C_LFGList.GetPlaystyleString(playstyle: LFGEntryPlaystyle, generalPlaystyle: LFGEntryGeneralPlaystyle, activityInfo: GroupFinderActivityInfo) -> playstyleString: string
```

`SecretArguments=AllowedWhenUntainted`

### GetPremadeGroupFinderStyle

```lua
C_LFGList.GetPremadeGroupFinderStyle() -> style: PremadeGroupFinderStyle
```

### GetSearchResultInfo

```lua
C_LFGList.GetSearchResultInfo(searchResultID: number) -> searchResultData: LfgSearchResultData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretInChatMessagingLockdown`

### GetSearchResultLeaderInfo

```lua
C_LFGList.GetSearchResultLeaderInfo(searchResultID: number) -> leaderInfo: LfgSearchResultPlayerInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretInChatMessagingLockdown`

### GetSearchResultPlayerInfo

```lua
C_LFGList.GetSearchResultPlayerInfo(searchResultID: number, memberIndex: luaIndex) -> playerInfo: LfgSearchResultPlayerInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretInChatMessagingLockdown`

### GetSearchResults

```lua
C_LFGList.GetSearchResults() -> totalResultsFound: number, results: number[]
```

Returns:

| Name | Type | Notes |
|---|---|---|
| `totalResultsFound` | `number` | default `0` |
| `results` | `number[]` |  |

### HasActiveEntryInfo

```lua
C_LFGList.HasActiveEntryInfo() -> hasActiveEntryInfo: bool
```

### HasSearchResultInfo

```lua
C_LFGList.HasSearchResultInfo(searchResultID: number) -> hasSearchResultInfo: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsCensoredActiveEntryUnresolved

```lua
C_LFGList.IsCensoredActiveEntryUnresolved() -> isUnresolved: bool
```

### IsPlayerAuthenticatedForLFG

```lua
C_LFGList.IsPlayerAuthenticatedForLFG(activityCategoryID: number?) -> isAuthenticated: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsPlayerValidForEndgameFieldEdits

```lua
C_LFGList.IsPlayerValidForEndgameFieldEdits() -> isValid: bool
```

### IsPremadeGroupFinderEnabled

```lua
C_LFGList.IsPremadeGroupFinderEnabled() -> enabled: bool
```

### ListingUsesEndgameEditRestrictions

```lua
C_LFGList.ListingUsesEndgameEditRestrictions(activityID: number) -> isEndgameListing: bool
```

`SecretArguments=AllowedWhenUntainted`

### ReportGroupAsAdvertisement

```lua
C_LFGList.ReportGroupAsAdvertisement(searchResultID: number)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### RevealCensoredActiveEntry

```lua
C_LFGList.RevealCensoredActiveEntry()
```

### RevealCensoredSearchResult

```lua
C_LFGList.RevealCensoredSearchResult(searchResultID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SaveAdvancedFilter

```lua
C_LFGList.SaveAdvancedFilter(options: AdvancedFilterOptions)
```

`SecretArguments=AllowedWhenUntainted`

### Search

```lua
C_LFGList.Search(categoryID: number, filter: number, preferredFilters: number, languageFilter: WowLocale?, searchCrossFactionListings: bool?, advancedFilter: AdvancedFilterOptions?, activityIDsFilter: number[]?)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `categoryID` | `number` |  |
| `filter` | `number` | default `0` |
| `preferredFilters` | `number` | default `0` |
| `languageFilter` | `WowLocale?` |  |
| `searchCrossFactionListings` | `bool?` | default `false` |
| `advancedFilter` | `AdvancedFilterOptions?` |  |
| `activityIDsFilter` | `number[]?` | Activity IDs to filter by. |

### SetEntryTitle

```lua
C_LFGList.SetEntryTitle(activityID: number, groupID: number, playstyle: LFGEntryPlaystyle?, generalPlaystyle: LFGEntryGeneralPlaystyle?)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetSearchToActivity

```lua
C_LFGList.SetSearchToActivity(activityID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetSearchToQuestID

```lua
C_LFGList.SetSearchToQuestID(questID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetSearchToScenarioID

```lua
C_LFGList.SetSearchToScenarioID(scenarioID: number)
```

`SecretArguments=AllowedWhenUntainted`

### UpdateListing

```lua
C_LFGList.UpdateListing(createData: LfgListingCreateData) -> success: bool
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### ValidateRequiredDungeonScore

```lua
C_LFGList.ValidateRequiredDungeonScore(dungeonScore: number) -> passes: bool
```

`SecretArguments=AllowedWhenUntainted`

### ValidateRequiredPvpRatingForActivity

```lua
C_LFGList.ValidateRequiredPvpRatingForActivity(activityID: number, rating: number) -> passes: bool
```

`SecretArguments=AllowedWhenUntainted`

## Events

### LFG_GROUP_DELISTED_LEADERSHIP_CHANGE

```lua
LFG_GROUP_DELISTED_LEADERSHIP_CHANGE(listingName: string, automaticDelistTimeRemaining: number)
```

`SynchronousEvent`

### LFG_LIST_ACTIVE_ENTRY_UPDATE

```lua
LFG_LIST_ACTIVE_ENTRY_UPDATE(created: bool?)
```

`SynchronousEvent`

### LFG_LIST_APPLICANT_LIST_UPDATED

```lua
LFG_LIST_APPLICANT_LIST_UPDATED(newPendingEntry: bool?, newPendingEntryWithData: bool?)
```

`SynchronousEvent`

### LFG_LIST_APPLICANT_UPDATED

```lua
LFG_LIST_APPLICANT_UPDATED(applicantID: number)
```

`SynchronousEvent`

### LFG_LIST_APPLICATION_STATUS_UPDATED

```lua
LFG_LIST_APPLICATION_STATUS_UPDATED(searchResultID: number, newStatus: cstring, oldStatus: cstring, groupName: kstringLfgListChat)
```

`SynchronousEvent`

### LFG_LIST_AVAILABILITY_UPDATE

```lua
LFG_LIST_AVAILABILITY_UPDATE()
```

`SynchronousEvent`

### LFG_LIST_CENSORED_ACTIVE_ENTRY_UPDATE

```lua
LFG_LIST_CENSORED_ACTIVE_ENTRY_UPDATE(isCensored: bool)
```

`SynchronousEvent`

### LFG_LIST_ENTRY_CREATION_FAILED

```lua
LFG_LIST_ENTRY_CREATION_FAILED()
```

`SynchronousEvent`

### LFG_LIST_ENTRY_EXPIRED_TIMEOUT

```lua
LFG_LIST_ENTRY_EXPIRED_TIMEOUT()
```

`SynchronousEvent`

### LFG_LIST_ENTRY_EXPIRED_TOO_MANY_PLAYERS

```lua
LFG_LIST_ENTRY_EXPIRED_TOO_MANY_PLAYERS()
```

`SynchronousEvent`

### LFG_LIST_JOINED_GROUP

```lua
LFG_LIST_JOINED_GROUP(searchResultID: number, groupName: kstringLfgListChat)
```

`SynchronousEvent`

### LFG_LIST_REVEALED_CENSORED_ACTIVE_ENTRY

```lua
LFG_LIST_REVEALED_CENSORED_ACTIVE_ENTRY()
```

`SynchronousEvent`

### LFG_LIST_SEARCH_FAILED

```lua
LFG_LIST_SEARCH_FAILED(reason: cstring?)
```

`SynchronousEvent`

### LFG_LIST_SEARCH_RESULTS_RECEIVED

```lua
LFG_LIST_SEARCH_RESULTS_RECEIVED()
```

`SynchronousEvent`

### LFG_LIST_SEARCH_RESULT_UPDATED

```lua
LFG_LIST_SEARCH_RESULT_UPDATED(searchResultID: number)
```

`SynchronousEvent`

### LFG_LIST_SHOW_SEARCH

```lua
LFG_LIST_SHOW_SEARCH(activityIDsFilter: number[]?, showAllLevelRanges: bool)
```

`SynchronousEvent`

### LFG_LIST_UPDATE_SEARCH_RESULTS

```lua
LFG_LIST_UPDATE_SEARCH_RESULTS()
```

`SynchronousEvent`

## Types

### AdvancedFilterOptions

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `needsTank` | `bool` | default `false` |
| `needsHealer` | `bool` | default `false` |
| `needsDamage` | `bool` | default `false` |
| `needsMyClass` | `bool` | default `false` |
| `hasTank` | `bool` | default `false` |
| `hasHealer` | `bool` | default `false` |
| `activities` | `number[]` | Activity group IDs to filter by. |
| `minimumRating` | `number` | default `0` |
| `difficultyNormal` | `bool` | default `false` |
| `difficultyHeroic` | `bool` | default `false` |
| `difficultyMythic` | `bool` | default `false` |
| `difficultyMythicPlus` | `bool` | default `false` |
| `generalPlaystyle1` | `bool` | default `false` |
| `generalPlaystyle2` | `bool` | default `false` |
| `generalPlaystyle3` | `bool` | default `false` |
| `generalPlaystyle4` | `bool` | default `false` |

### BestDungeonScoreMapInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `mapScore` | `number` |  |
| `mapName` | `string` |  |
| `bestRunLevel` | `number` |  |
| `finishedSuccess` | `bool` |  |
| `bestRunDurationMs` | `number` |  |
| `bestLevelIncrement` | `number` |  |

### GroupFinderActivityInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `fullName` | `string` |  |
| `shortName` | `string` |  |
| `categoryID` | `number` |  |
| `groupFinderActivityGroupID` | `number` |  |
| `ilvlSuggestion` | `number` |  |
| `filters` | `number` |  |
| `minLevel` | `number` |  |
| `minLevelSuggestion` | `number` |  |
| `maxLevelSuggestion` | `number` |  |
| `maxNumPlayers` | `number` |  |
| `displayType` | `LFGListDisplayType` |  |
| `orderIndex` | `number` |  |
| `useHonorLevel` | `bool` |  |
| `showQuickJoinToast` | `bool` |  |
| `isMythicPlusActivity` | `bool` |  |
| `isRatedPvpActivity` | `bool` |  |
| `isCurrentRaidActivity` | `bool` |  |
| `isPvpActivity` | `bool` |  |
| `isMythicActivity` | `bool` |  |
| `allowCrossFaction` | `bool` |  |
| `isHeroicActivity` | `bool` |  |
| `isNormalActivity` | `bool` |  |
| `mapID` | `number` |  |
| `difficultyID` | `number` |  |
| `redirectedDifficultyID` | `number` |  |
| `useDungeonRoleExpectations` | `bool` |  |

### LfgApplicantData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `applicantID` | `number` |  |
| `applicationStatus` | `cstring` | `NeverSecret` |
| `pendingApplicationStatus` | `cstring?` | `NeverSecret` |
| `numMembers` | `number` | `NeverSecret` |
| `isNew` | `bool` |  |
| `comment` | `kstringLfgListApplicant` |  |
| `displayOrderID` | `number` |  |

### LfgCategoryData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `searchPromptOverride` | `cstring?` |  |
| `separateRecommended` | `bool` |  |
| `autoChooseActivity` | `bool` |  |
| `preferCurrentArea` | `bool` |  |
| `showPlaystyleDropdown` | `bool` |  |
| `allowCrossFaction` | `bool` |  |

### LfgEntryData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `activityIDs` | `number[]` | `NeverSecret` |
| `requiredItemLevel` | `number` |  |
| `requiredHonorLevel` | `number` |  |
| `name` | `kstringLfgListApplicant` |  |
| `comment` | `kstringLfgListApplicant` |  |
| `voiceChat` | `kstringLfgListApplicant` |  |
| `voiceMode` | `LFGEntryVoiceMode` |  |
| `censored` | `bool` |  |
| `duration` | `time_t` |  |
| `autoAccept` | `bool` |  |
| `privateGroup` | `bool` |  |
| `questID` | `number?` |  |
| `requiredDungeonScore` | `number?` |  |
| `requiredPvpRating` | `number?` |  |
| `playstyle` | `LFGEntryPlaystyle?` |  |
| `generalPlaystyle` | `LFGEntryGeneralPlaystyle?` |  |
| `isCrossFactionListing` | `bool` |  |
| `newPlayerFriendly` | `bool` |  |

### LfgListingCreateData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `activityIDs` | `number[]` |  |
| `questID` | `number?` |  |
| `isAutoAccept` | `bool` | default `false` |
| `isCrossFactionListing` | `bool` | default `false` |
| `isPrivateGroup` | `bool` | default `false` |
| `newPlayerFriendly` | `bool` | default `false` |
| `playstyle` | `LFGEntryPlaystyle` | default `"None"` |
| `generalPlaystyle` | `LFGEntryGeneralPlaystyle` | default `"None"` |
| `requiredDungeonScore` | `number` | default `0` |
| `requiredItemLevel` | `number` | default `0` |
| `requiredPvpRating` | `number` | default `0` |
| `voiceMode` | `LFGEntryVoiceMode` | default `"None"` |

### LfgSearchResultData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `searchResultID` | `number` |  |
| `activityIDs` | `number[]` |  |
| `leaderName` | `string?` |  |
| `name` | `kstringLfgListSearch` |  |
| `comment` | `kstringLfgListSearch` |  |
| `voiceChat` | `kstringLfgListSearch` |  |
| `voiceMode` | `LFGEntryVoiceMode` |  |
| `censored` | `bool` |  |
| `requiredItemLevel` | `number` |  |
| `requiredHonorLevel` | `number` |  |
| `hasSelf` | `bool` |  |
| `numMembers` | `number` |  |
| `numBNetFriends` | `number` |  |
| `numCharFriends` | `number` |  |
| `numGuildMates` | `number` |  |
| `isDelisted` | `bool` |  |
| `autoAccept` | `bool` |  |
| `isWarMode` | `bool` |  |
| `age` | `time_t` |  |
| `questID` | `number?` |  |
| `leaderOverallDungeonScore` | `number?` |  |
| `leaderDungeonScoreInfo` | `BestDungeonScoreMapInfo[]` |  |
| `leaderBestDungeonScoreInfo` | `BestDungeonScoreMapInfo?` |  |
| `leaderPvpRatingInfo` | `PvpRatingInfo[]` |  |
| `requiredDungeonScore` | `number?` |  |
| `requiredPvpRating` | `number?` |  |
| `playstyle` | `LFGEntryPlaystyle?` |  |
| `generalPlaystyle` | `LFGEntryGeneralPlaystyle?` |  |
| `crossFactionListing` | `bool?` |  |
| `leaderFactionGroup` | `number` |  |
| `newPlayerFriendly` | `bool?` |  |
| `partyGUID` | `WOWGUID` | `NeverSecret` |

### LfgSearchResultPlayerInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string?` |  |
| `level` | `number?` |  |
| `areaName` | `cstring?` |  |
| `className` | `cstring` |  |
| `classFilename` | `cstring` |  |
| `specName` | `cstring?` |  |
| `assignedRole` | `cstring` |  |
| `lfgRoles` | `LFGRoles` |  |
| `isLeader` | `bool` |  |
| `isLeaver` | `bool` | default `false` |

### PvpRatingInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `bracket` | `number` |  |
| `rating` | `number` |  |
| `activityName` | `string` |  |
| `tier` | `number` |  |

### WowLocale

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `enUS` | `bool` | default `false` |
| `koKR` | `bool` | default `false` |
| `frFR` | `bool` | default `false` |
| `deDE` | `bool` | default `false` |
| `zhCN` | `bool` | default `false` |
| `zhTW` | `bool` | default `false` |
| `esES` | `bool` | default `false` |
| `esMX` | `bool` | default `false` |
| `ruRU` | `bool` | default `false` |
| `ptBR` | `bool` | default `false` |
| `itIT` | `bool` | default `false` |
