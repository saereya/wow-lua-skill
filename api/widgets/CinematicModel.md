# CinematicModel

Widget methods (`FrameAPICinematicModel`) · inherits [`PlayerModel`](PlayerModel.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/frameapicinematicmodeldocumentation.lua` (FileDataID 5207353)

## Methods

### EquipItem

```lua
CinematicModel:EquipItem(itemID: number)
```

`SecretArguments=AllowedWhenUntainted`

### InitializeCamera

```lua
CinematicModel:InitializeCamera(scaleFactor: number)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `scaleFactor` | `number` | default `0` |

### InitializePanCamera

```lua
CinematicModel:InitializePanCamera(scaleFactor: number)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `scaleFactor` | `number` | default `0` |

### RefreshCamera

```lua
CinematicModel:RefreshCamera()
```

### SetAnimOffset

```lua
CinematicModel:SetAnimOffset(offset: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetCameraPosition

```lua
CinematicModel:SetCameraPosition(positionX: number, positionY: number, positionZ: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetCameraTarget

```lua
CinematicModel:SetCameraTarget(positionX: number, positionY: number, positionZ: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetCreatureData

```lua
CinematicModel:SetCreatureData(creatureID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetFacingLeft

```lua
CinematicModel:SetFacingLeft(isFacingLeft: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `isFacingLeft` | `bool` | default `false` |

### SetFadeTimes

```lua
CinematicModel:SetFadeTimes(fadeInSeconds: number, fadeOutSeconds: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetHeightFactor

```lua
CinematicModel:SetHeightFactor(factor: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetJumpInfo

```lua
CinematicModel:SetJumpInfo(jumpLength: number, jumpHeight: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetPanDistance

```lua
CinematicModel:SetPanDistance(scale: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetSpellVisualKit

```lua
CinematicModel:SetSpellVisualKit(visualKitID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetTargetDistance

```lua
CinematicModel:SetTargetDistance(scale: number)
```

`SecretArguments=AllowedWhenUntainted`

### StartPan

```lua
CinematicModel:StartPan(panType: luaIndex, durationSeconds: number, doFade: bool, visKitID: number, startPositionScale: number, speedMultiplier: number)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `panType` | `luaIndex` |  |
| `durationSeconds` | `number` |  |
| `doFade` | `bool` | default `false` |
| `visKitID` | `number` | default `0` |
| `startPositionScale` | `number` | default `0` |
| `speedMultiplier` | `number` | default `1` |

### StopPan

```lua
CinematicModel:StopPan()
```

### UnequipItems

```lua
CinematicModel:UnequipItems()
```
