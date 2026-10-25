# CharacterSelectionConstants

source `interface/addons/blizzard_apidocumentationgenerated/characterselectionconstantsdocumentation.lua` (FileDataID 5736129)

## Types

### WarbandEventState

*Enumeration* · 8 values, 0..7

Access values as `Enum.WarbandEventState.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `WarbandEventState` | = 0 |
| `DelayingEvent` | `WarbandEventState` | = 1 |
| `SheathingWeapon` | `WarbandEventState` | = 2 |
| `DelayingStandStateTransition` | `WarbandEventState` | = 3 |
| `StandStateTransitioning` | `WarbandEventState` | = 4 |
| `ShowingWeapon` | `WarbandEventState` | = 5 |
| `StandStateLooping` | `WarbandEventState` | = 6 |
| `NumWarbandEventStates` | `WarbandEventState` | = 7 |

### WarbandGroupFlags

*Enumeration* · 2 values, 0..1

Access values as `Enum.WarbandGroupFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `WarbandGroupFlags` | = 0 |
| `Collapsed` | `WarbandGroupFlags` | = 1 |

### WarbandPlacementDisplayInfoType

*Enumeration* · 3 values, 0..2

Access values as `Enum.WarbandPlacementDisplayInfoType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Model` | `WarbandPlacementDisplayInfoType` | = 0 |
| `Creature` | `WarbandPlacementDisplayInfoType` | = 1 |
| `Item` | `WarbandPlacementDisplayInfoType` | = 2 |

### WarbandSceneAnimationEvent

*Enumeration* · 10 values, 0..9

Access values as `Enum.WarbandSceneAnimationEvent.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `StartingPose` | `WarbandSceneAnimationEvent` | = 0 |
| `Idle` | `WarbandSceneAnimationEvent` | = 1 |
| `Mouseover` | `WarbandSceneAnimationEvent` | = 2 |
| `Select` | `WarbandSceneAnimationEvent` | = 3 |
| `Deselect` | `WarbandSceneAnimationEvent` | = 4 |
| `Insert` | `WarbandSceneAnimationEvent` | = 5 |
| `EnterWorld` | `WarbandSceneAnimationEvent` | = 6 |
| `Spin` | `WarbandSceneAnimationEvent` | = 7 |
| `Poke` | `WarbandSceneAnimationEvent` | = 8 |
| `Ffx` | `WarbandSceneAnimationEvent` | = 9 |

### WarbandSceneAnimationSheatheState

*Enumeration* · 3 values, 0..2

Access values as `Enum.WarbandSceneAnimationSheatheState.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Maintain` | `WarbandSceneAnimationSheatheState` | = 0 |
| `SheatheWeapons` | `WarbandSceneAnimationSheatheState` | = 1 |
| `ShowWeapons` | `WarbandSceneAnimationSheatheState` | = 2 |

### WarbandSceneAnimationStandState

*Enumeration* · 9 values, 0..8

Access values as `Enum.WarbandSceneAnimationStandState.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Maintain` | `WarbandSceneAnimationStandState` | = 0 |
| `Stand` | `WarbandSceneAnimationStandState` | = 1 |
| `SitOnGround` | `WarbandSceneAnimationStandState` | = 2 |
| `Kneel` | `WarbandSceneAnimationStandState` | = 3 |
| `ReadyStance` | `WarbandSceneAnimationStandState` | = 4 |
| `SitOnChairLow` | `WarbandSceneAnimationStandState` | = 5 |
| `SitOnChairMedium` | `WarbandSceneAnimationStandState` | = 6 |
| `SitOnChairHigh` | `WarbandSceneAnimationStandState` | = 7 |
| `Sleep` | `WarbandSceneAnimationStandState` | = 8 |

### WarbandSceneAnimationStandStateFlags

*Enumeration* · 9 values, 1..256

Access values as `Enum.WarbandSceneAnimationStandStateFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Maintain` | `WarbandSceneAnimationStandStateFlags` | = 1 |
| `Stand` | `WarbandSceneAnimationStandStateFlags` | = 2 |
| `SitOnGround` | `WarbandSceneAnimationStandStateFlags` | = 4 |
| `Kneel` | `WarbandSceneAnimationStandStateFlags` | = 8 |
| `ReadyStance` | `WarbandSceneAnimationStandStateFlags` | = 16 |
| `SitOnChairLow` | `WarbandSceneAnimationStandStateFlags` | = 32 |
| `SitOnChairMedium` | `WarbandSceneAnimationStandStateFlags` | = 64 |
| `SitOnChairHigh` | `WarbandSceneAnimationStandStateFlags` | = 128 |
| `Sleep` | `WarbandSceneAnimationStandStateFlags` | = 256 |

### WarbandScenePlacementType

*Enumeration* · 3 values, 0..2

Access values as `Enum.WarbandScenePlacementType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Character` | `WarbandScenePlacementType` | = 0 |
| `Pet` | `WarbandScenePlacementType` | = 1 |
| `Chair` | `WarbandScenePlacementType` | = 2 |
