# InstanceEncounter

Namespace `C_InstanceEncounter` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/instanceencounterdocumentation.lua` (FileDataID 4637104)

## Functions

### IsEncounterInProgress

```lua
C_InstanceEncounter.IsEncounterInProgress() -> isInProgress: bool
```

### IsEncounterLimitingResurrections

```lua
C_InstanceEncounter.IsEncounterLimitingResurrections() -> isLimitingResurrections: bool
```

### IsEncounterSuppressingRelease

```lua
C_InstanceEncounter.IsEncounterSuppressingRelease() -> isSuppressingRelease: bool
```

### ShouldShowTimelineForEncounter

```lua
C_InstanceEncounter.ShouldShowTimelineForEncounter() -> shouldShow: bool
```

## Events

### ENCOUNTER_STATE_CHANGED

```lua
ENCOUNTER_STATE_CHANGED(isInProgress: bool)
```

Signaled when the in-progress state of an encounter changes.

`SynchronousEvent` `CallbackEvent`

### INSTANCE_ENCOUNTER_ADD_TIMER

```lua
INSTANCE_ENCOUNTER_ADD_TIMER(timeRemaining: number)
```

`SynchronousEvent`

### INSTANCE_ENCOUNTER_ENGAGE_UNIT

```lua
INSTANCE_ENCOUNTER_ENGAGE_UNIT()
```

`SynchronousEvent`

### INSTANCE_ENCOUNTER_OBJECTIVE_COMPLETE

```lua
INSTANCE_ENCOUNTER_OBJECTIVE_COMPLETE(objectiveID: number)
```

`SynchronousEvent`

### INSTANCE_ENCOUNTER_OBJECTIVE_START

```lua
INSTANCE_ENCOUNTER_OBJECTIVE_START(objectiveID: number, objectiveProgress: number)
```

`SynchronousEvent`

### INSTANCE_ENCOUNTER_OBJECTIVE_UPDATE

```lua
INSTANCE_ENCOUNTER_OBJECTIVE_UPDATE(objectiveID: number, objectiveProgress: number)
```

`SynchronousEvent`
