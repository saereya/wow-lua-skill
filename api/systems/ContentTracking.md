# ContentTracking

Namespace `C_ContentTracking` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/contenttrackingdocumentation.lua` (FileDataID 5126422)

## Functions

### GetBestMapForTrackable

```lua
C_ContentTracking.GetBestMapForTrackable(trackableType: ContentTrackingType, trackableID: number, ignoreWaypoint: bool) -> result: ContentTrackingResult, mapID: number?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `trackableType` | `ContentTrackingType` |  |
| `trackableID` | `number` |  |
| `ignoreWaypoint` | `bool` | default `false` |

### GetCollectableSourceTrackingEnabled

```lua
C_ContentTracking.GetCollectableSourceTrackingEnabled() -> isEnabled: bool
```

### GetCollectableSourceTypes

```lua
C_ContentTracking.GetCollectableSourceTypes() -> collectableSourceTypes: ContentTrackingType[]
```

### GetCurrentTrackingTarget

```lua
C_ContentTracking.GetCurrentTrackingTarget(type: ContentTrackingType, id: number) -> targetType: ContentTrackingTargetType, targetID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetEncounterTrackingInfo

```lua
C_ContentTracking.GetEncounterTrackingInfo(journalEncounterID: number) -> trackingInfo: EncounterTrackingInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetNextWaypointForTrackable

```lua
C_ContentTracking.GetNextWaypointForTrackable(trackableType: ContentTrackingType, trackableID: number, uiMapID: number) -> result: ContentTrackingResult, mapInfo: ContentTrackingMapInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetObjectiveText

```lua
C_ContentTracking.GetObjectiveText(targetType: ContentTrackingTargetType, targetID: number, includeHyperlinks: bool) -> objectiveText: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `targetType` | `ContentTrackingTargetType` |  |
| `targetID` | `number` |  |
| `includeHyperlinks` | `bool` | default `true` |

### GetTitle

```lua
C_ContentTracking.GetTitle(trackableType: ContentTrackingType, trackableID: number) -> title: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetTrackablesOnMap

```lua
C_ContentTracking.GetTrackablesOnMap(trackableType: ContentTrackingType, uiMapID: number) -> result: ContentTrackingResult, trackableMapInfos: ContentTrackingMapInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetTrackedIDs

```lua
C_ContentTracking.GetTrackedIDs(trackableType: ContentTrackingType) -> entryIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetVendorTrackingInfo

```lua
C_ContentTracking.GetVendorTrackingInfo(collectableEntryID: number) -> vendorTrackingInfo: VendorTrackingInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetWaypointText

```lua
C_ContentTracking.GetWaypointText(trackableType: ContentTrackingType, trackableID: number) -> waypointText: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### IsNavigable

```lua
C_ContentTracking.IsNavigable(trackableType: ContentTrackingType, trackableID: number) -> result: ContentTrackingResult, isNavigable: bool
```

If successful, returns if the trackable is either on your current map, or if we're able to determine a route to that map from your location via waypoints.

`SecretArguments=AllowedWhenUntainted`

### IsTrackable

```lua
C_ContentTracking.IsTrackable(type: ContentTrackingType, id: number) -> isTrackable: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsTracking

```lua
C_ContentTracking.IsTracking(type: ContentTrackingType, id: number) -> isTracking: bool
```

`SecretArguments=AllowedWhenUntainted`

### StartTracking

```lua
C_ContentTracking.StartTracking(type: ContentTrackingType, id: number) -> error: ContentTrackingError?
```

`SecretArguments=AllowedWhenUntainted`

### StopTracking

```lua
C_ContentTracking.StopTracking(type: ContentTrackingType, id: number, stopType: ContentTrackingStopType)
```

`SecretArguments=AllowedWhenUntainted`

### ToggleTracking

```lua
C_ContentTracking.ToggleTracking(type: ContentTrackingType, id: number, stopType: ContentTrackingStopType) -> error: ContentTrackingError?
```

`SecretArguments=AllowedWhenUntainted`

## Events

### CONTENT_TRACKING_IS_ENABLED_UPDATE

```lua
CONTENT_TRACKING_IS_ENABLED_UPDATE(isEnabled: bool)
```

`SynchronousEvent`

### CONTENT_TRACKING_LIST_UPDATE

```lua
CONTENT_TRACKING_LIST_UPDATE()
```

`SynchronousEvent`

### CONTENT_TRACKING_UPDATE

```lua
CONTENT_TRACKING_UPDATE(type: ContentTrackingType, id: number, isTracked: bool)
```

`SynchronousEvent`

### TRACKABLE_INFO_UPDATE

```lua
TRACKABLE_INFO_UPDATE(type: ContentTrackingType, id: number)
```

`SynchronousEvent`

### TRACKING_TARGET_INFO_UPDATE

```lua
TRACKING_TARGET_INFO_UPDATE(targetType: ContentTrackingTargetType, targetID: number)
```

`SynchronousEvent`
