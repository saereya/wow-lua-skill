# AutoCompleteShared

source `interface/addons/blizzard_apidocumentationgenerated/autocompleteshareddocumentation.lua` (FileDataID 7733452)

## Types

### AutoCompleteEntryFlag

*Enumeration* · 9 values, 1..256

Access values as `Enum.AutoCompleteEntryFlag.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `InGroup` | `AutoCompleteEntryFlag` | = 1 |
| `InGuild` | `AutoCompleteEntryFlag` | = 2 |
| `Friend` | `AutoCompleteEntryFlag` | = 4 |
| `Bnet` | `AutoCompleteEntryFlag` | = 8 |
| `InteractedWith` | `AutoCompleteEntryFlag` | = 16 |
| `Online` | `AutoCompleteEntryFlag` | = 32 |
| `InAOI` | `AutoCompleteEntryFlag` | = 64 |
| `AccountCharacter` | `AutoCompleteEntryFlag` | = 128 |
| `RecentPlayer` | `AutoCompleteEntryFlag` | = 256 |

### AutoCompletePriority

*Enumeration* · 7 values, 0..6

Access values as `Enum.AutoCompletePriority.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Other` | `AutoCompletePriority` | = 0 |
| `Interacted` | `AutoCompletePriority` | = 1 |
| `InGroup` | `AutoCompletePriority` | = 2 |
| `Guild` | `AutoCompletePriority` | = 3 |
| `Friend` | `AutoCompletePriority` | = 4 |
| `AccountCharacter` | `AutoCompletePriority` | = 5 |
| `AccountCharacterSameRealm` | `AutoCompletePriority` | = 6 |
