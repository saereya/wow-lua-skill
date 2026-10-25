# RaidMarkers

Global functions · environment All · source `interface/addons/blizzard_apidocumentationgenerated/raidmarkersdocumentation.lua` (FileDataID 7036084)

## Functions

### CanBeRaidTarget

```lua
CanBeRaidTarget(target: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### ClearRaidMarker

```lua
ClearRaidMarker(raidMarkerIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `raidMarkerIndex` | `luaIndex` | default `MAX_RAID_MARKERS` |

### GetNextAvailableRaidTargetMarkerIndex

```lua
GetNextAvailableRaidTargetMarkerIndex(startIndex: luaIndex, reverseSearch: bool, wrapSearch: bool, treatDeadNonFriendlyAsAvailable: bool) -> nextAvailableRaidTargetMarkerIndex: luaIndex
```

`SecretArguments=AllowedWhenUntainted` `SecretInChatMessagingLockdown`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `startIndex` | `luaIndex` |  |
| `reverseSearch` | `bool` | default `false` |
| `wrapSearch` | `bool` | default `false` |
| `treatDeadNonFriendlyAsAvailable` | `bool` | default `false` |

### GetRaidTargetIndex

```lua
GetRaidTargetIndex(target: UnitToken) -> result: luaIndex?
```

`SecretArguments=AllowedWhenUntainted` `SecretReturns`

### IsRaidMarkerActive

```lua
IsRaidMarkerActive(index: luaIndex) -> result: bool
```

`SecretArguments=AllowedWhenUntainted` `SecretInChatMessagingLockdown`

### IsRaidMarkerSystemEnabled

```lua
IsRaidMarkerSystemEnabled() -> enabled: bool
```

### PlaceRaidMarker

```lua
PlaceRaidMarker(index: luaIndex, token: cstring?)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### RemoveRaidTargets

```lua
RemoveRaidTargets()
```

Removes all assigned raid target markers.

`HasRestrictions`

### SetRaidTarget

```lua
SetRaidTarget(target: UnitToken, userIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`
