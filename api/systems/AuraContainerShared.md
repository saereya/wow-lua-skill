# AuraContainerShared

source `interface/addons/blizzard_apidocumentationgenerated/auracontainershareddocumentation.lua` (FileDataID 8245098)

## Types

### CustomAuraButtonDispelTypeStealableFilter

*Enumeration* · 2 values, 0..1

Access values as `Enum.CustomAuraButtonDispelTypeStealableFilter.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Stealable` | `CustomAuraButtonDispelTypeStealableFilter` | = 0; Shows the dispel type only for stealable auras. |
| `NotStealable` | `CustomAuraButtonDispelTypeStealableFilter` | = 1; Shows the dispel type only for non-stealable auras. |

### CustomAuraButtonDispelTypeTextureStyle

*Enumeration* · 5 values, 0..4

Access values as `Enum.CustomAuraButtonDispelTypeTextureStyle.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Border` | `CustomAuraButtonDispelTypeTextureStyle` | = 0; Uses a built-in border based on the aura's dispel type. |
| `BorderWithIcon` | `CustomAuraButtonDispelTypeTextureStyle` | = 1; Uses a built-in border with a corner icon based on the aura's dispel type. |
| `Icon` | `CustomAuraButtonDispelTypeTextureStyle` | = 2; Uses a built-in icon based on the aura's dispel type. |
| `PreserveAsset` | `CustomAuraButtonDispelTypeTextureStyle` | = 3; Preserves the texture's existing asset. |
| `CustomAsset` | `CustomAuraButtonDispelTypeTextureStyle` | = 4; Uses a custom texture asset selected from the configured dispel type asset map. |

### CustomAuraButtonUpdateMode

*Enumeration* · 2 values, 0..1

Access values as `Enum.CustomAuraButtonUpdateMode.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Assignment` | `CustomAuraButtonUpdateMode` | = 0; Applies a newly assigned aura, resetting presentation state rather than transitioning from the previous aura. |
| `Update` | `CustomAuraButtonUpdateMode` | = 1; Refreshes the current aura assignment, allowing presentation state to retain continuity. |
