# ModelScene

Widget methods (`FrameAPIModelSceneFrame`) · inherits [`Frame`](Frame.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/frameapimodelsceneframedocumentation.lua` (FileDataID 5244964)

## Methods

### ClearFog

```lua
ModelScene:ClearFog()
```

### CreateActor

```lua
ModelScene:CreateActor(name: cstring, template: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### GetActorAtIndex

```lua
ModelScene:GetActorAtIndex(index: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### GetAllowOverlappedModels

```lua
ModelScene:GetAllowOverlappedModels() -> allowOverlappedModels: bool
```

### GetCameraFarClip

```lua
ModelScene:GetCameraFarClip() -> farClip: number
```

### GetCameraFieldOfView

```lua
ModelScene:GetCameraFieldOfView() -> fov: number
```

Field of view in radians

### GetCameraForward

```lua
ModelScene:GetCameraForward() -> forwardX: number, forwardY: number, forwardZ: number
```

### GetCameraNearClip

```lua
ModelScene:GetCameraNearClip() -> nearClip: number
```

### GetCameraPosition

```lua
ModelScene:GetCameraPosition() -> positionX: number, positionY: number, positionZ: number
```

### GetCameraRight

```lua
ModelScene:GetCameraRight() -> rightX: number, rightY: number, rightZ: number
```

### GetCameraUp

```lua
ModelScene:GetCameraUp() -> upX: number, upY: number, upZ: number
```

### GetDrawLayer

```lua
ModelScene:GetDrawLayer() -> layer: DrawLayer, sublevel: number
```

### GetFogColor

```lua
ModelScene:GetFogColor() -> colorR: number, colorG: number, colorB: number
```

### GetFogFar

```lua
ModelScene:GetFogFar() -> far: number
```

### GetFogNear

```lua
ModelScene:GetFogNear() -> near: number
```

### GetLightAmbientColor

```lua
ModelScene:GetLightAmbientColor() -> colorR: number, colorG: number, colorB: number
```

### GetLightDiffuseColor

```lua
ModelScene:GetLightDiffuseColor() -> colorR: number, colorG: number, colorB: number
```

### GetLightDirection

```lua
ModelScene:GetLightDirection() -> directionX: number, directionY: number, directionZ: number
```

### GetLightPosition

```lua
ModelScene:GetLightPosition() -> positionX: number, positionY: number, positionZ: number
```

### GetLightType

```lua
ModelScene:GetLightType() -> lightType: ModelLightType?
```

### GetNumActors

```lua
ModelScene:GetNumActors() -> numActors: number
```

### GetViewInsets

```lua
ModelScene:GetViewInsets() -> insets: uiRect
```

### GetViewTranslation

```lua
ModelScene:GetViewTranslation() -> translationX: number, translationY: number
```

### IsLightVisible

```lua
ModelScene:IsLightVisible() -> isVisible: bool
```

### Project3DPointTo2D

```lua
ModelScene:Project3DPointTo2D(pointX: number, pointY: number, pointZ: number) -> point2DX: number, point2DY: number, depth: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### SetAllowOverlappedModels

```lua
ModelScene:SetAllowOverlappedModels(allowOverlappedModels: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetCameraFarClip

```lua
ModelScene:SetCameraFarClip(farClip: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetCameraFieldOfView

```lua
ModelScene:SetCameraFieldOfView(fov: number)
```

Field of view in radians

`SecretArguments=AllowedWhenUntainted`

### SetCameraNearClip

```lua
ModelScene:SetCameraNearClip(nearClip: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetCameraOrientationByAxisVectors

```lua
ModelScene:SetCameraOrientationByAxisVectors(forwardX: number, forwardY: number, forwardZ: number, rightX: number, rightY: number, rightZ: number, upX: number, upY: number, upZ: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetCameraOrientationByYawPitchRoll

```lua
ModelScene:SetCameraOrientationByYawPitchRoll(yaw: number, pitch: number, roll: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetCameraPosition

```lua
ModelScene:SetCameraPosition(positionX: number, positionY: number, positionZ: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetDesaturation

```lua
ModelScene:SetDesaturation(strength: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetDrawLayer

```lua
ModelScene:SetDrawLayer(layer: DrawLayer)
```

`SecretArguments=AllowedWhenUntainted`

### SetFogColor

```lua
ModelScene:SetFogColor(colorR: number, colorG: number, colorB: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetFogFar

```lua
ModelScene:SetFogFar(far: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetFogNear

```lua
ModelScene:SetFogNear(near: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetLightAmbientColor

```lua
ModelScene:SetLightAmbientColor(colorR: number, colorG: number, colorB: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetLightDiffuseColor

```lua
ModelScene:SetLightDiffuseColor(colorR: number, colorG: number, colorB: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetLightDirection

```lua
ModelScene:SetLightDirection(directionX: number, directionY: number, directionZ: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetLightPosition

```lua
ModelScene:SetLightPosition(positionX: number, positionY: number, positionZ: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetLightType

```lua
ModelScene:SetLightType(lightType: ModelLightType)
```

`SecretArguments=AllowedWhenUntainted`

### SetLightVisible

```lua
ModelScene:SetLightVisible(visible: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `visible` | `bool` | default `false` |

### SetPaused

```lua
ModelScene:SetPaused(paused: bool, affectsGlobalPause: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `paused` | `bool` |  |
| `affectsGlobalPause` | `bool` | default `true` |

### SetViewInsets

```lua
ModelScene:SetViewInsets(insets: uiRect)
```

`SecretArguments=AllowedWhenUntainted`

### SetViewTranslation

```lua
ModelScene:SetViewTranslation(translationX: number, translationY: number)
```

`SecretArguments=AllowedWhenUntainted`

### TakeActor

```lua
ModelScene:TakeActor()
```
