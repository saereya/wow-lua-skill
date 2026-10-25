# TTSSettings

Namespace `C_TTSSettings` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/ttssettingsdocumentation.lua` (FileDataID 4637275)

## Functions

### GetChannelEnabled

```lua
C_TTSSettings.GetChannelEnabled(channelInfo: ChatChannelInfo) -> enabled: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetCharacterSettingsSaved

```lua
C_TTSSettings.GetCharacterSettingsSaved() -> settingsBeenSaved: bool
```

### GetChatTypeEnabled

```lua
C_TTSSettings.GetChatTypeEnabled(chatName: cstring) -> enabled: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetSetting

```lua
C_TTSSettings.GetSetting(setting: TtsBoolSetting) -> enabled: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetSpeechRate

```lua
C_TTSSettings.GetSpeechRate() -> rate: number
```

### GetSpeechVolume

```lua
C_TTSSettings.GetSpeechVolume() -> volume: number
```

### GetVoiceOptionID

```lua
C_TTSSettings.GetVoiceOptionID(voiceType: TtsVoiceType) -> voiceID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetVoiceOptionName

```lua
C_TTSSettings.GetVoiceOptionName(voiceType: TtsVoiceType) -> voiceName: cstring
```

`SecretArguments=AllowedWhenUntainted`

### MarkCharacterSettingsSaved

```lua
C_TTSSettings.MarkCharacterSettingsSaved()
```

### SetChannelEnabled

```lua
C_TTSSettings.SetChannelEnabled(channelInfo: ChatChannelInfo, newVal: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `channelInfo` | `ChatChannelInfo` |  |
| `newVal` | `bool` | default `false` |

### SetChannelKeyEnabled

```lua
C_TTSSettings.SetChannelKeyEnabled(channelKey: string, newVal: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `channelKey` | `string` |  |
| `newVal` | `bool` | default `false` |

### SetChatTypeEnabled

```lua
C_TTSSettings.SetChatTypeEnabled(chatName: cstring, newVal: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `chatName` | `cstring` |  |
| `newVal` | `bool` | default `false` |

### SetDefaultSettings

```lua
C_TTSSettings.SetDefaultSettings()
```

### SetSetting

```lua
C_TTSSettings.SetSetting(setting: TtsBoolSetting, newVal: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `setting` | `TtsBoolSetting` |  |
| `newVal` | `bool` | default `false` |

### SetSpeechRate

```lua
C_TTSSettings.SetSpeechRate(newVal: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetSpeechVolume

```lua
C_TTSSettings.SetSpeechVolume(newVal: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetVoiceOption

```lua
C_TTSSettings.SetVoiceOption(voiceType: TtsVoiceType, voiceID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetVoiceOptionName

```lua
C_TTSSettings.SetVoiceOptionName(voiceType: TtsVoiceType, voiceName: string)
```

`SecretArguments=AllowedWhenUntainted`

### ShouldOverrideMessage

```lua
C_TTSSettings.ShouldOverrideMessage(language: number, messageText: string) -> overrideMessage: bool
```

`SecretArguments=AllowedWhenUntainted`
