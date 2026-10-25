# UnitConstants

source `interface/addons/blizzard_apidocumentationgenerated/unitconstantsdocumentation.lua` (FileDataID 4637287)

## Types

### AddPrivateAuraAnchorArgs

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `unitToken` | `cstring` |  |
| `auraIndex` | `number` |  |
| `parent` | `SimpleFrame` |  |
| `showCooldownFrame` | `bool` | default `false` |
| `showCooldownEdge` | `bool` | default `false` |
| `showCountdownNumbers` | `bool` | default `false` |
| `showDispelIcon` | `bool` | default `false` |
| `isContainer` | `bool` | default `false` |
| `iconInfo` | `PrivateAuraIconInfo?` |  |
| `durationAnchor` | `AnchorBinding?` |  |

### GroupBuffVisualAlertInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `number` |  |
| `visualValue` | `VisualAlertType` |  |

### PrivateAuraIconInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `iconAnchor` | `AnchorBinding` |  |
| `iconWidth` | `uiUnit` |  |
| `iconHeight` | `uiUnit` |  |
| `borderScale` | `uiUnit?` |  |

### UnitAuraSoundInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `unitToken` | `string` |  |
| `spellID` | `number` |  |
| `soundFileName` | `string?` | Sound file to play. Playback stops after five seconds. |
| `soundFileID` | `number?` | Sound file to play. Playback stops after five seconds. |
| `outputChannel` | `string?` |  |
| `throttleSeconds` | `number?` | Minimum time in seconds between plays. Must be between 0 and 5 seconds, inclusive. Invalid values reject registration. |

### UnitAuraUpdateInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `isFullUpdate` | `bool` | default `false` |
| `removedAuraInstanceIDs` | `number[]?` |  |
| `addedAuras` | `AuraData[]?` |  |
| `updatedAuraInstanceIDs` | `number[]?` |  |

### UnitPrivateAuraAnchorInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `anchorID` | `number` |  |
| `unitToken` | `string` |  |
| `auraIndex` | `number` |  |
| `showCooldownFrame` | `bool` | default `false` |
| `showCooldownEdge` | `bool` | default `false` |
| `showCountdownNumbers` | `bool` | default `false` |
| `showDispelIcon` | `bool` | default `false` |
| `iconWidth` | `uiUnit?` |  |
| `iconHeight` | `uiUnit?` |  |
| `borderScale` | `uiUnit?` |  |
| `isContainer` | `bool?` |  |
| `parent` | `SimpleFrame` |  |
