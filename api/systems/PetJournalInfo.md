# PetJournalInfo

Namespace `C_PetJournal` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/petjournalinfodocumentation.lua` (FileDataID 4637161)

## Functions

### ClearHoveredBattlePet

```lua
C_PetJournal.ClearHoveredBattlePet()
```

### ClearSearchFilter

```lua
C_PetJournal.ClearSearchFilter()
```

### DismissSummonedPet

```lua
C_PetJournal.DismissSummonedPet(petID: WOWGUID)
```

`SecretArguments=AllowedWhenUntainted`

### GetDisplayIDByIndex

```lua
C_PetJournal.GetDisplayIDByIndex(speciesID: number, index: luaIndex) -> displayID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetDisplayProbabilityByIndex

```lua
C_PetJournal.GetDisplayProbabilityByIndex(speciesID: number, index: luaIndex) -> displayProbability: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetNonBattlePetLinkByIndex

```lua
C_PetJournal.GetNonBattlePetLinkByIndex(index: luaIndex) -> link: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetNumDisplays

```lua
C_PetJournal.GetNumDisplays(speciesID: number) -> numDisplays: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetNumPetsInJournal

```lua
C_PetJournal.GetNumPetsInJournal(creatureID: number) -> maxAllowed: number, numPets: number
```

`SecretArguments=AllowedWhenUntainted`

### GetOwnedPetIDs

```lua
C_PetJournal.GetOwnedPetIDs() -> ownedPetIDs: WOWGUID[]
```

### GetPetAbilityInfo

```lua
C_PetJournal.GetPetAbilityInfo(abilityID: number) -> name: string, icon: fileID, petType: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetPetAbilityListTable

```lua
C_PetJournal.GetPetAbilityListTable(speciesID: number) -> info: PetAbilityLevelInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetPetInfoTableByPetID

```lua
C_PetJournal.GetPetInfoTableByPetID(petID: WOWGUID) -> info: PetJournalPetInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetPetInfoTableBySpeciesID

```lua
C_PetJournal.GetPetInfoTableBySpeciesID(speciesID: number) -> petInfo: PetJournalPetInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetPetLoadOutInfo

```lua
C_PetJournal.GetPetLoadOutInfo(slot: luaIndex) -> petID: WOWGUID?, ability1ID: number, ability2ID: number, ability3ID: number, locked: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetPetSummonInfo

```lua
C_PetJournal.GetPetSummonInfo(battlePetGUID: WOWGUID) -> isSummonable: bool, error: PetJournalError, errorText: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetSearchFilter

```lua
C_PetJournal.GetSearchFilter() -> filterText: cstring
```

### HasFavoritePets

```lua
C_PetJournal.HasFavoritePets() -> hasFavorites: bool
```

### IsCurrentlySummoned

```lua
C_PetJournal.IsCurrentlySummoned(petID: WOWGUID) -> isSummoned: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsUsingDefaultFilters

```lua
C_PetJournal.IsUsingDefaultFilters() -> isUsingDefaultFilters: bool
```

### PetIsSummonable

```lua
C_PetJournal.PetIsSummonable(battlePetGUID: WOWGUID) -> isSummonable: bool
```

`SecretArguments=AllowedWhenUntainted`

### PetUsesRandomDisplay

```lua
C_PetJournal.PetUsesRandomDisplay(speciesID: number) -> usesRandomDisplay: bool?
```

`SecretArguments=AllowedWhenUntainted`

### SetDefaultFilters

```lua
C_PetJournal.SetDefaultFilters()
```

### SetHoveredBattlePet

```lua
C_PetJournal.SetHoveredBattlePet(battlePetGUID: WOWGUID)
```

`SecretArguments=AllowedWhenUntainted`

### SetSearchFilter

```lua
C_PetJournal.SetSearchFilter(filterText: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### SpellTargetBattlePet

```lua
C_PetJournal.SpellTargetBattlePet(battlePetGUID: WOWGUID)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### BATTLEPET_FORCE_NAME_DECLENSION

```lua
BATTLEPET_FORCE_NAME_DECLENSION(name: cstring, battlePetGUID: WOWGUID)
```

`SynchronousEvent`

### COMPANION_LEARNED

```lua
COMPANION_LEARNED()
```

`SynchronousEvent`

### COMPANION_UNLEARNED

```lua
COMPANION_UNLEARNED()
```

`SynchronousEvent`

### COMPANION_UPDATE

```lua
COMPANION_UPDATE(companionType: cstring?)
```

`SynchronousEvent`

### NEW_PET_ADDED

```lua
NEW_PET_ADDED(battlePetGUID: WOWGUID)
```

`SynchronousEvent`

### PET_JOURNAL_AUTO_SLOTTED_PET

```lua
PET_JOURNAL_AUTO_SLOTTED_PET(slotIndex: number, battlePetGUID: WOWGUID)
```

`SynchronousEvent`

### PET_JOURNAL_CAGE_FAILED

```lua
PET_JOURNAL_CAGE_FAILED()
```

`SynchronousEvent`

### PET_JOURNAL_LIST_UPDATE

```lua
PET_JOURNAL_LIST_UPDATE()
```

`SynchronousEvent` `UniqueEvent`

### PET_JOURNAL_NEW_BATTLE_SLOT

```lua
PET_JOURNAL_NEW_BATTLE_SLOT()
```

`SynchronousEvent`

### PET_JOURNAL_PET_DELETED

```lua
PET_JOURNAL_PET_DELETED(battlePetGUID: WOWGUID)
```

`SynchronousEvent`

### PET_JOURNAL_PET_RESTORED

```lua
PET_JOURNAL_PET_RESTORED(battlePetGUID: WOWGUID)
```

`SynchronousEvent`

### PET_JOURNAL_PET_REVOKED

```lua
PET_JOURNAL_PET_REVOKED(battlePetGUID: WOWGUID)
```

`SynchronousEvent`

### PET_JOURNAL_PETS_HEALED

```lua
PET_JOURNAL_PETS_HEALED()
```

`SynchronousEvent`

### PET_JOURNAL_TRAP_LEVEL_SET

```lua
PET_JOURNAL_TRAP_LEVEL_SET(trapLevel: number)
```

`SynchronousEvent`

### UPDATE_SUMMONPETS_ACTION

```lua
UPDATE_SUMMONPETS_ACTION()
```

`SynchronousEvent`

## Types

### PetJournalError

*Enumeration* · 6 values, 0..5

Access values as `Enum.PetJournalError.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `PetJournalError` | = 0 |
| `PetIsDead` | `PetJournalError` | = 1 |
| `JournalIsLocked` | `PetJournalError` | = 2 |
| `InvalidFaction` | `PetJournalError` | = 3 |
| `NoFavoritesToSummon` | `PetJournalError` | = 4 |
| `NoValidRandomSummon` | `PetJournalError` | = 5 |

### PetAbilityLevelInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `abilityID` | `number` |  |
| `level` | `number` |  |

### PetJournalPetInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `speciesID` | `number` |  |
| `customName` | `cstring?` |  |
| `petLevel` | `number?` |  |
| `xp` | `number?` |  |
| `maxXP` | `number?` |  |
| `displayID` | `number?` |  |
| `isFavorite` | `bool?` |  |
| `icon` | `fileID` |  |
| `petType` | `luaIndex` |  |
| `creatureID` | `number` |  |
| `name` | `cstring?` |  |
| `sourceText` | `cstring` |  |
| `description` | `cstring` |  |
| `isWild` | `bool?` |  |
| `canBattle` | `bool` |  |
| `tradable` | `bool` |  |
| `unique` | `bool` |  |
| `obtainable` | `bool` |  |
| `canAttachToDecor` | `bool` |  |
| `creatureModelScale` | `number?` |  |
