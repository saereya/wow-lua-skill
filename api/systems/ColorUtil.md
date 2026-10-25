# ColorUtil

Namespace `C_ColorUtil` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/colorutildocumentation.lua` (FileDataID 7570648)

## Functions

### ConvertHSLToHSV

```lua
C_ColorUtil.ConvertHSLToHSV(hslH: number, hslS: number, hslL: number) -> hsvH: number, hsvS: number, hsvV: number
```

Converts an unpacked HSL color to HSV.

`SecretArguments=AllowedWhenUntainted`

### ConvertHSVToHSL

```lua
C_ColorUtil.ConvertHSVToHSL(hsvH: number, hsvS: number, hsvV: number) -> hslH: number, hslS: number, hslL: number
```

Converts an unpacked HSV color to HSL.

`SecretArguments=AllowedWhenUntainted`

### ConvertHSVToRGB

```lua
C_ColorUtil.ConvertHSVToRGB(hsvH: number, hsvS: number, hsvV: number) -> rgbR: number, rgbG: number, rgbB: number
```

Converts an unpacked HSV color to RGB.

`SecretArguments=AllowedWhenUntainted`

### ConvertRGBToHSV

```lua
C_ColorUtil.ConvertRGBToHSV(rgbR: number, rgbG: number, rgbB: number) -> hsvH: number, hsvS: number, hsvV: number
```

Converts an unpacked RGB color to HSV. For achromatic inputs, the returned hue will be -1.

`SecretArguments=AllowedWhenUntainted`

### GenerateTextColorCode

```lua
C_ColorUtil.GenerateTextColorCode(color: colorRGB) -> textColorCode: string
```

Generates a hex color code suitable for use in text color code markup.

`SecretArguments=AllowedWhenTainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `color` | `colorRGB` | Color to generate a hex color code from.; `Mixin=ColorMixin` |

Returns:

| Name | Type | Notes |
|---|---|---|
| `textColorCode` | `string` | Hex representation of the color formatted as an 8-byte ARGB string, with alpha forced to 255. |

### WrapTextInColor

```lua
C_ColorUtil.WrapTextInColor(text: cstring, color: colorRGB) -> coloredText: string
```

Wraps a given string with color code markup.

`SecretArguments=AllowedWhenTainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` | Text to be wrapped in color markup. |
| `color` | `colorRGB` | Color to apply to the text.; `Mixin=ColorMixin` |

Returns:

| Name | Type | Notes |
|---|---|---|
| `coloredText` | `string` | The input text wrapped in '\|c' and '\|r' quoted code sequences for the supplied color. |

### WrapTextInColorCode

```lua
C_ColorUtil.WrapTextInColorCode(text: cstring, textColorCode: cstring) -> coloredText: string
```

Wraps a given string with color code markup.

`SecretArguments=AllowedWhenTainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` | Text to be wrapped in color markup. |
| `textColorCode` | `cstring` | Color to apply to the text, formatted as an 8-byte ARGB string as returned by GenerateTextColorCode. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `coloredText` | `string` | The input text wrapped in '\|c' and '\|r' quoted code sequences for the supplied color. |
