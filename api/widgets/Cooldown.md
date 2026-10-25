# Cooldown

Widget methods (`FrameAPICooldown`) · inherits [`Frame`](Frame.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/frameapicooldowndocumentation.lua` (FileDataID 5154513)

## Methods

### Clear

```lua
Cooldown:Clear()
```

`IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### GetCooldownDisplayDuration

```lua
Cooldown:GetCooldownDisplayDuration() -> duration: number
```

The returned duration unit is milliseconds, unaffected by modRate.

`SecretReturnsForAspect={ Enum.SecretAspect.Cooldown }`

### GetCooldownDuration

```lua
Cooldown:GetCooldownDuration() -> duration: number
```

The returned duration unit is milliseconds and is multiplied by the modRate.

`SecretReturnsForAspect={ Enum.SecretAspect.Cooldown }`

### GetCooldownTimes

```lua
Cooldown:GetCooldownTimes() -> start: number, duration: number
```

`SecretReturnsForAspect={ Enum.SecretAspect.Cooldown }`

### GetCountdownAbbrevThreshold

```lua
Cooldown:GetCountdownAbbrevThreshold() -> seconds: Seconds
```

Returns the threshold below which cooldown numbers are displayed as an abbreviated form without a unit suffix (eg. '1:31').

### GetCountdownFontString

```lua
Cooldown:GetCountdownFontString() -> countdownString: SimpleFontString
```

### GetCountdownFormatter

```lua
Cooldown:GetCountdownFormatter() -> formatter: NumericFormatter?
```

### GetCountdownMillisecondsThreshold

```lua
Cooldown:GetCountdownMillisecondsThreshold() -> seconds: Seconds
```

Returns the threshold below which cooldown numbers are displayed as a decimal value with one place for milliseconds (eg. '8.7').

### GetDrawBling

```lua
Cooldown:GetDrawBling() -> drawBling: bool
```

`SecretReturnsForAspect={ Enum.SecretAspect.CooldownStyle }`

### GetDrawEdge

```lua
Cooldown:GetDrawEdge() -> drawEdge: bool
```

`SecretReturnsForAspect={ Enum.SecretAspect.CooldownStyle }`

### GetDrawSwipe

```lua
Cooldown:GetDrawSwipe() -> drawSwipe: bool
```

`SecretReturnsForAspect={ Enum.SecretAspect.CooldownStyle }`

### GetEdgeScale

```lua
Cooldown:GetEdgeScale() -> edgeScale: number
```

### GetHideCountdownNumbers

```lua
Cooldown:GetHideCountdownNumbers() -> hideNumbers: bool
```

### GetMinimumCountdownDuration

```lua
Cooldown:GetMinimumCountdownDuration() -> milliseconds: Milliseconds
```

### GetReverse

```lua
Cooldown:GetReverse() -> reverse: bool
```

### GetRotation

```lua
Cooldown:GetRotation() -> rotationRadians: number
```

### GetUseAuraDisplayTime

```lua
Cooldown:GetUseAuraDisplayTime() -> useAuraDisplayTime: bool
```

### IsPaused

```lua
Cooldown:IsPaused() -> isPaused: bool
```

### Pause

```lua
Cooldown:Pause()
```

### Resume

```lua
Cooldown:Resume()
```

### SetBlingTexture

```lua
Cooldown:SetBlingTexture(texture: FileAsset, colorR: number, colorG: number, colorB: number, colorA: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetCooldown

```lua
Cooldown:SetCooldown(start: Seconds, duration: Seconds, modRate: number)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction` `SecretArgumentsAddAspect={ Enum.SecretAspect.Cooldown }`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `start` | `Seconds` |  |
| `duration` | `Seconds` |  |
| `modRate` | `number` | default `1` |

### SetCooldownDuration

```lua
Cooldown:SetCooldownDuration(duration: Seconds, modRate: number)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction` `SecretArgumentsAddAspect={ Enum.SecretAspect.Cooldown }`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `duration` | `Seconds` |  |
| `modRate` | `number` | default `1` |

### SetCooldownFromDurationObject

```lua
Cooldown:SetCooldownFromDurationObject(duration: LuaDurationObject, clearIfZero: bool)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `duration` | `LuaDurationObject` |  |
| `clearIfZero` | `bool` | default `true` |

### SetCooldownFromExpirationTime

```lua
Cooldown:SetCooldownFromExpirationTime(expirationTime: Seconds, duration: Seconds, modRate: number)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction` `SecretArgumentsAddAspect={ Enum.SecretAspect.Cooldown }`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `expirationTime` | `Seconds` |  |
| `duration` | `Seconds` |  |
| `modRate` | `number` | default `1` |

### SetCooldownUNIX

```lua
Cooldown:SetCooldownUNIX(start: number, duration: number, modRate: number)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction` `SecretArgumentsAddAspect={ Enum.SecretAspect.Cooldown }`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `start` | `number` |  |
| `duration` | `number` |  |
| `modRate` | `number` | default `1` |

### SetCountdownAbbrevThreshold

```lua
Cooldown:SetCountdownAbbrevThreshold(seconds: Seconds)
```

Sets the threshold below which cooldown numbers are displayed as an abbreviated form without a unit suffix (eg. '1:31').

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `seconds` | `Seconds` | Number of seconds below which numbers will be abbreviated. If above one hour or below one minute, no abbreviation will be performed. |

### SetCountdownFont

```lua
Cooldown:SetCountdownFont(fontName: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### SetCountdownFormatter

```lua
Cooldown:SetCountdownFormatter(formatter: NumericFormatter?)
```

`SecretArguments=AllowedWhenUntainted`

### SetCountdownMillisecondsThreshold

```lua
Cooldown:SetCountdownMillisecondsThreshold(seconds: Seconds)
```

Sets the threshold below which cooldown numbers are displayed as a decimal value with one place for milliseconds (eg. '8.7').

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `seconds` | `Seconds` | Number of seconds below which numbers are displayed with milliseconds. |

### SetDrawBling

```lua
Cooldown:SetDrawBling(drawBling: bool)
```

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.CooldownStyle }`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `drawBling` | `bool` | default `false` |

### SetDrawEdge

```lua
Cooldown:SetDrawEdge(drawEdge: bool)
```

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.CooldownStyle }`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `drawEdge` | `bool` | default `false` |

### SetDrawSwipe

```lua
Cooldown:SetDrawSwipe(drawSwipe: bool)
```

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.CooldownStyle }`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `drawSwipe` | `bool` | default `false` |

### SetEdgeColor

```lua
Cooldown:SetEdgeColor(colorR: number, colorG: number, colorB: number, a: SingleColorValue?)
```

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.CooldownStyle }`

### SetEdgeScale

```lua
Cooldown:SetEdgeScale(scale: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetEdgeTexture

```lua
Cooldown:SetEdgeTexture(texture: FileAsset, colorR: number, colorG: number, colorB: number, colorA: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetHideCountdownNumbers

```lua
Cooldown:SetHideCountdownNumbers(hideNumbers: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `hideNumbers` | `bool` | default `false` |

### SetMinimumCountdownDuration

```lua
Cooldown:SetMinimumCountdownDuration(milliseconds: Milliseconds)
```

Controls the minimum duration above which countdown text will be shown. This is applied based upon the total duration of the cooldown, not the remaining duration as it ticks down.

`SecretArguments=AllowedWhenUntainted`

### SetPaused

```lua
Cooldown:SetPaused(paused: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetReverse

```lua
Cooldown:SetReverse(reverse: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `reverse` | `bool` | default `false` |

### SetRotation

```lua
Cooldown:SetRotation(rotationRadians: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetSwipeColor

```lua
Cooldown:SetSwipeColor(colorR: number, colorG: number, colorB: number, a: SingleColorValue?)
```

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.CooldownStyle }`

### SetSwipeTexture

```lua
Cooldown:SetSwipeTexture(texture: FileAsset?, colorR: number, colorG: number, colorB: number, colorA: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetTexCoordRange

```lua
Cooldown:SetTexCoordRange(low: vector2, high: vector2)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `low` | `vector2` | `Mixin=Vector2DMixin` |
| `high` | `vector2` | `Mixin=Vector2DMixin` |

### SetUseAuraDisplayTime

```lua
Cooldown:SetUseAuraDisplayTime(useAuraDisplayTime: bool)
```

Aura durations are displayed slightly differently than cooldown durations. Setting this to true will adjust the display logic to stay in sync with aura timers.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `useAuraDisplayTime` | `bool` | default `false` |

### SetUseCircularEdge

```lua
Cooldown:SetUseCircularEdge(useCircularEdge: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `useCircularEdge` | `bool` | default `false` |
