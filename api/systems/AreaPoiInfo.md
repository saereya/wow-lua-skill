# AreaPoiInfo

Namespace `C_AreaPoiInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/areapoiinfodocumentation.lua` (FileDataID 4637019)

## Functions

### GetAreaPOIForMap

```lua
C_AreaPoiInfo.GetAreaPOIForMap(uiMapID: number) -> areaPoiIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetAreaPOIInfo

```lua
C_AreaPoiInfo.GetAreaPOIInfo(uiMapID: number?, areaPoiID: number) -> poiInfo: AreaPOIInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetAreaPOISecondsLeft

```lua
C_AreaPoiInfo.GetAreaPOISecondsLeft(areaPoiID: number) -> secondsLeft: number
```

Returns the number of seconds until the POI expires.

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetDelvesForMap

```lua
C_AreaPoiInfo.GetDelvesForMap(uiMapID: number) -> areaPoiIDs: number[]
```

Returns all area POIInfos flagged as delves for the given map.

`SecretArguments=AllowedWhenUntainted`

### GetDragonridingRacesForMap

```lua
C_AreaPoiInfo.GetDragonridingRacesForMap(uiMapID: number) -> areaPoiIDs: number[]
```

Returns all area POIInfos flagged as dragonriding races for the given map.

`SecretArguments=AllowedWhenUntainted`

### GetEventsForMap

```lua
C_AreaPoiInfo.GetEventsForMap(uiMapID: number) -> areaPoiIDs: number[]
```

Returns all area POIInfos flagged as events for the given map.

`SecretArguments=AllowedWhenUntainted`

### GetQuestHubsForMap

```lua
C_AreaPoiInfo.GetQuestHubsForMap(uiMapID: number) -> areaPoiIDs: number[]
```

Returns all area POIInfos flagged as quest hubs for the given map.

`SecretArguments=AllowedWhenUntainted`

### IsAreaPOITimed

```lua
C_AreaPoiInfo.IsAreaPOITimed(areaPoiID: number) -> isTimed: bool, hideTimerInTooltip: bool?
```

This statically determines if the POI is timed, GetAreaPOITimeLeft retrieves the value from the server and may return nothing for long intervals

`SecretArguments=AllowedWhenUntainted`

## Events

### AREA_POIS_UPDATED

```lua
AREA_POIS_UPDATED()
```

`UniqueEvent`

## Types

### AreaPOIInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `areaPoiID` | `number` |  |
| `position` | `vector2` | `Mixin=Vector2DMixin` |
| `name` | `cstring` |  |
| `description` | `cstring?` |  |
| `linkedUiMapID` | `number?` |  |
| `textureIndex` | `number?` |  |
| `tooltipWidgetSet` | `number?` |  |
| `iconWidgetSet` | `number?` |  |
| `atlasName` | `string?` |  |
| `uiTextureKit` | `textureKit?` |  |
| `shouldGlow` | `bool` |  |
| `factionID` | `number?` |  |
| `isPrimaryMapForPOI` | `bool` |  |
| `isAlwaysOnFlightmap` | `bool` |  |
| `addPaddingAboveTooltipWidgets` | `bool?` |  |
| `highlightWorldQuestsOnHover` | `bool` |  |
| `highlightVignettesOnHover` | `bool` |  |
| `isCurrentEvent` | `bool` |  |
| `isSuppressible` | `bool` |  |
| `isLocked` | `bool` | default `false` |
