# SuperTrackManager

Namespace `C_SuperTrack` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/supertrackmanagerdocumentation.lua` (FileDataID 4637248)

## Functions

### ClearAllSuperTracked

```lua
C_SuperTrack.ClearAllSuperTracked()
```

### ClearSuperTrackedContent

```lua
C_SuperTrack.ClearSuperTrackedContent()
```

### ClearSuperTrackedMapPin

```lua
C_SuperTrack.ClearSuperTrackedMapPin()
```

### GetHighestPrioritySuperTrackingType

```lua
C_SuperTrack.GetHighestPrioritySuperTrackingType() -> type: SuperTrackingType?
```

### GetSuperTrackedContent

```lua
C_SuperTrack.GetSuperTrackedContent() -> trackableType: ContentTrackingType, trackableID: number
```

`MayReturnNothing`

### GetSuperTrackedItemName

```lua
C_SuperTrack.GetSuperTrackedItemName() -> name: string, description: string
```

`MayReturnNothing`

### GetSuperTrackedMapPin

```lua
C_SuperTrack.GetSuperTrackedMapPin() -> type: SuperTrackingMapPinType, typeID: number
```

`MayReturnNothing`

### GetSuperTrackedQuestID

```lua
C_SuperTrack.GetSuperTrackedQuestID() -> questID: number?
```

### GetSuperTrackedVignette

```lua
C_SuperTrack.GetSuperTrackedVignette() -> vignetteGUID: WOWGUID?
```

### IsSuperTrackingAnything

```lua
C_SuperTrack.IsSuperTrackingAnything() -> isSuperTracking: bool
```

### IsSuperTrackingContent

```lua
C_SuperTrack.IsSuperTrackingContent() -> isSuperTracking: bool
```

### IsSuperTrackingCorpse

```lua
C_SuperTrack.IsSuperTrackingCorpse() -> isSuperTracking: bool
```

### IsSuperTrackingMapPin

```lua
C_SuperTrack.IsSuperTrackingMapPin() -> isSuperTracking: bool
```

### IsSuperTrackingQuest

```lua
C_SuperTrack.IsSuperTrackingQuest() -> isSuperTracking: bool
```

### IsSuperTrackingUserWaypoint

```lua
C_SuperTrack.IsSuperTrackingUserWaypoint() -> isSuperTracking: bool
```

### SetSuperTrackedContent

```lua
C_SuperTrack.SetSuperTrackedContent(trackableType: ContentTrackingType, trackableID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetSuperTrackedMapPin

```lua
C_SuperTrack.SetSuperTrackedMapPin(type: SuperTrackingMapPinType, typeID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetSuperTrackedQuestID

```lua
C_SuperTrack.SetSuperTrackedQuestID(questID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetSuperTrackedUserWaypoint

```lua
C_SuperTrack.SetSuperTrackedUserWaypoint(superTracked: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetSuperTrackedVignette

```lua
C_SuperTrack.SetSuperTrackedVignette(vignetteGUID: WOWGUID)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### SUPER_TRACKING_CHANGED

```lua
SUPER_TRACKING_CHANGED()
```

`UniqueEvent`

### SUPER_TRACKING_PATH_UPDATED

```lua
SUPER_TRACKING_PATH_UPDATED()
```

`UniqueEvent`
