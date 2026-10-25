# EncounterWarnings

Namespace `C_EncounterWarnings` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/encounterwarningsdocumentation.lua` (FileDataID 7489753)

## Functions

### GetColorForSeverity

```lua
C_EncounterWarnings.GetColorForSeverity(severity: EncounterEventSeverity) -> color: colorRGBA
```

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `color` | `colorRGBA` | `Mixin=ColorMixin` |

### GetEditModeWarningInfo

```lua
C_EncounterWarnings.GetEditModeWarningInfo(severity: EncounterEventSeverity) -> warningInfo: EncounterWarningInfo
```

`SecretArguments=AllowedWhenUntainted`

### GetPlayCustomSoundsWhenHidden

```lua
C_EncounterWarnings.GetPlayCustomSoundsWhenHidden() -> play: bool
```

Returns true if custom sound alerts are allowed to play for hidden warning messages.

### GetSoundKitForSeverity

```lua
C_EncounterWarnings.GetSoundKitForSeverity(severity: EncounterEventSeverity) -> soundKitID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetWarningsShown

```lua
C_EncounterWarnings.GetWarningsShown() -> shown: bool
```

Returns true if text messages for encounter events are allowed to be shown.

### IsFeatureAvailable

```lua
C_EncounterWarnings.IsFeatureAvailable() -> isAvailable: bool
```

### IsFeatureEnabled

```lua
C_EncounterWarnings.IsFeatureEnabled() -> isAvailableAndEnabled: bool
```

### PlaySound

```lua
C_EncounterWarnings.PlaySound(severity: EncounterEventSeverity) -> soundHandle: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### SetPlayCustomSoundsWhenHidden

```lua
C_EncounterWarnings.SetPlayCustomSoundsWhenHidden(play: bool)
```

Controls whether custom sound alerts for encounter events are allowed to play for warning messages that are hidden.

`SecretArguments=NotAllowed`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `play` | `bool` | If true, allow playing custom sound alerts. Note that sound alerts will not be played if the encounter warnings feature has been disabled. |

### SetWarningsShown

```lua
C_EncounterWarnings.SetWarningsShown(shown: bool)
```

Controls whether text messages for encounter events are allowed to be shown.

`SecretArguments=NotAllowed`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `shown` | `bool` | If false, hides all warning messages in the default UI. |

## Events

### ENCOUNTER_WARNING

```lua
ENCOUNTER_WARNING(encounterWarningInfo: EncounterWarningInfo)
```

`SynchronousEvent`

## Types

### EncounterWarningInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` | `SecretValue` |
| `casterGUID` | `WOWGUID` | `SecretValue` |
| `casterName` | `cstring` | `SecretValue` |
| `targetGUID` | `WOWGUID` | `SecretValue` |
| `targetName` | `cstring` | `SecretValue` |
| `iconFileID` | `number` | `SecretValue` |
| `tooltipSpellID` | `number` | `SecretValue` |
| `isDeadly` | `bool` | `SecretValue` |
| `color` | `colorRGBA` | `Mixin=ColorMixin`; `SecretValue` |
| `duration` | `Seconds` |  |
| `severity` | `EncounterEventSeverity` |  |
| `shouldPlaySound` | `bool` |  |
| `shouldShowChatMessage` | `bool` |  |
| `shouldShowWarning` | `bool` |  |
