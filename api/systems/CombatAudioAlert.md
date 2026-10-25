# CombatAudioAlert

Namespace `C_CombatAudioAlert` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/combataudioalertdocumentation.lua` (FileDataID 7543874)

## Functions

### AddToKnownTargetingList

```lua
C_CombatAudioAlert.AddToKnownTargetingList(unit: UnitToken) -> added: bool
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

Returns:

| Name | Type | Notes |
|---|---|---|
| `added` | `bool` | `SecretValue` |

### GetCategoryVoice

```lua
C_CombatAudioAlert.GetCategoryVoice(category: CombatAudioAlertCategory) -> voice: number
```

`SecretArguments=AllowedWhenUntainted`

### GetCategoryVolume

```lua
C_CombatAudioAlert.GetCategoryVolume(category: CombatAudioAlertCategory) -> volume: number
```

`SecretArguments=AllowedWhenUntainted`

### GetFormatSetting

```lua
C_CombatAudioAlert.GetFormatSetting(unit: CombatAudioAlertUnit, alertType: CombatAudioAlertType) -> formatVal: number
```

`SecretArguments=AllowedWhenUntainted`

### GetSpeakerSpeed

```lua
C_CombatAudioAlert.GetSpeakerSpeed() -> speed: number
```

### GetSpecSetting

```lua
C_CombatAudioAlert.GetSpecSetting(setting: CombatAudioAlertSpecSetting) -> value: number
```

`SecretArguments=AllowedWhenUntainted`

### GetThrottle

```lua
C_CombatAudioAlert.GetThrottle(throttleType: CombatAudioAlertThrottle) -> throttle: number
```

`SecretArguments=AllowedWhenUntainted`

### IsEnabled

```lua
C_CombatAudioAlert.IsEnabled() -> isEnabled: bool
```

### RemoveFromKnownTargetingList

```lua
C_CombatAudioAlert.RemoveFromKnownTargetingList(unit: UnitToken) -> removed: bool
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

Returns:

| Name | Type | Notes |
|---|---|---|
| `removed` | `bool` | `SecretValue` |

### SetCategoryVoice

```lua
C_CombatAudioAlert.SetCategoryVoice(category: CombatAudioAlertCategory, newVal: number) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetCategoryVolume

```lua
C_CombatAudioAlert.SetCategoryVolume(category: CombatAudioAlertCategory, newVal: number) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetFormatSetting

```lua
C_CombatAudioAlert.SetFormatSetting(unit: CombatAudioAlertUnit, alertType: CombatAudioAlertType, newVal: number) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetSpeakerSpeed

```lua
C_CombatAudioAlert.SetSpeakerSpeed(newVal: number) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetSpecSetting

```lua
C_CombatAudioAlert.SetSpecSetting(setting: CombatAudioAlertSpecSetting, newVal: number) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetThrottle

```lua
C_CombatAudioAlert.SetThrottle(throttleType: CombatAudioAlertThrottle, newVal: number) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### SpeakText

```lua
C_CombatAudioAlert.SpeakText(text: string, category: CombatAudioAlertCategory, allowOverlap: bool) -> utteranceID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `text` | `string` |  |
| `category` | `CombatAudioAlertCategory` |  |
| `allowOverlap` | `bool` | default `true` |
