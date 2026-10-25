# ContributionCollector

Namespace `C_ContributionCollector` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/contributioncollectordocumentation.lua` (FileDataID 4637070)

## Functions

### Close

```lua
C_ContributionCollector.Close()
```

### Contribute

```lua
C_ContributionCollector.Contribute(contributionID: number)
```

`SecretArguments=AllowedWhenUntainted`

### GetActive

```lua
C_ContributionCollector.GetActive() -> contributionID: number
```

Returns:

| Name | Type | Notes |
|---|---|---|
| `contributionID` | `number` | `StrideIndex=1` |

### GetAtlases

```lua
C_ContributionCollector.GetAtlases(contributionID: number) -> atlasName: textureAtlas[]
```

`SecretArguments=AllowedWhenUntainted`

### GetBuffs

```lua
C_ContributionCollector.GetBuffs(contributionID: number) -> spellID: number
```

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `number` | `StrideIndex=1` |

### GetContributionAppearance

```lua
C_ContributionCollector.GetContributionAppearance(contributionID: number, contributionState: ContributionState) -> appearance: ContributionAppearance?
```

`SecretArguments=AllowedWhenUntainted`

### GetContributionCollectorsForMap

```lua
C_ContributionCollector.GetContributionCollectorsForMap(uiMapID: number) -> contributionCollectors: ContributionMapInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetContributionResult

```lua
C_ContributionCollector.GetContributionResult(contributionID: number) -> result: ContributionResult
```

`SecretArguments=AllowedWhenUntainted`

### GetDescription

```lua
C_ContributionCollector.GetDescription(contributionID: number) -> description: cstring
```

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `description` | `cstring` | default `""` |

### GetManagedContributionsForCreatureID

```lua
C_ContributionCollector.GetManagedContributionsForCreatureID(creatureID: number) -> contributionID: number
```

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `contributionID` | `number` | `StrideIndex=1` |

### GetName

```lua
C_ContributionCollector.GetName(contributionID: number) -> name: cstring
```

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` | default `""` |

### GetOrderIndex

```lua
C_ContributionCollector.GetOrderIndex(contributionID: number) -> orderIndex: number
```

`SecretArguments=AllowedWhenUntainted`

### GetRequiredContributionCurrency

```lua
C_ContributionCollector.GetRequiredContributionCurrency(contributionID: number) -> currencyID: number, currencyAmount: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `currencyID` | `number` | default `0` |
| `currencyAmount` | `number` | default `0` |

### GetRequiredContributionItem

```lua
C_ContributionCollector.GetRequiredContributionItem(contributionID: number) -> itemID: number, itemCount: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `itemID` | `number` | default `0` |
| `itemCount` | `number` | default `0` |

### GetRewardQuestID

```lua
C_ContributionCollector.GetRewardQuestID(contributionID: number) -> questID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetState

```lua
C_ContributionCollector.GetState(contributionID: number) -> contributionState: ContributionState, contributionPercentageComplete: number, timeOfNextStateChange: time_t?, startTime: time_t
```

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `contributionState` | `ContributionState` | default `"None"` |
| `contributionPercentageComplete` | `number` |  |
| `timeOfNextStateChange` | `time_t?` |  |
| `startTime` | `time_t` |  |

### HasPendingContribution

```lua
C_ContributionCollector.HasPendingContribution(contributionID: number) -> hasPending: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsAwaitingRewardQuestData

```lua
C_ContributionCollector.IsAwaitingRewardQuestData(contributionID: number) -> awaitingData: bool
```

`SecretArguments=AllowedWhenUntainted`

## Events

### CONTRIBUTION_CHANGED

```lua
CONTRIBUTION_CHANGED(state: ContributionState, result: ContributionResult, name: string, contributionID: number)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `state` | `ContributionState` |  |
| `result` | `ContributionResult` |  |
| `name` | `string` |  |
| `contributionID` | `number` | `StrideIndex=1` |

### CONTRIBUTION_COLLECTOR_PENDING

```lua
CONTRIBUTION_COLLECTOR_PENDING(contributionID: number, isPending: bool, result: number)
```

`SynchronousEvent`

### CONTRIBUTION_COLLECTOR_UPDATE

```lua
CONTRIBUTION_COLLECTOR_UPDATE()
```

`UniqueEvent`

### CONTRIBUTION_COLLECTOR_UPDATE_SINGLE

```lua
CONTRIBUTION_COLLECTOR_UPDATE_SINGLE(contributionID: number)
```

`SynchronousEvent`

## Types

### ContributionResult

*Enumeration* · 8 values, 0..7

Access values as `Enum.ContributionResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Success` | `ContributionResult` | = 0 |
| `MustBeNearNpc` | `ContributionResult` | = 1 |
| `IncorrectState` | `ContributionResult` | = 2 |
| `InvalidID` | `ContributionResult` | = 3 |
| `QuestDataMissing` | `ContributionResult` | = 4 |
| `FailedConditionCheck` | `ContributionResult` | = 5 |
| `UnableToCompleteTurnIn` | `ContributionResult` | = 6 |
| `InternalError` | `ContributionResult` | = 7 |

### ContributionAppearance

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `stateName` | `cstring` |  |
| `stateColor` | `colorRGB` | `Mixin=ColorMixin` |
| `tooltipLine` | `cstring` |  |
| `tooltipUseTimeRemaining` | `bool` |  |
| `statusBarAtlas` | `textureAtlas` |  |
| `borderAtlas` | `textureAtlas` |  |
| `bannerAtlas` | `textureAtlas` |  |

### ContributionMapInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `areaPoiID` | `number` |  |
| `position` | `vector2` | `Mixin=Vector2DMixin` |
| `name` | `cstring` |  |
| `atlasName` | `string` |  |
| `collectorCreatureID` | `number` |  |
