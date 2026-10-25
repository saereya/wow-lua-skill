# ClickBindingsConstants

source `interface/addons/blizzard_apidocumentationgenerated/clickbindingsconstantsdocumentation.lua` (FileDataID 4637048)

## Types

### ClickBindingInteraction

*Enumeration* · 2 values, 1..2

Access values as `Enum.ClickBindingInteraction.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Target` | `ClickBindingInteraction` | = 1 |
| `OpenContextMenu` | `ClickBindingInteraction` | = 2 |

### ClickBindingType

*Enumeration* · 5 values, 0..4

Access values as `Enum.ClickBindingType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `ClickBindingType` | = 0 |
| `Spell` | `ClickBindingType` | = 1 |
| `Macro` | `ClickBindingType` | = 2 |
| `Interaction` | `ClickBindingType` | = 3 |
| `PetAction` | `ClickBindingType` | = 4 |

### ClickBindingInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `type` | `ClickBindingType` |  |
| `actionID` | `number` | Base spellID for spell, macro index for macro, ClickBindingInteraction for interaction, spellID for PetAction |
| `button` | `cstring` |  |
| `modifiers` | `number` |  |
