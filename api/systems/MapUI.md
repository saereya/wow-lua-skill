# MapUI

Namespace `C_Map` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/mapdocumentation.lua` (FileDataID 4637132)

## Functions

### CanSetUserWaypointOnMap

```lua
C_Map.CanSetUserWaypointOnMap(uiMapID: number) -> canSet: bool
```

`SecretArguments=AllowedWhenUntainted`

### ClearUserWaypoint

```lua
C_Map.ClearUserWaypoint()
```

### CloseWorldMapInteraction

```lua
C_Map.CloseWorldMapInteraction()
```

### GetAreaInfo

```lua
C_Map.GetAreaInfo(areaID: number) -> name: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetBestMapForUnit

```lua
C_Map.GetBestMapForUnit(unitToken: UnitToken) -> uiMapID: number?
```

Only works for the player and party members.

`SecretArguments=AllowedWhenUntainted`

### GetBountySetMaps

```lua
C_Map.GetBountySetMaps(bountySetID: number) -> mapIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetFallbackWorldMapID

```lua
C_Map.GetFallbackWorldMapID() -> uiMapID: number
```

### GetMapArtBackgroundAtlas

```lua
C_Map.GetMapArtBackgroundAtlas(uiMapID: number) -> atlasName: textureAtlas
```

`SecretArguments=AllowedWhenUntainted`

### GetMapArtHelpTextPosition

```lua
C_Map.GetMapArtHelpTextPosition(uiMapID: number) -> position: MapCanvasPosition
```

`SecretArguments=AllowedWhenUntainted`

### GetMapArtID

```lua
C_Map.GetMapArtID(uiMapID: number) -> uiMapArtID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetMapArtLayers

```lua
C_Map.GetMapArtLayers(uiMapID: number) -> layerInfo: UiMapLayerInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetMapArtLayerTextures

```lua
C_Map.GetMapArtLayerTextures(uiMapID: number, layerIndex: luaIndex) -> textures: fileID[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetMapArtZoneTextPosition

```lua
C_Map.GetMapArtZoneTextPosition(uiMapID: number) -> position: MapCanvasPosition
```

`SecretArguments=AllowedWhenUntainted`

### GetMapBannersForMap

```lua
C_Map.GetMapBannersForMap(uiMapID: number) -> mapBanners: MapBannerInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetMapChildrenInfo

```lua
C_Map.GetMapChildrenInfo(uiMapID: number, mapType: UIMapType?, allDescendants: bool?) -> info: UiMapDetails[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetMapDisplayInfo

```lua
C_Map.GetMapDisplayInfo(uiMapID: number) -> hideIcons: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetMapGroupID

```lua
C_Map.GetMapGroupID(uiMapID: number) -> uiMapGroupID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetMapGroupMembersInfo

```lua
C_Map.GetMapGroupMembersInfo(uiMapGroupID: number) -> info: UiMapGroupMemberInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetMapHighlightInfoAtPosition

```lua
C_Map.GetMapHighlightInfoAtPosition(uiMapID: number, x: number, y: number) -> fileDataID: fileID, atlasID: textureAtlas, texturePercentageX: number, texturePercentageY: number, textureX: number, textureY: number, scrollChildX: number, scrollChildY: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetMapHighlightPulseInfo

```lua
C_Map.GetMapHighlightPulseInfo(uiMapID: number) -> fileDataID: fileID, atlasID: textureAtlas, texturePercentageX: number, texturePercentageY: number, textureX: number, textureY: number, scrollChildX: number, scrollChildY: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetMapInfo

```lua
C_Map.GetMapInfo(uiMapID: number) -> info: UiMapDetails
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetMapInfoAtPosition

```lua
C_Map.GetMapInfoAtPosition(uiMapID: number, x: number, y: number, ignoreZoneMapPositionData: bool?) -> info: UiMapDetails
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetMapLevels

```lua
C_Map.GetMapLevels(uiMapID: number) -> playerMinLevel: number, playerMaxLevel: number, petMinLevel: number, petMaxLevel: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `playerMinLevel` | `number` |  |
| `playerMaxLevel` | `number` |  |
| `petMinLevel` | `number` | default `0` |
| `petMaxLevel` | `number` | default `0` |

### GetMapLinksForMap

```lua
C_Map.GetMapLinksForMap(uiMapID: number) -> mapLinks: MapLinkInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetMapPosFromWorldPos

```lua
C_Map.GetMapPosFromWorldPos(continentID: number, worldPosition: vector2, overrideUiMapID: number?) -> uiMapID: number, mapPosition: vector2
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `continentID` | `number` |  |
| `worldPosition` | `vector2` | `Mixin=Vector2DMixin` |
| `overrideUiMapID` | `number?` |  |

Returns:

| Name | Type | Notes |
|---|---|---|
| `uiMapID` | `number` |  |
| `mapPosition` | `vector2` | `Mixin=Vector2DMixin` |

### GetMapRectOnMap

```lua
C_Map.GetMapRectOnMap(uiMapID: number, topUiMapID: number) -> minX: number, maxX: number, minY: number, maxY: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetMapWorldSize

```lua
C_Map.GetMapWorldSize(uiMapID: number) -> width: number, height: number
```

Returns the size in yards of the area represented by the map.

`SecretArguments=AllowedWhenUntainted`

### GetPlayerMapPosition

```lua
C_Map.GetPlayerMapPosition(uiMapID: number, unitToken: UnitToken) -> position: vector2?
```

Only works for the player and party members.

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `position` | `vector2?` | `Mixin=Vector2DMixin` |

### GetUserWaypoint

```lua
C_Map.GetUserWaypoint() -> point: UiMapPoint
```

`MayReturnNothing`

### GetUserWaypointFromHyperlink

```lua
C_Map.GetUserWaypointFromHyperlink(hyperlink: string) -> point: UiMapPoint
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetUserWaypointHyperlink

```lua
C_Map.GetUserWaypointHyperlink() -> hyperlink: string
```

`MayReturnNothing`

### GetUserWaypointPositionForMap

```lua
C_Map.GetUserWaypointPositionForMap(uiMapID: number) -> mapPosition: vector2
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `mapPosition` | `vector2` | `Mixin=Vector2DMixin` |

### GetWorldPosFromMapPos

```lua
C_Map.GetWorldPosFromMapPos(uiMapID: number, mapPosition: vector2) -> continentID: number, worldPosition: vector2
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `uiMapID` | `number` |  |
| `mapPosition` | `vector2` | `Mixin=Vector2DMixin` |

Returns:

| Name | Type | Notes |
|---|---|---|
| `continentID` | `number` |  |
| `worldPosition` | `vector2` | `Mixin=Vector2DMixin` |

### HasUserWaypoint

```lua
C_Map.HasUserWaypoint() -> hasUserWaypoint: bool
```

### IsCityMap

```lua
C_Map.IsCityMap(uiMapID: number) -> isCityMap: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsMapValidForNavBarDropdown

```lua
C_Map.IsMapValidForNavBarDropdown(uiMapID: number) -> isValid: bool
```

`SecretArguments=AllowedWhenUntainted`

### MapHasArt

```lua
C_Map.MapHasArt(uiMapID: number) -> hasArt: bool
```

`SecretArguments=AllowedWhenUntainted`

### OpenWorldMap

```lua
C_Map.OpenWorldMap(uiMapID: number?)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### RequestPreloadMap

```lua
C_Map.RequestPreloadMap(uiMapID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetUserWaypoint

```lua
C_Map.SetUserWaypoint(point: UiMapPoint) -> wasSet: bool
```

`SecretArguments=AllowedWhenUntainted`

## Events

### NEW_WMO_CHUNK

```lua
NEW_WMO_CHUNK()
```

`SynchronousEvent`

### PLAYER_MAP_CHANGED

```lua
PLAYER_MAP_CHANGED(oldMapID: number, newMapID: number)
```

`SynchronousEvent`

### USER_WAYPOINT_UPDATED

```lua
USER_WAYPOINT_UPDATED()
```

`SynchronousEvent`

### WORLD_MAP_OPEN

```lua
WORLD_MAP_OPEN(uiMapID: number?)
```

`SynchronousEvent`

### ZONE_CHANGED

```lua
ZONE_CHANGED()
```

`SynchronousEvent`

### ZONE_CHANGED_INDOORS

```lua
ZONE_CHANGED_INDOORS()
```

`SynchronousEvent`

### ZONE_CHANGED_NEW_AREA

```lua
ZONE_CHANGED_NEW_AREA()
```

`SynchronousEvent`

## Types

### MapBannerInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `areaPoiID` | `number` |  |
| `name` | `cstring` |  |
| `atlasName` | `string` |  |
| `uiTextureKit` | `textureKit?` |  |

### MapLinkInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `areaPoiID` | `number` |  |
| `position` | `vector2` | `Mixin=Vector2DMixin` |
| `name` | `cstring` |  |
| `atlasName` | `string` |  |
| `linkedUiMapID` | `number` |  |

### UiMapDetails

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `mapID` | `number` |  |
| `name` | `cstring` |  |
| `mapType` | `UIMapType` |  |
| `parentMapID` | `number` |  |
| `flags` | `UIMapFlag` |  |

### UiMapGroupMemberInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `mapID` | `number` |  |
| `relativeHeightIndex` | `number` |  |
| `name` | `cstring` |  |

### UiMapHighlightInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `fileDataID` | `fileID` |  |
| `atlasID` | `textureAtlas` |  |
| `texturePercentageX` | `number` |  |
| `texturePercentageY` | `number` |  |
| `textureX` | `number` |  |
| `textureY` | `number` |  |
| `scrollChildX` | `number` |  |
| `scrollChildY` | `number` |  |

### UiMapLayerInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `layerWidth` | `number` |  |
| `layerHeight` | `number` |  |
| `tileWidth` | `number` |  |
| `tileHeight` | `number` |  |
| `minScale` | `number` |  |
| `maxScale` | `number` |  |
| `additionalZoomSteps` | `number` |  |
