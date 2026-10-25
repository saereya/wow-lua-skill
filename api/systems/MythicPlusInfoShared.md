# MythicPlusInfoShared

source `interface/addons/blizzard_apidocumentationgenerated/mythicplusinfoshareddocumentation.lua` (FileDataID 4637159)

## Types

### MythicPlusAffixScoreInfo

*Structure*

Information about a specific M+ run

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `score` | `number` |  |
| `level` | `number` |  |
| `durationSec` | `number` |  |
| `overTime` | `bool` |  |

### MythicPlusLeaderboardPlayerResult

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `playerGUID` | `WOWGUID` |  |
| `specID` | `number` |  |

### MythicPlusLeaderboardResult

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `completionTime` | `number` |  |
| `players` | `MythicPlusLeaderboardPlayerResult[]` |  |

### MythicPlusRatingLinkInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `mapChallengeModeID` | `number` |  |
| `level` | `number` |  |
| `completedInTime` | `number` |  |
| `dungeonScore` | `number` |  |
| `name` | `string` |  |
