# LossOfControl

Namespace `C_LossOfControl` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/lossofcontroldocumentation.lua` (FileDataID 4637135)

## Functions

### GetActiveLossOfControlData

```lua
C_LossOfControl.GetActiveLossOfControlData(index: luaIndex) -> event: LossOfControlData?
```

`SecretArguments=AllowedWhenUntainted`

### GetActiveLossOfControlDataByUnit

```lua
C_LossOfControl.GetActiveLossOfControlDataByUnit(unitToken: UnitToken, index: luaIndex) -> event: LossOfControlData?
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenLossOfControlInfoRestricted`

### GetActiveLossOfControlDataCount

```lua
C_LossOfControl.GetActiveLossOfControlDataCount() -> count: number
```

### GetActiveLossOfControlDataCountByUnit

```lua
C_LossOfControl.GetActiveLossOfControlDataCountByUnit(unitToken: UnitToken) -> count: number
```

`SecretArguments=AllowedWhenUntainted`

### GetActiveLossOfControlDuration

```lua
C_LossOfControl.GetActiveLossOfControlDuration(unitToken: UnitToken, index: luaIndex) -> duration: LuaDurationObject?
```

`SecretArguments=AllowedWhenUntainted`

## Events

### LOSS_OF_CONTROL_ADDED

```lua
LOSS_OF_CONTROL_ADDED(unitTarget: UnitTokenVariant, effectIndex: luaIndex)
```

`SynchronousEvent`

### LOSS_OF_CONTROL_COMMENTATOR_ADDED

```lua
LOSS_OF_CONTROL_COMMENTATOR_ADDED(victim: WOWGUID, effectIndex: luaIndex)
```

`SynchronousEvent`

### LOSS_OF_CONTROL_COMMENTATOR_UPDATE

```lua
LOSS_OF_CONTROL_COMMENTATOR_UPDATE(victim: WOWGUID)
```

`SynchronousEvent` `UniqueEvent`

### LOSS_OF_CONTROL_UPDATE

```lua
LOSS_OF_CONTROL_UPDATE(unitTarget: UnitTokenVariant)
```

`SynchronousEvent` `UniqueEvent`

### PLAYER_CONTROL_GAINED

```lua
PLAYER_CONTROL_GAINED()
```

`SynchronousEvent`

### PLAYER_CONTROL_LOST

```lua
PLAYER_CONTROL_LOST()
```

`SynchronousEvent`

## Types

### LossOfControlData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `locType` | `cstring` |  |
| `spellID` | `number` |  |
| `displayText` | `cstring` |  |
| `iconTexture` | `number` |  |
| `startTime` | `number?` |  |
| `timeRemaining` | `number?` |  |
| `duration` | `number?` |  |
| `lockoutSchool` | `number` |  |
| `priority` | `number` | `NeverSecret` |
| `displayType` | `number` | `NeverSecret` |
| `auraInstanceID` | `number?` |  |
