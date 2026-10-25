# Instance

Global functions · environment All · source `interface/addons/blizzard_apidocumentationgenerated/instancedocumentation.lua` (FileDataID 5559340)

## Functions

### CanChangePlayerDifficulty

```lua
CanChangePlayerDifficulty() -> canChange: bool, notOnCooldown: bool
```

`MayReturnNothing`

### CanMapChangeDifficulty

```lua
CanMapChangeDifficulty(mapID: number?) -> canChange: bool
```

`SecretArguments=AllowedWhenUntainted`

### CanShowResetInstances

```lua
CanShowResetInstances() -> result: bool
```

### GetBaseDifficultyID

```lua
GetBaseDifficultyID(difficultyID: number) -> baseDifficultyID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetDifficultyInfo

```lua
GetDifficultyInfo(difficultyID: number) -> name: cstring, instanceType: cstring, isHeroic: bool, isChallengeMode: bool, displayHeroic: bool, displayMythic: bool, toggleDifficultyID: number?, isLFR: bool, minPlayers: number?, maxPlayers: number?, isUserSelectable: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetDungeonDifficultyID

```lua
GetDungeonDifficultyID() -> result: number
```

### GetInstanceBootTimeRemaining

```lua
GetInstanceBootTimeRemaining() -> result: number
```

### GetInstanceInfo

```lua
GetInstanceInfo() -> name: cstring, instanceType: cstring, difficultyID: number, difficultyName: cstring, maxPlayers: number, dynamicDifficulty: number, isDynamic: bool?, instanceID: number, instanceGroupSize: number, lfgDungeonID: number?, hasWorldTier: bool
```

Returns:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `instanceType` | `cstring` |  |
| `difficultyID` | `number` |  |
| `difficultyName` | `cstring` |  |
| `maxPlayers` | `number` |  |
| `dynamicDifficulty` | `number` |  |
| `isDynamic` | `bool?` |  |
| `instanceID` | `number` |  |
| `instanceGroupSize` | `number` |  |
| `lfgDungeonID` | `number?` |  |
| `hasWorldTier` | `bool` | default `false` |

### GetInstanceLockTimeRemaining

```lua
GetInstanceLockTimeRemaining() -> timeLeft: number, extending: bool, encountersTotal: number, encountersCompleted: number
```

### GetInstanceLockTimeRemainingEncounter

```lua
GetInstanceLockTimeRemainingEncounter(encounterIndex: luaIndex) -> encounterName: cstring, texture: cstring, isKilled: bool, ineligible: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetLegacyRaidDifficultyID

```lua
GetLegacyRaidDifficultyID() -> result: number?
```

### GetRaidDifficultyID

```lua
GetRaidDifficultyID() -> result: number?
```

### IsInInstance

```lua
IsInInstance() -> isInInstance: bool, instanceType: cstring
```

### IsLegacyDifficulty

```lua
IsLegacyDifficulty(difficultyID: number) -> result: bool?
```

`SecretArguments=AllowedWhenUntainted`

### ResetInstances

```lua
ResetInstances()
```

### SetDungeonDifficultyID

```lua
SetDungeonDifficultyID(difficultyID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetLegacyRaidDifficultyID

```lua
SetLegacyRaidDifficultyID(difficultyID: number, force: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `difficultyID` | `number` |  |
| `force` | `bool` | default `false` |

### SetRaidDifficultyID

```lua
SetRaidDifficultyID(difficultyID: number, force: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `difficultyID` | `number` |  |
| `force` | `bool` | default `false` |

## Types

### DifficultyInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `instanceType` | `cstring` |  |
| `isHeroic` | `bool` |  |
| `isChallengeMode` | `bool` |  |
| `displayHeroic` | `bool` |  |
| `displayMythic` | `bool` |  |
| `toggleDifficultyID` | `number?` |  |
| `isLFR` | `bool` |  |
| `minPlayers` | `number?` |  |
| `maxPlayers` | `number?` |  |
| `isUserSelectable` | `bool` |  |

### DungeonEncounterInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `encounterName` | `cstring` |  |
| `texture` | `cstring` |  |
| `isKilled` | `bool` |  |
| `ineligible` | `bool` |  |

### InstanceInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `instanceType` | `cstring` |  |
| `difficultyID` | `number` |  |
| `difficultyName` | `cstring` |  |
| `maxPlayers` | `number` |  |
| `dynamicDifficulty` | `number` |  |
| `isDynamic` | `bool?` |  |
| `instanceID` | `number` |  |
| `instanceGroupSize` | `number` |  |
| `lfgDungeonID` | `number?` |  |
| `hasWorldTier` | `bool` | default `false` |
