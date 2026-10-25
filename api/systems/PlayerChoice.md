# PlayerChoice

Namespace `C_PlayerChoice` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/playerchoicedocumentation.lua` (FileDataID 4637166)

## Functions

### GetCurrentPlayerChoiceInfo

```lua
C_PlayerChoice.GetCurrentPlayerChoiceInfo() -> choiceInfo: PlayerChoiceInfo
```

`MayReturnNothing`

### GetNumRerolls

```lua
C_PlayerChoice.GetNumRerolls() -> numRerolls: number
```

### GetRemainingTime

```lua
C_PlayerChoice.GetRemainingTime() -> remainingTime: number?
```

### IsWaitingForPlayerChoiceResponse

```lua
C_PlayerChoice.IsWaitingForPlayerChoiceResponse() -> isWaitingForResponse: bool
```

### OnUIClosed

```lua
C_PlayerChoice.OnUIClosed()
```

### RequestRerollPlayerChoice

```lua
C_PlayerChoice.RequestRerollPlayerChoice()
```

### SendPlayerChoiceResponse

```lua
C_PlayerChoice.SendPlayerChoiceResponse(responseID: number)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### PLAYER_CHOICE_CLOSE

```lua
PLAYER_CHOICE_CLOSE()
```

`SynchronousEvent`

### PLAYER_CHOICE_UPDATE

```lua
PLAYER_CHOICE_UPDATE()
```

`UniqueEvent`

## Types

### PlayerChoiceRarity

*Enumeration* · 4 values, 0..3

Access values as `Enum.PlayerChoiceRarity.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Common` | `PlayerChoiceRarity` | = 0 |
| `Uncommon` | `PlayerChoiceRarity` | = 1 |
| `Rare` | `PlayerChoiceRarity` | = 2 |
| `Epic` | `PlayerChoiceRarity` | = 3 |

### PlayerChoiceInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `objectGUID` | `WOWGUID` |  |
| `choiceID` | `number` |  |
| `questionText` | `string` |  |
| `pendingChoiceText` | `string` |  |
| `uiTextureKit` | `textureKit` |  |
| `hideWarboardHeader` | `bool` |  |
| `keepOpenAfterChoice` | `bool` |  |
| `requiresSelection` | `bool` |  |
| `hideAnswerArt` | `bool` |  |
| `playerChoiceLayout` | `PlayerChoiceLayout` |  |
| `options` | `PlayerChoiceOptionInfo[]` |  |
| `soundKitID` | `number?` |  |
| `closeUISoundKitID` | `number?` |  |

### PlayerChoiceOptionButtonInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `id` | `number` |  |
| `text` | `string` |  |
| `disabled` | `bool` |  |
| `showCheckmark` | `bool` |  |
| `hideButtonShowText` | `bool` |  |
| `selected` | `bool` |  |
| `confirmation` | `string?` |  |
| `tooltip` | `string?` |  |
| `rewardQuestID` | `number?` |  |
| `soundKitID` | `number?` |  |
| `listText` | `string?` |  |

### PlayerChoiceOptionInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `id` | `number` |  |
| `description` | `string` |  |
| `header` | `string` |  |
| `choiceArtID` | `number` |  |
| `desaturatedArt` | `bool` |  |
| `disabledOption` | `bool` |  |
| `hasRewards` | `bool` |  |
| `rewardInfo` | `PlayerChoiceOptionRewardInfo` |  |
| `uiTextureKit` | `textureKit` |  |
| `maxStacks` | `number` |  |
| `buttons` | `PlayerChoiceOptionButtonInfo[]` |  |
| `widgetSetID` | `number?` |  |
| `spellID` | `number?` |  |
| `rarity` | `PlayerChoiceRarity?` |  |
| `typeArtID` | `number?` |  |
| `headerIconAtlasElement` | `string?` |  |
| `subHeader` | `string?` |  |
| `consolidateWidgets` | `bool` |  |

### PlayerChoiceOptionRewardInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `currencyRewards` | `PlayerChoiceRewardCurrencyInfo[]` |  |
| `itemRewards` | `PlayerChoiceRewardItemInfo[]` |  |
| `repRewards` | `PlayerChoiceRewardReputationInfo[]` |  |

### PlayerChoiceRewardCurrencyInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `currencyId` | `number` |  |
| `name` | `string` |  |
| `currencyTexture` | `number` |  |
| `quantity` | `number` |  |
| `isCurrencyContainer` | `bool` |  |

### PlayerChoiceRewardItemInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `itemId` | `number` |  |
| `name` | `string` |  |
| `quantity` | `number` |  |

### PlayerChoiceRewardReputationInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `factionId` | `number` |  |
| `quantity` | `number` |  |
