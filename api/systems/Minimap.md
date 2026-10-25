# Minimap

Namespace `C_Minimap` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/minimapdocumentation.lua` (FileDataID 4637146)

## Functions

### CanTrackBattlePets

```lua
C_Minimap.CanTrackBattlePets() -> CanTrackBattlePets: bool
```

### ClearAllTracking

```lua
C_Minimap.ClearAllTracking()
```

### ClearMinimapInsetInfo

```lua
C_Minimap.ClearMinimapInsetInfo()
```

### GetDefaultTrackingValue

```lua
C_Minimap.GetDefaultTrackingValue(filterType: MinimapTrackingFilter) -> defaultValue: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetDrawGroundTextures

```lua
C_Minimap.GetDrawGroundTextures() -> draw: bool
```

### GetNumQuestPOIWorldEffects

```lua
C_Minimap.GetNumQuestPOIWorldEffects() -> worldEffectCount: number
```

### GetNumTrackingTypes

```lua
C_Minimap.GetNumTrackingTypes() -> numTrackingTypes: number
```

### GetPOITextureCoords

```lua
C_Minimap.GetPOITextureCoords(index: number?) -> textureCoordsX: number, textureCoordsY: number, textureCoordsZ: number, textureCoordsW: number
```

`SecretArguments=AllowedWhenUntainted`

### GetTrackingFilter

```lua
C_Minimap.GetTrackingFilter(spellIndex: luaIndex) -> trackingType: MinimapScriptTrackingFilter
```

`SecretArguments=AllowedWhenUntainted`

### GetTrackingInfo

```lua
C_Minimap.GetTrackingInfo(spellIndex: luaIndex) -> trackingInfo: MinimapScriptTrackingInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetUiMapID

```lua
C_Minimap.GetUiMapID() -> uiMapID: number?
```

### GetViewRadius

```lua
C_Minimap.GetViewRadius() -> yards: number
```

### IsFilteredOut

```lua
C_Minimap.IsFilteredOut(filterType: MinimapTrackingFilter) -> isFiltered: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsInsideQuestBlob

```lua
C_Minimap.IsInsideQuestBlob(questID: number) -> isInside: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsRotateMinimapIgnored

```lua
C_Minimap.IsRotateMinimapIgnored() -> isIgnored: bool
```

### IsTrackingAccountCompletedQuests

```lua
C_Minimap.IsTrackingAccountCompletedQuests() -> IsTrackingAccountCompletedQuests: bool
```

### IsTrackingBattlePets

```lua
C_Minimap.IsTrackingBattlePets() -> isTrackingBattlePets: bool
```

### IsTrackingHiddenQuests

```lua
C_Minimap.IsTrackingHiddenQuests() -> isTrackingHiddenQuests: bool
```

### SetDrawGroundTextures

```lua
C_Minimap.SetDrawGroundTextures(draw: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetIgnoreRotateMinimap

```lua
C_Minimap.SetIgnoreRotateMinimap(ignore: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetMinimapInsetInfo

```lua
C_Minimap.SetMinimapInsetInfo(minAngle: number, maxAngle: number, scalar: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetTracking

```lua
C_Minimap.SetTracking(index: luaIndex, on: bool)
```

`SecretArguments=AllowedWhenUntainted`

### ShouldUseHybridMinimap

```lua
C_Minimap.ShouldUseHybridMinimap() -> shouldUse: bool
```

## Events

### MINIMAP_PING

```lua
MINIMAP_PING(unitTarget: UnitTokenVariant, y: number, x: number)
```

`SecretPayloads` `HasRestrictions` `CallbackEvent`

### MINIMAP_UPDATE_TRACKING

```lua
MINIMAP_UPDATE_TRACKING()
```

`UniqueEvent`

### MINIMAP_UPDATE_ZOOM

```lua
MINIMAP_UPDATE_ZOOM()
```

`UniqueEvent`

### PLAYER_INSIDE_QUEST_BLOB_STATE_CHANGED

```lua
PLAYER_INSIDE_QUEST_BLOB_STATE_CHANGED(questID: number, isInside: bool)
```

`SynchronousEvent`

## Types

### MinimapScriptTrackingFilter

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `number?` |  |
| `filterID` | `MinimapTrackingFilter?` |  |

### MinimapScriptTrackingInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `texture` | `fileID` |  |
| `active` | `bool` |  |
| `type` | `cstring` |  |
| `subType` | `number` |  |
| `spellID` | `number?` |  |
