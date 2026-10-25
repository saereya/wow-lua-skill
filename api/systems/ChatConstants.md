# ChatConstants

source `interface/addons/blizzard_apidocumentationgenerated/chatconstantsdocumentation.lua` (FileDataID 4637042)

## Types

### ChannelPlayerFlags

*Enumeration* · 5 values, 0..8

Access values as `Enum.ChannelPlayerFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `ChannelPlayerNone` | `ChannelPlayerFlags` | = 0 |
| `ChannelPlayerOwner` | `ChannelPlayerFlags` | = 1 |
| `ChannelPlayerModerator` | `ChannelPlayerFlags` | = 2 |
| `ChannelPlayerTextAllow` | `ChannelPlayerFlags` | = 4 |
| `ChannelPlayerHidden` | `ChannelPlayerFlags` | = 8 |

### ChatChannelRuleset

*Enumeration* · 9 values, 0..8

Access values as `Enum.ChatChannelRuleset.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `ChatChannelRuleset` | = 0 |
| `Mentor` | `ChatChannelRuleset` | = 1 |
| `Disabled` | `ChatChannelRuleset` | = 2 |
| `ChromieTimeCataclysm` | `ChatChannelRuleset` | = 3 |
| `ChromieTimeBuringCrusade` | `ChatChannelRuleset` | = 4 |
| `ChromieTimeWrath` | `ChatChannelRuleset` | = 5 |
| `ChromieTimeMists` | `ChatChannelRuleset` | = 6 |
| `ChromieTimeWoD` | `ChatChannelRuleset` | = 7 |
| `ChromieTimeLegion` | `ChatChannelRuleset` | = 8 |

### ChatChannelType

*Enumeration* · 8 values, 0..7

Access values as `Enum.ChatChannelType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `ChatChannelType` | = 0 |
| `Custom` | `ChatChannelType` | = 1 |
| `PrivateParty` | `ChatChannelType` | = 2 |
| `PublicParty` | `ChatChannelType` | = 3 |
| `Communities` | `ChatChannelType` | = 4 |
| `DiscordParty` | `ChatChannelType` | = 5 |
| `DiscordGuild` | `ChatChannelType` | = 6 |
| `DiscordSolo` | `ChatChannelType` | = 7 |

### ChatToxityFilterOptOut

*Enumeration* · 4 values, 0..4294967295

Access values as `Enum.ChatToxityFilterOptOut.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `FilterAll` | `ChatToxityFilterOptOut` | = 0 |
| `ExcludeFilterFriend` | `ChatToxityFilterOptOut` | = 1 |
| `ExcludeFilterGuild` | `ChatToxityFilterOptOut` | = 2 |
| `ExcludeFilterAll` | `ChatToxityFilterOptOut` | = 4294967295 |

### ChatWhisperTargetStatus

*Enumeration* · 4 values, 0..3

Access values as `Enum.ChatWhisperTargetStatus.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `CanWhisper` | `ChatWhisperTargetStatus` | = 0 |
| `CanWhisperGuild` | `ChatWhisperTargetStatus` | = 1 |
| `Offline` | `ChatWhisperTargetStatus` | = 2 |
| `WrongFaction` | `ChatWhisperTargetStatus` | = 3 |

### ExcludedCensorSources

*Enumeration* · 10 values, 0..255

Access values as `Enum.ExcludedCensorSources.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `ExcludedCensorSources` | = 0 |
| `Friends` | `ExcludedCensorSources` | = 1 |
| `Guild` | `ExcludedCensorSources` | = 2 |
| `Reserve1` | `ExcludedCensorSources` | = 4 |
| `Reserve2` | `ExcludedCensorSources` | = 8 |
| `Reserve3` | `ExcludedCensorSources` | = 16 |
| `Reserve4` | `ExcludedCensorSources` | = 32 |
| `Reserve5` | `ExcludedCensorSources` | = 64 |
| `Reserve6` | `ExcludedCensorSources` | = 128 |
| `All` | `ExcludedCensorSources` | = 255 |

### LanguageFlag

*Enumeration* · 3 values, 1..4

Access values as `Enum.LanguageFlag.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `IsExotic` | `LanguageFlag` | = 1 |
| `HiddenFromPlayer` | `LanguageFlag` | = 2 |
| `HideLanguageNameInChat` | `LanguageFlag` | = 4 |

### PermanentChatChannelType

*Enumeration* · 4 values, 0..3

Access values as `Enum.PermanentChatChannelType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `PermanentChatChannelType` | = 0 |
| `Zone` | `PermanentChatChannelType` | = 1 |
| `Communities` | `PermanentChatChannelType` | = 2 |
| `Custom` | `PermanentChatChannelType` | = 3 |

### RegisterAddonMessagePrefixResult

*Enumeration* · 4 values, 0..3

Access values as `Enum.RegisterAddonMessagePrefixResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Success` | `RegisterAddonMessagePrefixResult` | = 0 |
| `DuplicatePrefix` | `RegisterAddonMessagePrefixResult` | = 1 |
| `InvalidPrefix` | `RegisterAddonMessagePrefixResult` | = 2 |
| `MaxPrefixes` | `RegisterAddonMessagePrefixResult` | = 3 |

### SendAddonMessageResult

*Enumeration* · 13 values, 0..12

Access values as `Enum.SendAddonMessageResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Success` | `SendAddonMessageResult` | = 0 |
| `InvalidPrefix` | `SendAddonMessageResult` | = 1 |
| `InvalidMessage` | `SendAddonMessageResult` | = 2 |
| `AddonMessageThrottle` | `SendAddonMessageResult` | = 3 |
| `InvalidChatType` | `SendAddonMessageResult` | = 4 |
| `NotInGroup` | `SendAddonMessageResult` | = 5 |
| `TargetRequired` | `SendAddonMessageResult` | = 6 |
| `InvalidChannel` | `SendAddonMessageResult` | = 7 |
| `ChannelThrottle` | `SendAddonMessageResult` | = 8 |
| `GeneralError` | `SendAddonMessageResult` | = 9 |
| `NotInGuild` | `SendAddonMessageResult` | = 10 |
| `AddOnMessageLockdown` | `SendAddonMessageResult` | = 11 |
| `TargetOffline` | `SendAddonMessageResult` | = 12 |

### TtsBoolSetting

*Enumeration* · 5 values, 0..4

Access values as `Enum.TtsBoolSetting.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `PlaySoundSeparatingChatLineBreaks` | `TtsBoolSetting` | = 0 |
| `AddCharacterNameToSpeech` | `TtsBoolSetting` | = 1 |
| `PlayActivitySoundWhenNotFocused` | `TtsBoolSetting` | = 2 |
| `AlternateSystemVoice` | `TtsBoolSetting` | = 3 |
| `NarrateMyMessages` | `TtsBoolSetting` | = 4 |

### TtsVoiceType

*Enumeration* · 2 values, 0..1

Access values as `Enum.TtsVoiceType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Standard` | `TtsVoiceType` | = 0 |
| `Alternate` | `TtsVoiceType` | = 1 |

### ChatChannelInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `shortcut` | `cstring` |  |
| `localID` | `number` |  |
| `instanceID` | `number` |  |
| `zoneChannelID` | `number` |  |
| `channelType` | `PermanentChatChannelType` |  |

### ChatFrameConstants

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `MaxChatWindows` | `number` | = `10` |
| `MaxChatChannels` | `number` | = `20` |
| `MaxCharacterNameBytes` | `number` | = `FULLNAME_MAX_CHAR` |

### TTSConstants

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `TTSRateMin` | `number` | = `-10` |
| `TTSRateMax` | `number` | = `10` |
| `TTSRateDefault` | `number` | = `0` |
| `TTSVolumeMin` | `number` | = `0` |
| `TTSVolumeMax` | `number` | = `100` |
| `TTSVolumeDefault` | `number` | = `100` |

## Predicates

Conditions referenced by the flags above.

- `RestrictedForMacroChatMessages` *Precondition*: Restricts sending chat messages on chat types that can be observed by external players. Only applies during instance encounters for messages initiated from macros.
