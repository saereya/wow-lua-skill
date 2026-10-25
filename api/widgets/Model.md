# Model

Widget methods (`SimpleModelAPI`) · inherits [`Frame`](Frame.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/simplemodelapidocumentation.lua` (FileDataID 4637220)

## Methods

### AdvanceTime

```lua
Model:AdvanceTime()
```

### ClearFog

```lua
Model:ClearFog()
```

### ClearModel

```lua
Model:ClearModel()
```

### ClearTransform

```lua
Model:ClearTransform()
```

### GetCameraDistance

```lua
Model:GetCameraDistance() -> distance: number
```

### GetCameraFacing

```lua
Model:GetCameraFacing() -> radians: number
```

### GetCameraPosition

```lua
Model:GetCameraPosition() -> positionX: number, positionY: number, positionZ: number
```

### GetCameraRoll

```lua
Model:GetCameraRoll() -> radians: number
```

### GetCameraTarget

```lua
Model:GetCameraTarget() -> targetX: number, targetY: number, targetZ: number
```

### GetDesaturation

```lua
Model:GetDesaturation() -> strength: number
```

### GetFacing

```lua
Model:GetFacing() -> facing: number
```

### GetFogColor

```lua
Model:GetFogColor() -> colorR: number, colorG: number, colorB: number, colorA: number
```

### GetFogFar

```lua
Model:GetFogFar() -> fogFar: number
```

### GetFogNear

```lua
Model:GetFogNear() -> fogNear: number
```

### GetLight

```lua
Model:GetLight() -> enabled: bool, light: ModelLight
```

### GetModelAlpha

```lua
Model:GetModelAlpha() -> alpha: number
```

### GetModelDrawLayer

```lua
Model:GetModelDrawLayer() -> layer: DrawLayer, sublayer: number
```

### GetModelFileID

```lua
Model:GetModelFileID() -> modelFileID: fileID
```

### GetModelScale

```lua
Model:GetModelScale() -> scale: number
```

### GetPaused

```lua
Model:GetPaused() -> paused: bool
```

### GetPitch

```lua
Model:GetPitch() -> pitch: number
```

### GetPosition

```lua
Model:GetPosition() -> positionX: number, positionY: number, positionZ: number
```

### GetRoll

```lua
Model:GetRoll() -> roll: number
```

### GetShadowEffect

```lua
Model:GetShadowEffect() -> strength: number
```

### GetViewInsets

```lua
Model:GetViewInsets() -> left: uiUnit, right: uiUnit, top: uiUnit, bottom: uiUnit
```

### GetViewTranslation

```lua
Model:GetViewTranslation() -> x: uiUnit, y: uiUnit
```

### GetWorldScale

```lua
Model:GetWorldScale() -> worldScale: number
```

### HasAttachmentPoints

```lua
Model:HasAttachmentPoints() -> hasAttachmentPoints: bool
```

### HasCustomCamera

```lua
Model:HasCustomCamera() -> hasCustomCamera: bool
```

### IsUsingModelCenterToTransform

```lua
Model:IsUsingModelCenterToTransform() -> useCenter: bool
```

### MakeCurrentCameraCustom

```lua
Model:MakeCurrentCameraCustom()
```

### ReplaceIconTexture

```lua
Model:ReplaceIconTexture(asset: FileAsset)
```

`SecretArguments=AllowedWhenUntainted`

### SetCamera

```lua
Model:SetCamera(cameraIndex: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetCameraDistance

```lua
Model:SetCameraDistance(distance: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetCameraFacing

```lua
Model:SetCameraFacing(radians: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetCameraPosition

```lua
Model:SetCameraPosition(positionX: number, positionY: number, positionZ: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetCameraRoll

```lua
Model:SetCameraRoll(radians: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetCameraTarget

```lua
Model:SetCameraTarget(targetX: number, targetY: number, targetZ: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetCustomCamera

```lua
Model:SetCustomCamera(cameraIndex: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetDesaturation

```lua
Model:SetDesaturation(strength: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetFacing

```lua
Model:SetFacing(facing: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetFogColor

```lua
Model:SetFogColor(colorR: number, colorG: number, colorB: number, a: SingleColorValue?)
```

`SecretArguments=AllowedWhenUntainted`

### SetFogFar

```lua
Model:SetFogFar(fogFar: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetFogNear

```lua
Model:SetFogNear(fogNear: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetGlow

```lua
Model:SetGlow(glow: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetGradientMask

```lua
Model:SetGradientMask(grad0: number, grad1: number, grad2: number, grad3: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetLight

```lua
Model:SetLight(enabled: bool, light: ModelLight)
```

`SecretArguments=AllowedWhenUntainted`

### SetModel

```lua
Model:SetModel(asset: ModelAsset, noMip: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `asset` | `ModelAsset` |  |
| `noMip` | `bool` | default `false` |

### SetModelAlpha

```lua
Model:SetModelAlpha(alpha: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetModelDrawLayer

```lua
Model:SetModelDrawLayer(layer: DrawLayer)
```

`SecretArguments=AllowedWhenUntainted`

### SetModelScale

```lua
Model:SetModelScale(scale: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetParticlesEnabled

```lua
Model:SetParticlesEnabled(enabled: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetPaused

```lua
Model:SetPaused(paused: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetPitch

```lua
Model:SetPitch(pitch: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetPosition

```lua
Model:SetPosition(positionX: number, positionY: number, positionZ: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetRoll

```lua
Model:SetRoll(roll: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetSequence

```lua
Model:SetSequence(sequence: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetSequenceTime

```lua
Model:SetSequenceTime(sequence: number, timeOffset: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetShadowEffect

```lua
Model:SetShadowEffect(strength: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetTransform

```lua
Model:SetTransform(translation: vector3?, rotation: vector3?, scale: number?)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `translation` | `vector3?` | `Mixin=Vector3DMixin` |
| `rotation` | `vector3?` | `Mixin=Vector3DMixin` |
| `scale` | `number?` |  |

### SetUseGBuffer

```lua
Model:SetUseGBuffer(useGBuffer: bool)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetViewInsets

```lua
Model:SetViewInsets(left: uiUnit, right: uiUnit, top: uiUnit, bottom: uiUnit)
```

`SecretArguments=AllowedWhenUntainted`

### SetViewTranslation

```lua
Model:SetViewTranslation(x: uiUnit, y: uiUnit)
```

`SecretArguments=AllowedWhenUntainted`

### TransformCameraSpaceToModelSpace

```lua
Model:TransformCameraSpaceToModelSpace(cameraPosition: vector3) -> modelPosition: vector3
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `cameraPosition` | `vector3` | `Mixin=Vector3DMixin` |

Returns:

| Name | Type | Notes |
|---|---|---|
| `modelPosition` | `vector3` | `Mixin=Vector3DMixin` |

### UseModelCenterToTransform

```lua
Model:UseModelCenterToTransform(useCenter: bool)
```

`SecretArguments=AllowedWhenUntainted`
