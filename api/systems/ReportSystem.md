# ReportSystem

Namespace `C_ReportSystem` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/reportsystemdocumentation.lua` (FileDataID 4637184)

## Functions

### CanReportPlayer

```lua
C_ReportSystem.CanReportPlayer(playerLocation: PlayerLocation) -> canReport: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `playerLocation` | `PlayerLocation` | `Mixin=PlayerLocationMixin` |

### CanReportPlayerForLanguage

```lua
C_ReportSystem.CanReportPlayerForLanguage(playerLocation: PlayerLocation) -> canReport: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `playerLocation` | `PlayerLocation` | `Mixin=PlayerLocationMixin` |

### GetMajorCategoriesForReportType

```lua
C_ReportSystem.GetMajorCategoriesForReportType(reportType: ReportType) -> majorCategories: ReportMajorCategory[]
```

`SecretArguments=AllowedWhenUntainted`

### GetMajorCategoryString

```lua
C_ReportSystem.GetMajorCategoryString(majorCategory: ReportMajorCategory) -> majorCategoryString: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetMinorCategoriesForReportTypeAndMajorCategory

```lua
C_ReportSystem.GetMinorCategoriesForReportTypeAndMajorCategory(reportType: ReportType, majorCategory: ReportMajorCategory) -> minorCategories: ReportMinorCategory[]
```

`SecretArguments=AllowedWhenUntainted`

### GetMinorCategoryString

```lua
C_ReportSystem.GetMinorCategoryString(minorCategory: ReportMinorCategory) -> minorCategoryString: cstring
```

`SecretArguments=AllowedWhenUntainted`

### ReportServerLag

```lua
C_ReportSystem.ReportServerLag()
```

### ReportStuckInCombat

```lua
C_ReportSystem.ReportStuckInCombat()
```

### RequiresScreenshotForReportType

```lua
C_ReportSystem.RequiresScreenshotForReportType(reportType: ReportType, majorCategory: ReportMajorCategory) -> requiresScreenshot: bool
```

`SecretArguments=AllowedWhenUntainted`

### SendReport

```lua
C_ReportSystem.SendReport(reportInfo: ReportInfo, playerLocation: PlayerLocation?)
```

Not allowed to be called by addons

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `reportInfo` | `ReportInfo` | `Mixin=ReportInfoMixin` |
| `playerLocation` | `PlayerLocation?` | `Mixin=PlayerLocationMixin` |

### SetScreenshotPreviewTexture

```lua
C_ReportSystem.SetScreenshotPreviewTexture(textureObject: SimpleTexture)
```

`SecretArguments=AllowedWhenUntainted`

### TakeReportScreenshot

```lua
C_ReportSystem.TakeReportScreenshot()
```

## Events

### REPORT_PLAYER_RESULT

```lua
REPORT_PLAYER_RESULT(result: SendReportResult, reportType: ReportType)
```

`SynchronousEvent`

### REPORT_SCREENSHOT_READY

```lua
REPORT_SCREENSHOT_READY()
```

`SynchronousEvent`
