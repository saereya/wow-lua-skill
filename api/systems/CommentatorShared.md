# CommentatorShared

source `interface/addons/blizzard_apidocumentationgenerated/commentatorshareddocumentation.lua` (FileDataID 5233589)

## Types

### TrackedSpellCategory

*Enumeration* · 5 values, 0..4

Access values as `Enum.TrackedSpellCategory.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `TrackedSpellCategory` | = 0 |
| `Offensive` | `TrackedSpellCategory` | = 1 |
| `Defensive` | `TrackedSpellCategory` | = 2 |
| `Debuff` | `TrackedSpellCategory` | = 3 |
| `RacialAbility` | `TrackedSpellCategory` | = 4 |

## Predicates

Conditions referenced by the flags above.

- `RequiresActiveCommentator` *Precondition* (failure mode: ReturnNothing)
- `RequiresCommentator` *Precondition* (failure mode: ReturnNothing)
