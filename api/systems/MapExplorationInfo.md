# MapExplorationInfo

Namespace `C_MapExplorationInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/mapexplorationdocumentation.lua` (FileDataID 4637142)

## Functions

### GetExploredAreaIDsAtPosition

```lua
C_MapExplorationInfo.GetExploredAreaIDsAtPosition(uiMapID: number, normalizedPosition: vector2) -> areaID: number[]?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `uiMapID` | `number` |  |
| `normalizedPosition` | `vector2` | `Mixin=Vector2DMixin` |

### GetExploredMapTextures

```lua
C_MapExplorationInfo.GetExploredMapTextures(uiMapID: number) -> overlayInfo: UiMapExplorationInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

## Events

### MAP_EXPLORATION_UPDATED

```lua
MAP_EXPLORATION_UPDATED()
```

`SynchronousEvent`

## Types

### UiMapExplorationHitRect

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `top` | `number` |  |
| `bottom` | `number` |  |
| `left` | `number` |  |
| `right` | `number` |  |

### UiMapExplorationInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `textureWidth` | `number` |  |
| `textureHeight` | `number` |  |
| `offsetX` | `number` |  |
| `offsetY` | `number` |  |
| `isShownByMouseOver` | `bool` |  |
| `isDrawOnTopLayer` | `bool` |  |
| `fileDataIDs` | `number[]` |  |
| `hitRect` | `UiMapExplorationHitRect` |  |
