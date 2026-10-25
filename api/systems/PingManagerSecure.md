# PingManagerSecure

Namespace `C_PingSecure` · environment SecureOnly · source `interface/addons/blizzard_apidocumentationgenerated/pingmanagersecuredocumentation.lua` (FileDataID 5369225)

## Functions

### ClearHitTestPingInfo

```lua
C_PingSecure.ClearHitTestPingInfo()
```

`HasRestrictions`

### CreateFrame

```lua
C_PingSecure.CreateFrame()
```

`HasRestrictions`

### DisplayError

```lua
C_PingSecure.DisplayError(error: cstring)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### GetTargetPingReceiver

```lua
C_PingSecure.GetTargetPingReceiver(mousePosX: number, mousePosY: number) -> frame: ScriptRegion
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SendHitTestPing

```lua
C_PingSecure.SendHitTestPing(type: PingSubjectType?) -> result: SendPingResult
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SendPlayerItemPing

```lua
C_PingSecure.SendPlayerItemPing(itemID: number) -> result: SendPingResult
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SendPlayerSpellCategoryPing

```lua
C_PingSecure.SendPlayerSpellCategoryPing(spellCategoryID: number) -> result: SendPingResult
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SendPlayerSpellPing

```lua
C_PingSecure.SendPlayerSpellPing(spellID: number) -> result: SendPingResult
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SendUnitPing

```lua
C_PingSecure.SendUnitPing(target: WOWGUID, type: PingSubjectType?, isPlayerResource: bool?) -> result: SendPingResult
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `target` | `WOWGUID` |  |
| `type` | `PingSubjectType?` |  |
| `isPlayerResource` | `bool?` | Player unit frame contextual pings have the optional ability to call out the player's health and in some cases mana. This field does nothing for non player pings. |

### SetHitTestPingTarget

```lua
C_PingSecure.SetHitTestPingTarget(mousePosX: number, mousePosY: number, forcePointPing: bool?) -> state: PingSetTargetState
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetHitTestTargetAndSendPing

```lua
C_PingSecure.SetHitTestTargetAndSendPing() -> result: SendPingResult
```

`HasRestrictions`

### SetPendingPingOffScreenCallback

```lua
C_PingSecure.SetPendingPingOffScreenCallback(cb: PendingPingOffScreenCallback)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetPingCooldownStartedCallback

```lua
C_PingSecure.SetPingCooldownStartedCallback(cb: PingCooldownStartedCallback)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetPingPinFrameAddedCallback

```lua
C_PingSecure.SetPingPinFrameAddedCallback(cb: PingPinFrameAddedCallback)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetPingPinFrameRemovedCallback

```lua
C_PingSecure.SetPingPinFrameRemovedCallback(cb: PingPinFrameRemovedCallback)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetPingPinFrameScreenClampStateUpdatedCallback

```lua
C_PingSecure.SetPingPinFrameScreenClampStateUpdatedCallback(cb: PingPinFrameScreenClampStateUpdatedCallback)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetPingRadialWheelCreatedCallback

```lua
C_PingSecure.SetPingRadialWheelCreatedCallback(cb: PingRadialWheelCreatedCallback)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetSendMacroPingCallback

```lua
C_PingSecure.SetSendMacroPingCallback(cb: SendMacroPingCallback)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetTogglePingListenerCallback

```lua
C_PingSecure.SetTogglePingListenerCallback(cb: TogglePingListenerCallback)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

## Events

### UNIT_PING_PIN_ADDED

```lua
UNIT_PING_PIN_ADDED(guid: WOWGUID, uiTextureKit: textureKit)
```

`HasRestrictions` `SynchronousEvent`

### UNIT_PING_PIN_REMOVED

```lua
UNIT_PING_PIN_REMOVED(guid: WOWGUID)
```

`HasRestrictions` `SynchronousEvent`

## Types

### PingActionCooldownUIInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `durationMs` | `number` | default `0` |
| `remainingMs` | `number` | default `0` |

### PingActionUIInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `number` | default `0` |
| `itemID` | `number` | default `0` |
| `textureFileDataID` | `number` | default `0` |
| `cooldownInfo` | `PingActionCooldownUIInfo?` |  |
| `spellCategoryID` | `number` | default `0` |

### SendPingResult

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `type` | `PingSubjectType?` |  |
| `result` | `PingResult` |  |

### PendingPingOffScreenCallback

*CallbackType*

### PingCooldownStartedCallback

*CallbackType*

Arguments:

| Name | Type | Notes |
|---|---|---|
| `info` | `PingCooldownInfo` |  |

### PingPinFrameAddedCallback

*CallbackType*

Arguments:

| Name | Type | Notes |
|---|---|---|
| `region` | `ScriptRegion` |  |
| `uiTextureKit` | `textureKit` |  |
| `isWorldPoint` | `bool` |  |
| `actionInfo` | `PingActionUIInfo?` |  |

### PingPinFrameRemovedCallback

*CallbackType*

Arguments:

| Name | Type | Notes |
|---|---|---|
| `region` | `ScriptRegion` |  |

### PingPinFrameScreenClampStateUpdatedCallback

*CallbackType*

Arguments:

| Name | Type | Notes |
|---|---|---|
| `region` | `ScriptRegion` |  |
| `state` | `bool` |  |

### PingRadialWheelCreatedCallback

*CallbackType*

Arguments:

| Name | Type | Notes |
|---|---|---|
| `region` | `ScriptRegion` |  |

### SendMacroPingCallback

*CallbackType*

Arguments:

| Name | Type | Notes |
|---|---|---|
| `macroInfo` | `PingMacroInfo` |  |

### TogglePingListenerCallback

*CallbackType*

Arguments:

| Name | Type | Notes |
|---|---|---|
| `down` | `bool` |  |
