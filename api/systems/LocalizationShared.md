# LocalizationShared

source `interface/addons/blizzard_apidocumentationgenerated/localizationshareddocumentation.lua` (FileDataID 7569777)

## Types

### AbbreviationDataError

*Enumeration* · 4 values, 1..8

Access values as `Enum.AbbreviationDataError.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `InvalidBreakpoint` | `AbbreviationDataError` | = 1 |
| `InvalidSignificandDivisor` | `AbbreviationDataError` | = 2 |
| `InvalidFractionDivisor` | `AbbreviationDataError` | = 4 |
| `NotMultipleOfTen` | `AbbreviationDataError` | = 8 |

### NamePartType

*Enumeration* · 2 values, 0..1

Access values as `Enum.NamePartType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Firstname` | `NamePartType` | = 0 |
| `Surname` | `NamePartType` | = 1 |

### NumberAbbreviationBreakpoint

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `breakpoint` | `number` | Breakpoints should generally be specified as pairs, with one at the named order (1,000) with fractionDivisor = 10, and one a single order higher (eg. 10,000) with fractionDivisor = 1., This ruleset means numbers like '1234' will be abbreviated to '1.2k' and numbers like '12345' to '12k'. |
| `abbreviation` | `string` | Abbreviation name to be looked up as a global string. |
| `significandDivisor` | `number` | significandDivisor and fractionDivisor should multiply such that they become equal to a named order of magnitude, such as thousands or  millions. |
| `fractionDivisor` | `number` |  |
| `abbreviationIsGlobal` | `bool` | default `true`; Defaults to true. Set to false to skip the global string lookup and use the raw abbreviation string when formatting results |

## Predicates

Conditions referenced by the flags above.

- `RequiresRestrictedAbbreviationBreakpoints` *Precondition* (failure mode: Error)
- `RequiresValidAbbreviationBreakpoints` *Precondition* (failure mode: Error)
