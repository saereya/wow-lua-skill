# PerksActivities

Namespace `C_PerksActivities` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/perksactivitiesdocumentation.lua` (FileDataID 4637819)

## Functions

### AddTrackedPerksActivity

```lua
C_PerksActivities.AddTrackedPerksActivity(perksActivityID: number)
```

`SecretArguments=AllowedWhenUntainted`

### ClearPerksActivitiesPendingCompletion

```lua
C_PerksActivities.ClearPerksActivitiesPendingCompletion()
```

### GetAllPerksActivityTags

```lua
C_PerksActivities.GetAllPerksActivityTags() -> tags: PerksActivityTags
```

### GetPerksActivitiesInfo

```lua
C_PerksActivities.GetPerksActivitiesInfo() -> info: PerksActivitiesInfo
```

### GetPerksActivitiesPendingCompletion

```lua
C_PerksActivities.GetPerksActivitiesPendingCompletion() -> pending: PerksActivitiesPending
```

### GetPerksActivityChatLink

```lua
C_PerksActivities.GetPerksActivityChatLink(perksActivityID: number) -> link: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetPerksActivityInfo

```lua
C_PerksActivities.GetPerksActivityInfo(perksActivityID: number) -> info: PerksActivityInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetPerksUIThemePrefix

```lua
C_PerksActivities.GetPerksUIThemePrefix() -> kitPrefix: string
```

### GetTrackedPerksActivities

```lua
C_PerksActivities.GetTrackedPerksActivities() -> trackedPerksActivities: PerksActivitiesTracked
```

### RemoveTrackedPerksActivity

```lua
C_PerksActivities.RemoveTrackedPerksActivity(perksActivityID: number)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### PERKS_ACTIVITIES_TRACKED_LIST_CHANGED

```lua
PERKS_ACTIVITIES_TRACKED_LIST_CHANGED(perksActivityID: number, added: bool)
```

`SynchronousEvent`

### PERKS_ACTIVITIES_TRACKED_UPDATED

```lua
PERKS_ACTIVITIES_TRACKED_UPDATED()
```

`UniqueEvent`

### PERKS_ACTIVITIES_UPDATED

```lua
PERKS_ACTIVITIES_UPDATED()
```

`UniqueEvent`

### PERKS_ACTIVITY_COMPLETED

```lua
PERKS_ACTIVITY_COMPLETED(perksActivityID: number)
```

`SynchronousEvent`

## Types

### PerksActivitiesInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `activePerksMonth` | `number` |  |
| `displayMonthName` | `cstring` |  |
| `secondsRemaining` | `time_t` |  |
| `activities` | `PerksActivityInfo[]` |  |
| `thresholds` | `PerksActivityThresholdInfo[]` |  |

### PerksActivitiesPending

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `pendingIDs` | `number[]` |  |

### PerksActivitiesTracked

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `trackedIDs` | `number[]` |  |

### PerksActivityCondition

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `isMet` | `bool` |  |
| `text` | `cstring` |  |
| `uiPriority` | `number` |  |

### PerksActivityInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ID` | `number` |  |
| `activityName` | `cstring` |  |
| `description` | `string` |  |
| `thresholdContributionAmount` | `number` |  |
| `completed` | `bool` |  |
| `inProgress` | `bool` |  |
| `tracked` | `bool` |  |
| `supersedes` | `number` |  |
| `uiPriority` | `number` |  |
| `areAllConditionsMet` | `bool` |  |
| `conditions` | `PerksActivityCondition[]` |  |
| `eventName` | `cstring?` |  |
| `eventStartTime` | `time_t?` |  |
| `eventEndTime` | `time_t?` |  |
| `requirementsList` | `CriteriaRequirement[]` |  |
| `criteriaList` | `CriteriaRequiredValue[]` |  |
| `tagNames` | `string[]` |  |

### PerksActivityTags

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `tagName` | `string[]` |  |

### PerksActivityThresholdInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `thresholdOrderIndex` | `number` |  |
| `currencyAwardAmount` | `number` |  |
| `requiredContributionAmount` | `number` |  |
| `pendingReward` | `bool` |  |
| `itemReward` | `number?` |  |
