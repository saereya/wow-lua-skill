# IntlSharedTypes

source `interface/addons/blizzard_apidocumentationgenerated/intlsharedtypesdocumentation.lua` (FileDataID 8281694)

## Types

### BreakType

*Enumeration* · 4 values, 0..3

Access values as `Enum.BreakType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Character` | `BreakType` | = 0; Locate extended grapheme cluster boundaries, which are treated as user-perceived character units. |
| `Word` | `BreakType` | = 1; Locate word boundaries for selection, search, and whole-word operations, including locale dictionary support where available. |
| `Sentence` | `BreakType` | = 2; Locate sentence boundaries while handling cases such as periods in numbers or abbreviations and trailing punctuation. |
| `Line` | `BreakType` | = 3; Locate positions where text can wrap, using Unicode line-breaking rules that handle punctuation and hyphenated words. |

### CollationStrength

*Enumeration* · 5 values, 0..4

Access values as `Enum.CollationStrength.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Primary` | `CollationStrength` | = 0; Compare base-character differences and ignore accents, case, and later collation levels. |
| `Secondary` | `CollationStrength` | = 1; Compare accent or diacritic differences after base characters match, while ignoring tertiary differences such as case. |
| `Tertiary` | `CollationStrength` | = 2; Compare case, letter variants, and similar tertiary differences after primary and secondary differences match. |
| `Quaternary` | `CollationStrength` | = 3; Distinguish punctuation, whitespace, symbols, or Japanese Hiragana/Katakana differences after the first three levels match. |
| `Identical` | `CollationStrength` | = 4; Use NFD Unicode code point order as a final tie-breaker after all other collation levels match. |

### CurrencyNameStyle

*Enumeration* · 5 values, 0..4

Access values as `Enum.CurrencyNameStyle.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Symbol` | `CurrencyNameStyle` | = 0; A symbolic name for a currency, such as '$' for USD. |
| `NarrowSymbol` | `CurrencyNameStyle` | = 1; The shortest narrow currency symbol, such as '$' instead of 'US$' for USD in en-CA. |
| `Long` | `CurrencyNameStyle` | = 2; The long name for a currency, such as 'US Dollar' for USD. |
| `FormalSymbol` | `CurrencyNameStyle` | = 3; The formal currency symbol is similar to the regular currency symbol, but it always takes the form used in formal settings such as banking; for example, 'NT$' instead of '$' for TWD in zh-TW. |
| `VariantSymbol` | `CurrencyNameStyle` | = 4; The variant symbol for a currency is an alternative symbol that is not necessarily as widely used as the regular symbol. |

### DateTimeStyle

*Enumeration* · 5 values, 0..4

Access values as `Enum.DateTimeStyle.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `DateTimeStyle` | = 0; Do not include this date or time portion in the formatter. |
| `Short` | `DateTimeStyle` | = 1; Use the shortest locale format, generally numeric, such as 12/13/52 or 3:30pm. |
| `Medium` | `DateTimeStyle` | = 2; Use a longer locale format than Short, such as abbreviated month names for dates. |
| `Long` | `DateTimeStyle` | = 3; Use a longer locale format with fuller names or time fields than Medium. |
| `Full` | `DateTimeStyle` | = 4; Use the most completely specified locale format, such as weekday, era, or time zone when applicable. |

### LocaleTransform

*Enumeration* · 8 values, 0..7

Access values as `Enum.LocaleTransform.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Canonicalize` | `LocaleTransform` | = 0; Canonicalizes the locale identifier into ICU's canonical locale ID form. |
| `AddLikelySubtags` | `LocaleTransform` | = 1; Adds likely script and region subtags according to CLDR likely-subtags data. |
| `RemoveLikelySubtags` | `LocaleTransform` | = 2; Minimizes script and region subtags according to CLDR likely-subtags data. |
| `Language` | `LocaleTransform` | = 3; Gets the language code from the locale identifier. |
| `Script` | `LocaleTransform` | = 4; Gets the script code from the locale identifier. |
| `Region` | `LocaleTransform` | = 5; Gets the region code from the locale identifier. |
| `Variant` | `LocaleTransform` | = 6; Gets the variant code from the locale identifier. |
| `ParentLocale` | `LocaleTransform` | = 7; Gets the parent locale identifier. |

### NormalizationForm

*Enumeration* · 4 values, 0..3

Access values as `Enum.NormalizationForm.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Nfc` | `NormalizationForm` | = 0; Canonical decomposition followed by canonical composition. |
| `Nfd` | `NormalizationForm` | = 1; Canonical decomposition. |
| `Nfkc` | `NormalizationForm` | = 2; Compatibility decomposition followed by canonical composition. |
| `Nfkd` | `NormalizationForm` | = 3; Compatibility decomposition. |

### NumberStyle

*Enumeration* · 4 values, 0..3

Access values as `Enum.NumberStyle.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Decimal` | `NumberStyle` | = 0; Use normal decimal number format for the locale. |
| `Integer` | `NumberStyle` | = 1; Use decimal formatting with zero minimum and maximum fraction digits in this wrapper. |
| `Percent` | `NumberStyle` | = 2; Use percent number format for the locale. |
| `Currency` | `NumberStyle` | = 3; Use generic currency format with a currency symbol and non-accounting minus-sign negatives. |

### PluralType

*Enumeration* · 2 values, 0..1

Access values as `Enum.PluralType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Cardinal` | `PluralType` | = 0; Use plural rules for counted quantities, such as 1 file vs. 2 files. |
| `Ordinal` | `PluralType` | = 1; Use plural rules for ordered values, such as 1st, 2nd, 3rd, and 4th. |

### CharacterProperties

*Structure*

Unicode property values for the first code point in a string.

Fields:

| Name | Type | Notes |
|---|---|---|
| `codePoint` | `number` | The Unicode code point tested for character properties. |
| `isAlphabetic` | `bool` | True if the code point is a letter character with general category L. |
| `isDigit` | `bool` | True if the code point is a digit character with general category Nd. |
| `isWhitespace` | `bool` | True if the code point has the Unicode White_Space property. |
| `generalCategory` | `string` | The short Unicode property value name for the code point's general category. |
| `scriptCode` | `string` | The short ISO 15924 script code for the code point's script. |
| `blockCode` | `string` | The short Unicode property value name for the code point's block. |

### CurrencyParseResult

*Structure*

A parsed numeric amount and currency from a localized currency string.

Fields:

| Name | Type | Notes |
|---|---|---|
| `amount` | `number` | The numeric amount parsed by the currency parser. |
| `currencyCode` | `string` | The ISO 4217 currency code parsed alongside the amount. |
