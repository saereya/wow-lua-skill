# ScenarioInfo

Namespace `C_ScenarioInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/scenarioinfodocumentation.lua` (FileDataID 4637200)

## Functions

### GetCriteriaInfo

```lua
C_ScenarioInfo.GetCriteriaInfo(criteriaIndex: number) -> scenarioCriteriaInfo: ScenarioCriteriaInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetCriteriaInfoByStep

```lua
C_ScenarioInfo.GetCriteriaInfoByStep(stepID: number, criteriaIndex: number) -> scenarioCriteriaInfo: ScenarioCriteriaInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetDisplayInfo

```lua
C_ScenarioInfo.GetDisplayInfo() -> info: ScenarioDisplayInfo
```

`MayReturnNothing`

### GetJailersTowerTypeString

```lua
C_ScenarioInfo.GetJailersTowerTypeString(runType: JailersTowerType) -> typeString: cstring?
```

`SecretArguments=AllowedWhenUntainted`

### GetScenarioIconInfo

```lua
C_ScenarioInfo.GetScenarioIconInfo(uiMapID: number) -> scenarioInfos: ScenarioIconInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetScenarioInfo

```lua
C_ScenarioInfo.GetScenarioInfo() -> scenarioInfo: ScenarioInformation
```

`MayReturnNothing`

### GetScenarioStepInfo

```lua
C_ScenarioInfo.GetScenarioStepInfo(scenarioStepID: number?) -> scenarioStepInfo: ScenarioStepInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetTieredEntranceActiveSpells

```lua
C_ScenarioInfo.GetTieredEntranceActiveSpells() -> spellIDs: number[]?
```

Returns list of active challenge spells if inside a tiered entrance scenario

### GetUnitCriteriaProgressValues

```lua
C_ScenarioInfo.GetUnitCriteriaProgressValues(unit: UnitToken) -> actualValue: number, percentValue: number, percentValueString: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretWhenUnitIdentityRestricted`

### IsTieredEntranceScenario

```lua
C_ScenarioInfo.IsTieredEntranceScenario() -> isTieredEntrance: bool
```

## Events

### JAILERS_TOWER_LEVEL_UPDATE

```lua
JAILERS_TOWER_LEVEL_UPDATE(level: number, type: JailersTowerType)
```

`SynchronousEvent`

### SCENARIO_BONUS_OBJECTIVE_COMPLETE

```lua
SCENARIO_BONUS_OBJECTIVE_COMPLETE(bonusObjectiveID: number)
```

`SynchronousEvent`

### SCENARIO_BONUS_VISIBILITY_UPDATE

```lua
SCENARIO_BONUS_VISIBILITY_UPDATE()
```

`SynchronousEvent`

### SCENARIO_COMPLETED

```lua
SCENARIO_COMPLETED(questID: number?, xp: number?, money: number?)
```

`SynchronousEvent`

### SCENARIO_CRITERIA_SHOW_STATE_UPDATE

```lua
SCENARIO_CRITERIA_SHOW_STATE_UPDATE(show: bool)
```

`SynchronousEvent`

### SCENARIO_CRITERIA_UPDATE

```lua
SCENARIO_CRITERIA_UPDATE(criteriaID: number)
```

`SynchronousEvent`

### SCENARIO_POI_UPDATE

```lua
SCENARIO_POI_UPDATE()
```

`SynchronousEvent`

### SCENARIO_SPELL_UPDATE

```lua
SCENARIO_SPELL_UPDATE()
```

`SynchronousEvent`

### SCENARIO_UPDATE

```lua
SCENARIO_UPDATE(newStep: bool?)
```

`SynchronousEvent`

## Types

### JailersTowerType

*Enumeration* · 15 values, 0..14

Access values as `Enum.JailersTowerType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `TwistingCorridors` | `JailersTowerType` | = 0 |
| `SkoldusHalls` | `JailersTowerType` | = 1 |
| `FractureChambers` | `JailersTowerType` | = 2 |
| `Soulforges` | `JailersTowerType` | = 3 |
| `Coldheart` | `JailersTowerType` | = 4 |
| `Mortregar` | `JailersTowerType` | = 5 |
| `UpperReaches` | `JailersTowerType` | = 6 |
| `ArkobanHall` | `JailersTowerType` | = 7 |
| `TormentChamberJaina` | `JailersTowerType` | = 8 |
| `TormentChamberThrall` | `JailersTowerType` | = 9 |
| `TormentChamberAnduin` | `JailersTowerType` | = 10 |
| `AdamantVaults` | `JailersTowerType` | = 11 |
| `ForgottenCatacombs` | `JailersTowerType` | = 12 |
| `Ossuary` | `JailersTowerType` | = 13 |
| `BossRush` | `JailersTowerType` | = 14 |

### ScenarioCriteriaInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `description` | `string` |  |
| `criteriaType` | `number` | default `0` |
| `completed` | `bool` | default `false` |
| `quantity` | `number` | default `0` |
| `totalQuantity` | `number` | default `0` |
| `flags` | `number` | default `0` |
| `assetID` | `number` | default `0` |
| `criteriaID` | `number` |  |
| `duration` | `number` | default `0` |
| `elapsed` | `number` | default `0` |
| `failed` | `bool` | default `false` |
| `isWeightedProgress` | `bool` | default `false` |
| `isFormatted` | `bool` | default `false` |
| `quantityString` | `string` |  |

### ScenarioDisplayInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `themeColor` | `colorRGB?` | `Mixin=ColorMixin` |
| `startSoundKitID` | `number?` |  |

### ScenarioIconInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `x` | `number` |  |
| `y` | `number` |  |
| `atlas` | `textureAtlas` |  |
| `description` | `cstring` |  |

### ScenarioInformation

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `currentStage` | `number` |  |
| `numStages` | `number` |  |
| `flags` | `number` |  |
| `isComplete` | `bool` |  |
| `xp` | `number` |  |
| `money` | `number` |  |
| `type` | `number` |  |
| `area` | `string` |  |
| `uiTextureKit` | `textureKit` |  |
| `scenarioID` | `number` |  |

### ScenarioStepInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `title` | `string` |  |
| `description` | `string` |  |
| `numCriteria` | `number` |  |
| `stepFailed` | `bool` |  |
| `isBonusStep` | `bool` |  |
| `isForCurrentStepOnly` | `bool` |  |
| `shouldShowBonusObjective` | `bool` |  |
| `spells` | `ScenarioStepSpellInfo[]` |  |
| `weightedProgress` | `number?` |  |
| `rewardQuestID` | `number` |  |
| `widgetSetID` | `number?` |  |
| `stepID` | `number` |  |

### ScenarioStepSpellInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `number` |  |
| `name` | `string` |  |
| `icon` | `number` |  |
