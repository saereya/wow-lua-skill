# SpecializationConstants

source `interface/addons/blizzard_apidocumentationgenerated/specializationconstantsdocumentation.lua` (FileDataID 8020054)

## Types

### ChrSpecializationFlags

*Enumeration* · 9 values, 1..256

Access values as `Enum.ChrSpecializationFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `IsCaster` | `ChrSpecializationFlags` | = 1 |
| `IsRanged` | `ChrSpecializationFlags` | = 2 |
| `IsMelee` | `ChrSpecializationFlags` | = 4 |
| `ChallengeModeSpiritAsHit` | `ChrSpecializationFlags` | = 8 |
| `SheatheInvertedForDualWield` | `ChrSpecializationFlags` | = 16 |
| `OverrideSpec` | `ChrSpecializationFlags` | = 32 |
| `RecommendedSpec` | `ChrSpecializationFlags` | = 64 |
| `DisabledForTesting` | `ChrSpecializationFlags` | = 128 |
| `AllowedSpecForBoost` | `ChrSpecializationFlags` | = 256 |

### SpecGroup

*Enumeration* · 2 values, 0..1

Access values as `Enum.SpecGroup.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Primary` | `SpecGroup` | = 0 |
| `Secondary` | `SpecGroup` | = 1 |

### SpecializationSpellsFlag

*Enumeration* · 1 values, 1..1

Access values as `Enum.SpecializationSpellsFlag.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `DevOnly` | `SpecializationSpellsFlag` | = 1 |
