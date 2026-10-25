# RestrictedActionsConstants

source `interface/addons/blizzard_apidocumentationgenerated/restrictedactionsconstantsdocumentation.lua` (FileDataID 7644354)

## Types

### AddOnRestrictionState

*Enumeration* · 3 values, 0..2

Access values as `Enum.AddOnRestrictionState.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Inactive` | `AddOnRestrictionState` | = 0; State used when an addon restriction is not being enforced. |
| `Activating` | `AddOnRestrictionState` | = 1; State used during the dispatch of ADDON_RESTRICTION_STATE_CHANGED to infer that a restriction is about to become active, but won't be enforced until event dispatch has completed. |
| `Active` | `AddOnRestrictionState` | = 2; State used when an addon restriction is presently being enforced. |

### AddOnRestrictionType

*Enumeration* · 6 values, 0..5

Access values as `Enum.AddOnRestrictionType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Combat` | `AddOnRestrictionType` | = 0; The player is actively affecting combat. |
| `Encounter` | `AddOnRestrictionType` | = 1; The player is actively participating in an instance encounter. |
| `ChallengeMode` | `AddOnRestrictionType` | = 2; The player is in an active and incomplete challenge mode or mythic keystone dungeon. |
| `PvPMatch` | `AddOnRestrictionType` | = 3; The player is in an active and incomplete PvP match. |
| `Map` | `AddOnRestrictionType` | = 4; The player is on a map that applies addon restrictions. |
| `Chat` | `AddOnRestrictionType` | = 5; The player is in a state where addon chat communications are restricted. |
