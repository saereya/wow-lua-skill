# RecentAllies

Namespace `C_RecentAllies` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/recentalliesdocumentation.lua` (FileDataID 7083868)

## Functions

### CanSetRecentAllyNote

```lua
C_RecentAllies.CanSetRecentAllyNote(characterGUID: WOWGUID) -> canSetNote: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresRecentAllies`

### GetRecentAllies

```lua
C_RecentAllies.GetRecentAllies() -> recentAlliesData: RecentAllyData[]
```

`RequiresRecentAllies`

### GetRecentAllyByFullName

```lua
C_RecentAllies.GetRecentAllyByFullName(fullCharacterName: cstring) -> recentAllyData: RecentAllyData?
```

`SecretArguments=AllowedWhenUntainted` `RequiresRecentAllies`

### GetRecentAllyByGUID

```lua
C_RecentAllies.GetRecentAllyByGUID(characterGUID: WOWGUID) -> recentAllyData: RecentAllyData?
```

`SecretArguments=AllowedWhenUntainted` `RequiresRecentAllies`

### IsInteractionCategoryFilterSupportedForCurrentGameType

```lua
C_RecentAllies.IsInteractionCategoryFilterSupportedForCurrentGameType(interactionCategoryFilter: RecentAlliesInteractionCategoryFilter) -> isInteractionCategoryFilterSupportedForCurrentGameType: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsRecentAllyByFullName

```lua
C_RecentAllies.IsRecentAllyByFullName(fullCharacterName: cstring) -> isRecentAlly: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresRecentAllies`

### IsRecentAllyByGUID

```lua
C_RecentAllies.IsRecentAllyByGUID(characterGUID: WOWGUID) -> isRecentAlly: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresRecentAllies`

### IsRecentAllyDataReady

```lua
C_RecentAllies.IsRecentAllyDataReady() -> isReady: bool
```

`RequiresRecentAllies`

### IsRecentAllyPinned

```lua
C_RecentAllies.IsRecentAllyPinned(characterGUID: WOWGUID) -> isPinned: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresRecentAllies`

### IsSystemEnabled

```lua
C_RecentAllies.IsSystemEnabled() -> isRecentAllySystemEnabled: bool
```

### IsSystemSupported

```lua
C_RecentAllies.IsSystemSupported() -> isRecentAllySystemSupported: bool
```

### SearchRecentAllies

```lua
C_RecentAllies.SearchRecentAllies(searchInfo: RecentAlliesSearchInfo) -> recentAlliesData: RecentAllyData[]
```

`SecretArguments=AllowedWhenUntainted` `RequiresRecentAllies`

### SetRecentAllyNote

```lua
C_RecentAllies.SetRecentAllyNote(characterGUID: WOWGUID, note: cstring)
```

`SecretArguments=AllowedWhenUntainted` `RequiresRecentAllies`

### SetRecentAllyPinned

```lua
C_RecentAllies.SetRecentAllyPinned(characterGUID: WOWGUID, isPinned: bool)
```

`SecretArguments=AllowedWhenUntainted` `RequiresRecentAllies`

### TryRequestRecentAlliesData

```lua
C_RecentAllies.TryRequestRecentAlliesData()
```

`RequiresRecentAllies` `HasRestrictions`

## Events

### LET_RECENT_ALLIES_SEE_LOCATION_SETTING_UPDATED

```lua
LET_RECENT_ALLIES_SEE_LOCATION_SETTING_UPDATED()
```

`SynchronousEvent`

### RECENT_ALLIES_CACHE_UPDATE

```lua
RECENT_ALLIES_CACHE_UPDATE()
```

`UniqueEvent`

### RECENT_ALLIES_DATA_READY

```lua
RECENT_ALLIES_DATA_READY()
```

`SynchronousEvent`

### RECENT_ALLIES_SYSTEM_STATUS_UPDATED

```lua
RECENT_ALLIES_SYSTEM_STATUS_UPDATED()
```

`SynchronousEvent`

### RECENT_ALLY_DATA_UPDATED

```lua
RECENT_ALLY_DATA_UPDATED(characterGUID: WOWGUID)
```

`SynchronousEvent`

## Types

### RecentAlliesSearchInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `searchText` | `string` |  |
| `isOnline` | `bool` |  |
| `isDND` | `bool` |  |
| `isAFK` | `bool` |  |
| `isOffline` | `bool` |  |
| `interactionCategoryFilters` | `RecentAlliesInteractionCategoryFilter[]` |  |

### RecentAllyCharacterData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `guid` | `WOWGUID` |  |
| `name` | `string` |  |
| `fullName` | `string` |  |
| `realmName` | `string` |  |
| `level` | `number` |  |
| `classID` | `number` |  |
| `raceID` | `number` |  |
| `sex` | `UnitSex` |  |

### RecentAllyData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `stateData` | `RecentAllyStateData` |  |
| `characterData` | `RecentAllyCharacterData` |  |
| `interactionData` | `RecentAllyInteractionData` |  |

### RecentAllyInteraction

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `type` | `RolodexType` |  |
| `description` | `cstring` |  |
| `timestamp` | `time_t` |  |
| `contextData` | `RecentAllyInteractionContextData` |  |

### RecentAllyInteractionContextData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `itemID` | `number?` |  |
| `locationName` | `cstring?` |  |
| `activityDifficultyID` | `number?` |  |
| `activityDifficultyLevel` | `number?` |  |

### RecentAllyInteractionData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `interactions` | `RecentAllyInteraction[]` |  |
| `note` | `string?` |  |

### RecentAllyStateData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `isOnline` | `bool` |  |
| `isDND` | `bool` |  |
| `isAFK` | `bool` |  |
| `isConvertedLegacyFriend` | `bool` |  |
| `pinExpirationDate` | `time_t?` |  |
| `friendRequestSentThisSession` | `bool` |  |
| `currentLocation` | `string?` |  |

## Predicates

Conditions referenced by the flags above.

- `RequiresRecentAllies` *Precondition* (failure mode: ReturnNothing)
