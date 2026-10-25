# ClubFinderInfo

Namespace `C_ClubFinder` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/clubfinderdocumentation.lua` (FileDataID 4637066)

## Functions

### ApplicantAcceptClubInvite

```lua
C_ClubFinder.ApplicantAcceptClubInvite(clubFinderGUID: WOWGUID)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### ApplicantDeclineClubInvite

```lua
C_ClubFinder.ApplicantDeclineClubInvite(clubFinderGUID: WOWGUID)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### CancelMembershipRequest

```lua
C_ClubFinder.CancelMembershipRequest(clubFinderGUID: WOWGUID)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### CheckAllPlayerApplicantSettings

```lua
C_ClubFinder.CheckAllPlayerApplicantSettings()
```

### ClearAllFinderCache

```lua
C_ClubFinder.ClearAllFinderCache()
```

### ClearClubApplicantsCache

```lua
C_ClubFinder.ClearClubApplicantsCache()
```

### ClearClubFinderPostingsCache

```lua
C_ClubFinder.ClearClubFinderPostingsCache()
```

### DoesPlayerBelongToClubFromClubGUID

```lua
C_ClubFinder.DoesPlayerBelongToClubFromClubGUID(clubFinderGUID: WOWGUID) -> belongsToClub: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetClubFinderDisableReason

```lua
C_ClubFinder.GetClubFinderDisableReason() -> disableReason: ClubFinderDisableReason?
```

### GetClubRecruitmentSettings

```lua
C_ClubFinder.GetClubRecruitmentSettings() -> settings: ClubSettingsInfo
```

### GetClubTypeFromFinderGUID

```lua
C_ClubFinder.GetClubTypeFromFinderGUID(clubFinderGUID: WOWGUID) -> clubType: ClubFinderRequestType
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetFocusIndexFromFlag

```lua
C_ClubFinder.GetFocusIndexFromFlag(flags: number) -> index: number
```

`SecretArguments=AllowedWhenUntainted`

### GetPlayerApplicantLocaleFlags

```lua
C_ClubFinder.GetPlayerApplicantLocaleFlags() -> localeFlags: number
```

### GetPlayerApplicantSettings

```lua
C_ClubFinder.GetPlayerApplicantSettings() -> settings: ClubSettingsInfo
```

### GetPlayerClubApplicationStatus

```lua
C_ClubFinder.GetPlayerClubApplicationStatus(clubFinderGUID: WOWGUID) -> clubStatus: PlayerClubRequestStatus
```

`SecretArguments=AllowedWhenUntainted`

### GetPlayerSettingsFocusFlagsSelectedCount

```lua
C_ClubFinder.GetPlayerSettingsFocusFlagsSelectedCount() -> focusCount: number
```

### GetPostingIDFromClubFinderGUID

```lua
C_ClubFinder.GetPostingIDFromClubFinderGUID(clubFinderGUID: WOWGUID) -> postingID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetRecruitingClubInfoFromClubID

```lua
C_ClubFinder.GetRecruitingClubInfoFromClubID(clubId: ClubId) -> clubInfo: RecruitingClubInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetRecruitingClubInfoFromFinderGUID

```lua
C_ClubFinder.GetRecruitingClubInfoFromFinderGUID(clubFinderGUID: WOWGUID) -> clubInfo: RecruitingClubInfo
```

`SecretArguments=AllowedWhenUntainted`

### GetStatusOfPostingFromClubId

```lua
C_ClubFinder.GetStatusOfPostingFromClubId(postingID: ClubId) -> postingFlags: ClubFinderClubPostingStatusFlags[]
```

`SecretArguments=AllowedWhenUntainted`

### GetTotalMatchingCommunityListSize

```lua
C_ClubFinder.GetTotalMatchingCommunityListSize() -> totalSize: number
```

### GetTotalMatchingGuildListSize

```lua
C_ClubFinder.GetTotalMatchingGuildListSize() -> totalSize: number
```

### HasAlreadyAppliedToLinkedPosting

```lua
C_ClubFinder.HasAlreadyAppliedToLinkedPosting(clubFinderGUID: WOWGUID) -> hasAlreadyApplied: bool
```

`SecretArguments=AllowedWhenUntainted`

### HasPostingBeenDelisted

```lua
C_ClubFinder.HasPostingBeenDelisted(postingID: ClubId) -> postingDelisted: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsCommunityFinderEnabled

```lua
C_ClubFinder.IsCommunityFinderEnabled() -> isEnabled: bool
```

### IsEnabled

```lua
C_ClubFinder.IsEnabled() -> isEnabled: bool
```

### IsListingEnabledFromFlags

```lua
C_ClubFinder.IsListingEnabledFromFlags(flags: number) -> isListed: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsPostingBanned

```lua
C_ClubFinder.IsPostingBanned(postingID: ClubId) -> postingBanned: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsValidSearchString

```lua
C_ClubFinder.IsValidSearchString(name: cstring) -> isApproved: bool
```

`SecretArguments=AllowedWhenUntainted`

### LookupClubPostingFromClubFinderGUID

```lua
C_ClubFinder.LookupClubPostingFromClubFinderGUID(clubFinderGUID: WOWGUID, isLinkedPosting: bool)
```

`SecretArguments=AllowedWhenUntainted`

### PlayerGetClubInvitationList

```lua
C_ClubFinder.PlayerGetClubInvitationList() -> inviteList: RecruitingClubInfo[]
```

`MayReturnNothing`

### PlayerRequestPendingClubsList

```lua
C_ClubFinder.PlayerRequestPendingClubsList(type: ClubFinderRequestType)
```

`SecretArguments=AllowedWhenUntainted`

### PlayerReturnPendingCommunitiesList

```lua
C_ClubFinder.PlayerReturnPendingCommunitiesList() -> info: RecruitingClubInfo[]
```

### PlayerReturnPendingGuildsList

```lua
C_ClubFinder.PlayerReturnPendingGuildsList() -> info: RecruitingClubInfo[]
```

### PostClub

```lua
C_ClubFinder.PostClub(clubId: ClubId, itemLevelRequirement: number, name: string, description: string, avatarId: number, specs: number[], type: ClubFinderRequestType, crossFaction: bool) -> succesful: bool
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `clubId` | `ClubId` |  |
| `itemLevelRequirement` | `number` |  |
| `name` | `string` |  |
| `description` | `string` |  |
| `avatarId` | `number` |  |
| `specs` | `number[]` |  |
| `type` | `ClubFinderRequestType` |  |
| `crossFaction` | `bool` | default `false` |

### RequestApplicantList

```lua
C_ClubFinder.RequestApplicantList(type: ClubFinderRequestType)
```

`SecretArguments=AllowedWhenUntainted`

### RequestClubsList

```lua
C_ClubFinder.RequestClubsList(guildListRequested: bool, searchString: string, specIDs: number[])
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### RequestMembershipToClub

```lua
C_ClubFinder.RequestMembershipToClub(clubFinderGUID: WOWGUID, comment: string, specIDs: number[])
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### RequestNextCommunityPage

```lua
C_ClubFinder.RequestNextCommunityPage(startingIndex: number, pageSize: number)
```

`SecretArguments=AllowedWhenUntainted`

### RequestNextGuildPage

```lua
C_ClubFinder.RequestNextGuildPage(startingIndex: number, pageSize: number)
```

`SecretArguments=AllowedWhenUntainted`

### RequestPostingInformationFromClubId

```lua
C_ClubFinder.RequestPostingInformationFromClubId(clubId: ClubId) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### RequestSubscribedClubPostingIDs

```lua
C_ClubFinder.RequestSubscribedClubPostingIDs()
```

### ResetClubPostingMapCache

```lua
C_ClubFinder.ResetClubPostingMapCache()
```

### RespondToApplicant

```lua
C_ClubFinder.RespondToApplicant(clubFinderGUID: WOWGUID, playerGUID: WOWGUID, shouldAccept: bool, requestType: ClubFinderRequestType, playerName: string, forceAccept: bool, reported: bool?)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### ReturnClubApplicantList

```lua
C_ClubFinder.ReturnClubApplicantList(clubId: ClubId) -> info: ClubFinderApplicantInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### ReturnMatchingCommunityList

```lua
C_ClubFinder.ReturnMatchingCommunityList() -> recruitingClubs: RecruitingClubInfo[]
```

### ReturnMatchingGuildList

```lua
C_ClubFinder.ReturnMatchingGuildList() -> recruitingClubs: RecruitingClubInfo[]
```

### ReturnPendingClubApplicantList

```lua
C_ClubFinder.ReturnPendingClubApplicantList(clubId: ClubId) -> info: ClubFinderApplicantInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### SendChatWhisper

```lua
C_ClubFinder.SendChatWhisper(clubFinderGUID: WOWGUID, playerGUID: WOWGUID, applicantType: ClubFinderRequestType, name: string)
```

`SecretArguments=AllowedWhenUntainted`

### SetAllRecruitmentSettings

```lua
C_ClubFinder.SetAllRecruitmentSettings(value: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetPlayerApplicantLocaleFlags

```lua
C_ClubFinder.SetPlayerApplicantLocaleFlags(localeFlags: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetPlayerApplicantSettings

```lua
C_ClubFinder.SetPlayerApplicantSettings(index: number, checked: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetRecruitmentLocale

```lua
C_ClubFinder.SetRecruitmentLocale(locale: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetRecruitmentSettings

```lua
C_ClubFinder.SetRecruitmentSettings(index: number, checked: bool)
```

`SecretArguments=AllowedWhenUntainted`

### ShouldShowClubFinder

```lua
C_ClubFinder.ShouldShowClubFinder() -> shouldShow: bool
```

## Events

### CLUB_FINDER_APPLICANT_INVITE_RECIEVED

```lua
CLUB_FINDER_APPLICANT_INVITE_RECIEVED(clubFinderGUIDs: WOWGUID[])
```

`SynchronousEvent`

### CLUB_FINDER_APPLICATIONS_UPDATED

```lua
CLUB_FINDER_APPLICATIONS_UPDATED(type: ClubFinderRequestType, clubFinderGUIDs: WOWGUID[])
```

`SynchronousEvent`

### CLUB_FINDER_CAN_WHISPER_APPLICANT

```lua
CLUB_FINDER_CAN_WHISPER_APPLICANT(applicant: WOWGUID)
```

`SynchronousEvent`

### CLUB_FINDER_CLUB_LIST_RETURNED

```lua
CLUB_FINDER_CLUB_LIST_RETURNED(type: ClubFinderRequestType)
```

Signals when we recieve club data that can be used

`SynchronousEvent`

### CLUB_FINDER_CLUB_REPORTED

```lua
CLUB_FINDER_CLUB_REPORTED(type: ClubFinderRequestType, clubFinderGUID: WOWGUID)
```

Sends an update to the UI about a reported guild or community.

`SynchronousEvent`

### CLUB_FINDER_COMMUNITY_OFFLINE_JOIN

```lua
CLUB_FINDER_COMMUNITY_OFFLINE_JOIN(clubId: ClubId)
```

Signals to the UI that you (the player) have joined a community offline.

`SynchronousEvent`

### CLUB_FINDER_ENABLED_OR_DISABLED

```lua
CLUB_FINDER_ENABLED_OR_DISABLED()
```

Sends an update to the UI that the club finder feature has been enabled or disabled.

`SynchronousEvent`

### CLUB_FINDER_GUILD_REALM_NAME_UPDATED

```lua
CLUB_FINDER_GUILD_REALM_NAME_UPDATED(clubFinderGUID: WOWGUID, realmName: string)
```

Sends an update to the UI if the realm name of a guild was found asynchronously.

`SynchronousEvent`

### CLUB_FINDER_LINKED_CLUB_RETURNED

```lua
CLUB_FINDER_LINKED_CLUB_RETURNED(clubInfo: RecruitingClubInfo)
```

When a player clicks a club link, this returns that information back about the club they clicked on

`SynchronousEvent`

### CLUB_FINDER_MEMBERSHIP_LIST_CHANGED

```lua
CLUB_FINDER_MEMBERSHIP_LIST_CHANGED()
```

`SynchronousEvent`

### CLUB_FINDER_PLAYER_PENDING_LIST_RECIEVED

```lua
CLUB_FINDER_PLAYER_PENDING_LIST_RECIEVED(type: ClubFinderRequestType)
```

`SynchronousEvent`

### CLUB_FINDER_POST_UPDATED

```lua
CLUB_FINDER_POST_UPDATED(clubFinderGUIDs: WOWGUID[])
```

`SynchronousEvent`

### CLUB_FINDER_RECRUIT_LIST_CHANGED

```lua
CLUB_FINDER_RECRUIT_LIST_CHANGED()
```

`SynchronousEvent`

### CLUB_FINDER_RECRUITMENT_POST_RETURNED

```lua
CLUB_FINDER_RECRUITMENT_POST_RETURNED(type: ClubFinderRequestType)
```

Signals when our recruitment post we just requested is returned back to us

`SynchronousEvent`

### CLUB_FINDER_RECRUITS_UPDATED

```lua
CLUB_FINDER_RECRUITS_UPDATED(type: ClubFinderRequestType)
```

Signals when we recieve the recruits list

`SynchronousEvent`

## Types

### ClubFinderApplicationUpdateType

*Enumeration* · 4 values, 0..3

Access values as `Enum.ClubFinderApplicationUpdateType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `ClubFinderApplicationUpdateType` | = 0 |
| `AcceptInvite` | `ClubFinderApplicationUpdateType` | = 1 |
| `DeclineInvite` | `ClubFinderApplicationUpdateType` | = 2 |
| `Cancel` | `ClubFinderApplicationUpdateType` | = 3 |

### ClubFinderClubPostingStatusFlags

*Enumeration* · 9 values, 0..8

Access values as `Enum.ClubFinderClubPostingStatusFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `ClubFinderClubPostingStatusFlags` | = 0 |
| `NeedsCacheUpdate` | `ClubFinderClubPostingStatusFlags` | = 1 |
| `ForceDescriptionChange` | `ClubFinderClubPostingStatusFlags` | = 2 |
| `ForceNameChange` | `ClubFinderClubPostingStatusFlags` | = 3 |
| `UnderReview` | `ClubFinderClubPostingStatusFlags` | = 4 |
| `Banned` | `ClubFinderClubPostingStatusFlags` | = 5 |
| `FakePost` | `ClubFinderClubPostingStatusFlags` | = 6 |
| `PendingDelete` | `ClubFinderClubPostingStatusFlags` | = 7 |
| `PostDelisted` | `ClubFinderClubPostingStatusFlags` | = 8 |

### ClubFinderDisableReason

*Enumeration* · 3 values, 0..2

Access values as `Enum.ClubFinderDisableReason.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Muted` | `ClubFinderDisableReason` | = 0 |
| `Silenced` | `ClubFinderDisableReason` | = 1 |
| `VeteranTrial` | `ClubFinderDisableReason` | = 2 |

### ClubFinderPostingReportType

*Enumeration* · 5 values, 0..4

Access values as `Enum.ClubFinderPostingReportType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `PostersName` | `ClubFinderPostingReportType` | = 0 |
| `ClubName` | `ClubFinderPostingReportType` | = 1 |
| `PostingDescription` | `ClubFinderPostingReportType` | = 2 |
| `ApplicantsName` | `ClubFinderPostingReportType` | = 3 |
| `JoinNote` | `ClubFinderPostingReportType` | = 4 |

### ClubFinderRequestType

*Enumeration* · 4 values, 0..3

Access values as `Enum.ClubFinderRequestType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `ClubFinderRequestType` | = 0 |
| `Guild` | `ClubFinderRequestType` | = 1 |
| `Community` | `ClubFinderRequestType` | = 2 |
| `All` | `ClubFinderRequestType` | = 3 |

### ClubFinderSettingFlags

*Enumeration* · 26 values, 0..25

Access values as `Enum.ClubFinderSettingFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `ClubFinderSettingFlags` | = 0 |
| `Dungeons` | `ClubFinderSettingFlags` | = 1 |
| `Raids` | `ClubFinderSettingFlags` | = 2 |
| `PvP` | `ClubFinderSettingFlags` | = 3 |
| `RP` | `ClubFinderSettingFlags` | = 4 |
| `Social` | `ClubFinderSettingFlags` | = 5 |
| `Small` | `ClubFinderSettingFlags` | = 6 |
| `Medium` | `ClubFinderSettingFlags` | = 7 |
| `Large` | `ClubFinderSettingFlags` | = 8 |
| `Tank` | `ClubFinderSettingFlags` | = 9 |
| `Healer` | `ClubFinderSettingFlags` | = 10 |
| `Damage` | `ClubFinderSettingFlags` | = 11 |
| `EnableListing` | `ClubFinderSettingFlags` | = 12 |
| `MaxLevelOnly` | `ClubFinderSettingFlags` | = 13 |
| `AutoAccept` | `ClubFinderSettingFlags` | = 14 |
| `FactionHorde` | `ClubFinderSettingFlags` | = 15 |
| `FactionAlliance` | `ClubFinderSettingFlags` | = 16 |
| `FactionNeutral` | `ClubFinderSettingFlags` | = 17 |
| `SortRelevance` | `ClubFinderSettingFlags` | = 18 |
| `SortMemberCount` | `ClubFinderSettingFlags` | = 19 |
| `SortNewest` | `ClubFinderSettingFlags` | = 20 |
| `LanguageReserved1` | `ClubFinderSettingFlags` | = 21 |
| `LanguageReserved2` | `ClubFinderSettingFlags` | = 22 |
| `LanguageReserved3` | `ClubFinderSettingFlags` | = 23 |
| `LanguageReserved4` | `ClubFinderSettingFlags` | = 24 |
| `LanguageReserved5` | `ClubFinderSettingFlags` | = 25 |

### PlayerClubRequestStatus

*Enumeration* · 8 values, 0..7

Access values as `Enum.PlayerClubRequestStatus.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `PlayerClubRequestStatus` | = 0 |
| `Pending` | `PlayerClubRequestStatus` | = 1 |
| `AutoApproved` | `PlayerClubRequestStatus` | = 2 |
| `Declined` | `PlayerClubRequestStatus` | = 3 |
| `Approved` | `PlayerClubRequestStatus` | = 4 |
| `Joined` | `PlayerClubRequestStatus` | = 5 |
| `JoinedAnother` | `PlayerClubRequestStatus` | = 6 |
| `Canceled` | `PlayerClubRequestStatus` | = 7 |

### ClubFinderApplicantInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `clubFinderGUID` | `WOWGUID` |  |
| `playerGUID` | `WOWGUID` |  |
| `closed` | `number` |  |
| `name` | `string` |  |
| `message` | `string` |  |
| `level` | `number` |  |
| `classID` | `number` |  |
| `ilvl` | `number` |  |
| `specIds` | `number[]` |  |
| `requestStatus` | `PlayerClubRequestStatus` |  |
| `lookupSuccess` | `bool` |  |
| `lastUpdatedTime` | `BigInteger` |  |
| `faction` | `number` |  |

### ClubSettingsInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `playStyleDungeon` | `bool` |  |
| `playStyleRaids` | `bool` |  |
| `playStylePvp` | `bool` |  |
| `playStyleRP` | `bool` |  |
| `playStyleSocial` | `bool` |  |
| `roleTank` | `bool` |  |
| `roleHealer` | `bool` |  |
| `roleDps` | `bool` |  |
| `sizeSmall` | `bool` |  |
| `sizeMedium` | `bool` |  |
| `sizeLarge` | `bool` |  |
| `maxLevelOnly` | `bool` |  |
| `enableListing` | `bool` |  |
| `sortRelevance` | `bool` |  |
| `sortMembers` | `bool` |  |
| `sortNewest` | `bool` |  |
| `autoAccept` | `bool` |  |
| `crossFaction` | `bool` |  |

### RecruitingClubInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `clubFinderGUID` | `WOWGUID` |  |
| `numActiveMembers` | `number` |  |
| `name` | `string` |  |
| `comment` | `string` |  |
| `guildLeader` | `string` |  |
| `isGuild` | `bool` |  |
| `emblemInfo` | `number` |  |
| `tabardInfo` | `GuildTabardInfo?` |  |
| `recruitingSpecIds` | `number[]` |  |
| `recruitmentFlags` | `number` |  |
| `localeSet` | `bool` |  |
| `recruitmentLocale` | `number` |  |
| `minILvl` | `number` |  |
| `cached` | `number` |  |
| `cacheRequested` | `number` |  |
| `lastPosterGUID` | `WOWGUID` |  |
| `clubId` | `ClubId` |  |
| `lastUpdatedTime` | `BigInteger` |  |
| `isCrossFaction` | `bool` |  |
| `realmName` | `string?` |  |
