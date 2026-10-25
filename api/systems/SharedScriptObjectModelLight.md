# SharedScriptObjectModelLight

source `interface/addons/blizzard_apidocumentationgenerated/sharedscriptobjectmodellightdocumentation.lua` (FileDataID 4637195)

## Types

### ModelLight

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `omnidirectional` | `bool` | default `false` |
| `point` | `vector3` | If this light is omnidirectional then point refers to a position, otherwise it refers to a direction; `Mixin=Vector3DMixin` |
| `ambientIntensity` | `number` | default `0` |
| `ambientColor` | `colorRGB?` | `Mixin=ColorMixin` |
| `diffuseIntensity` | `number` | default `0` |
| `diffuseColor` | `colorRGB?` | `Mixin=ColorMixin` |
