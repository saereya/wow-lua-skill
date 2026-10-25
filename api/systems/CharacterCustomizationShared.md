# CharacterCustomizationShared

source `interface/addons/blizzard_apidocumentationgenerated/charactercustomizationshareddocumentation.lua` (FileDataID 4637049)

## Types

### CharCustomizationType

*Enumeration* · 9 values, 0..8

Access values as `Enum.CharCustomizationType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Skin` | `CharCustomizationType` | = 0 |
| `Face` | `CharCustomizationType` | = 1 |
| `Hair` | `CharCustomizationType` | = 2 |
| `HairColor` | `CharCustomizationType` | = 3 |
| `FacialHair` | `CharCustomizationType` | = 4 |
| `CustomOptionTattoo` | `CharCustomizationType` | = 5 |
| `CustomOptionHorn` | `CharCustomizationType` | = 6 |
| `CustomOptionFacewear` | `CharCustomizationType` | = 7 |
| `CustomOptionTattooColor` | `CharCustomizationType` | = 8 |

### ChrCustomizationCategoryFlag

*Enumeration* · 2 values, 1..2

Access values as `Enum.ChrCustomizationCategoryFlag.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `UndressModel` | `ChrCustomizationCategoryFlag` | = 1 |
| `Subcategory` | `ChrCustomizationCategoryFlag` | = 2 |

### ChrCustomizationOptionType

*Enumeration* · 3 values, 0..2

Access values as `Enum.ChrCustomizationOptionType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Dropdown` | `ChrCustomizationOptionType` | = 0 |
| `Checkbox` | `ChrCustomizationOptionType` | = 1 |
| `Slider` | `ChrCustomizationOptionType` | = 2 |

### ChrModelFeatureFlags

*Enumeration* · 8 values, 0..64

Access values as `Enum.ChrModelFeatureFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `ChrModelFeatureFlags` | = 0 |
| `Summons` | `ChrModelFeatureFlags` | = 1 |
| `Forms` | `ChrModelFeatureFlags` | = 2 |
| `Identity` | `ChrModelFeatureFlags` | = 4 |
| `Deprecated0` | `ChrModelFeatureFlags` | = 8 |
| `Mounts` | `ChrModelFeatureFlags` | = 16 |
| `HunterPets` | `ChrModelFeatureFlags` | = 32 |
| `Players` | `ChrModelFeatureFlags` | = 64 |

### NewCharGear

*Enumeration* · 2 values, 0..1

Access values as `Enum.NewCharGear.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Start` | `NewCharGear` | = 0 |
| `Preview` | `NewCharGear` | = 1 |

### CharCustomizationCategory

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `id` | `number` |  |
| `orderIndex` | `number` |  |
| `name` | `cstring` |  |
| `icon` | `textureAtlas` |  |
| `selectedIcon` | `textureAtlas` |  |
| `undressModel` | `bool` |  |
| `subcategory` | `bool` |  |
| `cameraZoomLevel` | `number` |  |
| `cameraDistanceOffset` | `number` |  |
| `spellShapeshiftFormID` | `number?` |  |
| `chrModelID` | `number?` |  |
| `options` | `CharCustomizationOption[]` |  |
| `hasNewChoices` | `bool` |  |
| `needsNativeFormCategory` | `bool` |  |

### CharCustomizationChoice

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `id` | `number` |  |
| `name` | `cstring` |  |
| `ineligibleChoice` | `bool` |  |
| `isNew` | `bool` |  |
| `swatchColor1` | `colorRGB?` | `Mixin=ColorMixin` |
| `swatchColor2` | `colorRGB?` | `Mixin=ColorMixin` |
| `soundKit` | `number?` |  |
| `isLocked` | `bool` |  |
| `lockedText` | `string?` |  |

### CharCustomizationConstants

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `CHAR_CUSTOMIZE_CUSTOM_DISPLAY_OPTION_FIRST` | `CharCustomizationType` | = `"CustomOptionTattoo"` |
| `CHAR_CUSTOMIZE_CUSTOM_DISPLAY_OPTION_LAST` | `CharCustomizationType` | = `"CustomOptionTattooColor"` |
| `NUM_CUSTOM_DISPLAY` | `number` | = `Constants.CharCustomizationConstants.CHAR_CUSTOMIZE_CUSTOM_DISPLAY_OPTION_LAST - Constants.CharCustomizationConstants.CHAR_CUSTOMIZE_CUSTOM_DISPLAY_OPTION_FIRST + 1` |
| `NAME_RESERVATION_DAYS` | `number` | = `30` |

### CharCustomizationOption

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `id` | `number` |  |
| `name` | `cstring` |  |
| `orderIndex` | `number` |  |
| `optionType` | `ChrCustomizationOptionType` |  |
| `choices` | `CharCustomizationChoice[]` |  |
| `currentChoiceIndex` | `luaIndex?` |  |
| `hasNewChoices` | `bool` |  |
| `isSound` | `bool` |  |
