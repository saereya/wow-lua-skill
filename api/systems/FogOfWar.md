# FogOfWar

Namespace `C_FogOfWar` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/fogofwardocumentation.lua` (FileDataID 4637093)

## Functions

### GetFogOfWarForMap

```lua
C_FogOfWar.GetFogOfWarForMap(uiMapID: number) -> fogOfWarID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetFogOfWarInfo

```lua
C_FogOfWar.GetFogOfWarInfo(fogOfWarID: number) -> fogOfWarInfo: FogOfWarInfo?
```

`SecretArguments=AllowedWhenUntainted`

## Events

### FOG_OF_WAR_UPDATED

```lua
FOG_OF_WAR_UPDATED()
```

`UniqueEvent`

## Types

### FogOfWarInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `fogOfWarID` | `number` |  |
| `backgroundAtlas` | `textureAtlas` |  |
| `maskAtlas` | `textureAtlas` |  |
| `maskScalar` | `number` |  |
