# ScriptedAnimations

Namespace `C_ScriptedAnimations` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/scriptedanimationsdocumentation.lua` (FileDataID 4637186)

## Functions

### GetAllScriptedAnimationEffects

```lua
C_ScriptedAnimations.GetAllScriptedAnimationEffects() -> scriptedAnimationEffects: ScriptedAnimationEffect[]
```

## Events

### SCRIPTED_ANIMATIONS_UPDATE

```lua
SCRIPTED_ANIMATIONS_UPDATE()
```

`SynchronousEvent`

## Types

### ScriptedAnimationBehavior

*Enumeration* · 6 values, 0..5

Access values as `Enum.ScriptedAnimationBehavior.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `ScriptedAnimationBehavior` | = 0 |
| `TargetShake` | `ScriptedAnimationBehavior` | = 1 |
| `TargetKnockBack` | `ScriptedAnimationBehavior` | = 2 |
| `SourceRecoil` | `ScriptedAnimationBehavior` | = 3 |
| `SourceCollideWithTarget` | `ScriptedAnimationBehavior` | = 4 |
| `UIParentShake` | `ScriptedAnimationBehavior` | = 5 |

### ScriptedAnimationFlags

*Enumeration* · 1 values, 1..1

Access values as `Enum.ScriptedAnimationFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `UseTargetAsSource` | `ScriptedAnimationFlags` | = 1 |

### ScriptedAnimationTrajectory

*Enumeration* · 7 values, 0..6

Access values as `Enum.ScriptedAnimationTrajectory.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `AtSource` | `ScriptedAnimationTrajectory` | = 0 |
| `AtTarget` | `ScriptedAnimationTrajectory` | = 1 |
| `Straight` | `ScriptedAnimationTrajectory` | = 2 |
| `CurveLeft` | `ScriptedAnimationTrajectory` | = 3 |
| `CurveRight` | `ScriptedAnimationTrajectory` | = 4 |
| `CurveRandom` | `ScriptedAnimationTrajectory` | = 5 |
| `HalfwayBetween` | `ScriptedAnimationTrajectory` | = 6 |

### ScriptedAnimationEffect

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `id` | `number` |  |
| `visual` | `fileID` |  |
| `visualScale` | `number` |  |
| `duration` | `number` |  |
| `trajectory` | `ScriptedAnimationTrajectory` |  |
| `yawRadians` | `number` |  |
| `pitchRadians` | `number` |  |
| `rollRadians` | `number` |  |
| `offsetX` | `number` |  |
| `offsetY` | `number` |  |
| `offsetZ` | `number` |  |
| `animation` | `number` |  |
| `animationSpeed` | `number` |  |
| `alpha` | `number` |  |
| `useTargetAsSource` | `bool` |  |
| `startBehavior` | `ScriptedAnimationBehavior?` |  |
| `startSoundKitID` | `number?` |  |
| `finishEffectID` | `number?` |  |
| `finishBehavior` | `ScriptedAnimationBehavior?` |  |
| `finishSoundKitID` | `number?` |  |
| `startAlphaFade` | `number?` |  |
| `startAlphaFadeDuration` | `number?` |  |
| `endAlphaFade` | `number?` |  |
| `endAlphaFadeDuration` | `number?` |  |
| `animationStartOffset` | `number?` |  |
| `loopingSoundKitID` | `number?` |  |
| `particleOverrideScale` | `number?` |  |
