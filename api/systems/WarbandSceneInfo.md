# WarbandSceneInfo

Namespace `C_WarbandScene` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/warbandsceneinfodocumentation.lua` (FileDataID 6322703)

## Functions

### GetRandomEntryID

```lua
C_WarbandScene.GetRandomEntryID() -> warbandSceneID: number
```

### GetWarbandSceneEntry

```lua
C_WarbandScene.GetWarbandSceneEntry(warbandSceneID: number) -> warbandSceneEntry: WarbandSceneEntry
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### HasWarbandScene

```lua
C_WarbandScene.HasWarbandScene(warbandSceneID: number) -> owned: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsFavorite

```lua
C_WarbandScene.IsFavorite(warbandSceneID: number) -> favorite: bool
```

`SecretArguments=AllowedWhenUntainted`

### SearchWarbandSceneEntries

```lua
C_WarbandScene.SearchWarbandSceneEntries(searchParams: WarbandSceneSearchInfo) -> matchingEntryIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### SetFavorite

```lua
C_WarbandScene.SetFavorite(warbandSceneID: number, favorite: bool)
```

`SecretArguments=AllowedWhenUntainted`

### WarbandScenesAvailable

```lua
C_WarbandScene.WarbandScenesAvailable() -> areWarbandScenesAvailable: bool
```

## Events

### NEW_WARBAND_SCENE_ADDED

```lua
NEW_WARBAND_SCENE_ADDED(warbandScenID: number)
```

`SynchronousEvent`

### WARBAND_SCENE_FAVORITES_UPDATED

```lua
WARBAND_SCENE_FAVORITES_UPDATED()
```

`SynchronousEvent`

## Types

### WarbandSceneEntry

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `warbandSceneID` | `number` | default `0` |
| `name` | `cstring` |  |
| `description` | `cstring` |  |
| `source` | `cstring` |  |
| `quality` | `number` |  |
| `textureKit` | `textureKit` |  |
| `isFavorite` | `bool` | default `false` |
| `hasFanfare` | `bool` | default `false` |
| `sourceType` | `number` | default `0` |

### WarbandSceneSearchInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ownedOnly` | `bool` | default `false` |
| `favoritesOnly` | `bool` | default `false` |
