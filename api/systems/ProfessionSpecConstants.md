# ProfessionSpecConstants

source `interface/addons/blizzard_apidocumentationgenerated/professionspecconstantsdocumentation.lua` (FileDataID 4637172)

## Types

### ProfTraitPerkNodeFlags

*Enumeration* · 2 values, 1..2

Access values as `Enum.ProfTraitPerkNodeFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `UnlocksSubpath` | `ProfTraitPerkNodeFlags` | = 1 |
| `IsMajorBonus` | `ProfTraitPerkNodeFlags` | = 2 |

### ProfessionsSpecPathState

*Enumeration* · 3 values, 0..2

Access values as `Enum.ProfessionsSpecPathState.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Locked` | `ProfessionsSpecPathState` | = 0 |
| `Progressing` | `ProfessionsSpecPathState` | = 1 |
| `Completed` | `ProfessionsSpecPathState` | = 2 |

### ProfessionsSpecPerkState

*Enumeration* · 3 values, 0..2

Access values as `Enum.ProfessionsSpecPerkState.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Unearned` | `ProfessionsSpecPerkState` | = 0 |
| `Pending` | `ProfessionsSpecPerkState` | = 1 |
| `Earned` | `ProfessionsSpecPerkState` | = 2 |

### ProfessionsSpecTabState

*Enumeration* · 3 values, 0..2

Access values as `Enum.ProfessionsSpecTabState.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Locked` | `ProfessionsSpecTabState` | = 0 |
| `Unlocked` | `ProfessionsSpecTabState` | = 1 |
| `Unlockable` | `ProfessionsSpecTabState` | = 2 |

### ProfTabHighlight

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `description` | `cstring` |  |

### ProfTabInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `rootNodeID` | `number` |  |
| `name` | `cstring` |  |
| `description` | `cstring` |  |
| `rootIconID` | `number` |  |
| `highlights` | `ProfTabHighlight[]` |  |

### SpecPerkInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `perkID` | `number` |  |
| `isMajorPerk` | `bool` |  |

### SpecializationCurrencyInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `numAvailable` | `number` |  |
| `currencyName` | `cstring` |  |

### SpecializationTabInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `enabled` | `bool` | default `true` |
| `errorReason` | `cstring` |  |
