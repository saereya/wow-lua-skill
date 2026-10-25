# Discord

Namespace `C_Discord` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/discorddocumentation.lua` (FileDataID 6728062)

## Functions

### Authorize

```lua
C_Discord.Authorize()
```

`HasRestrictions`

### GetDiscordChannelName

```lua
C_Discord.GetDiscordChannelName(serverIndex: luaIndex, channelIndex: luaIndex) -> name: string
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### GetDiscordUserID

```lua
C_Discord.GetDiscordUserID() -> userID: DiscordMemberOpaqueID
```

`HasRestrictions`

### GetDiscordUserName

```lua
C_Discord.GetDiscordUserName(userID: DiscordMemberOpaqueID) -> userName: KStringDiscordUserName
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### GetDisplayNameType

```lua
C_Discord.GetDisplayNameType() -> type: DiscordDisplayNameType
```

`HasRestrictions`

### GetGuildLinkStatus

```lua
C_Discord.GetGuildLinkStatus() -> isFullyLinked: bool, linkedChannelName: string, linkedServerName: string
```

`HasRestrictions`

### GetNumDiscordChannels

```lua
C_Discord.GetNumDiscordChannels(serverIndex: luaIndex) -> count: number, valid: bool
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### GetNumDiscordServers

```lua
C_Discord.GetNumDiscordServers() -> count: number
```

`HasRestrictions`

### GetServerLinkableChannels

```lua
C_Discord.GetServerLinkableChannels(index: luaIndex)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### GetServerName

```lua
C_Discord.GetServerName(index: luaIndex) -> name: string
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### GuildLink

```lua
C_Discord.GuildLink(serverIndex: luaIndex, channelIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### GuildUnlink

```lua
C_Discord.GuildUnlink()
```

`HasRestrictions`

### IsEnabled

```lua
C_Discord.IsEnabled() -> enabled: bool
```

### IsGuildChannelLinked

```lua
C_Discord.IsGuildChannelLinked() -> isLinked: bool
```

`HasRestrictions`

### IsGuildSettingSet

```lua
C_Discord.IsGuildSettingSet(setting: DiscordGuildSettings) -> isSet: bool
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### IsUserOAuthed

```lua
C_Discord.IsUserOAuthed() -> hasOAuth: bool
```

`HasRestrictions`

### IsVoiceEnabled

```lua
C_Discord.IsVoiceEnabled() -> enabled: bool
```

### RefreshAuth

```lua
C_Discord.RefreshAuth()
```

`HasRestrictions`

### SetGuildSetting

```lua
C_Discord.SetGuildSetting(setting: DiscordGuildSettings, set: bool)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### UpdateDiscordServers

```lua
C_Discord.UpdateDiscordServers()
```

`HasRestrictions`

### UpdateGuildLobby

```lua
C_Discord.UpdateGuildLobby()
```

`HasRestrictions`

## Events

### DISCORD_GUILD_ACHIEVEMENT

```lua
DISCORD_GUILD_ACHIEVEMENT(achievementID: number)
```

`SynchronousEvent`

### DISCORD_GUILD_LOBBY_UPDATE

```lua
DISCORD_GUILD_LOBBY_UPDATE()
```

`SynchronousEvent`

### DISCORD_GUILD_SETTINGS_UPDATE

```lua
DISCORD_GUILD_SETTINGS_UPDATE()
```

`SynchronousEvent`

### DISCORD_LINK_UPDATE

```lua
DISCORD_LINK_UPDATE()
```

`SynchronousEvent`

### DISCORD_SERVER_LIST_UPDATE

```lua
DISCORD_SERVER_LIST_UPDATE()
```

`SynchronousEvent`

### DISCORD_STATUS_UPDATE

```lua
DISCORD_STATUS_UPDATE()
```

`SynchronousEvent`
