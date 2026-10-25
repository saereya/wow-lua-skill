# HouseEditorUI

Namespace `C_HouseEditor` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/houseeditoruidocumentation.lua` (FileDataID 6324857)

## Functions

### ActivateHouseEditorMode

```lua
C_HouseEditor.ActivateHouseEditorMode(editMode: HouseEditorMode) -> result: HousingResult
```

Attempts switch the House Editor to a specific House Editor mode

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `result` | `HousingResult` | The initial result of the attempt to activate the mode; If Success, mode is either already active, or we've succesfully started making required requests to server; Listen for MODE_CHANGED or MODE_CHANGE_FAILURE events for ultimate end result after server calls |

### EnterHouseEditor

```lua
C_HouseEditor.EnterHouseEditor() -> result: HousingResult
```

Attempts to open the House Editor to the default House Editor mode

Returns:

| Name | Type | Notes |
|---|---|---|
| `result` | `HousingResult` | The initial result of the attempt to open the Editor; If Success, Editor is either already active, or we've succesfully started making required requests to server; Listen for MODE_CHANGED or MODE_CHANGE_FAILURE events for ultimate end result after server calls |

### GetActiveHouseEditorMode

```lua
C_HouseEditor.GetActiveHouseEditorMode() -> editMode: HouseEditorMode
```

### GetHouseEditorAvailability

```lua
C_HouseEditor.GetHouseEditorAvailability() -> result: HousingResult
```

Returns the availability state of the House Editor overall

### GetHouseEditorModeAvailability

```lua
C_HouseEditor.GetHouseEditorModeAvailability(editMode: HouseEditorMode) -> result: HousingResult
```

Returns the availability of a specific House Editor mode

`SecretArguments=AllowedWhenUntainted`

### GetHouseEditorPlayerType

```lua
C_HouseEditor.GetHouseEditorPlayerType() -> playerType: HouseEditorPlayerType
```

### IsHouseEditorActive

```lua
C_HouseEditor.IsHouseEditorActive() -> isEditorActive: bool
```

Returns whether the House Editor is active, in any mode

### IsHouseEditorModeActive

```lua
C_HouseEditor.IsHouseEditorModeActive(editMode: HouseEditorMode) -> isModeActive: bool
```

Returns whether the specific House Editor mode is active

`SecretArguments=AllowedWhenUntainted`

### IsHouseEditorStatusAvailable

```lua
C_HouseEditor.IsHouseEditorStatusAvailable() -> editorStatusAvailable: bool
```

Returns true if the HouseEditor currently able process mode availability and switching; May be false if not in a house or plot, or while waiting to get house settings back from the server

### LeaveHouseEditor

```lua
C_HouseEditor.LeaveHouseEditor()
```

## Events

### HOUSE_EDITOR_AVAILABILITY_CHANGED

```lua
HOUSE_EDITOR_AVAILABILITY_CHANGED()
```

`SynchronousEvent`

### HOUSE_EDITOR_MODE_CHANGED

```lua
HOUSE_EDITOR_MODE_CHANGED(currentEditMode: HouseEditorMode)
```

`SynchronousEvent`

### HOUSE_EDITOR_MODE_CHANGE_FAILURE

```lua
HOUSE_EDITOR_MODE_CHANGE_FAILURE(result: HousingResult)
```

`SynchronousEvent`

## Types

### HouseEditorPlayerType

*Enumeration* · 3 values, 0..2

Access values as `Enum.HouseEditorPlayerType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HouseEditorPlayerType` | = 0; Not in a house or plot, or at one without even sufficient visiting permissions |
| `Owner` | `HouseEditorPlayerType` | = 1; Owner of the current house or plot |
| `Visitor` | `HouseEditorPlayerType` | = 2; A visitor of the current house or plot |
