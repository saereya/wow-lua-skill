# LootHistory

Namespace `C_LootHistory` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/loothistorydocumentation.lua` (FileDataID 5157300)

## Functions

### GetAllEncounterInfos

```lua
C_LootHistory.GetAllEncounterInfos() -> infos: EncounterLootInfo[]
```

### GetInfoForEncounter

```lua
C_LootHistory.GetInfoForEncounter(encounterID: number) -> info: EncounterLootInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetLootHistoryTime

```lua
C_LootHistory.GetLootHistoryTime() -> time: number
```

### GetSortedDropsForEncounter

```lua
C_LootHistory.GetSortedDropsForEncounter(encounterID: number) -> drops: EncounterLootDropInfo[]?
```

`SecretArguments=AllowedWhenUntainted`

### GetSortedInfoForDrop

```lua
C_LootHistory.GetSortedInfoForDrop(encounterID: number, lootListKey: number) -> info: EncounterLootDropInfo?
```

`SecretArguments=AllowedWhenUntainted`

## Events

### LOOT_HISTORY_CLEAR_HISTORY

```lua
LOOT_HISTORY_CLEAR_HISTORY()
```

`SynchronousEvent`

### LOOT_HISTORY_GO_TO_ENCOUNTER

```lua
LOOT_HISTORY_GO_TO_ENCOUNTER(encounterID: number)
```

`UniqueEvent`

### LOOT_HISTORY_ONE_HUNDRED_ROLL

```lua
LOOT_HISTORY_ONE_HUNDRED_ROLL(encounterID: number, lootListKey: number)
```

`SynchronousEvent`

### LOOT_HISTORY_UPDATE_DROP

```lua
LOOT_HISTORY_UPDATE_DROP(encounterID: number, lootListKey: number)
```

`UniqueEvent`

### LOOT_HISTORY_UPDATE_ENCOUNTER

```lua
LOOT_HISTORY_UPDATE_ENCOUNTER(encounterID: number)
```

`UniqueEvent`

## Types

### EncounterLootDropRollState

*Enumeration* · 6 values, 0..5

Access values as `Enum.EncounterLootDropRollState.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `NeedMainSpec` | `EncounterLootDropRollState` | = 0 |
| `NeedOffSpec` | `EncounterLootDropRollState` | = 1 |
| `Transmog` | `EncounterLootDropRollState` | = 2 |
| `Greed` | `EncounterLootDropRollState` | = 3 |
| `NoRoll` | `EncounterLootDropRollState` | = 4 |
| `Pass` | `EncounterLootDropRollState` | = 5 |

### EncounterLootDropInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `lootListKey` | `number` |  |
| `itemHyperlink` | `string` |  |
| `playerRollState` | `EncounterLootDropRollState` |  |
| `currentLeader` | `EncounterLootDropRollInfo?` |  |
| `isTied` | `bool` | default `false` |
| `winner` | `EncounterLootDropRollInfo?` |  |
| `allPassed` | `bool` | default `false` |
| `rollInfos` | `EncounterLootDropRollInfo[]` |  |
| `startTime` | `number` |  |
| `duration` | `number` |  |

### EncounterLootDropRollInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `playerName` | `string` |  |
| `playerGUID` | `WOWGUID` |  |
| `playerClass` | `string` |  |
| `isSelf` | `bool` |  |
| `state` | `EncounterLootDropRollState` |  |
| `isWinner` | `bool` | default `false` |
| `roll` | `number?` |  |

### EncounterLootDrops

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `encounterID` | `number` |  |
| `drops` | `EncounterLootDropInfo[]` |  |

### EncounterLootInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `encounterName` | `string` |  |
| `encounterID` | `number` |  |
| `startTime` | `number` |  |
| `duration` | `number` |  |
