# WarCampaign

Namespace `C_CampaignInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/warcampaigndocumentation.lua` (FileDataID 4637301)

## Functions

### GetAvailableCampaigns

```lua
C_CampaignInfo.GetAvailableCampaigns() -> campaignIDs: number[]
```

### GetCampaignChapterInfo

```lua
C_CampaignInfo.GetCampaignChapterInfo(campaignChapterID: number) -> campaignChapterInfo: CampaignChapterInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetCampaignID

```lua
C_CampaignInfo.GetCampaignID(questID: number) -> campaignID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetCampaignInfo

```lua
C_CampaignInfo.GetCampaignInfo(campaignID: number) -> campaignInfo: CampaignInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetChapterIDs

```lua
C_CampaignInfo.GetChapterIDs(campaignID: number) -> chapterIDs: number[]?
```

`SecretArguments=AllowedWhenUntainted`

### GetCurrentChapterID

```lua
C_CampaignInfo.GetCurrentChapterID(campaignID: number) -> currentChapterID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetFailureReason

```lua
C_CampaignInfo.GetFailureReason(campaignID: number) -> failureReason: CampaignFailureReason?
```

`SecretArguments=AllowedWhenUntainted`

### GetState

```lua
C_CampaignInfo.GetState(campaignID: number) -> state: CampaignState
```

`SecretArguments=AllowedWhenUntainted`

### IsCampaignQuest

```lua
C_CampaignInfo.IsCampaignQuest(questID: number) -> isCampaignQuest: bool
```

`SecretArguments=AllowedWhenUntainted`

### SortAsNormalQuest

```lua
C_CampaignInfo.SortAsNormalQuest(campaignID: number) -> sortAsNormalQuest: bool
```

`SecretArguments=AllowedWhenUntainted`

## Types

### CampaignState

*Enumeration* · 4 values, 0..3

Access values as `Enum.CampaignState.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Invalid` | `CampaignState` | = 0 |
| `Complete` | `CampaignState` | = 1 |
| `InProgress` | `CampaignState` | = 2 |
| `Stalled` | `CampaignState` | = 3 |

### CampaignChapterInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `description` | `cstring` |  |
| `rewardQuestID` | `number` |  |

### CampaignFailureReason

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `text` | `string` |  |
| `questID` | `number?` |  |
| `mapID` | `number?` |  |

### CampaignInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `description` | `cstring` |  |
| `uiTextureKit` | `textureKit` |  |
| `isWarCampaign` | `bool` |  |
| `usesNormalQuestIcons` | `bool` |  |
| `isContainerCampaign` | `bool` |  |
| `sortAsNormalQuest` | `bool` |  |
| `hideFutureChapters` | `bool` |  |
