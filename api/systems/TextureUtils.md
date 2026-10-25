# TextureUtils

Namespace `C_Texture` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/textureutilsdocumentation.lua` (FileDataID 4637274)

## Functions

### ClearTitleIconTexture

```lua
C_Texture.ClearTitleIconTexture(texture: SimpleTexture)
```

`SecretArguments=AllowedWhenUntainted`

### GetAtlasElementID

```lua
C_Texture.GetAtlasElementID(atlas: textureAtlas) -> elementID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetAtlasElements

```lua
C_Texture.GetAtlasElements() -> atlases: textureAtlas[]
```

### GetAtlasExists

```lua
C_Texture.GetAtlasExists(atlas: textureAtlas) -> atlasExists: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetAtlasID

```lua
C_Texture.GetAtlasID(atlas: textureAtlas) -> atlasID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetAtlasInfo

```lua
C_Texture.GetAtlasInfo(atlas: textureAtlas) -> info: AtlasInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetFilenameFromFileDataID

```lua
C_Texture.GetFilenameFromFileDataID(fileDataID: number) -> filename: string
```

`SecretArguments=AllowedWhenUntainted`

### GetTitleIconTexture

```lua
C_Texture.GetTitleIconTexture(titleID: string, version: TitleIconVersion, callback: GetTitleIconTextureCallback)
```

`SecretArguments=AllowedWhenUntainted`

### IsTitleIconTextureReady

```lua
C_Texture.IsTitleIconTextureReady(titleID: string, version: TitleIconVersion) -> ready: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetTitleIconTexture

```lua
C_Texture.SetTitleIconTexture(texture: SimpleTexture, titleID: string, version: TitleIconVersion)
```

`SecretArguments=AllowedWhenUntainted`

### SetURLTexture

```lua
C_Texture.SetURLTexture(texture: SimpleTexture, url: cstring)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

## Events

### URL_TEXTURE_REQUEST_RESULT

```lua
URL_TEXTURE_REQUEST_RESULT(texture: SimpleTexture, result: UrlTextureResult)
```

`SynchronousEvent`

## Types

### TitleIconVersion

*Enumeration* · 3 values, 0..2

Access values as `Enum.TitleIconVersion.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Small` | `TitleIconVersion` | = 0 |
| `Medium` | `TitleIconVersion` | = 1 |
| `Large` | `TitleIconVersion` | = 2 |

### UrlTextureResult

*Enumeration* · 4 values, 1..4

Access values as `Enum.UrlTextureResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Found` | `UrlTextureResult` | = 1 |
| `NotFound` | `UrlTextureResult` | = 2 |
| `Requested` | `UrlTextureResult` | = 3 |
| `NotAllowed` | `UrlTextureResult` | = 4 |

### AtlasInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `elementName` | `cstring` |  |
| `width` | `number` |  |
| `height` | `number` |  |
| `rawSize` | `vector2` | `Mixin=Vector2DMixin` |
| `leftTexCoord` | `number` |  |
| `rightTexCoord` | `number` |  |
| `topTexCoord` | `number` |  |
| `bottomTexCoord` | `number` |  |
| `tilesHorizontally` | `bool` |  |
| `tilesVertically` | `bool` |  |
| `file` | `fileID?` |  |
| `filename` | `string?` |  |
| `sliceData` | `UITextureSliceData?` |  |

### GetTitleIconTextureCallback

*CallbackType*

Arguments:

| Name | Type | Notes |
|---|---|---|
| `success` | `bool` |  |
| `texture` | `fileID` |  |
