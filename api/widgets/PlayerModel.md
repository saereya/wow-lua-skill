# PlayerModel

Widget methods (`FrameAPICharacterModelBase`) · inherits [`Model`](Model.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/frameapicharactermodelbasedocumentation.lua` (FileDataID 5197112)

## Methods

### ApplySpellVisualKit

```lua
PlayerModel:ApplySpellVisualKit(spellVisualKitID: number, oneShot: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellVisualKitID` | `number` |  |
| `oneShot` | `bool` | default `false` |

### CanSetUnit

```lua
PlayerModel:CanSetUnit(unit: UnitToken)
```

`SecretArguments=AllowedWhenUntainted`

### FreezeAnimation

```lua
PlayerModel:FreezeAnimation(anim: AnimationDataEnum, variation: number, frame: number)
```

`SecretArguments=AllowedWhenUntainted`

### GetDisplayInfo

```lua
PlayerModel:GetDisplayInfo() -> displayID: number
```

### GetDoBlend

```lua
PlayerModel:GetDoBlend() -> doBlend: bool
```

### GetKeepModelOnHide

```lua
PlayerModel:GetKeepModelOnHide() -> keepModelOnHide: bool
```

### HasAnimation

```lua
PlayerModel:HasAnimation(anim: AnimationDataEnum) -> hasAnimation: bool
```

`SecretArguments=AllowedWhenUntainted`

### PlayAnimKit

```lua
PlayerModel:PlayAnimKit(animKit: number, loop: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `animKit` | `number` |  |
| `loop` | `bool` | default `false` |

### RefreshCamera

```lua
PlayerModel:RefreshCamera()
```

### RefreshUnit

```lua
PlayerModel:RefreshUnit()
```

### SetAnimation

```lua
PlayerModel:SetAnimation(anim: AnimationDataEnum, variation: number?)
```

`SecretArguments=AllowedWhenUntainted`

### SetBarberShopAlternateForm

```lua
PlayerModel:SetBarberShopAlternateForm()
```

### SetCamDistanceScale

```lua
PlayerModel:SetCamDistanceScale(scale: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetCreature

```lua
PlayerModel:SetCreature(creatureID: number, displayID: number)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `creatureID` | `number` |  |
| `displayID` | `number` | default `0` |

### SetDisplayInfo

```lua
PlayerModel:SetDisplayInfo(displayID: number, mountDisplayID: number?)
```

`SecretArguments=AllowedWhenUntainted`

### SetDoBlend

```lua
PlayerModel:SetDoBlend(doBlend: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `doBlend` | `bool` | default `false` |

### SetItem

```lua
PlayerModel:SetItem(itemID: number, appearanceModID: number?, itemVisualID: number?)
```

`SecretArguments=AllowedWhenUntainted`

### SetItemAppearance

```lua
PlayerModel:SetItemAppearance(itemAppearanceID: number, itemVisualID: number?, itemSubclass: ItemWeaponSubclass?)
```

`SecretArguments=AllowedWhenUntainted`

### SetKeepModelOnHide

```lua
PlayerModel:SetKeepModelOnHide(keepModelOnHide: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetPortraitZoom

```lua
PlayerModel:SetPortraitZoom(zoom: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetRotation

```lua
PlayerModel:SetRotation(radians: number, animate: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `radians` | `number` |  |
| `animate` | `bool` | default `true` |

### SetUnit

```lua
PlayerModel:SetUnit(unit: UnitToken, blend: bool, useNativeForm: bool?) -> success: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresDeclassifiedUnitIdentity`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unit` | `UnitToken` |  |
| `blend` | `bool` | default `true` |
| `useNativeForm` | `bool?` |  |

### StopAnimKit

```lua
PlayerModel:StopAnimKit()
```

### ZeroCachedCenterXY

```lua
PlayerModel:ZeroCachedCenterXY()
```
