# UIEventToastManagerInfo

Namespace `C_EventToastManager` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/uieventtoastmanagerdocumentation.lua` (FileDataID 4637272)

## Functions

### GetLevelUpDisplayToastsFromLevel

```lua
C_EventToastManager.GetLevelUpDisplayToastsFromLevel(level: number) -> toastInfo: EventToastInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetNextToastToDisplay

```lua
C_EventToastManager.GetNextToastToDisplay() -> toastInfo: EventToastInfo
```

`MayReturnNothing`

### RemoveCurrentToast

```lua
C_EventToastManager.RemoveCurrentToast()
```

## Events

### DISPLAY_EVENT_TOAST_LINK

```lua
DISPLAY_EVENT_TOAST_LINK(link: string)
```

`SynchronousEvent`

### DISPLAY_EVENT_TOASTS

```lua
DISPLAY_EVENT_TOASTS()
```

`SynchronousEvent`

## Types

### EventToastInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `eventToastID` | `number` |  |
| `title` | `string` |  |
| `subtitle` | `string` |  |
| `instructionText` | `string` |  |
| `iconFileID` | `fileID` |  |
| `subIcon` | `textureAtlas?` |  |
| `link` | `string` |  |
| `qualityString` | `string?` |  |
| `quality` | `number?` |  |
| `eventType` | `EventToastEventType` |  |
| `displayType` | `EventToastDisplayType` |  |
| `uiTextureKit` | `textureKit` |  |
| `sortOrder` | `number` |  |
| `time` | `number?` |  |
| `uiWidgetSetID` | `number?` |  |
| `extraUiWidgetSetID` | `number?` |  |
| `titleTooltip` | `string?` |  |
| `subtitleTooltip` | `string?` |  |
| `titleTooltipUiWidgetSetID` | `number?` |  |
| `subtitleTooltipUiWidgetSetID` | `number?` |  |
| `showSoundKitID` | `number?` |  |
| `hideSoundKitID` | `number?` |  |
| `colorTint` | `colorRGB?` | `Mixin=ColorMixin` |
| `flags` | `number` |  |
