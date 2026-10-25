# DiscordConstants

source `interface/addons/blizzard_apidocumentationgenerated/discordconstantsdocumentation.lua` (FileDataID 6850895)

## Types

### DiscordAccountType

*Enumeration* · 2 values, 0..1

Access values as `Enum.DiscordAccountType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Normal` | `DiscordAccountType` | = 0 |
| `Provisional` | `DiscordAccountType` | = 1 |

### DiscordChannelID

*Enumeration* · 1 values, 0..0

Access values as `Enum.DiscordChannelID.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `InvalidDiscordID` | `DiscordChannelID` | = 0 |

### DiscordDisplayNameType

*Enumeration* · 3 values, 0..2

Access values as `Enum.DiscordDisplayNameType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Default` | `DiscordDisplayNameType` | = 0 |
| `LastOnline` | `DiscordDisplayNameType` | = 1 |
| `GlobalName` | `DiscordDisplayNameType` | = 2 |

### DiscordGuildID

*Enumeration* · 1 values, 0..0

Access values as `Enum.DiscordGuildID.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `InvalidDiscordID` | `DiscordGuildID` | = 0 |

### DiscordGuildSettings

*Enumeration* · 1 values, 1..1

Access values as `Enum.DiscordGuildSettings.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `SeparateStream` | `DiscordGuildSettings` | = 1 |

### DiscordID

*Enumeration* · 1 values, 0..0

Access values as `Enum.DiscordID.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `InvalidDiscordID` | `DiscordID` | = 0 |

### DiscordLobbyID

*Enumeration* · 1 values, 0..0

Access values as `Enum.DiscordLobbyID.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `InvalidDiscordID` | `DiscordLobbyID` | = 0 |

### DiscordMemberID

*Enumeration* · 1 values, 0..0

Access values as `Enum.DiscordMemberID.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `InvalidDiscordID` | `DiscordMemberID` | = 0 |

### DiscordMessageID

*Enumeration* · 1 values, 0..0

Access values as `Enum.DiscordMessageID.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `InvalidDiscordID` | `DiscordMessageID` | = 0 |

### DiscordChatInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `userID` | `DiscordMemberOpaqueID` |  |
| `globalName` | `string` |  |
| `type` | `DiscordDisplayNameType` | default `"Default"` |
| `lastOnlineGUID` | `WOWGUID` |  |
| `lastOnlineName` | `string` |  |
| `hasAttachment` | `bool` |  |
| `hasPoll` | `bool` |  |
| `hasEmbed` | `bool` |  |
| `hasSticker` | `bool` |  |
| `hasEmoji` | `bool` |  |
| `hasError` | `bool` |  |
| `hasForwardedMessage` | `bool` |  |
| `forwardedMessage` | `string` |  |
| `fromDiscord` | `bool` |  |
