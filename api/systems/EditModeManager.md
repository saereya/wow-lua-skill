# EditModeManager

Namespace `C_EditMode` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/editmodemanagerdocumentation.lua` (FileDataID 4637089)

## Functions

### ConvertLayoutInfoToString

```lua
C_EditMode.ConvertLayoutInfoToString(layoutInfo: EditModeLayoutInfo) -> layoutInfoAsString: string
```

`SecretArguments=AllowedWhenUntainted`

### ConvertStringToLayoutInfo

```lua
C_EditMode.ConvertStringToLayoutInfo(layoutInfoAsString: string) -> layoutInfo: EditModeLayoutInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetAccountSettings

```lua
C_EditMode.GetAccountSettings() -> accountSettings: EditModeSettingInfo[]
```

### GetEditModeDefaultLayout

```lua
C_EditMode.GetEditModeDefaultLayout() -> defaultLayout: number
```

### GetLayouts

```lua
C_EditMode.GetLayouts() -> layoutInfo: EditModeLayouts
```

### IsValidLayoutName

```lua
C_EditMode.IsValidLayoutName(name: cstring) -> isApproved: bool
```

`SecretArguments=AllowedWhenUntainted`

### OnEditModeExit

```lua
C_EditMode.OnEditModeExit()
```

### OnLayoutAdded

```lua
C_EditMode.OnLayoutAdded(addedLayoutIndex: luaIndex, activateNewLayout: bool, isLayoutImported: bool)
```

`SecretArguments=AllowedWhenUntainted`

### OnLayoutDeleted

```lua
C_EditMode.OnLayoutDeleted(deletedLayoutIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### SaveLayouts

```lua
C_EditMode.SaveLayouts(saveInfo: EditModeLayouts)
```

`SecretArguments=AllowedWhenUntainted`

### SetAccountSetting

```lua
C_EditMode.SetAccountSetting(setting: EditModeAccountSetting, value: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetActiveLayout

```lua
C_EditMode.SetActiveLayout(activeLayout: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### EDIT_MODE_LAYOUTS_UPDATED

```lua
EDIT_MODE_LAYOUTS_UPDATED(layoutInfo: EditModeLayouts, reconcileLayouts: bool)
```

`SynchronousEvent`

## Types

### EditModeAnchorInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `point` | `FramePoint` |  |
| `relativeTo` | `string` |  |
| `relativePoint` | `FramePoint` |  |
| `offsetX` | `number` |  |
| `offsetY` | `number` |  |

### EditModeLayoutInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `layoutName` | `string` |  |
| `layoutType` | `EditModeLayoutType` |  |
| `interfaceStyle` | `InputDeviceInterfaceType?` |  |
| `systems` | `EditModeSystemInfo[]` |  |

### EditModeLayouts

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `layouts` | `EditModeLayoutInfo[]` |  |
| `activeLayout` | `luaIndex` |  |

### EditModeSettingInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `setting` | `number` |  |
| `value` | `number` |  |

### EditModeSystemInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `system` | `EditModeSystem` |  |
| `systemIndex` | `luaIndex?` |  |
| `anchorInfo` | `EditModeAnchorInfo` |  |
| `anchorInfo2` | `EditModeAnchorInfo?` |  |
| `settings` | `EditModeSettingInfo[]` |  |
| `isInDefaultPosition` | `bool` |  |
