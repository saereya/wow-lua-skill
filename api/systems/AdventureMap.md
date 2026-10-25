# AdventureMap

Namespace `C_AdventureMap` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/adventuremapdocumentation.lua` (FileDataID 4637009)

## Functions

### GetAdventureMapTextureKit

```lua
C_AdventureMap.GetAdventureMapTextureKit() -> adventureMapTextureKit: textureKit
```

### GetNumMapInsets

```lua
C_AdventureMap.GetNumMapInsets() -> numMapInsets: number
```

### GetNumQuestOffers

```lua
C_AdventureMap.GetNumQuestOffers() -> numQuestOffers: number
```

### GetNumZoneChoices

```lua
C_AdventureMap.GetNumZoneChoices() -> numZoneChoices: number
```

### GetQuestPortraitInfo

```lua
C_AdventureMap.GetQuestPortraitInfo(questID: number) -> info: AdventureMapQuestPortraitInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

## Events

### ADVENTURE_MAP_CLOSE

```lua
ADVENTURE_MAP_CLOSE()
```

`SynchronousEvent`

### ADVENTURE_MAP_OPEN

```lua
ADVENTURE_MAP_OPEN(followerTypeID: number)
```

`SynchronousEvent`

### ADVENTURE_MAP_QUEST_UPDATE

```lua
ADVENTURE_MAP_QUEST_UPDATE(questID: number)
```

`SynchronousEvent`

### ADVENTURE_MAP_UPDATE_INSETS

```lua
ADVENTURE_MAP_UPDATE_INSETS()
```

`UniqueEvent`

### ADVENTURE_MAP_UPDATE_POIS

```lua
ADVENTURE_MAP_UPDATE_POIS()
```

`UniqueEvent`

## Types

### AdventureMapQuestPortraitInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `portraitDisplayID` | `number` |  |
| `mountPortraitDisplayID` | `number` |  |
| `name` | `string` |  |
| `text` | `string` |  |
| `modelSceneID` | `number?` |  |
