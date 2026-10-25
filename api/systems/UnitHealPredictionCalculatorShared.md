# UnitHealPredictionCalculatorShared

source `interface/addons/blizzard_apidocumentationgenerated/unithealpredictioncalculatorshareddocumentation.lua` (FileDataID 7669056)

## Types

### UnitDamageAbsorbClampMode

*Enumeration* · 3 values, 0..2

Access values as `Enum.UnitDamageAbsorbClampMode.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `MissingHealth` | `UnitDamageAbsorbClampMode` | = 0; Clamp damage absorb values to the amount of missing health with incoming heals subtracted. |
| `MissingHealthWithoutIncomingHeals` | `UnitDamageAbsorbClampMode` | = 1; Clamp damage absorb values to the amount of missing health. Incoming heals do not decrease missing health. |
| `MaximumHealth` | `UnitDamageAbsorbClampMode` | = 2; Clamp damage absorb values to the amount of maximum health. |

### UnitHealAbsorbClampMode

*Enumeration* · 2 values, 0..1

Access values as `Enum.UnitHealAbsorbClampMode.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `CurrentHealth` | `UnitHealAbsorbClampMode` | = 0; Clamp heal absorb values to the amount of current health. |
| `MaximumHealth` | `UnitHealAbsorbClampMode` | = 1; Clamp heal absorb values to the amount of maximum health. |

### UnitHealAbsorbMode

*Enumeration* · 2 values, 0..1

Access values as `Enum.UnitHealAbsorbMode.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `ReducedByIncomingHeals` | `UnitHealAbsorbMode` | = 0; Reduce heal absorb values by incoming heals, and vice versa, clamping to zero where necessary. |
| `Total` | `UnitHealAbsorbMode` | = 1; Use heal absorb and incoming heal values as-is without any reductions. |

### UnitIncomingHealClampMode

*Enumeration* · 2 values, 0..1

Access values as `Enum.UnitIncomingHealClampMode.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `MissingHealth` | `UnitIncomingHealClampMode` | = 0; Clamp incoming heal values to the amount of missing health with overflow applied. |
| `MaximumHealth` | `UnitIncomingHealClampMode` | = 1; Clamp incoming heal values to the amount of maximum health. |

### UnitMaximumHealthMode

*Enumeration* · 2 values, 0..1

Access values as `Enum.UnitMaximumHealthMode.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Default` | `UnitMaximumHealthMode` | = 0; Use maximum unit health as-is without adjustments. |
| `WithAbsorbs` | `UnitMaximumHealthMode` | = 1; Use maximum unit health with total damage absorb shields added. |

### UnitDamageAbsorbInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `amount` | `number` | Amount of applied damage absorb affects with potential reductions from clamping included. |
| `clamped` | `bool` | If true, the value is in excess of the clamp boundary. |

### UnitHealAbsorbInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `amount` | `number` | Amount of applied heal absorb affects with potential reductions from incoming heals and clamping included. |
| `clamped` | `bool` | If true, the value is in excess of the clamp boundary. |

### UnitHealPredictionValues

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `health` | `number` | default `0` |
| `healthMax` | `number` | default `0` |
| `totalIncomingHeals` | `number` | default `0` |
| `totalIncomingHealsFromHealer` | `number` | default `0` |
| `totalDamageAbsorbs` | `number` | default `0` |
| `totalHealAbsorbs` | `number` | default `0` |

### UnitIncomingHealInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `amount` | `number` | Amount of incoming heals across all units with potential reductions from heal absorb effects included. |
| `amountFromHealer` | `number` | Amount of incoming heals from the healer unit. Will never exceed the all-units value. |
| `amountFromOthers` | `number` | Amount of incoming heals from units other than theh healer. Calculated as the difference between amount and amount-from-healer. |
| `clamped` | `bool` | If true, the value is in excess of the clamp boundary. |
