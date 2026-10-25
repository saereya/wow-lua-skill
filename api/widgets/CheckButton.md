# CheckButton

Widget methods (`SimpleCheckboxAPI`) · inherits [`Button`](Button.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/simplecheckboxapidocumentation.lua` (FileDataID 4637211)

## Methods

### GetChecked

```lua
CheckButton:GetChecked() -> checked: bool
```

### GetCheckedTexture

```lua
CheckButton:GetCheckedTexture() -> texture: SimpleTexture
```

### GetDisabledCheckedTexture

```lua
CheckButton:GetDisabledCheckedTexture() -> texture: SimpleTexture
```

### SetChecked

```lua
CheckButton:SetChecked(checked: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `checked` | `bool` | default `false` |

### SetCheckedTexture

```lua
CheckButton:SetCheckedTexture(asset: TextureAsset)
```

`SecretArguments=AllowedWhenUntainted` `CheckAllowChangeParent`

### SetDisabledCheckedTexture

```lua
CheckButton:SetDisabledCheckedTexture(asset: TextureAsset)
```

`SecretArguments=AllowedWhenUntainted` `CheckAllowChangeParent`
