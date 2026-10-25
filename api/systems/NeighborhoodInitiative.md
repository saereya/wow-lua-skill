# NeighborhoodInitiative

Namespace `C_NeighborhoodInitiative` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/neighborhoodinitiativedocumentation.lua` (FileDataID 6999257)

## Functions

### AddTrackedInitiativeTask

```lua
C_NeighborhoodInitiative.AddTrackedInitiativeTask(initiativeTaskID: number)
```

`SecretArguments=AllowedWhenUntainted`

### GetActiveNeighborhood

```lua
C_NeighborhoodInitiative.GetActiveNeighborhood() -> neighborhoodGUID: WOWGUID
```

### GetAvailableHouseXP

```lua
C_NeighborhoodInitiative.GetAvailableHouseXP() -> availabeXP: number
```

### GetInitiativeActivityLogInfo

```lua
C_NeighborhoodInitiative.GetInitiativeActivityLogInfo() -> info: InitiativeActivityLogInfo?
```

### GetInitiativeTaskChatLink

```lua
C_NeighborhoodInitiative.GetInitiativeTaskChatLink(initiativeTaskID: number) -> link: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetInitiativeTaskInfo

```lua
C_NeighborhoodInitiative.GetInitiativeTaskInfo(initiativeTaskID: number) -> info: InitiativeTaskInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetInitiativeTaskRewardScaling

```lua
C_NeighborhoodInitiative.GetInitiativeTaskRewardScaling(taskID: number, numItems: number) -> scaledAmount: number
```

`SecretArguments=AllowedWhenUntainted`

### GetNeighborhoodInitiativeInfo

```lua
C_NeighborhoodInitiative.GetNeighborhoodInitiativeInfo() -> info: NeighborhoodInitiativeInfo?
```

### GetRequiredLevel

```lua
C_NeighborhoodInitiative.GetRequiredLevel() -> reqLevel: number
```

### GetTrackedInitiativeTasks

```lua
C_NeighborhoodInitiative.GetTrackedInitiativeTasks() -> trackedInitiativeTasks: InitiativeTasksTracked
```

### IsInitiativeEnabled

```lua
C_NeighborhoodInitiative.IsInitiativeEnabled() -> enabled: bool
```

### IsPlayerInNeighborhoodGroup

```lua
C_NeighborhoodInitiative.IsPlayerInNeighborhoodGroup() -> inValidGroup: bool
```

### IsViewingActiveNeighborhood

```lua
C_NeighborhoodInitiative.IsViewingActiveNeighborhood() -> isViewingActiveNeighborhood: bool
```

### PlayerHasInitiativeAccess

```lua
C_NeighborhoodInitiative.PlayerHasInitiativeAccess() -> success: bool
```

### PlayerMeetsRequiredLevel

```lua
C_NeighborhoodInitiative.PlayerMeetsRequiredLevel() -> success: bool
```

### RemoveTrackedInitiativeTask

```lua
C_NeighborhoodInitiative.RemoveTrackedInitiativeTask(initiativeTaskID: number)
```

`SecretArguments=AllowedWhenUntainted`

### RequestInitiativeActivityLog

```lua
C_NeighborhoodInitiative.RequestInitiativeActivityLog()
```

### RequestNeighborhoodInitiativeInfo

```lua
C_NeighborhoodInitiative.RequestNeighborhoodInitiativeInfo()
```

### SetActiveNeighborhood

```lua
C_NeighborhoodInitiative.SetActiveNeighborhood(neighborhoodGUID: WOWGUID)
```

`SecretArguments=AllowedWhenUntainted`

### SetViewingNeighborhood

```lua
C_NeighborhoodInitiative.SetViewingNeighborhood(neighborhoodGUID: WOWGUID)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### INITIATIVE_ACTIVITY_LOG_UPDATED

```lua
INITIATIVE_ACTIVITY_LOG_UPDATED()
```

`SynchronousEvent`

### INITIATIVE_COMPLETED

```lua
INITIATIVE_COMPLETED(initiativeTitle: string)
```

`SynchronousEvent`

### INITIATIVE_TASK_COMPLETED

```lua
INITIATIVE_TASK_COMPLETED(taskName: string)
```

`SynchronousEvent`

### INITIATIVE_TASKS_TRACKED_LIST_CHANGED

```lua
INITIATIVE_TASKS_TRACKED_LIST_CHANGED(initiativeTaskID: number, added: bool)
```

`SynchronousEvent`

### INITIATIVE_TASKS_TRACKED_UPDATED

```lua
INITIATIVE_TASKS_TRACKED_UPDATED()
```

`UniqueEvent`

### NEIGHBORHOOD_INITIATIVE_UPDATED

```lua
NEIGHBORHOOD_INITIATIVE_UPDATED()
```

`SynchronousEvent`

## Types

### InitiativeActivityLogEntry

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `taskID` | `number` |  |
| `playerName` | `string` |  |
| `taskName` | `cstring` |  |
| `completionTime` | `time_t` |  |
| `amount` | `number` |  |

### InitiativeActivityLogInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `isLoaded` | `bool` |  |
| `neighborhoodGUID` | `WOWGUID` |  |
| `nextUpdateTime` | `time_t` |  |
| `taskActivity` | `InitiativeActivityLogEntry[]` |  |

### InitiativeMilestoneInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `milestoneOrderIndex` | `number` |  |
| `requiredContributionAmount` | `number` |  |
| `rewards` | `InitiativeMilestoneRewardInfo[]` |  |

### InitiativeMilestoneRewardInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `title` | `string` |  |
| `description` | `string` |  |
| `decorID` | `number` |  |
| `decorQuantity` | `number` |  |
| `favor` | `number` |  |
| `money` | `WOWMONEY` |  |
| `rewardQuestID` | `number` |  |

### InitiativeTaskInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ID` | `number` |  |
| `taskName` | `cstring` |  |
| `description` | `string` |  |
| `progressContributionAmount` | `number` |  |
| `tracked` | `bool` |  |
| `supersedes` | `number` |  |
| `timesCompleted` | `number` |  |
| `completed` | `bool` |  |
| `inProgress` | `bool` |  |
| `taskType` | `NeighborhoodInitiativeTaskType` |  |
| `sortOrder` | `number` |  |
| `rewardQuestID` | `number` |  |
| `requirementsList` | `CriteriaRequirement[]` |  |
| `criteriaList` | `CriteriaRequiredValue[]` |  |

### InitiativeTasksTracked

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `trackedIDs` | `number[]` |  |

### NeighborhoodInitiativeInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `isLoaded` | `bool` |  |
| `neighborhoodGUID` | `WOWGUID` |  |
| `initiativeID` | `number` |  |
| `currentCycleID` | `number` |  |
| `progressRequired` | `number` |  |
| `currentProgress` | `number` |  |
| `playerTotalContribution` | `number` |  |
| `duration` | `time_t` |  |
| `tasks` | `InitiativeTaskInfo[]` |  |
| `milestones` | `InitiativeMilestoneInfo[]` |  |
| `title` | `string` |  |
| `description` | `string` |  |
