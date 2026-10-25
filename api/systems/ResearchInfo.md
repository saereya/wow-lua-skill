# ResearchInfo

Namespace `C_ResearchInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/researchinfodocumentation.lua` (FileDataID 4637182)

## Functions

### GetDigSitesForMap

```lua
C_ResearchInfo.GetDigSitesForMap(uiMapID: number) -> digSites: DigSiteMapInfo[]
```

`SecretArguments=AllowedWhenUntainted`

## Events

### ARCHAEOLOGY_CLOSED

```lua
ARCHAEOLOGY_CLOSED()
```

`SynchronousEvent`

### ARCHAEOLOGY_FIND_COMPLETE

```lua
ARCHAEOLOGY_FIND_COMPLETE(numFindsCompleted: number, totalFinds: number, researchBranchID: number)
```

`SynchronousEvent`

### ARCHAEOLOGY_SURVEY_CAST

```lua
ARCHAEOLOGY_SURVEY_CAST(numFindsCompleted: number, totalFinds: number, researchBranchID: number, successfulFind: number)
```

`SynchronousEvent`

### ARCHAEOLOGY_TOGGLE

```lua
ARCHAEOLOGY_TOGGLE()
```

`SynchronousEvent`

### ARTIFACT_DIGSITE_COMPLETE

```lua
ARTIFACT_DIGSITE_COMPLETE(researchBranchID: number)
```

`SynchronousEvent`

### RESEARCH_ARTIFACT_COMPLETE

```lua
RESEARCH_ARTIFACT_COMPLETE(name: cstring)
```

`SynchronousEvent`

### RESEARCH_ARTIFACT_DIG_SITE_UPDATED

```lua
RESEARCH_ARTIFACT_DIG_SITE_UPDATED()
```

`SynchronousEvent`

### RESEARCH_ARTIFACT_UPDATE

```lua
RESEARCH_ARTIFACT_UPDATE()
```

`SynchronousEvent`

## Types

### DigSiteMapInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `researchSiteID` | `number` |  |
| `position` | `vector2` | `Mixin=Vector2DMixin` |
| `name` | `cstring` |  |
| `poiBlobID` | `number` |  |
| `textureIndex` | `number` |  |
