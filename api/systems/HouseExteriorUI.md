# HouseExteriorUI

Namespace `C_HouseExterior` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/houseexterioruidocumentation.lua` (FileDataID 7289997)

## Functions

### CancelActiveExteriorEditing

```lua
C_HouseExterior.CancelActiveExteriorEditing()
```

Cancels all in-progress editing of house exterior fixtures, which will deselect any active targets

### GetCoreFixtureOptionsInfo

```lua
C_HouseExterior.GetCoreFixtureOptionsInfo(coreFixtureType: HousingFixtureType) -> coreFixtureOptionsInfo: HousingCoreFixtureInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetCurrentHouseExteriorSize

```lua
C_HouseExterior.GetCurrentHouseExteriorSize() -> houseExteriorSize: HousingFixtureSize?
```

### GetCurrentHouseExteriorType

```lua
C_HouseExterior.GetCurrentHouseExteriorType() -> houseExteriorTypeID: number?, houseExteriorTypeName: cstring?
```

### GetHouseExteriorSizeOptions

```lua
C_HouseExterior.GetHouseExteriorSizeOptions() -> options: HouseExteriorSizeOptionsInfo?
```

### GetHouseExteriorTypeOptions

```lua
C_HouseExterior.GetHouseExteriorTypeOptions() -> options: HouseExteriorTypeOptionsInfo?
```

### GetSelectedFixturePointInfo

```lua
C_HouseExterior.GetSelectedFixturePointInfo() -> fixturePointInfo: HousingFixturePointInfo?
```

### HasHoveredFixture

```lua
C_HouseExterior.HasHoveredFixture() -> anyHoveredFixture: bool
```

### HasSelectedFixturePoint

```lua
C_HouseExterior.HasSelectedFixturePoint() -> anySelectedFixturePoint: bool
```

### IsAnyDecorAttachedToCoreFixture

```lua
C_HouseExterior.IsAnyDecorAttachedToCoreFixture(coreFixtureType: HousingFixtureType) -> anyAttachedDecor: bool
```

Returns true if any decor is attached to the specified core fixture type, OR any child fixtures attached to it; Will also return false if the type provided is not a core fixture type, or if not in Exterior Customization mode on an owned plot

`SecretArguments=AllowedWhenUntainted`

### IsAnyDecorAttachedToDoor

```lua
C_HouseExterior.IsAnyDecorAttachedToDoor() -> anyAttachedDecor: bool
```

Returns true if any decor is attached to the current House Exterior's door; Will also return false if not in Exterior Customization mode on an owned plot

### IsAnyDecorAttachedToHouseExterior

```lua
C_HouseExterior.IsAnyDecorAttachedToHouseExterior() -> anyAttachedDecor: bool
```

Returns true if any decor is attached to any component of the current House Exterior; Will also return false if not in House Exterior Customization mode on an owned Plot

### IsAnyDecorAttachedToSelectedFixturePoint

```lua
C_HouseExterior.IsAnyDecorAttachedToSelectedFixturePoint() -> anyAttachedDecor: bool
```

Returns true if any decor is attached to the Fixture occupying the currently selected fixture point; Will also return false if no point is currently selected, or if there is currently no Fixture there

### IsExteriorDecorHidden

```lua
C_HouseExterior.IsExteriorDecorHidden() -> decorHidden: bool
```

### RemoveFixtureFromSelectedPoint

```lua
C_HouseExterior.RemoveFixtureFromSelectedPoint(attachedDecorAction: HousingFixtureDecorAction)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `attachedDecorAction` | `HousingFixtureDecorAction` | default `"Store"`; What to do with any decor currently attached to the fixture |

### SelectCoreFixtureOption

```lua
C_HouseExterior.SelectCoreFixtureOption(fixtureID: number, attachedDecorAction: HousingFixtureDecorAction)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `fixtureID` | `number` |  |
| `attachedDecorAction` | `HousingFixtureDecorAction` | default `"Store"`; What to do with any decor attached to the old core fixture; If the fixture being swapped is a variant (ie recolor) of the existing one, attached decor will always be reparented directly to the new one |

### SelectFixtureOption

```lua
C_HouseExterior.SelectFixtureOption(fixtureID: number, attachedDecorAction: HousingFixtureDecorAction)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `fixtureID` | `number` |  |
| `attachedDecorAction` | `HousingFixtureDecorAction` | default `"Store"`; If this fixture choice is replacing an existing one that has decor attached, what to do with any decor attached to the old one |

### SetExteriorDecorHidden

```lua
C_HouseExterior.SetExteriorDecorHidden(decorHidden: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetHouseExteriorSize

```lua
C_HouseExterior.SetHouseExteriorSize(size: HousingFixtureSize, attachedDecorAction: HousingFixtureDecorAction)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `size` | `HousingFixtureSize` |  |
| `attachedDecorAction` | `HousingFixtureDecorAction` | default `"Store"`; What to do with decor attached to any of the house's existing exterior components |

### SetHouseExteriorType

```lua
C_HouseExterior.SetHouseExteriorType(houseExteriorTypeID: number, attachedDecorAction: HousingFixtureDecorAction)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `houseExteriorTypeID` | `number` |  |
| `attachedDecorAction` | `HousingFixtureDecorAction` | default `"Store"`; What to do with decor attached to any of the house's existing exterior components |

## Events

### HOUSE_EXTERIOR_DECOR_HIDDEN_CHANGED

```lua
HOUSE_EXTERIOR_DECOR_HIDDEN_CHANGED(isDecorHidden: bool)
```

`SynchronousEvent`

### HOUSE_EXTERIOR_TYPE_UNLOCKED

```lua
HOUSE_EXTERIOR_TYPE_UNLOCKED(fixtureID: number)
```

`UniqueEvent`

### HOUSING_CORE_FIXTURE_CHANGED

```lua
HOUSING_CORE_FIXTURE_CHANGED(coreFixtureType: HousingFixtureType)
```

`UniqueEvent`

### HOUSING_FIXTURE_HOVER_CHANGED

```lua
HOUSING_FIXTURE_HOVER_CHANGED(anyHovered: bool)
```

`SynchronousEvent`

### HOUSING_FIXTURE_POINT_FRAME_ADDED

```lua
HOUSING_FIXTURE_POINT_FRAME_ADDED(pointFrame: HousingFixturePointFrame)
```

`SynchronousEvent`

### HOUSING_FIXTURE_POINT_FRAME_RELEASED

```lua
HOUSING_FIXTURE_POINT_FRAME_RELEASED(pointFrame: HousingFixturePointFrame)
```

`SynchronousEvent`

### HOUSING_FIXTURE_POINT_FRAMES_RELEASED

```lua
HOUSING_FIXTURE_POINT_FRAMES_RELEASED()
```

`SynchronousEvent`

### HOUSING_FIXTURE_POINT_SELECTION_CHANGED

```lua
HOUSING_FIXTURE_POINT_SELECTION_CHANGED(hasSelection: bool)
```

`SynchronousEvent`

### HOUSING_FIXTURE_UNLOCKED

```lua
HOUSING_FIXTURE_UNLOCKED(fixtureID: number)
```

`UniqueEvent`

### HOUSING_SET_EXTERIOR_HOUSE_SIZE_RESPONSE

```lua
HOUSING_SET_EXTERIOR_HOUSE_SIZE_RESPONSE(result: HousingResult)
```

`SynchronousEvent`

### HOUSING_SET_EXTERIOR_HOUSE_TYPE_RESPONSE

```lua
HOUSING_SET_EXTERIOR_HOUSE_TYPE_RESPONSE(result: HousingResult)
```

`SynchronousEvent`

### HOUSING_SET_FIXTURE_RESPONSE

```lua
HOUSING_SET_FIXTURE_RESPONSE(result: HousingResult)
```

`SynchronousEvent`
