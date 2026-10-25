# ModelInfo

Namespace `C_ModelInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/uimodelinfodocumentation.lua` (FileDataID 4637279)

## Functions

### AddActiveModelScene

```lua
C_ModelInfo.AddActiveModelScene(modelSceneFrame: ModelSceneFrame, modelSceneID: number)
```

This function does nothing in public clients

`SecretArguments=AllowedWhenUntainted`

### AddActiveModelSceneActor

```lua
C_ModelInfo.AddActiveModelSceneActor(modelSceneFrameActor: ModelSceneFrameActor, modelSceneActorID: number)
```

This function does nothing in public clients

`SecretArguments=AllowedWhenUntainted`

### ClearActiveModelScene

```lua
C_ModelInfo.ClearActiveModelScene(modelSceneFrame: ModelSceneFrame)
```

This function does nothing in public clients

`SecretArguments=AllowedWhenUntainted`

### ClearActiveModelSceneActor

```lua
C_ModelInfo.ClearActiveModelSceneActor(modelSceneFrameActor: ModelSceneFrameActor)
```

This function does nothing in public clients

`SecretArguments=AllowedWhenUntainted`

### GetModelSceneActorDisplayInfoByID

```lua
C_ModelInfo.GetModelSceneActorDisplayInfoByID(modelActorDisplayID: number) -> actorDisplayInfo: UIModelSceneActorDisplayInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetModelSceneActorInfoByID

```lua
C_ModelInfo.GetModelSceneActorInfoByID(modelActorID: number) -> actorInfo: UIModelSceneActorInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetModelSceneCameraInfoByID

```lua
C_ModelInfo.GetModelSceneCameraInfoByID(modelSceneCameraID: number) -> modelSceneCameraInfo: UIModelSceneCameraInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetModelSceneInfoByID

```lua
C_ModelInfo.GetModelSceneInfoByID(modelSceneID: number) -> modelSceneType: ModelSceneType, modelCameraIDs: number[], modelActorsIDs: number[], flags: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

## Events

### UI_MODEL_SCENE_INFO_UPDATED

```lua
UI_MODEL_SCENE_INFO_UPDATED()
```

`UniqueEvent`

## Types

### UIModelSceneActorDisplayInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `animation` | `number` |  |
| `animationVariation` | `number` |  |
| `animSpeed` | `number` |  |
| `animationKitID` | `number?` |  |
| `spellVisualKitID` | `number?` |  |
| `alpha` | `number` |  |
| `scale` | `number` |  |

### UIModelSceneActorInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `modelActorID` | `number` |  |
| `scriptTag` | `cstring` |  |
| `position` | `vector3` | `Mixin=Vector3DMixin` |
| `yaw` | `number` |  |
| `pitch` | `number` |  |
| `roll` | `number` |  |
| `normalizeScaleAggressiveness` | `number?` |  |
| `useCenterForOriginX` | `bool` |  |
| `useCenterForOriginY` | `bool` |  |
| `useCenterForOriginZ` | `bool` |  |
| `modelActorDisplayID` | `number?` |  |

### UIModelSceneCameraInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `modelSceneCameraID` | `number` |  |
| `scriptTag` | `cstring` |  |
| `cameraType` | `cstring` |  |
| `target` | `vector3` | `Mixin=Vector3DMixin` |
| `yaw` | `number` |  |
| `pitch` | `number` |  |
| `roll` | `number` |  |
| `zoomDistance` | `number` |  |
| `minZoomDistance` | `number` |  |
| `maxZoomDistance` | `number` |  |
| `zoomedTargetOffset` | `vector3` | `Mixin=Vector3DMixin` |
| `zoomedYawOffset` | `number` |  |
| `zoomedPitchOffset` | `number` |  |
| `zoomedRollOffset` | `number` |  |
| `flags` | `ModelSceneSetting` |  |
