# Texture

Widget methods (`SimpleTextureAPI`) · inherits [`TextureBase`](TextureBase.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/simpletextureapidocumentation.lua` (FileDataID 4637233)

## Methods

### AddMaskTexture

```lua
Texture:AddMaskTexture(mask: SimpleMaskTexture)
```

`SecretArguments=AllowedWhenUntainted`

### GetMaskTexture

```lua
Texture:GetMaskTexture(index: luaIndex) -> mask: SimpleMaskTexture
```

`SecretArguments=AllowedWhenUntainted` `SecretReturnsForAspect={ Enum.SecretAspect.Hierarchy }` `ConstSecretAccessor`

### GetNumMaskTextures

```lua
Texture:GetNumMaskTextures() -> count: size
```

`SecretReturnsForAspect={ Enum.SecretAspect.Hierarchy }`

### RemoveMaskTexture

```lua
Texture:RemoveMaskTexture(mask: SimpleMaskTexture)
```

`SecretArguments=AllowedWhenUntainted`
