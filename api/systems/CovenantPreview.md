# CovenantPreview

Namespace `C_CovenantPreview` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/covenantpreviewdocumentation.lua` (FileDataID 4637080)

## Functions

### CloseFromUI

```lua
C_CovenantPreview.CloseFromUI()
```

### GetCovenantInfoForPlayerChoiceResponseID

```lua
C_CovenantPreview.GetCovenantInfoForPlayerChoiceResponseID(playerChoiceResponseID: number) -> previewInfo: CovenantPreviewInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

## Events

### COVENANT_PREVIEW_CLOSE

```lua
COVENANT_PREVIEW_CLOSE()
```

`SynchronousEvent`

### COVENANT_PREVIEW_OPEN

```lua
COVENANT_PREVIEW_OPEN(previewInfo: CovenantPreviewInfo)
```

`SynchronousEvent`

## Types

### CovenantAbilityInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `number` |  |
| `type` | `CovenantAbilityType` |  |

### CovenantFeatureInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `description` | `cstring` |  |
| `texture` | `number` |  |

### CovenantPreviewInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `textureKit` | `textureKit` |  |
| `transmogSetID` | `number` |  |
| `mountID` | `number` |  |
| `covenantName` | `string` |  |
| `covenantZone` | `string` |  |
| `description` | `string` |  |
| `covenantCrest` | `textureAtlas` |  |
| `covenantAbilities` | `CovenantAbilityInfo[]` |  |
| `fromPlayerChoice` | `bool` |  |
| `covenantSoulbinds` | `CovenantSoulbindInfo[]` |  |
| `featureInfo` | `CovenantFeatureInfo` |  |

### CovenantSoulbindInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `number` |  |
| `uiTextureKit` | `textureKit` |  |
| `name` | `cstring` |  |
| `description` | `cstring` |  |
| `sortOrder` | `number` |  |
