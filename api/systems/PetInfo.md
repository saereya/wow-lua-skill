# PetInfo

Namespace `C_PetInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/petinfodocumentation.lua` (FileDataID 4637151)

## Functions

### CanPetEatItem

```lua
C_PetInfo.CanPetEatItem(itemID: number) -> canEat: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetPetFoodTypes

```lua
C_PetInfo.GetPetFoodTypes() -> foodTypes: string[]
```

### GetPetHappiness

```lua
C_PetInfo.GetPetHappiness() -> happiness: number, damagePercentage: number, loyaltyRate: number
```

`MayReturnNothing`

### GetPetLoyalty

```lua
C_PetInfo.GetPetLoyalty() -> loyaltyName: string
```

`MayReturnNothing`

### GetPetTalentTree

```lua
C_PetInfo.GetPetTalentTree() -> talentTreeName: stringView
```

`MayReturnNothing`

### GetPetTamersForMap

```lua
C_PetInfo.GetPetTamersForMap(uiMapID: number) -> petTamers: PetTamerMapInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetPetTrainingPoints

```lua
C_PetInfo.GetPetTrainingPoints() -> totalPoints: number, usedPoints: number
```

### GetPetUIModelSceneID

```lua
C_PetInfo.GetPetUIModelSceneID() -> modelSceneID: number
```

### GetSpellForPetAction

```lua
C_PetInfo.GetSpellForPetAction(actionID: number) -> spellID: number?
```

`SecretArguments=AllowedWhenUntainted`

### IsPetActionPassive

```lua
C_PetInfo.IsPetActionPassive(actionID: number) -> isPassive: bool
```

`SecretArguments=AllowedWhenUntainted`

### PetAbandon

```lua
C_PetInfo.PetAbandon(petNumber: number?)
```

`SecretArguments=AllowedWhenUntainted`

### PetAssistMode

```lua
C_PetInfo.PetAssistMode()
```

### PetRename

```lua
C_PetInfo.PetRename(name: cstring, petNumber: number?, declensions: cstring[]?)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### PET_ATTACK_START

```lua
PET_ATTACK_START()
```

`SynchronousEvent`

### PET_ATTACK_STOP

```lua
PET_ATTACK_STOP()
```

`SynchronousEvent`

### PET_BAR_HIDEGRID

```lua
PET_BAR_HIDEGRID()
```

`SynchronousEvent`

### PET_BAR_SHOWGRID

```lua
PET_BAR_SHOWGRID()
```

`SynchronousEvent`

### PET_BAR_UPDATE_COOLDOWN

```lua
PET_BAR_UPDATE_COOLDOWN()
```

`SynchronousEvent`

### PET_DISMISS_START

```lua
PET_DISMISS_START(delay: number)
```

`SynchronousEvent`

### PET_FORCE_NAME_DECLENSION

```lua
PET_FORCE_NAME_DECLENSION(name: cstring, petNumber: number?, declinedName1: cstring?, declinedName2: cstring?, declinedName3: cstring?, declinedName4: cstring?, declinedName5: cstring?)
```

`SynchronousEvent`

### PET_UI_CLOSE

```lua
PET_UI_CLOSE()
```

`SynchronousEvent`

### RAISED_AS_GHOUL

```lua
RAISED_AS_GHOUL()
```

`SynchronousEvent`

### UPDATE_POSSESS_BAR

```lua
UPDATE_POSSESS_BAR()
```

`SynchronousEvent`

### UPDATE_VEHICLE_ACTIONBAR

```lua
UPDATE_VEHICLE_ACTIONBAR()
```

`SynchronousEvent`

## Types

### PetTamerMapInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `areaPoiID` | `number` |  |
| `position` | `vector2` | `Mixin=Vector2DMixin` |
| `name` | `cstring` |  |
| `atlasName` | `string?` |  |
| `textureIndex` | `number?` |  |
