# GamePad

Namespace `C_GamePad` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/gamepaddocumentation.lua` (FileDataID 4637096)

## Functions

### AddSDLMapping

```lua
C_GamePad.AddSDLMapping(platform: ClientPlatformType, mapping: cstring) -> success: bool
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### ApplyConfigs

```lua
C_GamePad.ApplyConfigs()
```

`HasRestrictions`

### AxisIndexToConfigName

```lua
C_GamePad.AxisIndexToConfigName(axisIndex: number) -> configName: cstring?
```

`SecretArguments=AllowedWhenUntainted`

### ButtonBindingToIndex

```lua
C_GamePad.ButtonBindingToIndex(bindingName: cstring) -> buttonIndex: number?
```

`SecretArguments=AllowedWhenUntainted`

### ButtonIndexToBinding

```lua
C_GamePad.ButtonIndexToBinding(buttonIndex: number) -> bindingName: cstring?
```

`SecretArguments=AllowedWhenUntainted`

### ButtonIndexToConfigName

```lua
C_GamePad.ButtonIndexToConfigName(buttonIndex: number) -> configName: cstring?
```

`SecretArguments=AllowedWhenUntainted`

### ClearLedColor

```lua
C_GamePad.ClearLedColor()
```

### DeleteConfig

```lua
C_GamePad.DeleteConfig(configID: GamePadConfigID)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### GetActiveDeviceID

```lua
C_GamePad.GetActiveDeviceID() -> deviceID: number
```

### GetAllConfigIDs

```lua
C_GamePad.GetAllConfigIDs() -> configIDs: GamePadConfigID[]
```

### GetAllDeviceIDs

```lua
C_GamePad.GetAllDeviceIDs() -> deviceIDs: number[]
```

### GetAllowHoverEventsWithFreeLook

```lua
C_GamePad.GetAllowHoverEventsWithFreeLook() -> enabled: bool
```

### GetCombinedDeviceID

```lua
C_GamePad.GetCombinedDeviceID() -> deviceID: number
```

### GetConfig

```lua
C_GamePad.GetConfig(configID: GamePadConfigID) -> config: GamePadConfig?
```

`SecretArguments=AllowedWhenUntainted`

### GetDeviceMappedState

```lua
C_GamePad.GetDeviceMappedState(deviceID: number?) -> state: GamePadMappedState?
```

`SecretArguments=AllowedWhenUntainted`

### GetDeviceRawState

```lua
C_GamePad.GetDeviceRawState(deviceID: number) -> rawState: GamePadRawState?
```

`SecretArguments=AllowedWhenUntainted`

### GetLedColor

```lua
C_GamePad.GetLedColor() -> color: colorRGB
```

Returns:

| Name | Type | Notes |
|---|---|---|
| `color` | `colorRGB` | `Mixin=ColorMixin` |

### GetPowerLevel

```lua
C_GamePad.GetPowerLevel(deviceID: number?) -> powerLevel: GamePadPowerLevel
```

`SecretArguments=AllowedWhenUntainted`

### IsEnabled

```lua
C_GamePad.IsEnabled() -> enabled: bool
```

### SetAllowHoverEventsWithFreeLook

```lua
C_GamePad.SetAllowHoverEventsWithFreeLook(enable: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetConfig

```lua
C_GamePad.SetConfig(config: GamePadConfig)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetLedColor

```lua
C_GamePad.SetLedColor(color: colorRGB)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `color` | `colorRGB` | `Mixin=ColorMixin` |

### SetVibration

```lua
C_GamePad.SetVibration(vibrationType: cstring, intensity: number)
```

`SecretArguments=AllowedWhenUntainted`

### StickIndexToConfigName

```lua
C_GamePad.StickIndexToConfigName(stickIndex: number) -> configName: cstring?
```

`SecretArguments=AllowedWhenUntainted`

### StopVibration

```lua
C_GamePad.StopVibration()
```

## Events

### GAME_PAD_ACTIVE_CHANGED

```lua
GAME_PAD_ACTIVE_CHANGED(isActive: bool)
```

`SynchronousEvent`

### GAME_PAD_ALLOW_HOVER_EVENTS_WITH_FREE_LOOK_CHANGED

```lua
GAME_PAD_ALLOW_HOVER_EVENTS_WITH_FREE_LOOK_CHANGED(enabled: bool)
```

`SynchronousEvent`

### GAME_PAD_CONFIGS_CHANGED

```lua
GAME_PAD_CONFIGS_CHANGED()
```

`SynchronousEvent`

### GAME_PAD_CONNECTED

```lua
GAME_PAD_CONNECTED()
```

`SynchronousEvent`

### GAME_PAD_DISCONNECTED

```lua
GAME_PAD_DISCONNECTED()
```

`SynchronousEvent`

### GAME_PAD_POWER_CHANGED

```lua
GAME_PAD_POWER_CHANGED(powerLevel: GamePadPowerLevel)
```

`SynchronousEvent`

## Types

### GamePadAxisConfig

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `axis` | `string` |  |
| `shift` | `number?` |  |
| `scale` | `number?` |  |
| `deadzone` | `number?` |  |
| `buttonThreshold` | `number?` |  |
| `buttonPos` | `string?` |  |
| `buttonNeg` | `string?` |  |
| `comment` | `string?` |  |

### GamePadConfig

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `comment` | `string?` |  |
| `name` | `string?` |  |
| `configID` | `GamePadConfigID` |  |
| `labelStyle` | `string?` |  |
| `rawButtonMappings` | `GamePadRawButtonMapping[]` |  |
| `rawAxisMappings` | `GamePadRawAxisMapping[]` |  |
| `axisConfigs` | `GamePadAxisConfig[]` |  |
| `stickConfigs` | `GamePadStickConfig[]` |  |

### GamePadConfigID

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `vendorID` | `number?` |  |
| `productID` | `number?` |  |

### GamePadMappedState

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `labelStyle` | `string` |  |
| `buttonCount` | `number` |  |
| `axisCount` | `number` |  |
| `stickCount` | `number` |  |
| `buttons` | `bool[]` |  |
| `axes` | `number[]` |  |
| `sticks` | `GamePadStick[]` |  |

### GamePadRawAxisMapping

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `rawIndex` | `number` |  |
| `axis` | `string?` |  |
| `comment` | `string?` |  |

### GamePadRawButtonMapping

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `rawIndex` | `number` |  |
| `button` | `string?` |  |
| `axis` | `string?` |  |
| `axisValue` | `number?` |  |
| `comment` | `string?` |  |

### GamePadRawState

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `vendorID` | `number` |  |
| `productID` | `number` |  |
| `rawButtonCount` | `number` |  |
| `rawAxisCount` | `number` |  |
| `rawButtons` | `bool[]` |  |
| `rawAxes` | `number[]` |  |

### GamePadStick

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `x` | `number` |  |
| `y` | `number` |  |
| `len` | `number` |  |

### GamePadStickConfig

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `stick` | `string` |  |
| `axisX` | `string?` |  |
| `axisY` | `string?` |  |
| `deadzone` | `number?` |  |
| `deadzoneX` | `number?` |  |
| `deadzoneY` | `number?` |  |
| `comment` | `string?` |  |
