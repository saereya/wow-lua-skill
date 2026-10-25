# AddOnProfilerConstants

source `interface/addons/blizzard_apidocumentationgenerated/addonprofilerconstantsdocumentation.lua` (FileDataID 6377825)

## Types

### AddOnPerformanceMessageType

*Enumeration* · 3 values, 0..2

Access values as `Enum.AddOnPerformanceMessageType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `SpecificAddOnChatWarning` | `AddOnPerformanceMessageType` | = 0; Warning in chat when an AddOn is close to exceeding thresholds. |
| `SpecificAddOnErrorDialog` | `AddOnPerformanceMessageType` | = 1; Error message modal dialog when an AddOn has exceeded thresholds. |
| `OverallAddOnErrorDialog` | `AddOnPerformanceMessageType` | = 2; Error message modal dialog when all AddOns combined have exceeded thresholds. |

### AddOnProfilerMetric

*Enumeration* · 12 values, 0..11

Access values as `Enum.AddOnProfilerMetric.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `SessionAverageTime` | `AddOnProfilerMetric` | = 0; Average time since application startup |
| `RecentAverageTime` | `AddOnProfilerMetric` | = 1; Average time over the last 60 ticks |
| `EncounterAverageTime` | `AddOnProfilerMetric` | = 2; Average time over the duration of a boss encounter |
| `LastTime` | `AddOnProfilerMetric` | = 3; Total time in the most recent tick |
| `PeakTime` | `AddOnProfilerMetric` | = 4; Highest time recorded since application startup |
| `CountTimeOver1Ms` | `AddOnProfilerMetric` | = 5; Number of ticks where time exceeded 1ms |
| `CountTimeOver5Ms` | `AddOnProfilerMetric` | = 6; Number of ticks where time exceeded 5ms |
| `CountTimeOver10Ms` | `AddOnProfilerMetric` | = 7; Number of ticks where time exceeded 10ms |
| `CountTimeOver50Ms` | `AddOnProfilerMetric` | = 8; Number of ticks where time exceeded 50ms |
| `CountTimeOver100Ms` | `AddOnProfilerMetric` | = 9; Number of ticks where time exceeded 100ms |
| `CountTimeOver500Ms` | `AddOnProfilerMetric` | = 10; Number of ticks where time exceeded 500ms |
| `CountTimeOver1000Ms` | `AddOnProfilerMetric` | = 11; Number of ticks where time exceeded 1000ms |
