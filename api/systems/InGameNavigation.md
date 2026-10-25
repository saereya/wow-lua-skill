# InGameNavigation

Namespace `C_Navigation` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/ingamenavigationdocumentation.lua` (FileDataID 4637113)

## Functions

### GetDistance

```lua
C_Navigation.GetDistance() -> distance: number
```

### GetFrame

```lua
C_Navigation.GetFrame() -> frame: ScriptRegion?
```

### GetNearestPartyMemberToken

```lua
C_Navigation.GetNearestPartyMemberToken() -> unitToken: cstring
```

`HasRestrictions`

### GetNextWaypointForMap

```lua
C_Navigation.GetNextWaypointForMap(uiMapID: number) -> x: number, y: number, waypointDescription: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetTargetState

```lua
C_Navigation.GetTargetState() -> state: NavigationState
```

### HasValidScreenPosition

```lua
C_Navigation.HasValidScreenPosition() -> hasValidScreenPosition: bool
```

### WasClampedToScreen

```lua
C_Navigation.WasClampedToScreen() -> wasClamped: bool
```

## Events

### NAVIGATION_DESTINATION_REACHED

```lua
NAVIGATION_DESTINATION_REACHED(isWaypoint: bool)
```

`SynchronousEvent`

### NAVIGATION_FRAME_CREATED

```lua
NAVIGATION_FRAME_CREATED(region: ScriptRegion)
```

`SynchronousEvent`

### NAVIGATION_FRAME_DESTROYED

```lua
NAVIGATION_FRAME_DESTROYED()
```

`SynchronousEvent`

## Types

### NavigationState

*Enumeration* · 4 values, 0..3

Access values as `Enum.NavigationState.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Invalid` | `NavigationState` | = 0 |
| `Occluded` | `NavigationState` | = 1 |
| `InRange` | `NavigationState` | = 2 |
| `Disabled` | `NavigationState` | = 3 |
