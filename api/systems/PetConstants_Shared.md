# PetConstants_Shared

source `interface/addons/blizzard_apidocumentationgenerated/petconstants_shareddocumentation.lua` (FileDataID 7443833)

## Types

### PetActionFeedback

*Enumeration* · 5 values, 0..4

Access values as `Enum.PetActionFeedback.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Success` | `PetActionFeedback` | = 0 |
| `Dead` | `PetActionFeedback` | = 1 |
| `InvalidTarget` | `PetActionFeedback` | = 2 |
| `FriendlyTarget` | `PetActionFeedback` | = 3 |
| `NoPath` | `PetActionFeedback` | = 4 |

### PetMode

*Enumeration* · 4 values, 0..3

Access values as `Enum.PetMode.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Passive` | `PetMode` | = 0 |
| `Defensive` | `PetMode` | = 1 |
| `Aggressive` | `PetMode` | = 2 |
| `Assist` | `PetMode` | = 3 |

### PetOrders

*Enumeration* · 5 values, 0..4

Access values as `Enum.PetOrders.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Wait` | `PetOrders` | = 0 |
| `Follow` | `PetOrders` | = 1 |
| `Attack` | `PetOrders` | = 2 |
| `Dismiss` | `PetOrders` | = 3 |
| `MoveTo` | `PetOrders` | = 4 |

### PetOverride

*Enumeration* · 4 values, 0..4

Access values as `Enum.PetOverride.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `PetOverride` | = 0 |
| `AICombatControl` | `PetOverride` | = 1 |
| `AICombatPassive` | `PetOverride` | = 2 |
| `OwnerMounted` | `PetOverride` | = 4 |

### Pettameresult

*Enumeration* · 16 values, 0..15

Access values as `Enum.Pettameresult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Ok` | `Pettameresult` | = 0 |
| `Invalidcreature` | `Pettameresult` | = 1 |
| `Toomany` | `Pettameresult` | = 2 |
| `Creaturealreadyowned` | `Pettameresult` | = 3 |
| `Nottameable` | `Pettameresult` | = 4 |
| `Anothersummonactive` | `Pettameresult` | = 5 |
| `Unitscanttame` | `Pettameresult` | = 6 |
| `Nopetavailable` | `Pettameresult` | = 7 |
| `Internalerror` | `Pettameresult` | = 8 |
| `Toohighlevel` | `Pettameresult` | = 9 |
| `Dead` | `Pettameresult` | = 10 |
| `Notdead` | `Pettameresult` | = 11 |
| `Cantcontrolexotic` | `Pettameresult` | = 12 |
| `Invalidslot` | `Pettameresult` | = 13 |
| `EliteToohighlevel` | `Pettameresult` | = 14 |
| `Numresults` | `Pettameresult` | = 15 |

### StableResult

*Enumeration* · 17 values, 0..16

Access values as `Enum.StableResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `MaxSlots` | `StableResult` | = 0 |
| `InsufficientFunds` | `StableResult` | = 1 |
| `NotStableMaster` | `StableResult` | = 2 |
| `InvalidSlot` | `StableResult` | = 3 |
| `NoPet` | `StableResult` | = 4 |
| `AlreadyStabled` | `StableResult` | = 5 |
| `AlreadySummoned` | `StableResult` | = 6 |
| `NotFound` | `StableResult` | = 7 |
| `StableSuccess` | `StableResult` | = 8 |
| `UnstableSuccess` | `StableResult` | = 9 |
| `ReviveSuccess` | `StableResult` | = 10 |
| `CantControlExotic` | `StableResult` | = 11 |
| `InternalError` | `StableResult` | = 12 |
| `CheckForLuaHack` | `StableResult` | = 13 |
| `BuySlotSuccess` | `StableResult` | = 14 |
| `FavoriteToggle` | `StableResult` | = 15 |
| `PetRenamed` | `StableResult` | = 16 |

### UnitMirrorPetFlags

*Enumeration* · 5 values, 1..16

Access values as `Enum.UnitMirrorPetFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Renameable` | `UnitMirrorPetFlags` | = 1 |
| `Dismissable` | `UnitMirrorPetFlags` | = 2 |
| `RecentlyTamed` | `UnitMirrorPetFlags` | = 4 |
| `Stampede` | `UnitMirrorPetFlags` | = 8 |
| `ExtraPet` | `UnitMirrorPetFlags` | = 16 |
