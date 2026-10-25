# Sound

Namespace `C_Sound` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/sounddocumentation.lua` (FileDataID 4637249)

## Functions

### GetSoundScaledVolume

```lua
C_Sound.GetSoundScaledVolume(soundHandle: number) -> scaledVolume: number
```

`SecretArguments=AllowedWhenUntainted`

### IsPlaying

```lua
C_Sound.IsPlaying(soundHandle: number) -> isPlaying: bool
```

`SecretArguments=AllowedWhenUntainted`

### PlayItemSound

```lua
C_Sound.PlayItemSound(soundType: ItemSoundType, itemLocation: ItemLocation)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `soundType` | `ItemSoundType` |  |
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### PlaySound

```lua
C_Sound.PlaySound(soundKitID: number, uiSoundSubType: UISoundSubType, forceNoDuplicates: bool, runFinishCallback: bool, overridePriority: number?, volumeOverride: number?) -> success: bool, soundHandle: SoundHandle
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `soundKitID` | `number` |  |
| `uiSoundSubType` | `UISoundSubType` | default `"g_defaultSI3UISoundSubTypeForLua"` |
| `forceNoDuplicates` | `bool` | default `false` |
| `runFinishCallback` | `bool` | default `false` |
| `overridePriority` | `number?` |  |
| `volumeOverride` | `number?` |  |

### PlaySoundWithOptions

```lua
C_Sound.PlaySoundWithOptions(params: PlaySoundParams) -> success: bool, soundHandle: SoundHandle
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### PlayVocalErrorSound

```lua
C_Sound.PlayVocalErrorSound(vocalErrorSoundID: Vocalerrorsounds)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### SOUND_DEVICE_UPDATE

```lua
SOUND_DEVICE_UPDATE()
```

`SynchronousEvent`

### SOUNDKIT_FINISHED

```lua
SOUNDKIT_FINISHED(soundHandle: number)
```

`SynchronousEvent`

## Types

### PlaySoundParams

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `soundKitID` | `number` |  |
| `uiSoundSubType` | `UISoundSubType` | default `"g_defaultSI3UISoundSubTypeForLua"` |
| `forceNoDuplicates` | `bool` | default `false` |
| `runFinishCallback` | `bool` | default `false` |
| `overridePriority` | `number?` |  |
| `volumeOverride` | `number?` |  |

### PlaySoundResult

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `success` | `bool` |  |
| `soundHandle` | `SoundHandle` |  |
