# LuaCurveObjectConstants

source `interface/addons/blizzard_apidocumentationgenerated/luacurveobjectconstantsdocumentation.lua` (FileDataID 7507383)

## Types

### LuaCurveType

*Enumeration* · 4 values, 0..3

Access values as `Enum.LuaCurveType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Linear` | `LuaCurveType` | = 0; Linearly interpolates between points. |
| `Step` | `LuaCurveType` | = 1; Performs no interpolation between points, instead snapping to values exactly. |
| `Cosine` | `LuaCurveType` | = 2; Interpolates between points with cosine smoothing applied. |
| `Cubic` | `LuaCurveType` | = 3; Interpolates between points with cubic smoothing applied. Requires a minimum of four points be defined; less than this will fall back to Cosine interpolation. |
