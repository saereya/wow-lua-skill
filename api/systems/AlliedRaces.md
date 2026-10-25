# AlliedRaces

Namespace `C_AlliedRaces` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/alliedracesframedocumentation.lua` (FileDataID 4637012)

## Functions

### GetAllRacialAbilitiesFromID

```lua
C_AlliedRaces.GetAllRacialAbilitiesFromID(raceID: number) -> allDisplayInfo: AlliedRaceRacialAbility[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetRaceInfoByID

```lua
C_AlliedRaces.GetRaceInfoByID(raceID: number) -> info: AlliedRaceInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

## Events

### ALLIED_RACE_CLOSE

```lua
ALLIED_RACE_CLOSE()
```

`SynchronousEvent`

### ALLIED_RACE_OPEN

```lua
ALLIED_RACE_OPEN(raceID: number)
```

`SynchronousEvent`

## Types

### AlliedRaceInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `raceID` | `number` |  |
| `maleModelID` | `number` |  |
| `femaleModelID` | `number` |  |
| `achievementIds` | `number[]` |  |
| `maleName` | `cstring` |  |
| `femaleName` | `cstring` |  |
| `description` | `cstring` |  |
| `raceFileString` | `cstring` |  |
| `crestAtlas` | `textureAtlas` |  |
| `modelBackgroundAtlas` | `textureAtlas` |  |
| `bannerColor` | `colorRGB` | `Mixin=ColorMixin` |

### AlliedRaceRacialAbility

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `description` | `cstring` |  |
| `name` | `cstring` |  |
| `icon` | `fileID` |  |
