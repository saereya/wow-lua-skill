# FriendList

Namespace `C_FriendList` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/friendlistdocumentation.lua` (FileDataID 4637108)

## Functions

### AddFriend

```lua
C_FriendList.AddFriend(name: cstring, notes: cstring?)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RequiresFriendList`

### AddIgnore

```lua
C_FriendList.AddIgnore(name: cstring) -> added: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresFriendList`

### AddOrDelIgnore

```lua
C_FriendList.AddOrDelIgnore(name: cstring)
```

`SecretArguments=AllowedWhenUntainted` `RequiresFriendList`

### AddOrRemoveFriend

```lua
C_FriendList.AddOrRemoveFriend(name: cstring, notes: cstring)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RequiresFriendList`

### DelIgnore

```lua
C_FriendList.DelIgnore(name: cstring) -> removed: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresFriendList`

### DelIgnoreByIndex

```lua
C_FriendList.DelIgnoreByIndex(index: luaIndex)
```

`SecretArguments=AllowedWhenUntainted` `RequiresFriendList`

### GetFriendInfo

```lua
C_FriendList.GetFriendInfo(name: cstring) -> info: FriendInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresFriendList`

### GetFriendInfoByIndex

```lua
C_FriendList.GetFriendInfoByIndex(index: luaIndex) -> info: FriendInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresFriendList`

### GetIgnoreName

```lua
C_FriendList.GetIgnoreName(index: luaIndex) -> name: string?
```

`SecretArguments=AllowedWhenUntainted` `RequiresFriendList`

### GetNumFriends

```lua
C_FriendList.GetNumFriends() -> numFriends: number
```

`RequiresFriendList`

### GetNumIgnores

```lua
C_FriendList.GetNumIgnores() -> numIgnores: number
```

`RequiresFriendList`

### GetNumOnlineFriends

```lua
C_FriendList.GetNumOnlineFriends() -> numOnline: number
```

`RequiresFriendList`

### GetNumWhoResults

```lua
C_FriendList.GetNumWhoResults() -> numWhos: number, totalNumWhos: number
```

`RequiresFriendList`

### GetSelectedFriend

```lua
C_FriendList.GetSelectedFriend() -> index: luaIndex?
```

`RequiresFriendList`

### GetSelectedIgnore

```lua
C_FriendList.GetSelectedIgnore() -> index: luaIndex?
```

`RequiresFriendList`

### GetWhoInfo

```lua
C_FriendList.GetWhoInfo(index: luaIndex) -> info: WhoInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresFriendList`

### GetWhoRaceFilters

```lua
C_FriendList.GetWhoRaceFilters() -> filters: WhoFilter[]
```

`RequiresFriendList`

### IsFriend

```lua
C_FriendList.IsFriend(guid: WOWGUID) -> isFriend: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresFriendList`

### IsIgnored

```lua
C_FriendList.IsIgnored(token: cstring) -> isIgnored: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresFriendList`

### IsIgnoredByGuid

```lua
C_FriendList.IsIgnoredByGuid(guid: WOWGUID) -> isIgnored: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresFriendList`

### IsLegacyFriendSystemEnabled

```lua
C_FriendList.IsLegacyFriendSystemEnabled() -> isLegacyFriendSystemEnabled: bool
```

`RequiresFriendList`

### IsOnIgnoredList

```lua
C_FriendList.IsOnIgnoredList(token: cstring) -> isIgnored: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresFriendList`

### RemoveFriend

```lua
C_FriendList.RemoveFriend(name: cstring) -> removed: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresFriendList`

### RemoveFriendByIndex

```lua
C_FriendList.RemoveFriendByIndex(index: luaIndex)
```

`SecretArguments=AllowedWhenUntainted` `RequiresFriendList`

### SendWho

```lua
C_FriendList.SendWho(filter: cstring, origin: number?, filters: SendWhoFilters?)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RequiresFriendList`

### SetFriendNotes

```lua
C_FriendList.SetFriendNotes(name: cstring, notes: cstring) -> found: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresFriendList`

### SetFriendNotesByIndex

```lua
C_FriendList.SetFriendNotesByIndex(index: luaIndex, notes: cstring)
```

`SecretArguments=AllowedWhenUntainted` `RequiresFriendList`

### SetSelectedFriend

```lua
C_FriendList.SetSelectedFriend(index: luaIndex)
```

`SecretArguments=AllowedWhenUntainted` `RequiresFriendList`

### SetSelectedIgnore

```lua
C_FriendList.SetSelectedIgnore(index: luaIndex)
```

`SecretArguments=AllowedWhenUntainted` `RequiresFriendList`

### SetWhoToUi

```lua
C_FriendList.SetWhoToUi(whoToUi: bool)
```

`SecretArguments=AllowedWhenUntainted` `RequiresFriendList`

### ShowFriends

```lua
C_FriendList.ShowFriends()
```

`RequiresFriendList`

### SortWho

```lua
C_FriendList.SortWho(sorting: cstring, ascending: bool?)
```

`SecretArguments=AllowedWhenUntainted` `RequiresFriendList`

## Events

### BATTLE_NET_FRIEND_TAG_ENABLED_STATUS_UPDATED

```lua
BATTLE_NET_FRIEND_TAG_ENABLED_STATUS_UPDATED()
```

`SynchronousEvent`

### BATTLE_NET_TITLE_FRIEND_CUSTOM_NAME_ENABLED_STATUS_UPDATED

```lua
BATTLE_NET_TITLE_FRIEND_CUSTOM_NAME_ENABLED_STATUS_UPDATED()
```

`SynchronousEvent`

### BN_BLOCK_FAILED_TOO_MANY

```lua
BN_BLOCK_FAILED_TOO_MANY(blockType: cstring)
```

`SynchronousEvent`

### BN_BLOCK_LIST_UPDATED

```lua
BN_BLOCK_LIST_UPDATED()
```

`SynchronousEvent`

### BN_CHAT_WHISPER_UNDELIVERABLE

```lua
BN_CHAT_WHISPER_UNDELIVERABLE(senderID: number)
```

`SynchronousEvent`

### BN_CONNECTED

```lua
BN_CONNECTED(suppressNotification: bool)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `suppressNotification` | `bool` | default `false` |

### BN_CUSTOM_MESSAGE_CHANGED

```lua
BN_CUSTOM_MESSAGE_CHANGED(id: number?)
```

`SynchronousEvent`

### BN_CUSTOM_MESSAGE_LOADED

```lua
BN_CUSTOM_MESSAGE_LOADED()
```

`SynchronousEvent`

### BN_DISCONNECTED

```lua
BN_DISCONNECTED(result: bool, suppressNotification: bool)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `result` | `bool` |  |
| `suppressNotification` | `bool` | default `false` |

### BN_FRIEND_ACCOUNT_OFFLINE

```lua
BN_FRIEND_ACCOUNT_OFFLINE(friendId: number, isCompanionApp: bool)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `friendId` | `number` |  |
| `isCompanionApp` | `bool` | default `false` |

### BN_FRIEND_ACCOUNT_ONLINE

```lua
BN_FRIEND_ACCOUNT_ONLINE(friendId: number, isCompanionApp: bool)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `friendId` | `number` |  |
| `isCompanionApp` | `bool` | default `false` |

### BN_FRIEND_INFO_CHANGED

```lua
BN_FRIEND_INFO_CHANGED(friendIndex: luaIndex?)
```

`SynchronousEvent`

### BN_FRIEND_INVITE_ADDED

```lua
BN_FRIEND_INVITE_ADDED(accountID: number)
```

`SynchronousEvent`

### BN_FRIEND_INVITE_LIST_INITIALIZED

```lua
BN_FRIEND_INVITE_LIST_INITIALIZED(listSize: number)
```

`SynchronousEvent`

### BN_FRIEND_INVITE_REMOVED

```lua
BN_FRIEND_INVITE_REMOVED()
```

`SynchronousEvent`

### BN_FRIEND_LIST_SIZE_CHANGED

```lua
BN_FRIEND_LIST_SIZE_CHANGED(accountID: number?)
```

`SynchronousEvent`

### BN_INFO_CHANGED

```lua
BN_INFO_CHANGED()
```

`SynchronousEvent`

### BN_REQUEST_FOF_SUCCEEDED

```lua
BN_REQUEST_FOF_SUCCEEDED()
```

`SynchronousEvent`

### CONFIRM_BATTLE_NET_FRIEND_INVITE_SHOW

```lua
CONFIRM_BATTLE_NET_FRIEND_INVITE_SHOW(name: cstring, friendLevel: BattleNetFriendLevel)
```

`SynchronousEvent`

### FRIENDLIST_UPDATE

```lua
FRIENDLIST_UPDATE()
```

`SynchronousEvent`

### IGNORELIST_UPDATE

```lua
IGNORELIST_UPDATE()
```

`SynchronousEvent`

### LEGACY_FRIEND_SYSTEM_STATUS_UPDATED

```lua
LEGACY_FRIEND_SYSTEM_STATUS_UPDATED()
```

`SynchronousEvent`

### MUTELIST_UPDATE

```lua
MUTELIST_UPDATE()
```

`SynchronousEvent`

### NEW_MATCHMAKING_PARTY_INVITE

```lua
NEW_MATCHMAKING_PARTY_INVITE()
```

`SynchronousEvent`

### REJECTED_MATCHMAKING_PARTY_INVITE

```lua
REJECTED_MATCHMAKING_PARTY_INVITE(name: cstring)
```

`SynchronousEvent`

### SOCIAL_UI_FRIENDS_LIST_SYSTEM_STATUS_UPDATED

```lua
SOCIAL_UI_FRIENDS_LIST_SYSTEM_STATUS_UPDATED()
```

`SynchronousEvent`

### WHO_LIST_UPDATE

```lua
WHO_LIST_UPDATE()
```

`SynchronousEvent`

## Types

### FriendInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `connected` | `bool` |  |
| `name` | `string` |  |
| `className` | `string?` |  |
| `area` | `string?` |  |
| `notes` | `string?` |  |
| `guid` | `WOWGUID` |  |
| `level` | `number` |  |
| `dnd` | `bool` |  |
| `afk` | `bool` |  |
| `rafLinkType` | `RafLinkType` |  |

### SendWhoFilters

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `classIDs` | `number[]` |  |
| `raceIDs` | `number[]` |  |
| `uiMapIDs` | `number[]` |  |

### WhoFilter

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `ID` | `number` |  |

### WhoInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `fullName` | `string` |  |
| `fullGuildName` | `string` |  |
| `level` | `number` |  |
| `raceStr` | `string` |  |
| `classStr` | `string` |  |
| `area` | `string` |  |
| `filename` | `string?` |  |
| `gender` | `number` |  |
| `timerunningSeasonID` | `number?` |  |

## Predicates

Conditions referenced by the flags above.

- `RequiresFriendList` *Precondition* (failure mode: ReturnNothing)
