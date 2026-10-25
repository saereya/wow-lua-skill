# IslandsQueue

Namespace `C_IslandsQueue` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/islandsqueueuidocumentation.lua` (FileDataID 4637107)

## Functions

### CloseIslandsQueueScreen

```lua
C_IslandsQueue.CloseIslandsQueueScreen()
```

### GetIslandDifficultyInfo

```lua
C_IslandsQueue.GetIslandDifficultyInfo() -> islandDifficultyInfo: IslandsQueueDifficultyInfo[]
```

### GetIslandsMaxGroupSize

```lua
C_IslandsQueue.GetIslandsMaxGroupSize() -> maxGroupSize: number
```

### GetIslandsWeeklyQuestID

```lua
C_IslandsQueue.GetIslandsWeeklyQuestID() -> questID: number?
```

### QueueForIsland

```lua
C_IslandsQueue.QueueForIsland(difficultyID: number)
```

`SecretArguments=AllowedWhenUntainted`

### RequestPreloadRewardData

```lua
C_IslandsQueue.RequestPreloadRewardData(questId: number)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### ISLANDS_QUEUE_CLOSE

```lua
ISLANDS_QUEUE_CLOSE()
```

`SynchronousEvent`

### ISLANDS_QUEUE_OPEN

```lua
ISLANDS_QUEUE_OPEN()
```

`SynchronousEvent`

## Types

### IslandsQueueDifficultyInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `difficultyId` | `number` |  |
| `previewRewardQuestId` | `number` |  |
