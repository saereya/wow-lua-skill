# EncounterInfo

Namespace `C_EncounterInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/encounterinfodocumentation.lua` (FileDataID 4637083)

## Events

### BOSS_KILL

```lua
BOSS_KILL(encounterID: number, encounterName: cstring)
```

`SynchronousEvent`

### DISABLE_LOW_LEVEL_RAID

```lua
DISABLE_LOW_LEVEL_RAID()
```

`SynchronousEvent`

### ENABLE_LOW_LEVEL_RAID

```lua
ENABLE_LOW_LEVEL_RAID()
```

`SynchronousEvent`

### ENCOUNTER_END

```lua
ENCOUNTER_END(encounterID: number, encounterName: cstring, difficultyID: number, groupSize: number, success: number, encounterUnitStatus: EncounterUnitStatus[])
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `encounterID` | `number` |  |
| `encounterName` | `cstring` |  |
| `difficultyID` | `number` |  |
| `groupSize` | `number` |  |
| `success` | `number` |  |
| `encounterUnitStatus` | `EncounterUnitStatus[]` | List of all boss units engaged during this encounter. |

### ENCOUNTER_START

```lua
ENCOUNTER_START(encounterID: number, encounterName: cstring, difficultyID: number, groupSize: number)
```

`SynchronousEvent`

### INSTANCE_LOCK_START

```lua
INSTANCE_LOCK_START()
```

`SynchronousEvent`

### INSTANCE_LOCK_STOP

```lua
INSTANCE_LOCK_STOP()
```

`SynchronousEvent`

### INSTANCE_LOCK_WARNING

```lua
INSTANCE_LOCK_WARNING()
```

`SynchronousEvent`

### RAID_TARGET_UPDATE

```lua
RAID_TARGET_UPDATE()
```

`SynchronousEvent`

### UPDATE_INSTANCE_INFO

```lua
UPDATE_INSTANCE_INFO()
```

`SynchronousEvent`

## Types

### EncounterUnitStatus

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `creatureID` | `number` |  |
| `creatureName` | `string` |  |
| `remainingHealthPercent` | `number` |  |
