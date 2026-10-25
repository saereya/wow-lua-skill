# LoreText

Namespace `C_LoreText` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/loretextdocumentation.lua` (FileDataID 4637131)

## Functions

### RequestLoreTextForCampaignID

```lua
C_LoreText.RequestLoreTextForCampaignID(campaignID: number)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### LORE_TEXT_UPDATED_CAMPAIGN

```lua
LORE_TEXT_UPDATED_CAMPAIGN(campaignID: number, textEntries: LoreTextEntry[])
```

`SynchronousEvent`

## Types

### LoreTextEntry

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `text` | `string` |  |
| `isHeader` | `bool` |  |
