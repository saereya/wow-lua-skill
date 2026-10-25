# UnitPositionFrame

Widget methods (`FrameAPIUnitPositionFrame`) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/frameapiunitpositionframedocumentation.lua` (FileDataID 5196726)

## Methods

### AddUnit

```lua
UnitPositionFrame:AddUnit(unitTokenString: cstring, asset: TextureAssetDisk, width: uiUnit?, height: uiUnit?, r: number?, g: number?, b: number?, a: number?, sublayer: number?, showFacing: bool?)
```

`SecretArguments=AllowedWhenUntainted`

### ClearUnits

```lua
UnitPositionFrame:ClearUnits()
```

### FinalizeUnits

```lua
UnitPositionFrame:FinalizeUnits()
```

### GetMouseOverUnits

```lua
UnitPositionFrame:GetMouseOverUnits() -> units: UnitTokenType
```

Returns:

| Name | Type | Notes |
|---|---|---|
| `units` | `UnitTokenType` | `StrideIndex=1` |

### GetPlayerPingScale

```lua
UnitPositionFrame:GetPlayerPingScale() -> scale: number
```

### GetUiMapID

```lua
UnitPositionFrame:GetUiMapID() -> mapID: number
```

### SetPlayerPingScale

```lua
UnitPositionFrame:SetPlayerPingScale(scale: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetPlayerPingTexture

```lua
UnitPositionFrame:SetPlayerPingTexture(textureType: PingTextureType, asset: FileAsset, width: uiUnit, height: uiUnit)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `textureType` | `PingTextureType` |  |
| `asset` | `FileAsset` |  |
| `width` | `uiUnit` | default `0` |
| `height` | `uiUnit` | default `0` |

### SetUiMapID

```lua
UnitPositionFrame:SetUiMapID(mapID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetUnitColor

```lua
UnitPositionFrame:SetUnitColor(unit: UnitTokenType, colorR: number, colorG: number, colorB: number, colorA: number)
```

`SecretArguments=AllowedWhenUntainted`

### StartPlayerPing

```lua
UnitPositionFrame:StartPlayerPing(duration: number, fadeDuration: number)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `duration` | `number` | default `0` |
| `fadeDuration` | `number` | default `0` |

### StopPlayerPing

```lua
UnitPositionFrame:StopPlayerPing()
```
