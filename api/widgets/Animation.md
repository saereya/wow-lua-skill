# Animation

Widget methods (`SimpleAnimAPI`) · inherits [`Object`](Object.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/simpleanimapidocumentation.lua` (FileDataID 4637203)

## Methods

### GetDuration

```lua
Animation:GetDuration() -> durationSec: number
```

### GetElapsed

```lua
Animation:GetElapsed() -> elapsedSec: number
```

### GetEndDelay

```lua
Animation:GetEndDelay() -> delaySec: number
```

### GetOrder

```lua
Animation:GetOrder() -> order: number
```

### GetProgress

```lua
Animation:GetProgress() -> progress: number
```

### GetRegionParent

```lua
Animation:GetRegionParent() -> region: CScriptObject
```

### GetScript

```lua
Animation:GetScript(scriptTypeName: ScriptTypeName, bindingType: ScriptBindingType) -> script: LuaFunctionReference
```

`SecretArguments=AllowedWhenUntainted` `RequiresSupportedScript` `ConstSecretAccessor`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `scriptTypeName` | `ScriptTypeName` |  |
| `bindingType` | `ScriptBindingType` | default `"Extrinsic"` |

### GetSmoothing

```lua
Animation:GetSmoothing() -> weights: SmoothingType
```

### GetSmoothProgress

```lua
Animation:GetSmoothProgress() -> progress: number
```

### GetStartDelay

```lua
Animation:GetStartDelay() -> delaySec: number
```

### GetTarget

```lua
Animation:GetTarget() -> target: CScriptObject
```

### HasScript

```lua
Animation:HasScript(scriptName: cstring) -> hasScript: bool
```

`SecretArguments=AllowedWhenUntainted` `SecretReturnsForAspect={ Enum.SecretAspect.ObjectType }` `ConstSecretAccessor`

### HookScript

```lua
Animation:HookScript(scriptTypeName: ScriptTypeName, script: LuaFunctionReference, bindingType: ScriptBindingType) -> success: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresAssignableScript`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `scriptTypeName` | `ScriptTypeName` |  |
| `script` | `LuaFunctionReference` |  |
| `bindingType` | `ScriptBindingType` | default `"Extrinsic"` |

### IsDelaying

```lua
Animation:IsDelaying() -> isDelaying: bool
```

### IsDone

```lua
Animation:IsDone() -> isDone: bool
```

### IsPaused

```lua
Animation:IsPaused() -> isPaused: bool
```

### IsPlaying

```lua
Animation:IsPlaying() -> isPlaying: bool
```

### IsStopped

```lua
Animation:IsStopped() -> isStopped: bool
```

### Pause

```lua
Animation:Pause()
```

### Play

```lua
Animation:Play()
```

### Restart

```lua
Animation:Restart()
```

### SetChildKey

```lua
Animation:SetChildKey(childKey: cstring) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetDuration

```lua
Animation:SetDuration(durationSec: number, recomputeGroupDuration: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `durationSec` | `number` |  |
| `recomputeGroupDuration` | `bool` | default `true` |

### SetEndDelay

```lua
Animation:SetEndDelay(delaySec: number, recomputeGroupDuration: bool)
```

`SecretArguments=NotAllowed`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `delaySec` | `number` |  |
| `recomputeGroupDuration` | `bool` | default `true` |

### SetOrder

```lua
Animation:SetOrder(newOrder: number)
```

`SecretArguments=NotAllowed`

### SetParent

```lua
Animation:SetParent(parent: SimpleAnimGroup, order: number?)
```

`SecretArguments=AllowedWhenUntainted` `CheckAllowChangeParent`

### SetPlaying

```lua
Animation:SetPlaying(play: bool)
```

`SecretArguments=NotAllowed`

### SetScript

```lua
Animation:SetScript(scriptTypeName: ScriptTypeName, script: LuaFunctionReference?)
```

`SecretArguments=AllowedWhenUntainted` `RequiresAssignableScript`

### SetSmoothing

```lua
Animation:SetSmoothing(weights: SmoothingType)
```

`SecretArguments=AllowedWhenUntainted`

### SetSmoothProgress

```lua
Animation:SetSmoothProgress(durationSec: number)
```

`SecretArguments=NotAllowed`

### SetStartDelay

```lua
Animation:SetStartDelay(delaySec: number, recomputeGroupDuration: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `delaySec` | `number` |  |
| `recomputeGroupDuration` | `bool` | default `true` |

### SetTarget

```lua
Animation:SetTarget(target: CScriptObject) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetTargetKey

```lua
Animation:SetTargetKey(key: cstring) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetTargetName

```lua
Animation:SetTargetName(name: cstring) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetTargetParent

```lua
Animation:SetTargetParent() -> success: bool
```

### Stop

```lua
Animation:Stop()
```
