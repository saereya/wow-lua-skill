# Covenant

Namespace `C_Covenants` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/covenantsdocumentation.lua` (FileDataID 4637074)

## Functions

### GetActiveCovenantID

```lua
C_Covenants.GetActiveCovenantID() -> covenantID: number
```

### GetCovenantData

```lua
C_Covenants.GetCovenantData(covenantID: number) -> data: CovenantData?
```

`SecretArguments=AllowedWhenUntainted`

### GetCovenantIDs

```lua
C_Covenants.GetCovenantIDs() -> covenantID: number[]
```

## Events

### COVENANT_CHOSEN

```lua
COVENANT_CHOSEN(covenantID: number)
```

`SynchronousEvent`

## Types

### CovenantData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ID` | `number` |  |
| `textureKit` | `textureKit` |  |
| `celebrationSoundKit` | `number` |  |
| `animaChannelSelectSoundKit` | `number` |  |
| `animaChannelActiveSoundKit` | `number` |  |
| `animaGemsFullSoundKit` | `number` |  |
| `animaNewGemSoundKit` | `number` |  |
| `animaReinforceSelectSoundKit` | `number` |  |
| `upgradeTabSelectSoundKitID` | `number` |  |
| `reservoirFullSoundKitID` | `number` |  |
| `beginResearchSoundKitID` | `number` |  |
| `renownFanfareSoundKitID` | `number` |  |
| `factionID` | `number` |  |
| `name` | `cstring` |  |
| `soulbindIDs` | `number[]` |  |
