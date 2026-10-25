# ModelSceneActorBase

Widget methods (`FrameAPIModelSceneFrameActorBase`) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/frameapimodelsceneframeactorbasedocumentation.lua` (FileDataID 5264241)

## Methods

### ClearModel

```lua
ModelSceneActorBase:ClearModel()
```

### GetActiveBoundingBox

```lua
ModelSceneActorBase:GetActiveBoundingBox() -> boxBottom: vector3, boxTop: vector3
```

Returns:

| Name | Type | Notes |
|---|---|---|
| `boxBottom` | `vector3` | `Mixin=Vector3DMixin` |
| `boxTop` | `vector3` | `Mixin=Vector3DMixin` |

### GetAlpha

```lua
ModelSceneActorBase:GetAlpha() -> alpha: number
```

`SecretReturnsForAspect={ Enum.SecretAspect.Alpha }`

### GetAnimation

```lua
ModelSceneActorBase:GetAnimation() -> animation: AnimationDataEnum
```

### GetAnimationBlendOperation

```lua
ModelSceneActorBase:GetAnimationBlendOperation() -> blendOp: ModelBlendOperation
```

### GetAnimationVariation

```lua
ModelSceneActorBase:GetAnimationVariation() -> variation: number
```

### GetDesaturation

```lua
ModelSceneActorBase:GetDesaturation() -> strength: number
```

### GetMaxBoundingBox

```lua
ModelSceneActorBase:GetMaxBoundingBox() -> boxBottom: vector3, boxTop: vector3
```

Returns:

| Name | Type | Notes |
|---|---|---|
| `boxBottom` | `vector3` | `Mixin=Vector3DMixin` |
| `boxTop` | `vector3` | `Mixin=Vector3DMixin` |

### GetModelFileID

```lua
ModelSceneActorBase:GetModelFileID() -> file: fileID
```

### GetModelPath

```lua
ModelSceneActorBase:GetModelPath() -> path: string
```

### GetModelUnitGUID

```lua
ModelSceneActorBase:GetModelUnitGUID() -> guid: WOWGUID
```

### GetParticleOverrideScale

```lua
ModelSceneActorBase:GetParticleOverrideScale() -> scale: number?
```

### GetPitch

```lua
ModelSceneActorBase:GetPitch() -> pitch: number
```

### GetPosition

```lua
ModelSceneActorBase:GetPosition() -> positionX: number, positionY: number, positionZ: number
```

### GetRoll

```lua
ModelSceneActorBase:GetRoll() -> roll: number
```

### GetScale

```lua
ModelSceneActorBase:GetScale() -> scale: number
```

### GetSpellVisualKit

```lua
ModelSceneActorBase:GetSpellVisualKit() -> spellVisualKitID: number
```

### GetYaw

```lua
ModelSceneActorBase:GetYaw() -> yaw: number
```

### Hide

```lua
ModelSceneActorBase:Hide()
```

### IsLoaded

```lua
ModelSceneActorBase:IsLoaded() -> isLoaded: bool
```

### IsPreferringModelCollisionBounds

```lua
ModelSceneActorBase:IsPreferringModelCollisionBounds() -> preferringCollisionBounds: bool
```

### IsShown

```lua
ModelSceneActorBase:IsShown() -> isShown: bool
```

### IsUsingCenterForOrigin

```lua
ModelSceneActorBase:IsUsingCenterForOrigin() -> x: bool, y: bool, z: bool
```

### IsVisible

```lua
ModelSceneActorBase:IsVisible() -> isVisible: bool
```

### PlayAnimationKit

```lua
ModelSceneActorBase:PlayAnimationKit(animationKit: number, isLooping: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `animationKit` | `number` |  |
| `isLooping` | `bool` | default `false` |

### SetAlpha

```lua
ModelSceneActorBase:SetAlpha(alpha: number)
```

`SecretArguments=AllowedWhenUntainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.Alpha }`

### SetAnimation

```lua
ModelSceneActorBase:SetAnimation(animation: AnimationDataEnum, variation: number?, animSpeed: number, animOffsetSeconds: number)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `animation` | `AnimationDataEnum` |  |
| `variation` | `number?` |  |
| `animSpeed` | `number` | default `1` |
| `animOffsetSeconds` | `number` | default `0` |

### SetAnimationBlendOperation

```lua
ModelSceneActorBase:SetAnimationBlendOperation(blendOp: ModelBlendOperation)
```

`SecretArguments=AllowedWhenUntainted`

### SetDesaturation

```lua
ModelSceneActorBase:SetDesaturation(strength: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetGradientMask

```lua
ModelSceneActorBase:SetGradientMask(gradientIndex0: number, gradientIndex1: number, gradientIndex2: number, gradientIndex3: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetGradientMaskWithDyes

```lua
ModelSceneActorBase:SetGradientMaskWithDyes(grad0DyeColorID: number?, grad1DyeColorID: number?, grad2DyeColorID: number?)
```

`SecretArguments=AllowedWhenUntainted`

### SetModelByCreatureDisplayID

```lua
ModelSceneActorBase:SetModelByCreatureDisplayID(creatureDisplayID: number, useActivePlayerCustomizations: bool) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `creatureDisplayID` | `number` |  |
| `useActivePlayerCustomizations` | `bool` | default `false` |

### SetModelByFileID

```lua
ModelSceneActorBase:SetModelByFileID(asset: FileAsset, useMips: bool) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `asset` | `FileAsset` |  |
| `useMips` | `bool` | default `false` |

### SetModelByPath

```lua
ModelSceneActorBase:SetModelByPath(asset: FileAsset, useMips: bool) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `asset` | `FileAsset` |  |
| `useMips` | `bool` | default `false` |

### SetModelByUnit

```lua
ModelSceneActorBase:SetModelByUnit(unit: UnitToken, sheatheWeapons: bool, autoDress: bool, hideWeapons: bool, usePlayerNativeForm: bool, holdBowString: bool, customRaceID: number?) -> success: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresDeclassifiedUnitIdentity`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unit` | `UnitToken` |  |
| `sheatheWeapons` | `bool` | default `false` |
| `autoDress` | `bool` | default `true` |
| `hideWeapons` | `bool` | default `false` |
| `usePlayerNativeForm` | `bool` | default `true` |
| `holdBowString` | `bool` | default `false` |
| `customRaceID` | `number?` |  |

### SetModelByUnitCreatureDisplayID

```lua
ModelSceneActorBase:SetModelByUnitCreatureDisplayID(unit: UnitToken) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetParticleOverrideScale

```lua
ModelSceneActorBase:SetParticleOverrideScale(scale: number?)
```

`SecretArguments=AllowedWhenUntainted`

### SetPitch

```lua
ModelSceneActorBase:SetPitch(pitch: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetPlayerModelFromGlues

```lua
ModelSceneActorBase:SetPlayerModelFromGlues(characterIndex: number?, sheatheWeapons: bool, autoDress: bool, hideWeapons: bool, usePlayerNativeForm: bool, customRaceID: number?) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `characterIndex` | `number?` |  |
| `sheatheWeapons` | `bool` | default `false` |
| `autoDress` | `bool` | default `true` |
| `hideWeapons` | `bool` | default `false` |
| `usePlayerNativeForm` | `bool` | default `true` |
| `customRaceID` | `number?` |  |

### SetPosition

```lua
ModelSceneActorBase:SetPosition(positionX: number, positionY: number, positionZ: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetPreferModelCollisionBounds

```lua
ModelSceneActorBase:SetPreferModelCollisionBounds(preferCollisionBounds: bool)
```

If true, will try to use the collision bounds of models for sizing and centering. Will fall back to default model bounds if set to False, or if collision bounds are unavailable.

`SecretArguments=AllowedWhenUntainted`

### SetRoll

```lua
ModelSceneActorBase:SetRoll(roll: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetScale

```lua
ModelSceneActorBase:SetScale(scale: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetShown

```lua
ModelSceneActorBase:SetShown(show: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `show` | `bool` | default `false` |

### SetSpellVisualKit

```lua
ModelSceneActorBase:SetSpellVisualKit(spellVisualKitID: number, oneShot: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellVisualKitID` | `number` | default `0` |
| `oneShot` | `bool` | default `false` |

### SetUseCenterForOrigin

```lua
ModelSceneActorBase:SetUseCenterForOrigin(x: bool, y: bool, z: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `x` | `bool` | default `false` |
| `y` | `bool` | default `false` |
| `z` | `bool` | default `false` |

### SetYaw

```lua
ModelSceneActorBase:SetYaw(yaw: number)
```

`SecretArguments=AllowedWhenUntainted`

### Show

```lua
ModelSceneActorBase:Show()
```

### StopAnimationKit

```lua
ModelSceneActorBase:StopAnimationKit()
```

### TryOn

```lua
ModelSceneActorBase:TryOn(itemLinkOrItemModifiedAppearanceID: cstring, handSlotName: cstring?, spellEnchantmentID: number) -> reason: ItemTryOnReason?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLinkOrItemModifiedAppearanceID` | `cstring` |  |
| `handSlotName` | `cstring?` |  |
| `spellEnchantmentID` | `number` | default `0` |
