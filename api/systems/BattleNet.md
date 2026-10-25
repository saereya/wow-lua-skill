# BattleNet

Namespace `C_BattleNet` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/battlenetdocumentation.lua` (FileDataID 4637037)

## Functions

### AreFriendTagsEnabled

```lua
C_BattleNet.AreFriendTagsEnabled() -> areFriendTagsEnabled: bool
```

### AreHighResTexturesInstalled

```lua
C_BattleNet.AreHighResTexturesInstalled() -> installed: bool
```

### AreRealIDFriendsEnabled

```lua
C_BattleNet.AreRealIDFriendsEnabled() -> areRealIDFriendsEnabled: bool
```

### AreTitleFriendCustomNamesEnabled

```lua
C_BattleNet.AreTitleFriendCustomNamesEnabled() -> areTitleFriendCustomNamesEnabled: bool
```

### AreTitleFriendsEnabled

```lua
C_BattleNet.AreTitleFriendsEnabled() -> areTitleFriendsEnabled: bool
```

### BNCheckBattleTagInviteToRecentAlly

```lua
C_BattleNet.BNCheckBattleTagInviteToRecentAlly(recentAllyGUID: WOWGUID)
```

`SecretArguments=AllowedWhenUntainted`

### BNCheckTitleFriendInviteToUnit

```lua
C_BattleNet.BNCheckTitleFriendInviteToUnit(unit: UnitToken)
```

`SecretArguments=AllowedWhenUntainted`

### CanToggleHighResTexturesWithoutClientReload

```lua
C_BattleNet.CanToggleHighResTexturesWithoutClientReload() -> canToggle: bool
```

### GetAccountInfoByGUID

```lua
C_BattleNet.GetAccountInfoByGUID(guid: WOWGUID) -> accountInfo: BNetAccountInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetAccountInfoByID

```lua
C_BattleNet.GetAccountInfoByID(id: number, wowAccountGUID: WOWGUID?) -> accountInfo: BNetAccountInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetCustomTitleFriendName

```lua
C_BattleNet.GetCustomTitleFriendName(id: number) -> customName: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetFriendAccountInfo

```lua
C_BattleNet.GetFriendAccountInfo(friendIndex: luaIndex, wowAccountGUID: WOWGUID?) -> accountInfo: BNetAccountInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetFriendGameAccountInfo

```lua
C_BattleNet.GetFriendGameAccountInfo(friendIndex: luaIndex, accountIndex: luaIndex) -> gameAccountInfo: BNetGameAccountInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetFriendInviteInfo

```lua
C_BattleNet.GetFriendInviteInfo(inviteIndex: luaIndex) -> inviteInfo: BNetFriendInviteInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetFriendLevelFromInviteText

```lua
C_BattleNet.GetFriendLevelFromInviteText(inviteText: cstring) -> friendLevel: BattleNetFriendLevel
```

`SecretArguments=AllowedWhenUntainted`

### GetFriendNumGameAccounts

```lua
C_BattleNet.GetFriendNumGameAccounts(friendIndex: luaIndex) -> numGameAccounts: number
```

`SecretArguments=AllowedWhenUntainted`

### GetGameAccountInfoByGUID

```lua
C_BattleNet.GetGameAccountInfoByGUID(guid: WOWGUID) -> gameAccountInfo: BNetGameAccountInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetGameAccountInfoByID

```lua
C_BattleNet.GetGameAccountInfoByID(id: number) -> gameAccountInfo: BNetGameAccountInfo?
```

`SecretArguments=AllowedWhenUntainted`

### InstallHighResTextures

```lua
C_BattleNet.InstallHighResTextures()
```

`HasRestrictions`

### InviteFriend

```lua
C_BattleNet.InviteFriend(gameAccountID: number)
```

`SecretArguments=AllowedWhenUntainted`

### IsBattleNetFriendsListEnabled

```lua
C_BattleNet.IsBattleNetFriendsListEnabled() -> isBattleNetFriendsListEnabled: bool
```

### IsBattleNetFriendsListSupported

```lua
C_BattleNet.IsBattleNetFriendsListSupported() -> isBattleNetFriendsListSupported: bool
```

### IsFriendTagSupportedForCurrentGameType

```lua
C_BattleNet.IsFriendTagSupportedForCurrentGameType(friendTag: BattleNetFriendTag) -> isFriendTagSupportedForCurrentGameType: bool
```

`SecretArguments=AllowedWhenUntainted`

### SearchFriends

```lua
C_BattleNet.SearchFriends(searchInfo: AuroraFriendsSearchInfo) -> friendsData: luaIndex[]
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SendGameData

```lua
C_BattleNet.SendGameData(gameAccountID: number, prefix: stringView, data: stringView) -> result: SendAddonMessageResult
```

`SecretArguments=AllowedWhenUntainted`

### SendTitleFriendInviteByName

```lua
C_BattleNet.SendTitleFriendInviteByName(name: cstring)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SendVerifiedBattleNetFriendInvite

```lua
C_BattleNet.SendVerifiedBattleNetFriendInvite()
```

### SendWhisper

```lua
C_BattleNet.SendWhisper(bnetAccountID: number, text: stringView) -> success: bool
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RestrictedForMacroChatMessages`

### SetAFK

```lua
C_BattleNet.SetAFK(isAFK: bool)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `isAFK` | `bool` | default `true` |

### SetAppearOffline

```lua
C_BattleNet.SetAppearOffline(isAppearOffline: bool)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `isAppearOffline` | `bool` | default `true` |

### SetBlocked

```lua
C_BattleNet.SetBlocked(bnetAccountID: number, block: bool)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetCustomMessage

```lua
C_BattleNet.SetCustomMessage(text: cstring) -> success: bool
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetCustomTitleFriendName

```lua
C_BattleNet.SetCustomTitleFriendName(id: number, customName: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### SetDND

```lua
C_BattleNet.SetDND(isDND: bool)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `isDND` | `bool` | default `true` |

### SetFriendTags

```lua
C_BattleNet.SetFriendTags(id: number, friendTags: BattleNetFriendTag[])
```

`SecretArguments=AllowedWhenUntainted`

## Types

### AuroraFriendsSearchInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `searchText` | `string` |  |
| `isOnline` | `bool` |  |
| `isOffline` | `bool` |  |
| `isDND` | `bool` |  |
| `isAFK` | `bool` |  |
| `isInQueue` | `bool` |  |
| `isAvailableForQueue` | `bool` |  |
| `tags` | `BattleNetFriendTag[]` |  |

### BNetAccountInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `bnetAccountID` | `number` |  |
| `accountName` | `string` |  |
| `battleTag` | `string` |  |
| `isFriend` | `bool` |  |
| `isBattleTagFriend` | `bool` |  |
| `friendLevel` | `BattleNetFriendLevel?` |  |
| `lastOnlineTime` | `number` |  |
| `isAFK` | `bool` |  |
| `isDND` | `bool` |  |
| `isFavorite` | `bool` |  |
| `friendTags` | `BattleNetFriendTag[]` |  |
| `appearOffline` | `bool` |  |
| `customMessage` | `string` |  |
| `customMessageTime` | `number` |  |
| `note` | `string` |  |
| `rafLinkType` | `RafLinkType` |  |
| `gameAccountInfo` | `BNetGameAccountInfo` |  |

### BNetFriendInviteInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `inviteID` | `number` |  |
| `accountName` | `kstringAuroraName` |  |
| `creationTimestamp` | `number` |  |
| `friendLevel` | `BattleNetFriendLevel?` |  |

### BNetGameAccountInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `gameAccountID` | `number` |  |
| `clientProgram` | `string` |  |
| `isOnline` | `bool` |  |
| `isGameBusy` | `bool` |  |
| `isGameAFK` | `bool` |  |
| `isAppearOffline` | `bool` |  |
| `wowProjectID` | `number?` |  |
| `characterName` | `string?` |  |
| `realmName` | `string?` |  |
| `realmDisplayName` | `string?` |  |
| `realmID` | `number?` |  |
| `factionName` | `string?` |  |
| `raceName` | `string?` |  |
| `classID` | `number?` |  |
| `className` | `string?` |  |
| `classFilename` | `cstring?` |  |
| `areaName` | `string?` |  |
| `characterLevel` | `number?` |  |
| `richPresence` | `string?` |  |
| `playerGuid` | `WOWGUID?` |  |
| `canSummon` | `bool` |  |
| `hasFocus` | `bool` |  |
| `regionID` | `number` |  |
| `isInCurrentRegion` | `bool` |  |
| `timerunningSeasonID` | `number?` |  |
