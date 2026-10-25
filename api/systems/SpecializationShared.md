# SpecializationShared

Global functions · environment All · source `interface/addons/blizzard_apidocumentationgenerated/specializationshareddocumentation.lua` (FileDataID 5201003)

## Functions

### GetSpecializationInfoForClassID

```lua
GetSpecializationInfoForClassID(classID: number, index: luaIndex, gender: UnitSex?) -> id: number, name: cstring, description: string, icon: fileID, role: cstring, recommended: bool, allowedForBoost: bool, masterySpell1: number?, masterySpell2: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetSpecializationInfoForSpecID

```lua
GetSpecializationInfoForSpecID(specID: number, gender: UnitSex?) -> id: number, name: cstring, description: string, icon: fileID, role: cstring, recommended: bool, allowedForBoost: bool, masterySpell1: number?, masterySpell2: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetSpecializationNameForSpecID

```lua
GetSpecializationNameForSpecID(specID: number, gender: UnitSex?) -> name: cstring?
```

`SecretArguments=AllowedWhenUntainted`

### GetSpecializationSystem

```lua
GetSpecializationSystem() -> system: SpecializationSystem
```

### HasLootSpecializations

```lua
HasLootSpecializations() -> hasLootSpecializations: bool
```

## Types

### SpecializationSystem

*Enumeration* · 2 values, 0..1

Access values as `Enum.SpecializationSystem.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `TalentTab` | `SpecializationSystem` | = 0 |
| `ChrSpecialization` | `SpecializationSystem` | = 1 |

### SpecializationInfoResult

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `id` | `number` |  |
| `name` | `cstring` |  |
| `description` | `string` |  |
| `icon` | `fileID` |  |
| `role` | `cstring` |  |
| `recommended` | `bool` |  |
| `allowedForBoost` | `bool` |  |
| `masterySpell1` | `number?` |  |
| `masterySpell2` | `number?` |  |
