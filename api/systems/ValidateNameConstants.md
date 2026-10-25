# ValidateNameConstants

source `interface/addons/blizzard_apidocumentationgenerated/validatenameconstantsdocumentation.lua` (FileDataID 4675169)

## Types

### ScrubStringFlags

*Enumeration* · 4 values, 0..4

Access values as `Enum.ScrubStringFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `ScrubStringFlags` | = 0 |
| `TruncateNewLines` | `ScrubStringFlags` | = 1 |
| `AllowBarCodes` | `ScrubStringFlags` | = 2 |
| `StripControlCodes` | `ScrubStringFlags` | = 4 |

### ValidateNameResult

*Enumeration* · 18 values, 0..17

Access values as `Enum.ValidateNameResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Success` | `ValidateNameResult` | = 0 |
| `Failure` | `ValidateNameResult` | = 1 |
| `NoName` | `ValidateNameResult` | = 2 |
| `TooShort` | `ValidateNameResult` | = 3 |
| `TooLong` | `ValidateNameResult` | = 4 |
| `InvalidCharacter` | `ValidateNameResult` | = 5 |
| `MixedLanguages` | `ValidateNameResult` | = 6 |
| `Profane` | `ValidateNameResult` | = 7 |
| `Reserved` | `ValidateNameResult` | = 8 |
| `InvalidApostrophe` | `ValidateNameResult` | = 9 |
| `MultipleApostrophes` | `ValidateNameResult` | = 10 |
| `ThreeConsecutive` | `ValidateNameResult` | = 11 |
| `InvalidSpace` | `ValidateNameResult` | = 12 |
| `ConsecutiveSpaces` | `ValidateNameResult` | = 13 |
| `RussianConsecutiveSilentCharacters` | `ValidateNameResult` | = 14 |
| `RussianSilentCharacterAtBeginningOrEnd` | `ValidateNameResult` | = 15 |
| `DeclensionDoesntMatchBaseName` | `ValidateNameResult` | = 16 |
| `SpacesDisallowed` | `ValidateNameResult` | = 17 |
