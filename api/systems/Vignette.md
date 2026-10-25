# Vignette

Namespace `C_VignetteInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/vignetteinfodocumentation.lua` (FileDataID 4637307)

## Functions

### FindBestUniqueVignette

```lua
C_VignetteInfo.FindBestUniqueVignette(vignetteGUIDs: WOWGUID[]) -> bestUniqueVignetteIndex: luaIndex?
```

`SecretArguments=AllowedWhenUntainted`

### GetHealthPercent

```lua
C_VignetteInfo.GetHealthPercent(vignetteGUID: WOWGUID) -> healthPct: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetRecommendedGroupSize

```lua
C_VignetteInfo.GetRecommendedGroupSize(vignetteGUID: WOWGUID) -> minGroupSize: number, maxGroupSize: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetVignetteInfo

```lua
C_VignetteInfo.GetVignetteInfo(vignetteGUID: WOWGUID) -> vignetteInfo: VignetteInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetVignettePosition

```lua
C_VignetteInfo.GetVignettePosition(vignetteGUID: WOWGUID, uiMapID: number) -> vignettePosition: vector2, vignetteFacing: number?
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `vignettePosition` | `vector2` | `Mixin=Vector2DMixin` |
| `vignetteFacing` | `number?` |  |

### GetVignettes

```lua
C_VignetteInfo.GetVignettes() -> vignetteGUIDs: WOWGUID[]
```

## Events

### VIGNETTE_MINIMAP_UPDATED

```lua
VIGNETTE_MINIMAP_UPDATED(vignetteGUID: WOWGUID, onMinimap: bool)
```

`UniqueEvent`

### VIGNETTES_UPDATED

```lua
VIGNETTES_UPDATED()
```

`SynchronousEvent`

## Types

### VignetteInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `vignetteGUID` | `WOWGUID` |  |
| `objectGUID` | `WOWGUID` |  |
| `name` | `cstring` |  |
| `isDead` | `bool` |  |
| `onWorldMap` | `bool` |  |
| `zoneInfiniteAOI` | `bool` |  |
| `onMinimap` | `bool` |  |
| `isUnique` | `bool` |  |
| `inFogOfWar` | `bool` |  |
| `atlasName` | `textureAtlas` |  |
| `hasTooltip` | `bool` |  |
| `vignetteID` | `number` |  |
| `type` | `VignetteType` |  |
| `rewardQuestID` | `number` |  |
| `tooltipWidgetSet` | `number?` |  |
| `iconWidgetSet` | `number?` |  |
| `addPaddingAboveTooltipWidgets` | `bool?` |  |
| `mapPin` | `UIMapPinInfo?` |  |
| `objectiveType` | `VignetteObjectiveType?` |  |
