# AzeriteEssence

Namespace `C_AzeriteEssence` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/azeriteessencedocumentation.lua` (FileDataID 4637033)

## Functions

### ActivateEssence

```lua
C_AzeriteEssence.ActivateEssence(essenceID: number, milestoneID: number)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### CanActivateEssence

```lua
C_AzeriteEssence.CanActivateEssence(essenceID: number, milestoneID: number) -> canActivate: bool
```

`SecretArguments=AllowedWhenUntainted`

### CanDeactivateEssence

```lua
C_AzeriteEssence.CanDeactivateEssence(milestoneID: number) -> canDeactivate: bool
```

`SecretArguments=AllowedWhenUntainted`

### CanOpenUI

```lua
C_AzeriteEssence.CanOpenUI() -> canOpen: bool
```

### ClearPendingActivationEssence

```lua
C_AzeriteEssence.ClearPendingActivationEssence()
```

### CloseForge

```lua
C_AzeriteEssence.CloseForge()
```

### GetEssenceHyperlink

```lua
C_AzeriteEssence.GetEssenceHyperlink(essenceID: number, rank: number) -> link: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetEssenceInfo

```lua
C_AzeriteEssence.GetEssenceInfo(essenceID: number) -> info: AzeriteEssenceInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetEssences

```lua
C_AzeriteEssence.GetEssences() -> essences: AzeriteEssenceInfo[]
```

`MayReturnNothing`

### GetMilestoneEssence

```lua
C_AzeriteEssence.GetMilestoneEssence(milestoneID: number) -> essenceID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetMilestoneInfo

```lua
C_AzeriteEssence.GetMilestoneInfo(milestoneID: number) -> info: AzeriteMilestoneInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetMilestones

```lua
C_AzeriteEssence.GetMilestones() -> milestones: AzeriteMilestoneInfo[]
```

`MayReturnNothing`

### GetMilestoneSpell

```lua
C_AzeriteEssence.GetMilestoneSpell(milestoneID: number) -> spellID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetNumUnlockedEssences

```lua
C_AzeriteEssence.GetNumUnlockedEssences() -> numUnlockedEssences: number
```

### GetNumUsableEssences

```lua
C_AzeriteEssence.GetNumUsableEssences() -> numUsableEssences: number
```

### GetPendingActivationEssence

```lua
C_AzeriteEssence.GetPendingActivationEssence() -> essenceID: number
```

### HasNeverActivatedAnyEssences

```lua
C_AzeriteEssence.HasNeverActivatedAnyEssences() -> hasNeverActivatedAnyEssences: bool
```

### HasPendingActivationEssence

```lua
C_AzeriteEssence.HasPendingActivationEssence() -> hasEssence: bool
```

### IsAtForge

```lua
C_AzeriteEssence.IsAtForge() -> isAtForge: bool
```

### SetPendingActivationEssence

```lua
C_AzeriteEssence.SetPendingActivationEssence(essenceID: number)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### UnlockMilestone

```lua
C_AzeriteEssence.UnlockMilestone(milestoneID: number)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### AZERITE_ESSENCE_ACTIVATED

```lua
AZERITE_ESSENCE_ACTIVATED(slot: AzeriteEssenceSlot, essenceID: number)
```

`SynchronousEvent`

### AZERITE_ESSENCE_ACTIVATION_FAILED

```lua
AZERITE_ESSENCE_ACTIVATION_FAILED(slot: AzeriteEssenceSlot, essenceID: number)
```

`SynchronousEvent`

### AZERITE_ESSENCE_CHANGED

```lua
AZERITE_ESSENCE_CHANGED(essenceID: number, newRank: number)
```

`SynchronousEvent`

### AZERITE_ESSENCE_FORGE_CLOSE

```lua
AZERITE_ESSENCE_FORGE_CLOSE()
```

`SynchronousEvent`

### AZERITE_ESSENCE_FORGE_OPEN

```lua
AZERITE_ESSENCE_FORGE_OPEN()
```

`SynchronousEvent`

### AZERITE_ESSENCE_MILESTONE_UNLOCKED

```lua
AZERITE_ESSENCE_MILESTONE_UNLOCKED(milestoneID: number)
```

`SynchronousEvent`

### AZERITE_ESSENCE_UPDATE

```lua
AZERITE_ESSENCE_UPDATE()
```

`UniqueEvent`

### PENDING_AZERITE_ESSENCE_CHANGED

```lua
PENDING_AZERITE_ESSENCE_CHANGED(essenceID: number?)
```

`SynchronousEvent`

## Types

### AzeriteEssenceInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ID` | `number` |  |
| `name` | `cstring` |  |
| `rank` | `number` |  |
| `unlocked` | `bool` |  |
| `valid` | `bool` |  |
| `icon` | `fileID` |  |

### AzeriteMilestoneInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ID` | `number` |  |
| `requiredLevel` | `number` |  |
| `canUnlock` | `bool` |  |
| `unlocked` | `bool` |  |
| `rank` | `number?` |  |
| `slot` | `AzeriteEssenceSlot?` |  |
