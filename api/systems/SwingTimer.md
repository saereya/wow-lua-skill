# SwingTimer

Namespace `C_SwingTimer` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/swingtimerdocumentation.lua` (FileDataID 8448832)

## Functions

### EnableRangeCheck

```lua
C_SwingTimer.EnableRangeCheck(swingType: PlayerSwingType, enable: bool)
```

Used in conjunction with PlayerSwingRangeUpdate to inform the UI when the current target goes in or out of auto attack range.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `swingType` | `PlayerSwingType` |  |
| `enable` | `bool` | True if changes in range for the swing type should dispatch PlayerSwingRangeUpdate. False if the swing type no longer needs the event. |

### IsTargetWithinSwingRange

```lua
C_SwingTimer.IsTargetWithinSwingRange(swingType: PlayerSwingType) -> isInRange: bool?
```

Whether the current target is within range of the player's auto attack for the given swing type. Auto attacks only ever apply to the current target, so no other unit can be queried.

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `isInRange` | `bool?` | Nil when no range check could be made, for example there is no target, the target cannot be attacked, or no weapon is equipped for the swing type. Nil must not be treated as out of range. |

## Events

### PLAYER_SWING

```lua
PLAYER_SWING(swingDuration: number, swingType: PlayerSwingType)
```

`SynchronousEvent`

### PLAYER_SWING_RANGE_UPDATE

```lua
PLAYER_SWING_RANGE_UPDATE(swingType: PlayerSwingType, isInRange: bool, checksRange: bool)
```

Only signaled for swing types that have an active range check. See C_SwingTimer.EnableRangeCheck.

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `swingType` | `PlayerSwingType` |  |
| `isInRange` | `bool` | Whether the current target is within auto attack range. Should not be used if the 'checksRange' parameter is false. |
| `checksRange` | `bool` | Can be false if a range check was not made for any reason, for example there is not a current target. |

## Types

### PlayerSwingType

*Enumeration* · 3 values, 0..2

Access values as `Enum.PlayerSwingType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `MainHand` | `PlayerSwingType` | = 0 |
| `OffHand` | `PlayerSwingType` | = 1 |
| `Ranged` | `PlayerSwingType` | = 2 |
