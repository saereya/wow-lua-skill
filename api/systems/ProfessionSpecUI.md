# ProfessionSpecUI

Namespace `C_ProfSpecs` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/professionspecuidocumentation.lua` (FileDataID 4637171)

## Functions

### CanRefundPath

```lua
C_ProfSpecs.CanRefundPath(pathID: number, configID: number) -> canRefund: bool
```

`SecretArguments=AllowedWhenUntainted`

### CanUnlockTab

```lua
C_ProfSpecs.CanUnlockTab(tabTreeID: number, configID: number) -> canUnlock: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetChildrenForPath

```lua
C_ProfSpecs.GetChildrenForPath(pathID: number) -> childIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetConfigIDForSkillLine

```lua
C_ProfSpecs.GetConfigIDForSkillLine(skillLineID: number) -> configID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetCurrencyInfoForSkillLine

```lua
C_ProfSpecs.GetCurrencyInfoForSkillLine(skillLineID: number) -> info: SpecializationCurrencyInfo
```

`SecretArguments=AllowedWhenUntainted`

### GetDefaultSpecSkillLine

```lua
C_ProfSpecs.GetDefaultSpecSkillLine() -> defaultSpecSkillLine: number?
```

### GetDescriptionForPath

```lua
C_ProfSpecs.GetDescriptionForPath(pathID: number) -> description: string
```

`SecretArguments=AllowedWhenUntainted`

### GetDescriptionForPerk

```lua
C_ProfSpecs.GetDescriptionForPerk(perkID: number) -> description: string
```

`SecretArguments=AllowedWhenUntainted`

### GetEntryIDForPerk

```lua
C_ProfSpecs.GetEntryIDForPerk(perkID: number) -> entryID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetNewSpecReminderProfName

```lua
C_ProfSpecs.GetNewSpecReminderProfName() -> profName: cstring?
```

### GetPerksForPath

```lua
C_ProfSpecs.GetPerksForPath(pathID: number) -> perkInfos: SpecPerkInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetRootPathForTab

```lua
C_ProfSpecs.GetRootPathForTab(tabTreeID: number) -> rootPathID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetSourceTextForPath

```lua
C_ProfSpecs.GetSourceTextForPath(pathID: number, configID: number) -> sourceText: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetSpecTabIDsForSkillLine

```lua
C_ProfSpecs.GetSpecTabIDsForSkillLine(skillLineID: number) -> specTabIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetSpecTabInfo

```lua
C_ProfSpecs.GetSpecTabInfo() -> specTabInfo: SpecializationTabInfo
```

### GetSpendCurrencyForPath

```lua
C_ProfSpecs.GetSpendCurrencyForPath(pathID: number) -> currencyID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetSpendEntryForPath

```lua
C_ProfSpecs.GetSpendEntryForPath(pathID: number) -> entryID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetStateForPath

```lua
C_ProfSpecs.GetStateForPath(pathID: number, configID: number) -> state: ProfessionsSpecPathState
```

`SecretArguments=AllowedWhenUntainted`

### GetStateForPerk

```lua
C_ProfSpecs.GetStateForPerk(perkID: number, configID: number) -> state: ProfessionsSpecPerkState
```

`SecretArguments=AllowedWhenUntainted`

### GetStateForTab

```lua
C_ProfSpecs.GetStateForTab(tabTreeID: number, configID: number) -> tabInfo: ProfessionsSpecTabState
```

`SecretArguments=AllowedWhenUntainted`

### GetTabInfo

```lua
C_ProfSpecs.GetTabInfo(tabTreeID: number) -> tabInfo: ProfTabInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetUnlockEntryForPath

```lua
C_ProfSpecs.GetUnlockEntryForPath(pathID: number) -> entryID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetUnlockRankForPerk

```lua
C_ProfSpecs.GetUnlockRankForPerk(perkID: number) -> unlockRank: number?
```

`SecretArguments=AllowedWhenUntainted`

### ShouldShowPointsReminder

```lua
C_ProfSpecs.ShouldShowPointsReminder() -> showReminder: bool
```

### ShouldShowPointsReminderForSkillLine

```lua
C_ProfSpecs.ShouldShowPointsReminderForSkillLine(skillLineID: number) -> showReminder: bool
```

`SecretArguments=AllowedWhenUntainted`

### ShouldShowSpecTab

```lua
C_ProfSpecs.ShouldShowSpecTab() -> showSpecTab: bool
```

### SkillLineHasSpecialization

```lua
C_ProfSpecs.SkillLineHasSpecialization(skillLineID: number) -> hasSpecialization: bool
```

`SecretArguments=AllowedWhenUntainted`

## Events

### SKILL_LINE_SPECS_RANKS_CHANGED

```lua
SKILL_LINE_SPECS_RANKS_CHANGED()
```

`UniqueEvent`

### SKILL_LINE_SPECS_UNLOCKED

```lua
SKILL_LINE_SPECS_UNLOCKED(skillLineID: number, tradeSkillID: number)
```

`UniqueEvent`
