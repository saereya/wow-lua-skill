# AnimationGroup

Widget methods (`SimpleAnimGroupAPI`) · inherits [`Object`](Object.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/simpleanimgroupapidocumentation.lua` (FileDataID 4637198)

## Methods

### CreateAnimation

```lua
AnimationGroup:CreateAnimation(animationType: cstring?, name: cstring?, templateName: cstring?) -> anim: SimpleAnim
```

`SecretArguments=NotAllowed`

### Finish

```lua
AnimationGroup:Finish()
```

### GetAnimations

```lua
AnimationGroup:GetAnimations() -> anims: SimpleAnim
```

Returns:

| Name | Type | Notes |
|---|---|---|
| `anims` | `SimpleAnim` | `StrideIndex=1` |

### GetAnimationSpeedMultiplier

```lua
AnimationGroup:GetAnimationSpeedMultiplier() -> animationSpeedMultiplier: number
```

### GetDuration

```lua
AnimationGroup:GetDuration() -> durationSec: number
```

### GetElapsed

```lua
AnimationGroup:GetElapsed() -> elapsedSec: number
```

### GetLooping

```lua
AnimationGroup:GetLooping() -> loopType: LoopType
```

### GetLoopState

```lua
AnimationGroup:GetLoopState() -> loopState: cstring
```

### GetProgress

```lua
AnimationGroup:GetProgress() -> progress: number
```

### GetScript

```lua
AnimationGroup:GetScript(scriptTypeName: ScriptTypeName, bindingType: ScriptBindingType) -> script: LuaFunctionReference
```

`SecretArguments=AllowedWhenUntainted` `RequiresSupportedScript` `ConstSecretAccessor`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `scriptTypeName` | `ScriptTypeName` |  |
| `bindingType` | `ScriptBindingType` | default `"Extrinsic"` |

### HasScript

```lua
AnimationGroup:HasScript(scriptName: cstring) -> hasScript: bool
```

`SecretArguments=AllowedWhenUntainted` `SecretReturnsForAspect={ Enum.SecretAspect.ObjectType }` `ConstSecretAccessor`

### HookScript

```lua
AnimationGroup:HookScript(scriptTypeName: ScriptTypeName, script: LuaFunctionReference, bindingType: ScriptBindingType) -> success: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresAssignableScript`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `scriptTypeName` | `ScriptTypeName` |  |
| `script` | `LuaFunctionReference` |  |
| `bindingType` | `ScriptBindingType` | default `"Extrinsic"` |

### IsDone

```lua
AnimationGroup:IsDone() -> isDone: bool
```

### IsPaused

```lua
AnimationGroup:IsPaused() -> isPaused: bool
```

### IsPendingFinish

```lua
AnimationGroup:IsPendingFinish() -> isPendingFinish: bool
```

### IsPlaying

```lua
AnimationGroup:IsPlaying() -> isPlaying: bool
```

### IsReverse

```lua
AnimationGroup:IsReverse() -> isReverse: bool
```

### IsSetToFinalAlpha

```lua
AnimationGroup:IsSetToFinalAlpha() -> isSetToFinalAlpha: bool
```

### Pause

```lua
AnimationGroup:Pause()
```

### Play

```lua
AnimationGroup:Play(reverse: bool, offset: number)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `reverse` | `bool` | default `false` |
| `offset` | `number` | default `0` |

### RemoveAnimations

```lua
AnimationGroup:RemoveAnimations()
```

### Restart

```lua
AnimationGroup:Restart(reverse: bool, offset: number)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `reverse` | `bool` | default `false` |
| `offset` | `number` | default `0` |

### SetAnimationSpeedMultiplier

```lua
AnimationGroup:SetAnimationSpeedMultiplier(animationSpeedMultiplier: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetLooping

```lua
AnimationGroup:SetLooping(loopType: LoopType)
```

`SecretArguments=NotAllowed`

### SetPlaying

```lua
AnimationGroup:SetPlaying(play: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetScript

```lua
AnimationGroup:SetScript(scriptTypeName: ScriptTypeName, script: LuaFunctionReference?)
```

`SecretArguments=AllowedWhenUntainted` `RequiresAssignableScript`

### SetToFinalAlpha

```lua
AnimationGroup:SetToFinalAlpha(setToFinalAlpha: bool)
```

`SecretArguments=AllowedWhenUntainted`

### Stop

```lua
AnimationGroup:Stop()
```
