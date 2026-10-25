# Expansion

Global functions · environment All · source `interface/addons/blizzard_apidocumentationgenerated/expansiondocumentation.lua` (FileDataID 4637088)

## Functions

### CanUpgradeToCurrentExpansion

```lua
CanUpgradeToCurrentExpansion() -> canUpgradeExpansion: bool
```

### DoesCurrentLocaleSellExpansionLevels

```lua
DoesCurrentLocaleSellExpansionLevels() -> regionSellsExpansions: bool
```

### GetAccountExpansionLevel

```lua
GetAccountExpansionLevel() -> expansionLevel: number
```

### GetClientDisplayExpansionLevel

```lua
GetClientDisplayExpansionLevel() -> expansionLevel: number
```

### GetCreditsDisplayInfo

```lua
GetCreditsDisplayInfo() -> info: CreditsDisplayInfo[]
```

### GetCurrentRegionName

```lua
GetCurrentRegionName() -> regionName: cstring
```

### GetExpansionDisplayInfo

```lua
GetExpansionDisplayInfo(expansionLevel: number, desiredReleaseType: ReleaseType?) -> info: ExpansionDisplayInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetExpansionForLevel

```lua
GetExpansionForLevel(playerLevel: number) -> expansionLevel: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetExpansionLevel

```lua
GetExpansionLevel() -> expansionLevel: number
```

### GetExpansionTrialInfo

```lua
GetExpansionTrialInfo() -> isExpansionTrialAccount: bool, expansionTrialRemainingSeconds: time_t?
```

### GetMaximumExpansionLevel

```lua
GetMaximumExpansionLevel() -> expansionLevel: number
```

### GetMaxLevelForExpansionLevel

```lua
GetMaxLevelForExpansionLevel(expansionLevel: number) -> maxLevel: number
```

Maps an expansion level to a maximum character level for that expansion.

`SecretArguments=AllowedWhenUntainted`

### GetMaxLevelForLatestExpansion

```lua
GetMaxLevelForLatestExpansion() -> maxLevel: number
```

### GetMaxLevelForPlayerExpansion

```lua
GetMaxLevelForPlayerExpansion() -> maxLevel: number
```

### GetMinimumExpansionLevel

```lua
GetMinimumExpansionLevel() -> expansionLevel: number
```

### GetNumExpansions

```lua
GetNumExpansions() -> numExpansions: number
```

### GetServerExpansionLevel

```lua
GetServerExpansionLevel() -> serverExpansionLevel: number
```

### GetUpgradeExpansionLevel

```lua
GetUpgradeExpansionLevel() -> upgradeExpansionLevel: number
```

### IsDemonHunterAvailable

```lua
IsDemonHunterAvailable() -> available: bool
```

### IsExpansionTrial

```lua
IsExpansionTrial() -> isExpansionTrialAccount: bool
```

### IsTrialAccount

```lua
IsTrialAccount() -> isTrialAccount: bool
```

### IsVeteranTrialAccount

```lua
IsVeteranTrialAccount() -> isVeteranTrialAccount: bool
```

### SendSubscriptionInterstitialResponse

```lua
SendSubscriptionInterstitialResponse(response: SubscriptionInterstitialResponseType)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### ShouldShowExpansionUpgradeBanner

```lua
ShouldShowExpansionUpgradeBanner() -> showUpgradeBanner: bool
```

## Events

### MAX_EXPANSION_LEVEL_UPDATED

```lua
MAX_EXPANSION_LEVEL_UPDATED()
```

`SynchronousEvent`

### MIN_EXPANSION_LEVEL_UPDATED

```lua
MIN_EXPANSION_LEVEL_UPDATED()
```

`SynchronousEvent`

### SHOW_SUBSCRIPTION_INTERSTITIAL

```lua
SHOW_SUBSCRIPTION_INTERSTITIAL(type: SubscriptionInterstitialType)
```

`SynchronousEvent`

## Types

### SubscriptionInterstitialResponseType

*Enumeration* · 3 values, 0..2

Access values as `Enum.SubscriptionInterstitialResponseType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Clicked` | `SubscriptionInterstitialResponseType` | = 0 |
| `Closed` | `SubscriptionInterstitialResponseType` | = 1 |
| `WebRedirect` | `SubscriptionInterstitialResponseType` | = 2 |

### SubscriptionInterstitialType

*Enumeration* · 3 values, 0..2

Access values as `Enum.SubscriptionInterstitialType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Standard` | `SubscriptionInterstitialType` | = 0 |
| `LeftNpeArea` | `SubscriptionInterstitialType` | = 1 |
| `MaxLevel` | `SubscriptionInterstitialType` | = 2 |

### CreditsDisplayInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `isDefault` | `bool` |  |
| `creditsFileID` | `number` |  |
| `keyArt` | `string` |  |
| `background` | `string` |  |
| `name` | `string` |  |
| `logo` | `fileID` |  |
| `soundKit` | `number?` |  |

### ExpansionDisplayInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `logo` | `fileID` |  |
| `banner` | `textureAtlas` |  |
| `features` | `ExpansionDisplayInfoFeature[]` |  |
| `highResBackgroundID` | `fileID` |  |
| `lowResBackgroundID` | `fileID` |  |
| `textureKit` | `textureKit` |  |
| `glueAmbianceSoundKit` | `number?` |  |
| `glueMusicSoundKit` | `number?` |  |
| `glueCreditsSoundKit` | `number?` |  |

### ExpansionDisplayInfoFeature

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `icon` | `fileID` |  |
| `text` | `cstring` |  |
