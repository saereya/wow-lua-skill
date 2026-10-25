# StableInfo

Namespace `C_StableInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/stableinfodocumentation.lua` (FileDataID 4637262)

## Functions

### BuyStableSlot

```lua
C_StableInfo.BuyStableSlot()
```

### ClosePetStables

```lua
C_StableInfo.ClosePetStables()
```

### GetActivePetList

```lua
C_StableInfo.GetActivePetList() -> activePets: PetInfo[]
```

### GetAvailablePetSpecInfos

```lua
C_StableInfo.GetAvailablePetSpecInfos() -> petSpecInfos: PetSpecInfo[]
```

### GetNextStableSlotCost

```lua
C_StableInfo.GetNextStableSlotCost() -> cost: number
```

### GetNumActivePets

```lua
C_StableInfo.GetNumActivePets() -> numActivePets: number
```

### GetNumStablePets

```lua
C_StableInfo.GetNumStablePets() -> numStablePets: number
```

### GetNumStableSlots

```lua
C_StableInfo.GetNumStableSlots() -> numSlots: number
```

### GetStabledPetList

```lua
C_StableInfo.GetStabledPetList() -> stabledPets: PetInfo[]
```

### GetStablePetFoodTypes

```lua
C_StableInfo.GetStablePetFoodTypes(index: luaIndex) -> foodTypes: string[]
```

`SecretArguments=AllowedWhenUntainted`

### GetStablePetInfo

```lua
C_StableInfo.GetStablePetInfo(index: luaIndex) -> petInfo: PetInfo?
```

`SecretArguments=AllowedWhenUntainted`

### IsAtStableMaster

```lua
C_StableInfo.IsAtStableMaster() -> isAtStableMaster: bool
```

### IsBonusPetSlotAvailable

```lua
C_StableInfo.IsBonusPetSlotAvailable() -> isAvailable: bool
```

### IsPetFavorite

```lua
C_StableInfo.IsPetFavorite(slot: luaIndex) -> isFavorite: bool
```

`SecretArguments=AllowedWhenUntainted`

### PickupStablePet

```lua
C_StableInfo.PickupStablePet(index: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### SetPetFavorite

```lua
C_StableInfo.SetPetFavorite(slot: luaIndex, isFavorite: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetPetSlot

```lua
C_StableInfo.SetPetSlot(index: luaIndex, slot: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### PET_INFO_UPDATE

```lua
PET_INFO_UPDATE()
```

`UniqueEvent`

### PET_STABLE_CLOSED

```lua
PET_STABLE_CLOSED()
```

`SynchronousEvent`

### PET_STABLE_FAVORITES_UPDATED

```lua
PET_STABLE_FAVORITES_UPDATED()
```

`SynchronousEvent`

### PET_STABLE_SHOW

```lua
PET_STABLE_SHOW()
```

`SynchronousEvent`

### PET_STABLE_UPDATE

```lua
PET_STABLE_UPDATE()
```

`SynchronousEvent`

## Types

### PetInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `slotID` | `number` |  |
| `icon` | `fileID` |  |
| `name` | `string` |  |
| `level` | `number` |  |
| `familyName` | `string` |  |
| `specialization` | `string` |  |
| `type` | `string` |  |
| `petAbilities` | `number[]` |  |
| `specAbilities` | `number[]` |  |
| `displayID` | `number` |  |
| `isFavorite` | `bool` |  |
| `isExotic` | `bool` |  |
| `uiModelSceneID` | `number` | default `718` |
| `petNumber` | `number` |  |
| `creatureID` | `number` |  |
| `specID` | `number` |  |
| `loyaltyLevel` | `number` |  |
| `loyaltyName` | `string` |  |
| `happinessLevel` | `number` |  |
| `experience` | `number` |  |
| `experienceNeeded` | `number` |  |

### PetSpecInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `specID` | `number` |  |
| `specIndex` | `luaIndex` |  |
| `specializationName` | `string` |  |
