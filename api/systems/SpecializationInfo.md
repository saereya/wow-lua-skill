# SpecializationInfo

Namespace `C_SpecializationInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/specializationinfodocumentation.lua` (FileDataID 4637253)

## Functions

### CanPlayerUsePVPTalentUI

```lua
C_SpecializationInfo.CanPlayerUsePVPTalentUI() -> canUse: bool, failureReason: string
```

### CanPlayerUseTalentSpecUI

```lua
C_SpecializationInfo.CanPlayerUseTalentSpecUI() -> canUse: bool, failureReason: string
```

### CanPlayerUseTalentUI

```lua
C_SpecializationInfo.CanPlayerUseTalentUI() -> canUse: bool, failureReason: string
```

### GetActiveSpecGroup

```lua
C_SpecializationInfo.GetActiveSpecGroup(isInspect: bool?, isPet: bool?) -> groupIndex: luaIndex
```

`SecretArguments=AllowedWhenUntainted`

### GetAllClassIDs

```lua
C_SpecializationInfo.GetAllClassIDs() -> allClassIDs: number[]
```

### GetAllSelectedPvpTalentIDs

```lua
C_SpecializationInfo.GetAllSelectedPvpTalentIDs() -> selectedPvpTalentIDs: number[]
```

### GetClassIDFromSpecID

```lua
C_SpecializationInfo.GetClassIDFromSpecID(specID: number) -> classID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetCombatConfigIDForSpecGroup

```lua
C_SpecializationInfo.GetCombatConfigIDForSpecGroup(groupIndex: luaIndex) -> configID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetInspectSelectedPvpTalent

```lua
C_SpecializationInfo.GetInspectSelectedPvpTalent(inspectedUnit: UnitToken, talentIndex: number) -> selectedTalentID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetInspectSpecialization

```lua
C_SpecializationInfo.GetInspectSpecialization(unit: UnitToken) -> specializationID: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitIdentityRestricted`

### GetNumSpecializationsForClassID

```lua
C_SpecializationInfo.GetNumSpecializationsForClassID(classID: number) -> specCount: number
```

`SecretArguments=AllowedWhenUntainted`

### GetPvpTalentAlertStatus

```lua
C_SpecializationInfo.GetPvpTalentAlertStatus() -> hasUnspentSlot: bool, hasNewTalent: bool
```

### GetPvpTalentInfo

```lua
C_SpecializationInfo.GetPvpTalentInfo(talentID: number) -> talentInfo: PvpTalentInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetPvpTalentSlotInfo

```lua
C_SpecializationInfo.GetPvpTalentSlotInfo(talentIndex: number) -> slotInfo: PvpTalentSlotInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetPvpTalentSlotUnlockLevel

```lua
C_SpecializationInfo.GetPvpTalentSlotUnlockLevel(talentIndex: number) -> requiredLevel: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetPvpTalentUnlockLevel

```lua
C_SpecializationInfo.GetPvpTalentUnlockLevel(talentID: number) -> requiredLevel: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetSpecialization

```lua
C_SpecializationInfo.GetSpecialization(isInspect: bool?, isPet: bool?, specGroupIndex: luaIndex?) -> specializationIndex: luaIndex
```

`SecretArguments=AllowedWhenUntainted`

### GetSpecializationInfo

```lua
C_SpecializationInfo.GetSpecializationInfo(specializationIndex: luaIndex, isInspect: bool, isPet: bool, inspectTarget: string?, sex: number?, groupIndex: luaIndex?, classID: number?) -> specId: number, name: string?, description: string?, icon: fileID?, role: string?, primaryStat: luaIndex?, pointsSpent: number, background: string?, previewPointsSpent: number, isUnlocked: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `specializationIndex` | `luaIndex` |  |
| `isInspect` | `bool` | default `false` |
| `isPet` | `bool` | default `false` |
| `inspectTarget` | `string?` |  |
| `sex` | `number?` |  |
| `groupIndex` | `luaIndex?` |  |
| `classID` | `number?` |  |

Returns:

| Name | Type | Notes |
|---|---|---|
| `specId` | `number` | default `0` |
| `name` | `string?` |  |
| `description` | `string?` |  |
| `icon` | `fileID?` |  |
| `role` | `string?` |  |
| `primaryStat` | `luaIndex?` |  |
| `pointsSpent` | `number` | default `0` |
| `background` | `string?` |  |
| `previewPointsSpent` | `number` | default `0` |
| `isUnlocked` | `bool` | default `true` |

### GetSpecializationMasterySpells

```lua
C_SpecializationInfo.GetSpecializationMasterySpells(specializationIndex: luaIndex, isInspect: bool?, isPet: bool?) -> spellIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetSpecIDs

```lua
C_SpecializationInfo.GetSpecIDs(specSetID: number) -> specIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetSpellsDisplay

```lua
C_SpecializationInfo.GetSpellsDisplay(specializationID: number) -> spellID: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetTalentInfo

```lua
C_SpecializationInfo.GetTalentInfo(query: TalentInfoQuery) -> result: TalentInfoResult?
```

`SecretArguments=AllowedWhenUntainted`

### HasPlayerEarnedATalentPoint

```lua
C_SpecializationInfo.HasPlayerEarnedATalentPoint() -> hasEarned: bool
```

### IsInitialized

```lua
C_SpecializationInfo.IsInitialized() -> isSpecializationDataInitialized: bool
```

### IsPvpTalentLocked

```lua
C_SpecializationInfo.IsPvpTalentLocked(talentID: number) -> locked: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsSpecSelectionEnabled

```lua
C_SpecializationInfo.IsSpecSelectionEnabled(classID: number) -> enabled: bool
```

`SecretArguments=AllowedWhenUntainted`

### MatchesCurrentSpecSet

```lua
C_SpecializationInfo.MatchesCurrentSpecSet(specSetID: number) -> matches: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetActiveSpecGroup

```lua
C_SpecializationInfo.SetActiveSpecGroup(groupIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### SetPetSpecialization

```lua
C_SpecializationInfo.SetPetSpecialization(specIndex: luaIndex, petNumber: number?)
```

`SecretArguments=AllowedWhenUntainted`

### SetPvpTalentLocked

```lua
C_SpecializationInfo.SetPvpTalentLocked(talentID: number, locked: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetSpecialization

```lua
C_SpecializationInfo.SetSpecialization(specIndex: luaIndex) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

## Events

### ACTIVE_TALENT_GROUP_CHANGED

```lua
ACTIVE_TALENT_GROUP_CHANGED(curr: number, prev: number)
```

`SynchronousEvent`

### CONFIRM_PET_UNLEARN

```lua
CONFIRM_PET_UNLEARN(cost: number)
```

`SynchronousEvent`

### CONFIRM_TALENT_WIPE

```lua
CONFIRM_TALENT_WIPE(cost: number, respecType: number)
```

`SynchronousEvent`

### PET_SPECIALIZATION_CHANGED

```lua
PET_SPECIALIZATION_CHANGED()
```

`SynchronousEvent`

### PLAYER_LEARN_PVP_TALENT_FAILED

```lua
PLAYER_LEARN_PVP_TALENT_FAILED()
```

`SynchronousEvent`

### PLAYER_LEARN_TALENT_FAILED

```lua
PLAYER_LEARN_TALENT_FAILED()
```

`SynchronousEvent`

### PLAYER_PVP_TALENT_UPDATE

```lua
PLAYER_PVP_TALENT_UPDATE()
```

`SynchronousEvent`

### PLAYER_TALENT_UPDATE

```lua
PLAYER_TALENT_UPDATE()
```

`SynchronousEvent`

### SPEC_INVOLUNTARILY_CHANGED

```lua
SPEC_INVOLUNTARILY_CHANGED(isPet: bool)
```

`SynchronousEvent`

### TALENTS_INVOLUNTARILY_RESET

```lua
TALENTS_INVOLUNTARILY_RESET(isPetTalents: bool)
```

`SynchronousEvent`

## Types

### PvpTalentInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `talentID` | `number` |  |
| `name` | `string` |  |
| `icon` | `number` |  |
| `selected` | `bool` |  |
| `available` | `bool` |  |
| `spellID` | `number` |  |
| `unlocked` | `bool` |  |
| `known` | `bool` |  |
| `grantedByAura` | `bool` |  |
| `dependenciesUnmet` | `bool` |  |
| `dependenciesUnmetReason` | `string?` |  |

### PvpTalentSlotInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `enabled` | `bool` |  |
| `level` | `number` |  |
| `selectedTalentID` | `number?` |  |
| `availableTalentIDs` | `number[]` |  |

### SpecializationInfoOutput

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `specId` | `number` | default `0` |
| `name` | `string?` |  |
| `description` | `string?` |  |
| `icon` | `fileID?` |  |
| `role` | `string?` |  |
| `primaryStat` | `luaIndex?` |  |
| `pointsSpent` | `number` | default `0` |
| `background` | `string?` |  |
| `previewPointsSpent` | `number` | default `0` |
| `isUnlocked` | `bool` | default `true` |

### SpecializationInfoQuery

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `specializationIndex` | `luaIndex` |  |
| `isInspect` | `bool` | default `false` |
| `isPet` | `bool` | default `false` |
| `inspectTarget` | `string?` |  |
| `sex` | `number?` |  |
| `groupIndex` | `luaIndex?` |  |
| `classID` | `number?` |  |

### TalentInfoQuery

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `groupIndex` | `luaIndex?` |  |
| `isInspect` | `bool` | default `false` |
| `tier` | `luaIndex?` |  |
| `column` | `luaIndex?` |  |
| `target` | `UnitToken?` |  |
| `specializationIndex` | `luaIndex?` |  |
| `talentIndex` | `luaIndex?` |  |
| `isPet` | `bool` | default `false` |

### TalentInfoResult

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `talentID` | `number` | default `0` |
| `name` | `string` |  |
| `icon` | `fileID` |  |
| `tier` | `luaIndex` |  |
| `column` | `luaIndex` |  |
| `selected` | `bool` | default `false` |
| `available` | `bool` | default `false` |
| `spellID` | `number` | default `0` |
| `isPVPTalentUnlocked` | `bool` | default `false` |
| `known` | `bool` | default `false` |
| `grantedByAura` | `bool` | default `false` |
| `rank` | `luaIndex` |  |
| `maxRank` | `luaIndex` |  |
| `meetsPrereq` | `bool` | default `false` |
| `previewRank` | `luaIndex` |  |
| `meetsPreviewPrereq` | `bool` | default `false` |
| `isExceptional` | `bool` | default `false` |
| `hasGoldBorder` | `bool` | default `false` |
