# CreatureInfo

Namespace `C_CreatureInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/creatureinfodocumentation.lua` (FileDataID 4637076)

## Functions

### GetClassInfo

```lua
C_CreatureInfo.GetClassInfo(classID: number) -> classInfo: ClassInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetCreatureFamilyIDs

```lua
C_CreatureInfo.GetCreatureFamilyIDs() -> creatureFamilyIDs: number[]
```

### GetCreatureFamilyInfo

```lua
C_CreatureInfo.GetCreatureFamilyInfo(creatureFamilyID: number) -> creatureFamilyInfo: CreatureFamilyInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetCreatureID

```lua
C_CreatureInfo.GetCreatureID(creatureGUID: WOWGUID) -> creatureID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetCreatureTypeIDs

```lua
C_CreatureInfo.GetCreatureTypeIDs() -> creatureTypeIDs: number[]
```

### GetCreatureTypeInfo

```lua
C_CreatureInfo.GetCreatureTypeInfo(creatureTypeID: number) -> creatureTypeInfo: CreatureTypeInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetFactionInfo

```lua
C_CreatureInfo.GetFactionInfo(raceID: number) -> factionInfo: FactionInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetRaceInfo

```lua
C_CreatureInfo.GetRaceInfo(raceID: number) -> raceInfo: RaceInfo?
```

`SecretArguments=AllowedWhenUntainted`

## Types

### ClassInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `className` | `string` |  |
| `classFile` | `string` |  |
| `classID` | `number` |  |

### CreatureFamilyInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `id` | `number` |  |
| `name` | `cstring` |  |
| `iconFile` | `fileID?` |  |

### CreatureTypeInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `id` | `number` |  |
| `name` | `cstring` |  |

### FactionInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `groupTag` | `cstring` |  |

### RaceInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `raceName` | `string` |  |
| `clientFileString` | `string` |  |
| `raceID` | `number` |  |
