# UnitAuraShared

source `interface/addons/blizzard_apidocumentationgenerated/unitaurashareddocumentation.lua` (FileDataID 7649819)

## Types

### UnitAuraSortDirection

*Enumeration* · 2 values, 0..1

Access values as `Enum.UnitAuraSortDirection.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Normal` | `UnitAuraSortDirection` | = 0 |
| `Reverse` | `UnitAuraSortDirection` | = 1 |

### UnitAuraSortRule

*Enumeration* · 7 values, 0..6

Access values as `Enum.UnitAuraSortRule.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Unsorted` | `UnitAuraSortRule` | = 0; Applies no sorting to auras. |
| `Default` | `UnitAuraSortRule` | = 1; Sorts auras according first by whether or not the aura was applied by the player, else whether or not the player can apply the aura, and finally by aura instance ID. |
| `BigDefensive` | `UnitAuraSortRule` | = 2; Sorts auras according first by whether or not the aura was applied by another player, else by expiration time (longest to shortest), and finally by aura instance ID. |
| `Expiration` | `UnitAuraSortRule` | = 3; Sorts auras according first by whether or not the aura was applied by the player, else whether or not the player can apply the aura, then by expiration time (soonest to longest, followed by permanent auras), and finally by aura instance ID. |
| `ExpirationOnly` | `UnitAuraSortRule` | = 4; Sorts auras according only to expiration time. |
| `Name` | `UnitAuraSortRule` | = 5; Sorts auras according first by whether or not the aura was applied by the player, else whether or not the player can apply the aura, then by spell name, and finally by aura instance ID. |
| `NameOnly` | `UnitAuraSortRule` | = 6; Sorts auras according only their spell name. |

## Predicates

Conditions referenced by the flags above.

- `RequiresValidUnitAuraInstance` *Precondition* (failure mode: ReturnNothing)
