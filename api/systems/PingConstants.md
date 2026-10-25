# PingConstants

source `interface/addons/blizzard_apidocumentationgenerated/pingconstantsdocumentation.lua` (FileDataID 5152476)

## Types

### PingMode

*Enumeration* · 2 values, 0..1

Access values as `Enum.PingMode.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `KeyDown` | `PingMode` | = 0 |
| `ClickDrag` | `PingMode` | = 1 |

### PingResult

*Enumeration* · 9 values, 0..8

Access values as `Enum.PingResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Success` | `PingResult` | = 0 |
| `FailedGeneric` | `PingResult` | = 1 |
| `FailedSpamming` | `PingResult` | = 2 |
| `FailedDisabledByLeader` | `PingResult` | = 3 |
| `FailedDisabledBySettings` | `PingResult` | = 4 |
| `FailedOutOfPingArea` | `PingResult` | = 5 |
| `FailedSquelched` | `PingResult` | = 6 |
| `FailedUnspecified` | `PingResult` | = 7 |
| `FailedSilent` | `PingResult` | = 8 |

### PingSetTargetState

*Enumeration* · 3 values, 0..2

Access values as `Enum.PingSetTargetState.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Ok` | `PingSetTargetState` | = 0 |
| `Failed` | `PingSetTargetState` | = 1 |
| `FailedSilent` | `PingSetTargetState` | = 2 |

### PingSubjectType

*Enumeration* · 10 values, 0..9

Access values as `Enum.PingSubjectType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Attack` | `PingSubjectType` | = 0 |
| `Warning` | `PingSubjectType` | = 1 |
| `Assist` | `PingSubjectType` | = 2 |
| `OnMyWay` | `PingSubjectType` | = 3 |
| `AlertThreat` | `PingSubjectType` | = 4 |
| `AlertNotThreat` | `PingSubjectType` | = 5 |
| `ActionReady` | `PingSubjectType` | = 6 |
| `ActionOnCooldown` | `PingSubjectType` | = 7 |
| `ActionUnavailable` | `PingSubjectType` | = 8 |
| `ActionNotReady` | `PingSubjectType` | = 9 |

### PingTargetOption

*Enumeration* · 3 values, 0..2

Access values as `Enum.PingTargetOption.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `All` | `PingTargetOption` | = 0 |
| `Environment` | `PingTargetOption` | = 1 |
| `Units` | `PingTargetOption` | = 2 |

### PingTargetType

*Enumeration* · 3 values, 0..2

Access values as `Enum.PingTargetType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Unit` | `PingTargetType` | = 0 |
| `Point` | `PingTargetType` | = 1 |
| `Action` | `PingTargetType` | = 2 |

### PingTypeFlags

*Enumeration* · 1 values, 1..1

Access values as `Enum.PingTypeFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `DefaultPing` | `PingTypeFlags` | = 1 |
