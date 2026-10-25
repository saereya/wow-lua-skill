# SimpleStatusBarConstants

source `interface/addons/blizzard_apidocumentationgenerated/simplestatusbarconstantsdocumentation.lua` (FileDataID 7577822)

## Types

### StatusBarFillStyle

*Enumeration* · 4 values, 0..3

Access values as `Enum.StatusBarFillStyle.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Standard` | `StatusBarFillStyle` | = 0; Fills the bar regularly, either in a left-to-right or top-to-bottom direction as values increase. |
| `StandardNoRangeFill` | `StatusBarFillStyle` | = 1; Similar to standard, except if the range between the min and max values is zero instead render as-if the bar were 100% full. If the min and max values are both zero, will render as 0% full. |
| `Center` | `StatusBarFillStyle` | = 2; Fills the bar in an outward growing manner from the center. |
| `Reverse` | `StatusBarFillStyle` | = 3; Inverse of Standard, filling right-to-left or bottom-to-top as values increase. |

### StatusBarInterpolation

*Enumeration* · 2 values, 0..1

Access values as `Enum.StatusBarInterpolation.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Immediate` | `StatusBarInterpolation` | = 0; Immediately snap to the target value with no interpolation. |
| `ExponentialEaseOut` | `StatusBarInterpolation` | = 1; Interpolate the bar toward the target value with exponential ease-out style decay. |

### StatusBarRenderMode

*Enumeration* · 2 values, 0..1

Access values as `Enum.StatusBarRenderMode.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Linear` | `StatusBarRenderMode` | = 0; Render the status bar using the existing linear horizontal or vertical fill behavior. |
| `Radial` | `StatusBarRenderMode` | = 1; Render the status bar by driving the managed texture's radial progress fill percent instead of resizing the texture anchors. |

### StatusBarTimerDirection

*Enumeration* · 2 values, 0..1

Access values as `Enum.StatusBarTimerDirection.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `ElapsedTime` | `StatusBarTimerDirection` | = 0; Calculate status timer bar values using the elapsed time of a duration. |
| `RemainingTime` | `StatusBarTimerDirection` | = 1; Calculate status timer bar values using the remaining time of a duration. |
