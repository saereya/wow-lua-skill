# DamageMeter

Namespace `C_DamageMeter` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/damagemeterdocumentation.lua` (FileDataID 7494690)

## Functions

### GetAvailableCombatSessions

```lua
C_DamageMeter.GetAvailableCombatSessions() -> availableSessions: DamageMeterAvailableCombatSession[]
```

Returns a list of combat sessions currently being tracked.

### GetCombatSessionFromID

```lua
C_DamageMeter.GetCombatSessionFromID(sessionID: number, type: DamageMeterType) -> session: DamageMeterCombatSession
```

Returns the data for the player's combat session with the specified ID.

`SecretArguments=AllowedWhenUntainted` `SecretWhenInCombat`

### GetCombatSessionFromType

```lua
C_DamageMeter.GetCombatSessionFromType(sessionType: DamageMeterSessionType, type: DamageMeterType) -> session: DamageMeterCombatSession
```

Returns the data for the player's current combat session.

`SecretArguments=AllowedWhenUntainted` `SecretWhenInCombat`

### GetCombatSessionSourceFromID

```lua
C_DamageMeter.GetCombatSessionSourceFromID(sessionID: number, type: DamageMeterType, sourceGUID: WOWGUID?, sourceCreatureID: number?) -> sessionSource: DamageMeterCombatSessionSource
```

Returns the data for a single source (unit) in the player's current combat session with the specified ID.

`SecretArguments=AllowedWhenUntainted` `SecretWhenInCombat`

### GetCombatSessionSourceFromType

```lua
C_DamageMeter.GetCombatSessionSourceFromType(sessionType: DamageMeterSessionType, type: DamageMeterType, sourceGUID: WOWGUID?, sourceCreatureID: number?) -> sessionSource: DamageMeterCombatSessionSource
```

Returns the data for a single source (unit) in the player's current combat session.

`SecretArguments=AllowedWhenUntainted` `SecretWhenInCombat`

### GetSessionDurationSeconds

```lua
C_DamageMeter.GetSessionDurationSeconds(sessionType: DamageMeterSessionType) -> durationSeconds: number?
```

Returns the amount of time a combat session has lasted

`SecretArguments=AllowedWhenUntainted`

### IsDamageMeterAvailable

```lua
C_DamageMeter.IsDamageMeterAvailable() -> isAvailable: bool, failureReason: string
```

Returns whether the player can enable and use the Damage Meter.

### ResetAllCombatSessions

```lua
C_DamageMeter.ResetAllCombatSessions()
```

Clears the data for all the player's combat sessions.

## Events

### DAMAGE_METER_COMBAT_SESSION_UPDATED

```lua
DAMAGE_METER_COMBAT_SESSION_UPDATED(type: DamageMeterType, sessionID: number)
```

`UniqueEvent`

### DAMAGE_METER_CURRENT_SESSION_UPDATED

```lua
DAMAGE_METER_CURRENT_SESSION_UPDATED()
```

`UniqueEvent`

### DAMAGE_METER_RESET

```lua
DAMAGE_METER_RESET()
```

`UniqueEvent`

## Types

### DamageMeterAvailableCombatSession

*Structure*

Data for a combat session currently being tracked.

Fields:

| Name | Type | Notes |
|---|---|---|
| `sessionID` | `number` |  |
| `name` | `cstring` |  |
| `durationSeconds` | `number?` |  |

### DamageMeterCombatSession

*Structure*

Aggregated data for all sources (units) in a damage meter combat session.

Fields:

| Name | Type | Notes |
|---|---|---|
| `combatSources` | `DamageMeterCombatSource[]` |  |
| `maxAmount` | `number` | default `0` |
| `totalAmount` | `number` | default `0` |
| `durationSeconds` | `number?` |  |

### DamageMeterCombatSessionSource

*Structure*

Data for a single source (unit) in a combat session.

Fields:

| Name | Type | Notes |
|---|---|---|
| `combatSpells` | `DamageMeterCombatSpell[]` |  |
| `maxAmount` | `number` | default `0` |
| `totalAmount` | `number` | default `0` |

### DamageMeterCombatSource

*Structure*

Aggregated data for a single source (unit) in a damage meter combat session.

Fields:

| Name | Type | Notes |
|---|---|---|
| `sourceGUID` | `WOWGUID?` | `ConditionalSecret` |
| `sourceCreatureID` | `number?` |  |
| `name` | `cstring` | `ConditionalSecret` |
| `classFilename` | `cstring` | `NeverSecret` |
| `specIconID` | `fileID` | `NeverSecret` |
| `totalAmount` | `number` |  |
| `amountPerSecond` | `number` |  |
| `isLocalPlayer` | `bool` | `NeverSecret` |
| `deathRecapID` | `number` | `NeverSecret` |
| `deathTimeSeconds` | `number` |  |
| `classification` | `cstring` | `NeverSecret` |
| `sourceDisplayType` | `DamageMeterSourceDisplayType` |  |
| `factionGroup` | `cstring?` |  |

### DamageMeterCombatSpell

*Structure*

Aggregated data for all spells of the same ID cast by a single source (unit) in a combat session.

Fields:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `number` |  |
| `totalAmount` | `number` |  |
| `amountPerSecond` | `number` |  |
| `creatureName` | `cstring` |  |
| `overkillAmount` | `number` |  |
| `isAvoidable` | `bool` |  |
| `isDeadly` | `bool` |  |
| `combatSpellDetails` | `DamageMeterCombatSpellUnitDetails` |  |

### DamageMeterCombatSpellUnitDetails

*Structure*

Amount for a single target for all casts of the same spellID by a single source (unit) in a combat session.

Fields:

| Name | Type | Notes |
|---|---|---|
| `unitName` | `cstring` |  |
| `unitClassFilename` | `cstring` | `NeverSecret` |
| `classification` | `cstring` | `NeverSecret` |
| `isPet` | `bool` |  |
| `isMob` | `bool` |  |
| `amount` | `number` |  |
| `specIconID` | `fileID` | `NeverSecret` |
