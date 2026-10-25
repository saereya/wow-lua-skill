# RemixArtifactUI

Namespace `C_RemixArtifactUI` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/remixartifactuidocumentation.lua` (FileDataID 6855467)

## Functions

### ClearRemixArtifactItem

```lua
C_RemixArtifactUI.ClearRemixArtifactItem()
```

### GetAppearanceInfoByID

```lua
C_RemixArtifactUI.GetAppearanceInfoByID(artifactAppearanceID: number) -> uiCameraID: number, altHandUICameraID: number?
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetArtifactArtInfo

```lua
C_RemixArtifactUI.GetArtifactArtInfo() -> artifactArtInfo: RemixArtifactArtInfo
```

`MayReturnNothing`

### GetArtifactItemInfo

```lua
C_RemixArtifactUI.GetArtifactItemInfo() -> itemID: number, altItemID: number?, artifactAppearanceID: number, appearanceModID: number, itemAppearanceID: number?, altItemAppearanceID: number?, altOnTop: bool
```

`MayReturnNothing`

### GetCurrArtifactItemID

```lua
C_RemixArtifactUI.GetCurrArtifactItemID() -> reqitemID: number?
```

### GetCurrItemSpecIndex

```lua
C_RemixArtifactUI.GetCurrItemSpecIndex() -> specIndex: luaIndex?
```

### GetCurrTraitTreeID

```lua
C_RemixArtifactUI.GetCurrTraitTreeID() -> traitTreeID: number?
```

### ItemInSlotIsRemixArtifact

```lua
C_RemixArtifactUI.ItemInSlotIsRemixArtifact(invSlot: luaIndex) -> isRemixArtifact: bool
```

`SecretArguments=AllowedWhenUntainted`

## Events

### REMIX_ARTIFACT_ITEM_SPECS_LOADED

```lua
REMIX_ARTIFACT_ITEM_SPECS_LOADED(success: bool)
```

`SynchronousEvent`

### REMIX_ARTIFACT_UPDATE

```lua
REMIX_ARTIFACT_UPDATE()
```

`SynchronousEvent`

## Types

### RemixArtifactAppearanceInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `uiCameraID` | `number` |  |
| `altHandUICameraID` | `number?` |  |

### RemixArtifactArtInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `textureKit` | `textureKit` |  |
| `titleName` | `string` |  |
| `uiModelSceneID` | `number` |  |
| `spellVisualKitID` | `number` |  |

### RemixArtifactInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `itemID` | `number` |  |
| `altItemID` | `number?` |  |
| `artifactAppearanceID` | `number` |  |
| `appearanceModID` | `number` |  |
| `itemAppearanceID` | `number?` |  |
| `altItemAppearanceID` | `number?` |  |
| `altOnTop` | `bool` |  |
