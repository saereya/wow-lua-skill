# ChromieTimeInfo

Namespace `C_ChromieTime` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/chromietimeuidocumentation.lua` (FileDataID 4637051)

## Functions

### CloseUI

```lua
C_ChromieTime.CloseUI()
```

### GetChromieTimeExpansionOption

```lua
C_ChromieTime.GetChromieTimeExpansionOption(expansionRecID: number) -> info: ChromieTimeExpansionInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetChromieTimeExpansionOptions

```lua
C_ChromieTime.GetChromieTimeExpansionOptions() -> expansionOptions: ChromieTimeExpansionInfo[]
```

### SelectChromieTimeOption

```lua
C_ChromieTime.SelectChromieTimeOption(chromieTimeExpansionInfoId: number)
```

`SecretArguments=AllowedWhenUntainted`

## Types

### ChromieTimeExpansionInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `id` | `number` |  |
| `name` | `cstring` |  |
| `description` | `cstring` |  |
| `mapAtlas` | `textureAtlas` |  |
| `previewAtlas` | `textureAtlas` |  |
| `completed` | `bool` |  |
| `alreadyOn` | `bool` |  |
| `recommended` | `bool` |  |
| `sortPriority` | `number` |  |
