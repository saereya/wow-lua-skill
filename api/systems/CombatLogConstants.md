# CombatLogConstants

source `interface/addons/blizzard_apidocumentationgenerated/combatlogconstantsdocumentation.lua` (FileDataID 7036075)

## Types

### CombatLogObject

*Enumeration* · 20 values, 0..2147483648

Access values as `Enum.CombatLogObject.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Empty` | `CombatLogObject` | = 0 |
| `AffiliationMine` | `CombatLogObject` | = 1 |
| `AffiliationParty` | `CombatLogObject` | = 2 |
| `AffiliationRaid` | `CombatLogObject` | = 4 |
| `AffiliationOutsider` | `CombatLogObject` | = 8 |
| `ReactionFriendly` | `CombatLogObject` | = 16 |
| `ReactionNeutral` | `CombatLogObject` | = 32 |
| `ReactionHostile` | `CombatLogObject` | = 64 |
| `ControlPlayer` | `CombatLogObject` | = 256 |
| `ControlNpc` | `CombatLogObject` | = 512 |
| `TypePlayer` | `CombatLogObject` | = 1024 |
| `TypeNpc` | `CombatLogObject` | = 2048 |
| `TypePet` | `CombatLogObject` | = 4096 |
| `TypeGuardian` | `CombatLogObject` | = 8192 |
| `TypeObject` | `CombatLogObject` | = 16384 |
| `Target` | `CombatLogObject` | = 65536 |
| `Focus` | `CombatLogObject` | = 131072 |
| `Maintank` | `CombatLogObject` | = 262144 |
| `Mainassist` | `CombatLogObject` | = 524288 |
| `None` | `CombatLogObject` | = 2147483648 |

### CombatLogObjectTarget

*Enumeration* · 9 values, 1..2147483648

Access values as `Enum.CombatLogObjectTarget.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Raidtarget1` | `CombatLogObjectTarget` | = 1 |
| `Raidtarget2` | `CombatLogObjectTarget` | = 2 |
| `Raidtarget3` | `CombatLogObjectTarget` | = 4 |
| `Raidtarget4` | `CombatLogObjectTarget` | = 8 |
| `Raidtarget5` | `CombatLogObjectTarget` | = 16 |
| `Raidtarget6` | `CombatLogObjectTarget` | = 32 |
| `Raidtarget7` | `CombatLogObjectTarget` | = 64 |
| `Raidtarget8` | `CombatLogObjectTarget` | = 128 |
| `RaidNone` | `CombatLogObjectTarget` | = 2147483648 |

### CombatLogMessageLimits

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `CombatLogDefaultMessageLimit` | `number` | = `300` |
| `CombatLogMaximumMessageLimit` | `number` | = `1000` |

### CombatLogObjectMasks

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `COMBATLOG_OBJECT_AFFILIATION_MASK` | `CombatLogObject` | = `15` |
| `COMBATLOG_OBJECT_REACTION_MASK` | `CombatLogObject` | = `240` |
| `COMBATLOG_OBJECT_CONTROL_MASK` | `CombatLogObject` | = `768` |
| `COMBATLOG_OBJECT_TYPE_MASK` | `CombatLogObject` | = `64512` |
| `COMBATLOG_OBJECT_SPECIAL_MASK` | `CombatLogObject` | = `4294901760` |

### CombatLogObjectTargetMasks

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `COMBATLOG_OBJECT_RAID_TARGET_MASK` | `CombatLogObjectTarget` | = `255` |
| `COMBATLOG_OBJECT_RAID_MASK` | `CombatLogObjectTarget` | = `4294967295` |
