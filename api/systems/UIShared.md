# UIShared

source `interface/addons/blizzard_apidocumentationgenerated/uishareddocumentation.lua` (FileDataID 4637298)

## Types

### FontStringScaleAnimationMode

*Enumeration* · 2 values, 0..1

Access values as `Enum.FontStringScaleAnimationMode.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `FontSize` | `FontStringScaleAnimationMode` | = 0; Scale animations apply to the height of the font. This will cause small jumps between different font heights as the animation progresses, and may adjust the layout of text if used on a fixed-size font string. |
| `Vertex` | `FontStringScaleAnimationMode` | = 1; Scale animations apply to the vertices of the font. Scaling is smoother, but if used on non-slug fonts may cause significant pixelation of the font text, Layout of the text is not adjusted as the animation progresses, and the direction of scaling respects horizontal and vertical justification settings (eg. text at the bottom-right scaling up grows toward the top-left). |

### AnchorBinding

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `point` | `FramePoint` |  |
| `relativeTo` | `ScriptRegion` |  |
| `relativePoint` | `FramePoint` |  |
| `offsetX` | `uiUnit` |  |
| `offsetY` | `uiUnit` |  |

### uiBoundsRect

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `left` | `uiUnit` |  |
| `bottom` | `uiUnit` |  |
| `width` | `uiUnit` |  |
| `height` | `uiUnit` |  |

## Predicates

Conditions referenced by the flags above.

- `IsProtectedFunction` *Precondition* (failure mode: ReturnNothing)
