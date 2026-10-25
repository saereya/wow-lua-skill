# Vehicle

Namespace `C_Vehicle` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/vehicledocumentation.lua` (FileDataID 4637294)

## Events

### PLAYER_GAINS_VEHICLE_DATA

```lua
PLAYER_GAINS_VEHICLE_DATA(unitTarget: UnitTokenVariant, vehicleUIIndicatorID: number)
```

`SynchronousEvent`

### PLAYER_LOSES_VEHICLE_DATA

```lua
PLAYER_LOSES_VEHICLE_DATA(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_ENTERED_VEHICLE

```lua
UNIT_ENTERED_VEHICLE(unitTarget: UnitTokenVariant, showVehicleFrame: bool, isControlSeat: bool, vehicleUIIndicatorID: number, vehicleGUID: WOWGUID, mayChooseExit: bool, hasPitch: bool)
```

`SynchronousEvent`

### UNIT_ENTERING_VEHICLE

```lua
UNIT_ENTERING_VEHICLE(unitTarget: UnitTokenVariant, showVehicleFrame: bool, isControlSeat: bool, vehicleUIIndicatorID: number, vehicleGUID: WOWGUID, mayChooseExit: bool, hasPitch: bool)
```

`SynchronousEvent`

### UNIT_EXITED_VEHICLE

```lua
UNIT_EXITED_VEHICLE(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_EXITING_VEHICLE

```lua
UNIT_EXITING_VEHICLE(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### VEHICLE_ANGLE_SHOW

```lua
VEHICLE_ANGLE_SHOW(shouldShow: number?)
```

`SynchronousEvent`

### VEHICLE_PASSENGERS_CHANGED

```lua
VEHICLE_PASSENGERS_CHANGED()
```

`SynchronousEvent`

### VEHICLE_POWER_SHOW

```lua
VEHICLE_POWER_SHOW(shouldShow: number?)
```

`SynchronousEvent`

### VEHICLE_UPDATE

```lua
VEHICLE_UPDATE()
```

`SynchronousEvent`
