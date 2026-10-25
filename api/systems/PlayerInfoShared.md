# PlayerInfoShared

source `interface/addons/blizzard_apidocumentationgenerated/playerinfoshareddocumentation.lua` (FileDataID 4637821)

## Types

### CharacterAlternateFormData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `raceID` | `number` |  |
| `name` | `cstring` |  |
| `fileName` | `cstring` |  |
| `createScreenIconAtlas` | `textureAtlas` |  |

### PlayerInfoCharacterData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `fileName` | `cstring` |  |
| `alternateFormRaceData` | `CharacterAlternateFormData?` |  |
| `createScreenIconAtlas` | `textureAtlas` |  |
| `sex` | `UnitSex` |  |
