# CovenantSanctumUI

Namespace `C_CovenantSanctumUI` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/covenantsanctumdocumentation.lua` (FileDataID 4637067)

## Functions

### CanAccessReservoir

```lua
C_CovenantSanctumUI.CanAccessReservoir() -> canAccess: bool
```

### CanDepositAnima

```lua
C_CovenantSanctumUI.CanDepositAnima() -> canDeposit: bool
```

### DepositAnima

```lua
C_CovenantSanctumUI.DepositAnima()
```

### EndInteraction

```lua
C_CovenantSanctumUI.EndInteraction()
```

### GetAnimaInfo

```lua
C_CovenantSanctumUI.GetAnimaInfo() -> currencyID: number, maxDisplayableValue: number
```

### GetCurrentTalentTreeID

```lua
C_CovenantSanctumUI.GetCurrentTalentTreeID() -> currentTalentTreeID: number?
```

### GetFeatures

```lua
C_CovenantSanctumUI.GetFeatures() -> features: CovenantSanctumFeatureInfo[]
```

### GetRenownLevel

```lua
C_CovenantSanctumUI.GetRenownLevel() -> level: number
```

### GetRenownLevels

```lua
C_CovenantSanctumUI.GetRenownLevels(covenantID: number) -> levels: CovenantSanctumRenownLevelInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetRenownRewardsForLevel

```lua
C_CovenantSanctumUI.GetRenownRewardsForLevel(covenantID: number, renownLevel: number) -> rewards: CovenantSanctumRenownRewardInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetSanctumType

```lua
C_CovenantSanctumUI.GetSanctumType() -> sanctumType: GarrTalentFeatureSubtype?
```

### GetSoulCurrencies

```lua
C_CovenantSanctumUI.GetSoulCurrencies() -> currencyIDs: number[]
```

### HasMaximumRenown

```lua
C_CovenantSanctumUI.HasMaximumRenown() -> hasMaxRenown: bool
```

### IsPlayerInRenownCatchUpMode

```lua
C_CovenantSanctumUI.IsPlayerInRenownCatchUpMode() -> isInCatchUpMode: bool
```

### IsWeeklyRenownCapped

```lua
C_CovenantSanctumUI.IsWeeklyRenownCapped() -> isWeeklyCapped: bool
```

### RequestCatchUpState

```lua
C_CovenantSanctumUI.RequestCatchUpState()
```

## Events

### COVENANT_RENOWN_CATCH_UP_STATE_UPDATE

```lua
COVENANT_RENOWN_CATCH_UP_STATE_UPDATE()
```

`SynchronousEvent`

### COVENANT_SANCTUM_RENOWN_LEVEL_CHANGED

```lua
COVENANT_SANCTUM_RENOWN_LEVEL_CHANGED(newRenownLevel: number, oldRenownLevel: number)
```

`SynchronousEvent`

## Types

### CovenantSanctumFeatureInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `garrTalentTreeID` | `number` |  |
| `featureType` | `number` |  |
| `uiOrder` | `number` |  |

### CovenantSanctumRenownLevelInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `level` | `number` |  |
| `locked` | `bool` |  |
| `isMilestone` | `bool` |  |
| `isCapstone` | `bool` |  |

### CovenantSanctumRenownRewardInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `uiOrder` | `number` |  |
| `itemID` | `number?` |  |
| `spellID` | `number?` |  |
| `mountID` | `number?` |  |
| `transmogID` | `number?` |  |
| `transmogSetID` | `number?` |  |
| `titleMaskID` | `number?` |  |
| `garrFollowerID` | `number?` |  |
| `transmogIllusionSourceID` | `number?` |  |
| `icon` | `fileID?` |  |
| `name` | `cstring?` |  |
| `description` | `cstring?` |  |
| `toastDescription` | `cstring?` |  |
