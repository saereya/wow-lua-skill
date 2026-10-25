# SoulbindsConstants

source `interface/addons/blizzard_apidocumentationgenerated/soulbindsconstantsdocumentation.lua` (FileDataID 4637250)

## Types

### AddSoulbindConduitReason

*Enumeration* · 4 values, 0..3

Access values as `Enum.AddSoulbindConduitReason.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `AddSoulbindConduitReason` | = 0 |
| `Cheat` | `AddSoulbindConduitReason` | = 1 |
| `SpellEffect` | `AddSoulbindConduitReason` | = 2 |
| `Upgrade` | `AddSoulbindConduitReason` | = 3 |

### SoulbindConduitFlags

*Enumeration* · 1 values, 1..1

Access values as `Enum.SoulbindConduitFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `VisibleToGetallsoulbindconduitScript` | `SoulbindConduitFlags` | = 1 |

### SoulbindConduitInstallResult

*Enumeration* · 7 values, 0..6

Access values as `Enum.SoulbindConduitInstallResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Success` | `SoulbindConduitInstallResult` | = 0 |
| `InvalidItem` | `SoulbindConduitInstallResult` | = 1 |
| `InvalidConduit` | `SoulbindConduitInstallResult` | = 2 |
| `InvalidTalent` | `SoulbindConduitInstallResult` | = 3 |
| `DuplicateConduit` | `SoulbindConduitInstallResult` | = 4 |
| `ForgeNotInProximity` | `SoulbindConduitInstallResult` | = 5 |
| `SocketNotEmpty` | `SoulbindConduitInstallResult` | = 6 |

### SoulbindConduitTransactionType

*Enumeration* · 2 values, 0..1

Access values as `Enum.SoulbindConduitTransactionType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Install` | `SoulbindConduitTransactionType` | = 0 |
| `Uninstall` | `SoulbindConduitTransactionType` | = 1 |

### SoulbindConduitType

*Enumeration* · 4 values, 0..3

Access values as `Enum.SoulbindConduitType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Finesse` | `SoulbindConduitType` | = 0 |
| `Potency` | `SoulbindConduitType` | = 1 |
| `Endurance` | `SoulbindConduitType` | = 2 |
| `Flex` | `SoulbindConduitType` | = 3 |

### SoulbindNodeState

*Enumeration* · 4 values, 0..3

Access values as `Enum.SoulbindNodeState.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Unavailable` | `SoulbindNodeState` | = 0 |
| `Unselected` | `SoulbindNodeState` | = 1 |
| `Selectable` | `SoulbindNodeState` | = 2 |
| `Selected` | `SoulbindNodeState` | = 3 |
