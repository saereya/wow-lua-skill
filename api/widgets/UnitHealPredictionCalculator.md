# UnitHealPredictionCalculator

Widget methods (`UnitHealPredictionCalculatorAPI`) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/unithealpredictioncalculatorapidocumentation.lua` (FileDataID 7669055)

## Methods

### EvaluateCurrentHealthPercent

```lua
UnitHealPredictionCalculator:EvaluateCurrentHealthPercent(curve: LuaCurveObjectBase) -> result: LuaCurveEvaluatedResult
```

Calculates the percentage of current unit health and evaluates it against the supplied curve.

`SecretArguments=AllowedWhenUntainted`

### EvaluateMissingHealthPercent

```lua
UnitHealPredictionCalculator:EvaluateMissingHealthPercent(curve: LuaCurveObjectBase) -> result: LuaCurveEvaluatedResult
```

Calculates the percentage of missing unit health and evaluates it against the supplied curve.

`SecretArguments=AllowedWhenUntainted`

### GetCurrentHealth

```lua
UnitHealPredictionCalculator:GetCurrentHealth() -> currentHealth: number
```

Returns the base amount of unit health.

### GetCurrentHealthPercent

```lua
UnitHealPredictionCalculator:GetCurrentHealthPercent() -> currentHealthPercent: number
```

Returns the percentage of current unit health.

### GetDamageAbsorbClampMode

```lua
UnitHealPredictionCalculator:GetDamageAbsorbClampMode() -> damageAbsorbClampMode: UnitDamageAbsorbClampMode
```

Returns the configured damage absorb clamping mode.

`ReturnsNeverSecret`

### GetDamageAbsorbs

```lua
UnitHealPredictionCalculator:GetDamageAbsorbs() -> amount: number, clamped: bool
```

Calculates damage absorb values and clamping according to the configured options.

Returns:

| Name | Type | Notes |
|---|---|---|
| `amount` | `number` | Amount of applied damage absorb affects with potential reductions from clamping included. |
| `clamped` | `bool` | If true, the value is in excess of the clamp boundary. |

### GetHealAbsorbClampMode

```lua
UnitHealPredictionCalculator:GetHealAbsorbClampMode() -> healAbsorbClampMode: UnitHealAbsorbClampMode
```

Returns the configured heal absorb clamping mode.

`ReturnsNeverSecret`

### GetHealAbsorbMode

```lua
UnitHealPredictionCalculator:GetHealAbsorbMode() -> healAbsorbMode: UnitHealAbsorbMode
```

Returns the configured heal absorb processing mode.

`ReturnsNeverSecret`

### GetHealAbsorbs

```lua
UnitHealPredictionCalculator:GetHealAbsorbs() -> amount: number, clamped: bool
```

Calculates heal absorb values and clamping according to the configured options.

Returns:

| Name | Type | Notes |
|---|---|---|
| `amount` | `number` | Amount of applied heal absorb affects with potential reductions from incoming heals and clamping included. |
| `clamped` | `bool` | If true, the value is in excess of the clamp boundary. |

### GetIncomingHealClampMode

```lua
UnitHealPredictionCalculator:GetIncomingHealClampMode() -> incomingHealClampMode: UnitIncomingHealClampMode
```

Returns the configured incoming heal clamping mode.

`ReturnsNeverSecret`

### GetIncomingHealOverflowPercent

```lua
UnitHealPredictionCalculator:GetIncomingHealOverflowPercent() -> incomingHealOverflowPercent: number
```

Returns the configured incoming heal maximum overflow percentage.

`ReturnsNeverSecret`

### GetIncomingHeals

```lua
UnitHealPredictionCalculator:GetIncomingHeals() -> amount: number, amountFromHealer: number, amountFromOthers: number, clamped: bool
```

Calculates incoming heal values and clamping according to the configured options.

Returns:

| Name | Type | Notes |
|---|---|---|
| `amount` | `number` | Amount of incoming heals across all units with potential reductions from heal absorb effects included. |
| `amountFromHealer` | `number` | Amount of incoming heals from the healer unit. Will never exceed the all-units value. |
| `amountFromOthers` | `number` | Amount of incoming heals from units other than theh healer. Calculated as the difference between amount and amount-from-healer. |
| `clamped` | `bool` | If true, the value is in excess of the clamp boundary. |

### GetMaximumDamageAbsorbs

```lua
UnitHealPredictionCalculator:GetMaximumDamageAbsorbs() -> maximumDamageAbsorbs: number
```

Returns the maximum clamping amount for damage absorbs.

### GetMaximumHealAbsorbs

```lua
UnitHealPredictionCalculator:GetMaximumHealAbsorbs() -> maximumHealAbsorbs: number
```

Returns the maximum clamping amount for heal absorbs.

### GetMaximumHealth

```lua
UnitHealPredictionCalculator:GetMaximumHealth() -> maximumHealth: number
```

Returns the base amount of maximum unit health.

### GetMaximumHealthMode

```lua
UnitHealPredictionCalculator:GetMaximumHealthMode() -> maximumHealthMode: UnitMaximumHealthMode
```

Returns the configured maximum health mode.

`ReturnsNeverSecret`

### GetMaximumIncomingHeals

```lua
UnitHealPredictionCalculator:GetMaximumIncomingHeals() -> maximumIncomingHeals: number
```

Returns the maximum clamping amount for incoming heals.

### GetMissingHealth

```lua
UnitHealPredictionCalculator:GetMissingHealth() -> missingHealth: number
```

Returns the base amount of missing unit health.

### GetMissingHealthPercent

```lua
UnitHealPredictionCalculator:GetMissingHealthPercent() -> missingHealthPercent: number
```

Returns the percentage of missing unit health.

### GetPredictedValues

```lua
UnitHealPredictionCalculator:GetPredictedValues() -> predictedValues: UnitHealPredictionValues
```

Returns the raw total figures used for data calculations.

### GetTotalDamageAbsorbs

```lua
UnitHealPredictionCalculator:GetTotalDamageAbsorbs() -> totalDamageAbsorbs: number
```

Returns the base total amount of all applied damage absorb shields.

### GetTotalHealAbsorbs

```lua
UnitHealPredictionCalculator:GetTotalHealAbsorbs() -> totalHealAbsorbs: number
```

Returns the base total amount of all applied heal absorption effects.

### GetTotalIncomingHeals

```lua
UnitHealPredictionCalculator:GetTotalIncomingHeals() -> totalIncomingHeals: number
```

Returns the base total amount of all incoming heals.

### GetTotalIncomingHealsFromHealer

```lua
UnitHealPredictionCalculator:GetTotalIncomingHealsFromHealer() -> totalIncomingHealsFromHealer: number
```

Returns the base total amount of all incoming heals from the healer unit, if any.

### HasSecretValues

```lua
UnitHealPredictionCalculator:HasSecretValues() -> hasSecretValues: bool
```

Returns true if the object has been configured with any secret values.

`ReturnsNeverSecret`

### Reset

```lua
UnitHealPredictionCalculator:Reset()
```

Resets all stored state on the object.

### ResetPredictedValues

```lua
UnitHealPredictionCalculator:ResetPredictedValues()
```

Resets all stored healing values used for calculations.

### SetDamageAbsorbClampMode

```lua
UnitHealPredictionCalculator:SetDamageAbsorbClampMode(damageAbsorbClampMode: UnitDamageAbsorbClampMode)
```

Changes the clamping mode used when calculating damage absorb amounts.

`SecretArguments=NotAllowed`

### SetHealAbsorbClampMode

```lua
UnitHealPredictionCalculator:SetHealAbsorbClampMode(healAbsorbClampMode: UnitHealAbsorbClampMode)
```

Changes the clamping mode used when calculating heal absorb amounts.

`SecretArguments=NotAllowed`

### SetHealAbsorbMode

```lua
UnitHealPredictionCalculator:SetHealAbsorbMode(healAbsorbMode: UnitHealAbsorbMode)
```

Changes the processing mode used when calculating both heal absorb and incoming heal amounts.

`SecretArguments=NotAllowed`

### SetIncomingHealClampMode

```lua
UnitHealPredictionCalculator:SetIncomingHealClampMode(incomingHealClampMode: UnitIncomingHealClampMode)
```

Changes the clamping mode used when calculating incoming heal amounts.

`SecretArguments=NotAllowed`

### SetIncomingHealOverflowPercent

```lua
UnitHealPredictionCalculator:SetIncomingHealOverflowPercent(incomingHealOverflowPercent: number)
```

Changes the maximum overflow percentage for incoming heals. Increasing this to a value over 1.0 will mean that incoming heals can extend beyond maximum health.

`SecretArguments=NotAllowed`

### SetMaximumHealthMode

```lua
UnitHealPredictionCalculator:SetMaximumHealthMode(maximumHealthMode: UnitMaximumHealthMode)
```

Changes the calculation mode for maximum health values used for clamping.

`SecretArguments=NotAllowed`

### SetPredictedValues

```lua
UnitHealPredictionCalculator:SetPredictedValues(predictedValues: UnitHealPredictionValues)
```

Sets the healing values used for all calculations.

`SecretArguments=AllowedWhenUntainted`

### SetToDefaults

```lua
UnitHealPredictionCalculator:SetToDefaults()
```

Resets all state on the object, and clears the secret values flag.
