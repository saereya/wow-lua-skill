# GuildInfo

Namespace `C_GuildInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/guildinfodocumentation.lua` (FileDataID 4637110)

## Functions

### AreGuildEventsEnabled

```lua
C_GuildInfo.AreGuildEventsEnabled() -> enabled: bool
```

### CanEditOfficerNote

```lua
C_GuildInfo.CanEditOfficerNote() -> canEditOfficerNote: bool
```

### CanSpeakInGuildChat

```lua
C_GuildInfo.CanSpeakInGuildChat() -> canSpeakInGuildChat: bool
```

### CanViewOfficerNote

```lua
C_GuildInfo.CanViewOfficerNote() -> canViewOfficerNote: bool
```

### Demote

```lua
C_GuildInfo.Demote(name: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### Disband

```lua
C_GuildInfo.Disband()
```

### GetGuildNewsInfo

```lua
C_GuildInfo.GetGuildNewsInfo(index: luaIndex) -> newsInfo: GuildNewsInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetGuildRankOrder

```lua
C_GuildInfo.GetGuildRankOrder(guid: WOWGUID) -> rankOrder: luaIndex
```

`SecretArguments=AllowedWhenUntainted`

### GetGuildTabardInfo

```lua
C_GuildInfo.GetGuildTabardInfo(unit: UnitToken?) -> tabardInfo: GuildTabardInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetInfoText

```lua
C_GuildInfo.GetInfoText() -> infoText: string
```

`HasRestrictions`

### GetMOTD

```lua
C_GuildInfo.GetMOTD() -> motd: string
```

`HasRestrictions`

### GetPreferredPlaySettings

```lua
C_GuildInfo.GetPreferredPlaySettings() -> loaded: bool, preferredLocaleID: number, preferredDatacenterLocalityID: number, lastPreferredLocaleChangeDate: time_t, lastPreferredDatacenterLocalityChangeDate: time_t, changeCooldownDays: number
```

### GetPreferredPlaySettingsFeatures

```lua
C_GuildInfo.GetPreferredPlaySettingsFeatures() -> canChangeLocale: bool, canChangeDatacenterLocality: bool
```

### GuildControlGetRankFlags

```lua
C_GuildInfo.GuildControlGetRankFlags(rankOrder: luaIndex) -> permissions: bool[]
```

`SecretArguments=AllowedWhenUntainted`

### GuildRoster

```lua
C_GuildInfo.GuildRoster()
```

### Invite

```lua
C_GuildInfo.Invite(name: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### IsDiscordStreamSeparate

```lua
C_GuildInfo.IsDiscordStreamSeparate() -> separateStream: bool
```

### IsEncounterGuildNewsEnabled

```lua
C_GuildInfo.IsEncounterGuildNewsEnabled() -> enabled: bool
```

### IsGuildOfficer

```lua
C_GuildInfo.IsGuildOfficer() -> isOfficer: bool
```

### IsGuildRankAssignmentAllowed

```lua
C_GuildInfo.IsGuildRankAssignmentAllowed(guid: WOWGUID, rankOrder: luaIndex) -> isGuildRankAssignmentAllowed: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsGuildReputationEnabled

```lua
C_GuildInfo.IsGuildReputationEnabled() -> enabled: bool
```

### Leave

```lua
C_GuildInfo.Leave()
```

### MemberExistsByName

```lua
C_GuildInfo.MemberExistsByName(name: cstring) -> exists: bool
```

`SecretArguments=AllowedWhenUntainted`

### Promote

```lua
C_GuildInfo.Promote(name: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### QueryGuildMemberRecipes

```lua
C_GuildInfo.QueryGuildMemberRecipes(guildMemberGUID: WOWGUID, skillLineID: number)
```

`SecretArguments=AllowedWhenUntainted`

### QueryGuildMembersForRecipe

```lua
C_GuildInfo.QueryGuildMembersForRecipe(skillLineID: number, recipeSpellID: number, recipeLevel: luaIndex?) -> updatedRecipeSpellID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### RemoveFromGuild

```lua
C_GuildInfo.RemoveFromGuild(guid: WOWGUID)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### RequestGuildRename

```lua
C_GuildInfo.RequestGuildRename(desiredName: cstring)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### RequestGuildRenameRefund

```lua
C_GuildInfo.RequestGuildRenameRefund()
```

`HasRestrictions`

### RequestPreferredPlaySettings

```lua
C_GuildInfo.RequestPreferredPlaySettings() -> startedSuccessfully: bool
```

### RequestRenameNameCheck

```lua
C_GuildInfo.RequestRenameNameCheck(desiredName: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### RequestRenameStatus

```lua
C_GuildInfo.RequestRenameStatus() -> ableToRequest: bool
```

### SetGuildRankOrder

```lua
C_GuildInfo.SetGuildRankOrder(guid: WOWGUID, rankOrder: luaIndex)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetInfoText

```lua
C_GuildInfo.SetInfoText(infoText: cstring)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetLeader

```lua
C_GuildInfo.SetLeader(name: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### SetMOTD

```lua
C_GuildInfo.SetMOTD(motd: cstring)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetNote

```lua
C_GuildInfo.SetNote(guid: WOWGUID, note: cstring, isPublic: bool)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetPreferredPlaySettings

```lua
C_GuildInfo.SetPreferredPlaySettings(preferredLocaleID: number, preferredDatacenterLocalityID: number) -> startedSuccessfully: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `preferredLocaleID` | `number` | default `0` |
| `preferredDatacenterLocalityID` | `number` | default `0` |

### Uninvite

```lua
C_GuildInfo.Uninvite(name: cstring)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### CLOSE_TABARD_FRAME

```lua
CLOSE_TABARD_FRAME()
```

`SynchronousEvent`

### DISABLE_DECLINE_GUILD_INVITE

```lua
DISABLE_DECLINE_GUILD_INVITE()
```

`SynchronousEvent`

### ENABLE_DECLINE_GUILD_INVITE

```lua
ENABLE_DECLINE_GUILD_INVITE()
```

`SynchronousEvent`

### GUILD_CHALLENGE_COMPLETED

```lua
GUILD_CHALLENGE_COMPLETED(challengeType: number, currentCount: number, maxCount: number, goldAwarded: number)
```

`SynchronousEvent`

### GUILD_CHALLENGE_UPDATED

```lua
GUILD_CHALLENGE_UPDATED()
```

`SynchronousEvent`

### GUILD_EVENT_LOG_UPDATE

```lua
GUILD_EVENT_LOG_UPDATE()
```

`SynchronousEvent`

### GUILD_INVITE_CANCEL

```lua
GUILD_INVITE_CANCEL()
```

`SynchronousEvent`

### GUILD_INVITE_REQUEST

```lua
GUILD_INVITE_REQUEST(inviter: cstring, guildName: cstring, guildAchievementPoints: number, oldGuildName: cstring, isNewGuild: bool?, tabardInfo: GuildTabardInfo?)
```

`SynchronousEvent`

### GUILD_MOTD

```lua
GUILD_MOTD(motdText: cstring)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

### GUILD_NEWS_UPDATE

```lua
GUILD_NEWS_UPDATE()
```

`UniqueEvent`

### GUILD_PARTY_STATE_UPDATED

```lua
GUILD_PARTY_STATE_UPDATED(inGuildParty: bool)
```

`SynchronousEvent`

### GUILD_PREFERRED_PLAY_SETTINGS_UPDATED

```lua
GUILD_PREFERRED_PLAY_SETTINGS_UPDATED(status: PreferredPlaySettingsStatus, preferredLocaleID: number, preferredDatacenterLocalityID: number, lastPreferredLocaleChangeDate: time_t, lastPreferredDatacenterLocalityChangeDate: time_t)
```

`SynchronousEvent`

### GUILD_RANKS_UPDATE

```lua
GUILD_RANKS_UPDATE()
```

`SynchronousEvent`

### GUILD_RANKS_UPDATE_ACTIVE_PLAYER

```lua
GUILD_RANKS_UPDATE_ACTIVE_PLAYER()
```

`SynchronousEvent`

### GUILD_RECIPE_KNOWN_BY_MEMBERS

```lua
GUILD_RECIPE_KNOWN_BY_MEMBERS()
```

`SynchronousEvent`

### GUILD_REGISTRAR_CLOSED

```lua
GUILD_REGISTRAR_CLOSED()
```

`SynchronousEvent`

### GUILD_REGISTRAR_SHOW

```lua
GUILD_REGISTRAR_SHOW()
```

`SynchronousEvent`

### GUILD_RENAME_NAME_CHECK

```lua
GUILD_RENAME_NAME_CHECK(desiredName: cstring, status: GuildErrorType, nameErrorToken: cstring?)
```

`SynchronousEvent`

### GUILD_RENAME_REFUND_RESULT

```lua
GUILD_RENAME_REFUND_RESULT(guildName: cstring, status: GuildErrorType)
```

`SynchronousEvent`

### GUILD_RENAME_REQUIRED

```lua
GUILD_RENAME_REQUIRED(flagSet: bool)
```

`SynchronousEvent`

### GUILD_RENAME_STATUS_UPDATE

```lua
GUILD_RENAME_STATUS_UPDATE(status: GuildRenameStatus)
```

`SynchronousEvent`

### GUILD_REWARDS_LIST

```lua
GUILD_REWARDS_LIST()
```

`SynchronousEvent`

### GUILD_REWARDS_LIST_UPDATE

```lua
GUILD_REWARDS_LIST_UPDATE()
```

`UniqueEvent`

### GUILD_ROSTER_UPDATE

```lua
GUILD_ROSTER_UPDATE(canRequestRosterUpdate: bool)
```

`SynchronousEvent`

### GUILDTABARD_UPDATE

```lua
GUILDTABARD_UPDATE()
```

`SynchronousEvent`

### GUILD_TRADESKILL_UPDATE

```lua
GUILD_TRADESKILL_UPDATE()
```

`SynchronousEvent`

### OPEN_TABARD_FRAME

```lua
OPEN_TABARD_FRAME()
```

`SynchronousEvent`

### PLAYER_GUILD_UPDATE

```lua
PLAYER_GUILD_UPDATE(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### REQUESTED_GUILD_RENAME_RESULT

```lua
REQUESTED_GUILD_RENAME_RESULT(newName: cstring, status: GuildErrorType)
```

`SynchronousEvent`

### REQUIRED_GUILD_RENAME_RESULT

```lua
REQUIRED_GUILD_RENAME_RESULT(success: bool)
```

`SynchronousEvent`

### TABARD_CANSAVE_CHANGED

```lua
TABARD_CANSAVE_CHANGED()
```

`SynchronousEvent`

### TABARD_SAVE_PENDING

```lua
TABARD_SAVE_PENDING()
```

`SynchronousEvent`

### UNIT_GUILD_LEVEL

```lua
UNIT_GUILD_LEVEL(newLevel: number)
```

`SynchronousEvent`

## Types

### GuildNewsInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `isSticky` | `bool` |  |
| `isHeader` | `bool` |  |
| `newsType` | `number` |  |
| `whoText` | `string?` |  |
| `whatText` | `string?` |  |
| `newsDataID` | `number` |  |
| `data` | `number[]` |  |
| `weekday` | `number` |  |
| `day` | `number` |  |
| `month` | `number` |  |
| `year` | `number` |  |
| `guildMembersPresent` | `number` |  |

### GuildRenameStatus

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `isNameChangeEnabled` | `bool` |  |
| `isPlayerGuildMaster` | `bool` |  |
| `refundEligibleEndTime` | `time_t` |  |
| `nextRenameTime` | `time_t` |  |
| `renamePrice` | `WOWMONEY` |  |
| `refundAmount` | `WOWMONEY` |  |
| `currentGuildMoney` | `WOWMONEY` |  |
| `result` | `GuildErrorType` |  |
| `oldGuildName` | `cstring` |  |
| `reservedName` | `cstring` |  |
| `reservedNameExpirationTime` | `time_t` |  |
