# NeighborhoodInitiativesConstants

source `interface/addons/blizzard_apidocumentationgenerated/neighborhoodinitiativesconstantsdocumentation.lua` (FileDataID 7106802)

## Types

### InitiativeMilestoneFlags

*Enumeration* · 1 values, 1..1

Access values as `Enum.InitiativeMilestoneFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `FinalMilestone` | `InitiativeMilestoneFlags` | = 1 |

### InitiativeRewardFlags

*Enumeration* · 1 values, 1..1

Access values as `Enum.InitiativeRewardFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `PermanentWorldState` | `InitiativeRewardFlags` | = 1 |

### NeighborhoodInitiativeChestResult

*Enumeration* · 6 values, 0..5

Access values as `Enum.NeighborhoodInitiativeChestResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `NiSuccess` | `NeighborhoodInitiativeChestResult` | = 0 |
| `NiUnspecifiedFailure` | `NeighborhoodInitiativeChestResult` | = 1 |
| `NiNoHouseFound` | `NeighborhoodInitiativeChestResult` | = 2 |
| `NiNoRewards` | `NeighborhoodInitiativeChestResult` | = 3 |
| `NiThrottled` | `NeighborhoodInitiativeChestResult` | = 4 |
| `NiServiceDisabled` | `NeighborhoodInitiativeChestResult` | = 5 |

### NeighborhoodInitiativeFlags

*Enumeration* · 3 values, 1..4

Access values as `Enum.NeighborhoodInitiativeFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Disabled` | `NeighborhoodInitiativeFlags` | = 1 |
| `NoAbandon` | `NeighborhoodInitiativeFlags` | = 2 |
| `NoRepeat` | `NeighborhoodInitiativeFlags` | = 4 |

### NeighborhoodInitiativeNeighborhoodTypes

*Enumeration* · 2 values, 0..1

Access values as `Enum.NeighborhoodInitiativeNeighborhoodTypes.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `NiNeighborhoodTypeSingleton` | `NeighborhoodInitiativeNeighborhoodTypes` | = 0 |
| `NiNeighborhoodTypePool` | `NeighborhoodInitiativeNeighborhoodTypes` | = 1 |

### NeighborhoodInitiativeTaskType

*Enumeration* · 3 values, 0..2

Access values as `Enum.NeighborhoodInitiativeTaskType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Single` | `NeighborhoodInitiativeTaskType` | = 0 |
| `RepeatableFinite` | `NeighborhoodInitiativeTaskType` | = 1 |
| `RepeatableInfinite` | `NeighborhoodInitiativeTaskType` | = 2 |

### NeighborhoodInitiativeUpdateStatus

*Enumeration* · 4 values, 0..3

Access values as `Enum.NeighborhoodInitiativeUpdateStatus.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Started` | `NeighborhoodInitiativeUpdateStatus` | = 0 |
| `MilestoneCompleted` | `NeighborhoodInitiativeUpdateStatus` | = 1 |
| `Completed` | `NeighborhoodInitiativeUpdateStatus` | = 2 |
| `Failed` | `NeighborhoodInitiativeUpdateStatus` | = 3 |

### NeighborhoodInitiativesCompletionStates

*Enumeration* · 3 values, 0..2

Access values as `Enum.NeighborhoodInitiativesCompletionStates.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `NiCompletionStateNotCompleted` | `NeighborhoodInitiativesCompletionStates` | = 0 |
| `NiCompletionStatePlayerCompleted` | `NeighborhoodInitiativesCompletionStates` | = 1 |
| `NiCompletionStateSystemAbandoned` | `NeighborhoodInitiativesCompletionStates` | = 2 |
