# PlayerMentorship

Namespace `C_PlayerMentorship` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/playermentorshipdocumentation.lua` (FileDataID 4637157)

## Functions

### GetMentorLevelRequirement

```lua
C_PlayerMentorship.GetMentorLevelRequirement() -> level: number?
```

### GetMentorRequirements

```lua
C_PlayerMentorship.GetMentorRequirements() -> achievementIDs: number[], optionalAchievementIDs: number[], optionalCompleteAtLeastCount: number
```

### GetMentorshipStatus

```lua
C_PlayerMentorship.GetMentorshipStatus(playerLocation: PlayerLocation) -> status: PlayerMentorshipStatus
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `playerLocation` | `PlayerLocation` | `Mixin=PlayerLocationMixin` |

### IsActivePlayerConsideredNewcomer

```lua
C_PlayerMentorship.IsActivePlayerConsideredNewcomer() -> isConsideredNewcomer: bool
```

### IsMentorRestricted

```lua
C_PlayerMentorship.IsMentorRestricted() -> isRestricted: bool
```

## Events

### MENTORSHIP_STATUS_CHANGED

```lua
MENTORSHIP_STATUS_CHANGED()
```

`SynchronousEvent`

### NEWCOMER_GRADUATION

```lua
NEWCOMER_GRADUATION()
```

`SynchronousEvent`
