# GenericWidgetDisplay

Namespace `C_GenericWidgetDisplay` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/uigenericwidgetdisplaydocumentation.lua` (FileDataID 4870627)

## Functions

### Acknowledge

```lua
C_GenericWidgetDisplay.Acknowledge()
```

### Close

```lua
C_GenericWidgetDisplay.Close()
```

## Events

### GENERIC_WIDGET_DISPLAY_SHOW

```lua
GENERIC_WIDGET_DISPLAY_SHOW(info: GenericWidgetDisplayFrameInfo)
```

`SynchronousEvent`

## Types

### GenericWidgetDisplayFrameInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `uiWidgetSetID` | `number?` |  |
| `uiTextureKit` | `textureKit?` |  |
| `title` | `string?` |  |
| `frameWidth` | `number` |  |
| `frameHeight` | `number` |  |
| `extraButtonText` | `string?` |  |
| `closeButtonText` | `string?` |  |
