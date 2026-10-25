# ChatInfo

Namespace `C_ChatInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/chatinfodocumentation.lua` (FileDataID 4637043)

## Functions

### AreOutgoingAddonChatMessagesRestricted

```lua
C_ChatInfo.AreOutgoingAddonChatMessagesRestricted() -> isRestricted: bool
```

Returns false if addons are allowed to send outgoing chat messages. This is controlled on a realm-by-realm basis (tournament realms allow it), and the ability for addons to receive comms is controlled separately.

### CancelEmote

```lua
C_ChatInfo.CancelEmote()
```

### CanPlayerSpeakLanguage

```lua
C_ChatInfo.CanPlayerSpeakLanguage(languageId: number) -> canSpeakLanguage: bool
```

`SecretArguments=AllowedWhenUntainted`

### DropCautionaryChatMessage

```lua
C_ChatInfo.DropCautionaryChatMessage(confirmNumber: number)
```

`SecretArguments=AllowedWhenUntainted`

### GetChannelInfoFromIdentifier

```lua
C_ChatInfo.GetChannelInfoFromIdentifier(channelIdentifier: cstring) -> info: ChatChannelInfo?
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetChannelRosterInfo

```lua
C_ChatInfo.GetChannelRosterInfo(channelIndex: luaIndex, rosterIndex: luaIndex) -> name: string, owner: bool, moderator: bool, guid: WOWGUID
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetChannelRuleset

```lua
C_ChatInfo.GetChannelRuleset(channelIndex: luaIndex) -> ruleset: ChatChannelRuleset
```

`SecretArguments=AllowedWhenUntainted`

### GetChannelRulesetForChannelID

```lua
C_ChatInfo.GetChannelRulesetForChannelID(channelID: number) -> ruleset: ChatChannelRuleset
```

`SecretArguments=AllowedWhenUntainted`

### GetChannelShortcut

```lua
C_ChatInfo.GetChannelShortcut(channelIndex: luaIndex) -> shortcut: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetChannelShortcutForChannelID

```lua
C_ChatInfo.GetChannelShortcutForChannelID(channelID: number) -> shortcut: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetChatLineSenderGUID

```lua
C_ChatInfo.GetChatLineSenderGUID(chatLine: number) -> guid: WOWGUID
```

`SecretArguments=AllowedWhenUntainted` `SecretInChatMessagingLockdown`

### GetChatLineSenderName

```lua
C_ChatInfo.GetChatLineSenderName(chatLine: number) -> name: string
```

`SecretArguments=AllowedWhenUntainted` `SecretInChatMessagingLockdown`

### GetChatLineText

```lua
C_ChatInfo.GetChatLineText(chatLine: number) -> text: string
```

`SecretArguments=AllowedWhenUntainted` `SecretInChatMessagingLockdown`

### GetChatTypeName

```lua
C_ChatInfo.GetChatTypeName(typeID: number) -> name: string?
```

`SecretArguments=AllowedWhenUntainted`

### GetClubStreamIDs

```lua
C_ChatInfo.GetClubStreamIDs(clubID: ClubId) -> ids: ClubStreamId[]
```

`SecretArguments=AllowedWhenUntainted`

### GetColorForChatType

```lua
C_ChatInfo.GetColorForChatType(chatType: cstring) -> color: colorRGB?
```

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `color` | `colorRGB?` | `Mixin=ColorMixin` |

### GetGeneralChannelID

```lua
C_ChatInfo.GetGeneralChannelID() -> channelID: number
```

### GetGeneralChannelLocalID

```lua
C_ChatInfo.GetGeneralChannelLocalID() -> localID: number?
```

### GetMentorChannelID

```lua
C_ChatInfo.GetMentorChannelID() -> channelID: number
```

### GetNumActiveChannels

```lua
C_ChatInfo.GetNumActiveChannels() -> numChannels: number
```

### GetNumReservedChatWindows

```lua
C_ChatInfo.GetNumReservedChatWindows() -> numReserved: number
```

### GetRegisteredAddonMessagePrefixes

```lua
C_ChatInfo.GetRegisteredAddonMessagePrefixes() -> registeredPrefixes: cstring[]
```

### InChatMessagingLockdown

```lua
C_ChatInfo.InChatMessagingLockdown() -> isRestricted: bool
```

Returns true if API security restrictions regarding chat messaging are in effect.

### IsAddonMessagePrefixRegistered

```lua
C_ChatInfo.IsAddonMessagePrefixRegistered(prefix: cstring) -> isRegistered: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsChannelRegional

```lua
C_ChatInfo.IsChannelRegional(channelIndex: luaIndex) -> isRegional: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsChannelRegionalForChannelID

```lua
C_ChatInfo.IsChannelRegionalForChannelID(channelID: number) -> isRegional: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsChatLineCensored

```lua
C_ChatInfo.IsChatLineCensored(chatLine: number) -> isCensored: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsLoggingChat

```lua
C_ChatInfo.IsLoggingChat() -> enabled: bool
```

### IsLoggingCombat

```lua
C_ChatInfo.IsLoggingCombat() -> enabled: bool, advanced: bool
```

### IsPartyChannelType

```lua
C_ChatInfo.IsPartyChannelType(channelType: ChatChannelType) -> isPartyChannelType: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsRegionalServiceAvailable

```lua
C_ChatInfo.IsRegionalServiceAvailable() -> available: bool
```

### IsTimerunningPlayer

```lua
C_ChatInfo.IsTimerunningPlayer(playerGUID: WOWGUID) -> isTimerunning: bool
```

`SecretArguments=AllowedWhenTainted`

### IsValidChatLine

```lua
C_ChatInfo.IsValidChatLine(chatLine: number?) -> isValid: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsValidCombatFilterName

```lua
C_ChatInfo.IsValidCombatFilterName(name: cstring) -> isApproved: bool
```

`SecretArguments=AllowedWhenUntainted`

### PerformEmote

```lua
C_ChatInfo.PerformEmote(emoteName: cstring, targetName: cstring?, suppressMoveError: bool) -> success: bool
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `emoteName` | `cstring` |  |
| `targetName` | `cstring?` |  |
| `suppressMoveError` | `bool` | default `false` |

### RegisterAddonMessagePrefix

```lua
C_ChatInfo.RegisterAddonMessagePrefix(prefix: cstring) -> result: RegisterAddonMessagePrefixResult
```

Registers interest in addon messages with this prefix, cannot be an empty string.

`SecretArguments=AllowedWhenUntainted`

### ReplaceIconAndGroupExpressions

```lua
C_ChatInfo.ReplaceIconAndGroupExpressions(input: string, noIconReplacement: bool?, noGroupReplacement: bool?) -> output: string
```

`SecretArguments=AllowedWhenTainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `input` | `string` |  |
| `noIconReplacement` | `bool?` | `NeverSecret` |
| `noGroupReplacement` | `bool?` | `NeverSecret` |

### RequestCanLocalWhisperTarget

```lua
C_ChatInfo.RequestCanLocalWhisperTarget(whisperTarget: WOWGUID)
```

`SecretArguments=AllowedWhenUntainted`

### ResetDefaultZoneChannels

```lua
C_ChatInfo.ResetDefaultZoneChannels()
```

### SendAddonMessage

```lua
C_ChatInfo.SendAddonMessage(prefix: cstring, message: cstring, chatType: cstring?, target: cstring?) -> result: SendAddonMessageResult
```

Sends a text payload to other clients specified by chatChannel and target which are registered to listen for prefix.

`SecretArguments=NotAllowed`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `prefix` | `cstring` |  |
| `message` | `cstring` |  |
| `chatType` | `cstring?` | ChatType, defaults to SLASH_CMD_PARTY. |
| `target` | `cstring?` | Only applies for targeted channels |

### SendAddonMessageLogged

```lua
C_ChatInfo.SendAddonMessageLogged(prefix: cstring, message: cstring, chatType: cstring?, target: cstring?) -> result: SendAddonMessageResult?
```

Sends a text payload to other clients specified by chatChannel and target which are registered to listen for prefix. Intended for plain text payloads; logged and throttled.

`SecretArguments=NotAllowed`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `prefix` | `cstring` |  |
| `message` | `cstring` |  |
| `chatType` | `cstring?` | ChatType, defaults to SLASH_CMD_PARTY. |
| `target` | `cstring?` | Only applies for targeted channels |

### SendCautionaryChatMessage

```lua
C_ChatInfo.SendCautionaryChatMessage(confirmNumber: number)
```

`SecretArguments=AllowedWhenUntainted`

### SendChatMessage

```lua
C_ChatInfo.SendChatMessage(message: cstring, chatType: SendChatMessageType?, languageID: number?, target: cstring?)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RestrictedForMacroChatMessages`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `message` | `cstring` |  |
| `chatType` | `SendChatMessageType?` | Chat type string ('SAY', 'EMOTE', etc.). Defaults to 'SAY' if not specified. |
| `languageID` | `number?` | Language to send the message in. |
| `target` | `cstring?` | Name of the player to send a message to. Only applies to chat types that support targeted messages. |

### SwapChatChannelsByChannelIndex

```lua
C_ChatInfo.SwapChatChannelsByChannelIndex(firstChannelIndex: luaIndex, secondChannelIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### UncensorChatLine

```lua
C_ChatInfo.UncensorChatLine(chatLine: number)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### ALTERNATIVE_DEFAULT_LANGUAGE_CHANGED

```lua
ALTERNATIVE_DEFAULT_LANGUAGE_CHANGED()
```

`SynchronousEvent`

### BN_CHAT_MSG_ADDON

```lua
BN_CHAT_MSG_ADDON(prefix: cstring, text: cstring, channel: cstring, senderID: number)
```

`SynchronousEvent`

### CAN_LOCAL_WHISPER_TARGET_RESPONSE

```lua
CAN_LOCAL_WHISPER_TARGET_RESPONSE(whisperTarget: WOWGUID, status: ChatWhisperTargetStatus)
```

`UniqueEvent`

### CAN_PLAYER_SPEAK_LANGUAGE_CHANGED

```lua
CAN_PLAYER_SPEAK_LANGUAGE_CHANGED(languageId: number, canSpeakLanguage: bool)
```

`UniqueEvent`

### CAUTIONARY_CHANNEL_MESSAGE

```lua
CAUTIONARY_CHANNEL_MESSAGE(confirmNumber: number)
```

`SynchronousEvent`

### CAUTIONARY_CHAT_MESSAGE

```lua
CAUTIONARY_CHAT_MESSAGE(chatLineID: number, confirmNumber: number)
```

`SynchronousEvent`

### CHANNEL_COUNT_UPDATE

```lua
CHANNEL_COUNT_UPDATE(displayIndex: number, count: number)
```

`SynchronousEvent`

### CHANNEL_FLAGS_UPDATED

```lua
CHANNEL_FLAGS_UPDATED(displayIndex: number)
```

`SynchronousEvent`

### CHANNEL_INVITE_REQUEST

```lua
CHANNEL_INVITE_REQUEST(channelID: cstring, name: cstring)
```

`SynchronousEvent`

### CHANNEL_LEFT

```lua
CHANNEL_LEFT(chatChannelID: number, name: cstring)
```

`SynchronousEvent`

### CHANNEL_PASSWORD_REQUEST

```lua
CHANNEL_PASSWORD_REQUEST(channelID: cstring)
```

`SynchronousEvent`

### CHANNEL_ROSTER_UPDATE

```lua
CHANNEL_ROSTER_UPDATE(displayIndex: number, count: number)
```

`SynchronousEvent`

### CHANNEL_UI_UPDATE

```lua
CHANNEL_UI_UPDATE()
```

`SynchronousEvent`

### CHAT_COMBAT_MSG_ARENA_POINTS_GAIN

```lua
CHAT_COMBAT_MSG_ARENA_POINTS_GAIN(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_LOGGING_CHANGED

```lua
CHAT_LOGGING_CHANGED(whichLog: number, isEnabled: bool)
```

`SynchronousEvent`

### CHAT_MSG_ACHIEVEMENT

```lua
CHAT_MSG_ACHIEVEMENT(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_ADDON

```lua
CHAT_MSG_ADDON(prefix: cstring, text: cstring, channel: cstring, sender: cstring, target: cstring, zoneChannelID: number, localID: number, name: cstring, instanceID: number)
```

`SynchronousEvent`

### CHAT_MSG_ADDON_LOGGED

```lua
CHAT_MSG_ADDON_LOGGED(prefix: cstring, text: cstring, channel: cstring, sender: cstring, target: cstring, zoneChannelID: number, localID: number, name: cstring, instanceID: number)
```

`SynchronousEvent`

### CHAT_MSG_AFK

```lua
CHAT_MSG_AFK(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_BG_SYSTEM_ALLIANCE

```lua
CHAT_MSG_BG_SYSTEM_ALLIANCE(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_BG_SYSTEM_HORDE

```lua
CHAT_MSG_BG_SYSTEM_HORDE(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_BG_SYSTEM_NEUTRAL

```lua
CHAT_MSG_BG_SYSTEM_NEUTRAL(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_BN

```lua
CHAT_MSG_BN(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_BN_INLINE_TOAST_ALERT

```lua
CHAT_MSG_BN_INLINE_TOAST_ALERT(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_BN_INLINE_TOAST_BROADCAST

```lua
CHAT_MSG_BN_INLINE_TOAST_BROADCAST(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_BN_INLINE_TOAST_BROADCAST_INFORM

```lua
CHAT_MSG_BN_INLINE_TOAST_BROADCAST_INFORM(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_BN_INLINE_TOAST_CONVERSATION

```lua
CHAT_MSG_BN_INLINE_TOAST_CONVERSATION(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_BN_WHISPER

```lua
CHAT_MSG_BN_WHISPER(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_BN_WHISPER_INFORM

```lua
CHAT_MSG_BN_WHISPER_INFORM(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_BN_WHISPER_PLAYER_OFFLINE

```lua
CHAT_MSG_BN_WHISPER_PLAYER_OFFLINE(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_CHANNEL

```lua
CHAT_MSG_CHANNEL(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_CHANNEL_JOIN

```lua
CHAT_MSG_CHANNEL_JOIN(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_CHANNEL_LEAVE

```lua
CHAT_MSG_CHANNEL_LEAVE(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_CHANNEL_LEAVE_PREVENTED

```lua
CHAT_MSG_CHANNEL_LEAVE_PREVENTED(channelName: cstring)
```

`SynchronousEvent`

### CHAT_MSG_CHANNEL_LIST

```lua
CHAT_MSG_CHANNEL_LIST(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_CHANNEL_NOTICE

```lua
CHAT_MSG_CHANNEL_NOTICE(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_CHANNEL_NOTICE_USER

```lua
CHAT_MSG_CHANNEL_NOTICE_USER(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_COLLECTED_APPEARANCE

```lua
CHAT_MSG_COLLECTED_APPEARANCE(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_COMBAT_FACTION_CHANGE

```lua
CHAT_MSG_COMBAT_FACTION_CHANGE(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_COMBAT_HONOR_GAIN

```lua
CHAT_MSG_COMBAT_HONOR_GAIN(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_COMBAT_MISC_INFO

```lua
CHAT_MSG_COMBAT_MISC_INFO(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_COMBAT_XP_GAIN

```lua
CHAT_MSG_COMBAT_XP_GAIN(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_COMMUNITIES_CHANNEL

```lua
CHAT_MSG_COMMUNITIES_CHANNEL(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_CURRENCY

```lua
CHAT_MSG_CURRENCY(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_DND

```lua
CHAT_MSG_DND(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_EMOTE

```lua
CHAT_MSG_EMOTE(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_FILTERED

```lua
CHAT_MSG_FILTERED(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_GUILD

```lua
CHAT_MSG_GUILD(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_GUILD_ACHIEVEMENT

```lua
CHAT_MSG_GUILD_ACHIEVEMENT(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_GUILD_DISCORD

```lua
CHAT_MSG_GUILD_DISCORD(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_GUILD_ITEM_LOOTED

```lua
CHAT_MSG_GUILD_ITEM_LOOTED(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_IGNORED

```lua
CHAT_MSG_IGNORED(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_INSTANCE_CHAT

```lua
CHAT_MSG_INSTANCE_CHAT(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_INSTANCE_CHAT_LEADER

```lua
CHAT_MSG_INSTANCE_CHAT_LEADER(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_LOOT

```lua
CHAT_MSG_LOOT(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_MONEY

```lua
CHAT_MSG_MONEY(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_MONSTER_EMOTE

```lua
CHAT_MSG_MONSTER_EMOTE(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_MONSTER_PARTY

```lua
CHAT_MSG_MONSTER_PARTY(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_MONSTER_SAY

```lua
CHAT_MSG_MONSTER_SAY(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_MONSTER_WHISPER

```lua
CHAT_MSG_MONSTER_WHISPER(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_MONSTER_YELL

```lua
CHAT_MSG_MONSTER_YELL(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_OFFICER

```lua
CHAT_MSG_OFFICER(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_OPENING

```lua
CHAT_MSG_OPENING(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_PARTY

```lua
CHAT_MSG_PARTY(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_PARTY_LEADER

```lua
CHAT_MSG_PARTY_LEADER(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_PET_BATTLE_COMBAT_LOG

```lua
CHAT_MSG_PET_BATTLE_COMBAT_LOG(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_PET_BATTLE_INFO

```lua
CHAT_MSG_PET_BATTLE_INFO(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_PET_INFO

```lua
CHAT_MSG_PET_INFO(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_PING

```lua
CHAT_MSG_PING(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_RAID

```lua
CHAT_MSG_RAID(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_RAID_BOSS_EMOTE

```lua
CHAT_MSG_RAID_BOSS_EMOTE(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_RAID_BOSS_WHISPER

```lua
CHAT_MSG_RAID_BOSS_WHISPER(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_RAID_LEADER

```lua
CHAT_MSG_RAID_LEADER(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_RAID_WARNING

```lua
CHAT_MSG_RAID_WARNING(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_RESTRICTED

```lua
CHAT_MSG_RESTRICTED(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_SAY

```lua
CHAT_MSG_SAY(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_SKILL

```lua
CHAT_MSG_SKILL(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_SYSTEM

```lua
CHAT_MSG_SYSTEM(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_TARGETICONS

```lua
CHAT_MSG_TARGETICONS(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_TEXT_EMOTE

```lua
CHAT_MSG_TEXT_EMOTE(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_TRADESKILLS

```lua
CHAT_MSG_TRADESKILLS(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_VOICE_TEXT

```lua
CHAT_MSG_VOICE_TEXT(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_WHISPER

```lua
CHAT_MSG_WHISPER(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_WHISPER_INFORM

```lua
CHAT_MSG_WHISPER_INFORM(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_MSG_YELL

```lua
CHAT_MSG_YELL(text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### CHAT_REGIONAL_SEND_FAILED

```lua
CHAT_REGIONAL_SEND_FAILED()
```

`SynchronousEvent`

### CHAT_REGIONAL_STATUS_CHANGED

```lua
CHAT_REGIONAL_STATUS_CHANGED(isServiceAvailable: bool)
```

`SynchronousEvent`

### CHAT_SERVER_DISCONNECTED

```lua
CHAT_SERVER_DISCONNECTED(isInitialMessage: bool?)
```

`SynchronousEvent`

### CHAT_SERVER_RECONNECTED

```lua
CHAT_SERVER_RECONNECTED()
```

`SynchronousEvent`

### CLEAR_BOSS_EMOTES

```lua
CLEAR_BOSS_EMOTES()
```

`SynchronousEvent`

### DAILY_RESET_INSTANCE_WELCOME

```lua
DAILY_RESET_INSTANCE_WELCOME(mapname: cstring, timeLeft: number)
```

`SynchronousEvent`

### INSTANCE_RESET_WARNING

```lua
INSTANCE_RESET_WARNING(warningMessage: cstring, timeLeft: number)
```

`SynchronousEvent`

### LANGUAGE_LIST_CHANGED

```lua
LANGUAGE_LIST_CHANGED()
```

`SynchronousEvent`

### NOTIFY_CHAT_SUPPRESSED

```lua
NOTIFY_CHAT_SUPPRESSED()
```

`SynchronousEvent`

### QUEST_BOSS_EMOTE

```lua
QUEST_BOSS_EMOTE(text: cstring, playerName: cstring, displayTime: number, enableBossEmoteWarningSound: bool)
```

`SynchronousEvent`

### RAID_BOSS_EMOTE

```lua
RAID_BOSS_EMOTE(text: cstring, playerName: cstring, displayTime: number, enableBossEmoteWarningSound: bool)
```

`SynchronousEvent`

### RAID_BOSS_WHISPER

```lua
RAID_BOSS_WHISPER(text: cstring, playerName: cstring, displayTime: number, enableBossEmoteWarningSound: bool)
```

`SynchronousEvent`

### RAID_INSTANCE_WELCOME

```lua
RAID_INSTANCE_WELCOME(mapname: cstring, timeLeft: number, locked: number, extended: number)
```

`SynchronousEvent`

### UPDATE_CHAT_COLOR

```lua
UPDATE_CHAT_COLOR(name: cstring, r: number, g: number, b: number)
```

`SynchronousEvent`

### UPDATE_CHAT_COLOR_NAME_BY_CLASS

```lua
UPDATE_CHAT_COLOR_NAME_BY_CLASS(name: cstring, colorNameByClass: bool)
```

`SynchronousEvent`

### UPDATE_CHAT_WINDOWS

```lua
UPDATE_CHAT_WINDOWS()
```

`SynchronousEvent`

### UPDATE_FLOATING_CHAT_WINDOWS

```lua
UPDATE_FLOATING_CHAT_WINDOWS()
```

`SynchronousEvent`

## Types

### ChatMessageEventParams

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `playerName` | `cstring` |  |
| `languageName` | `cstring` | `NeverSecret` |
| `channelName` | `cstring` | `NeverSecret` |
| `playerName2` | `cstring` |  |
| `specialFlags` | `cstring` | `NeverSecret` |
| `zoneChannelID` | `number` | `NeverSecret` |
| `channelIndex` | `number` | `NeverSecret` |
| `channelBaseName` | `cstring` | `NeverSecret` |
| `languageID` | `number` | `NeverSecret` |
| `lineID` | `number` | `NeverSecret` |
| `guid` | `WOWGUID` |  |
| `bnSenderID` | `number` |  |
| `isMobile` | `bool` | `NeverSecret` |
| `isSubtitle` | `bool` | `NeverSecret` |
| `hideSenderInLetterbox` | `bool` | `NeverSecret` |
| `suppressRaidIcons` | `bool` | `NeverSecret` |
| `discordInfo` | `DiscordChatInfo` |  |

### SendChatMessageParams

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `message` | `cstring` |  |
| `chatType` | `SendChatMessageType?` | Chat type string ('SAY', 'EMOTE', etc.). Defaults to 'SAY' if not specified. |
| `languageID` | `number?` | Language to send the message in. |
| `target` | `cstring?` | Name of the player to send a message to. Only applies to chat types that support targeted messages. |
