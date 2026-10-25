# ReportSystemConstants

source `interface/addons/blizzard_apidocumentationgenerated/reportsystemconstantsdocumentation.lua` (FileDataID 4637189)

## Types

### ReportEvidenceType

*Enumeration* · 3 values, 0..2

Access values as `Enum.ReportEvidenceType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Invalid` | `ReportEvidenceType` | = 0 |
| `HouseScreenshot` | `ReportEvidenceType` | = 1 |
| `HouseLayoutJson` | `ReportEvidenceType` | = 2 |

### ReportMajorCategory

*Enumeration* · 6 values, 0..5

Access values as `Enum.ReportMajorCategory.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `InappropriateCommunication` | `ReportMajorCategory` | = 0 |
| `GameplaySabotage` | `ReportMajorCategory` | = 1 |
| `Cheating` | `ReportMajorCategory` | = 2 |
| `InappropriateName` | `ReportMajorCategory` | = 3 |
| `InappropriateDecor` | `ReportMajorCategory` | = 4 |
| `InappropriateBlueprint` | `ReportMajorCategory` | = 5 |

### ReportMinorCategory

*Enumeration* · 21 values, 1..1048576

Access values as `Enum.ReportMinorCategory.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `TextChat` | `ReportMinorCategory` | = 1 |
| `Boosting` | `ReportMinorCategory` | = 2 |
| `Spam` | `ReportMinorCategory` | = 4 |
| `Afk` | `ReportMinorCategory` | = 8 |
| `IntentionallyFeeding` | `ReportMinorCategory` | = 16 |
| `BlockingProgress` | `ReportMinorCategory` | = 32 |
| `Hacking` | `ReportMinorCategory` | = 64 |
| `Botting` | `ReportMinorCategory` | = 128 |
| `Advertisement` | `ReportMinorCategory` | = 256 |
| `BTag` | `ReportMinorCategory` | = 512 |
| `GroupName` | `ReportMinorCategory` | = 1024 |
| `CharacterName` | `ReportMinorCategory` | = 2048 |
| `GuildName` | `ReportMinorCategory` | = 4096 |
| `Description` | `ReportMinorCategory` | = 8192 |
| `Name` | `ReportMinorCategory` | = 16384 |
| `HarmfulToMinors` | `ReportMinorCategory` | = 32768 |
| `Disruption` | `ReportMinorCategory` | = 65536 |
| `TerroristAndViolentExtremistContent` | `ReportMinorCategory` | = 131072 |
| `ChildSexualExploitationAndAbuse` | `ReportMinorCategory` | = 262144 |
| `NeighborhoodName` | `ReportMinorCategory` | = 524288 |
| `HousingBlueprint` | `ReportMinorCategory` | = 1048576 |

### ReportSubComplaintTypes

*Enumeration* · 2 values, 0..1

Access values as `Enum.ReportSubComplaintTypes.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Inappropriate` | `ReportSubComplaintTypes` | = 0 |
| `Advertising` | `ReportSubComplaintTypes` | = 1 |

### ReportThrottleType

*Enumeration* · 3 values, 0..2

Access values as `Enum.ReportThrottleType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Invalid` | `ReportThrottleType` | = 0 |
| `General` | `ReportThrottleType` | = 1 |
| `Expensive` | `ReportThrottleType` | = 2 |

### ReportType

*Enumeration* · 22 values, 0..21

Access values as `Enum.ReportType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Chat` | `ReportType` | = 0 |
| `InWorld` | `ReportType` | = 1 |
| `ClubFinderPosting` | `ReportType` | = 2 |
| `ClubFinderApplicant` | `ReportType` | = 3 |
| `GroupFinderPosting` | `ReportType` | = 4 |
| `GroupFinderApplicant` | `ReportType` | = 5 |
| `ClubMember` | `ReportType` | = 6 |
| `GroupMember` | `ReportType` | = 7 |
| `Friend` | `ReportType` | = 8 |
| `Pet` | `ReportType` | = 9 |
| `BattlePet` | `ReportType` | = 10 |
| `Calendar` | `ReportType` | = 11 |
| `Mail` | `ReportType` | = 12 |
| `PvP` | `ReportType` | = 13 |
| `PvPScoreboard` | `ReportType` | = 14 |
| `PvPGroupMember` | `ReportType` | = 15 |
| `CraftingOrder` | `ReportType` | = 16 |
| `RecentAlly` | `ReportType` | = 17 |
| `HousingDecor` | `ReportType` | = 18 |
| `Neighborhood` | `ReportType` | = 19 |
| `NeighborhoodRoster` | `ReportType` | = 20 |
| `HousingBlueprint` | `ReportType` | = 21 |

### ScreenshotSource

*Enumeration* · 3 values, 0..2

Access values as `Enum.ScreenshotSource.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Automatic` | `ScreenshotSource` | = 0 |
| `PlayerReport` | `ScreenshotSource` | = 1 |
| `Cheat` | `ScreenshotSource` | = 2 |

### SendReportResult

*Enumeration* · 6 values, 0..5

Access values as `Enum.SendReportResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Success` | `SendReportResult` | = 0 |
| `GeneralError` | `SendReportResult` | = 1 |
| `TooManyReports` | `SendReportResult` | = 2 |
| `RequiresChatLine` | `SendReportResult` | = 3 |
| `RequiresChatLineOrVoice` | `SendReportResult` | = 4 |
| `RequiresScreenshot` | `SendReportResult` | = 5 |
