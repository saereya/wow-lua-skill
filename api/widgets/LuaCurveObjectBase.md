# LuaCurveObjectBase

Widget methods (`LuaCurveObjectBaseAPI`) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/luacurveobjectbaseapidocumentation.lua` (FileDataID 7657069)

## Methods

### GetType

```lua
LuaCurveObjectBase:GetType() -> curveType: LuaCurveType
```

Returns the configured type of the curve.

### HasSecretValues

```lua
LuaCurveObjectBase:HasSecretValues() -> hasSecretValues: bool
```

Returns true if the curve has been configured with any secret values. Curves with secret values always produce secret results when evaluated.

`ReturnsNeverSecret`

### SetType

```lua
LuaCurveObjectBase:SetType(type: LuaCurveType)
```

Changes the evaluation type of the curve.

`SecretArguments=AllowedWhenUntainted`
