# DamageConstants

source `interface/addons/blizzard_apidocumentationgenerated/damageconstantsdocumentation.lua` (FileDataID 4637092)

## Types

### Causeofdeath

*Enumeration* · 10 values, 0..9

Access values as `Enum.Causeofdeath.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `Causeofdeath` | = 0 |
| `PlayerPvP` | `Causeofdeath` | = 1 |
| `PlayerDuel` | `Causeofdeath` | = 2 |
| `Creature` | `Causeofdeath` | = 3 |
| `Falling` | `Causeofdeath` | = 4 |
| `Drowning` | `Causeofdeath` | = 5 |
| `Fatigue` | `Causeofdeath` | = 6 |
| `Slime` | `Causeofdeath` | = 7 |
| `Lava` | `Causeofdeath` | = 8 |
| `Fire` | `Causeofdeath` | = 9 |

### CauseofdeathFlags

*Enumeration* · 4 values, 0..4

Access values as `Enum.CauseofdeathFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `NoneNeeded` | `CauseofdeathFlags` | = 0 |
| `PlayerNameNeeded` | `CauseofdeathFlags` | = 1 |
| `CreatureNameNeeded` | `CauseofdeathFlags` | = 2 |
| `ZoneNameNeeded` | `CauseofdeathFlags` | = 4 |

### Damageclass

*Enumeration* · 46 values, 0..127

Access values as `Enum.Damageclass.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Physical` | `Damageclass` | = 0 |
| `Holy` | `Damageclass` | = 1 |
| `Fire` | `Damageclass` | = 2 |
| `Nature` | `Damageclass` | = 3 |
| `Frost` | `Damageclass` | = 4 |
| `Shadow` | `Damageclass` | = 5 |
| `Arcane` | `Damageclass` | = 6 |
| `FirstResist` | `Damageclass` | = 2 |
| `LastResist` | `Damageclass` | = 6 |
| `MaskNone` | `Damageclass` | = 0 |
| `MaskPhysical` | `Damageclass` | = 1 |
| `MaskHoly` | `Damageclass` | = 2 |
| `MaskFire` | `Damageclass` | = 4 |
| `MaskNature` | `Damageclass` | = 8 |
| `MaskFrost` | `Damageclass` | = 16 |
| `MaskShadow` | `Damageclass` | = 32 |
| `MaskArcane` | `Damageclass` | = 64 |
| `AllPhysical` | `Damageclass` | = 1 |
| `AllMagical` | `Damageclass` | = 126 |
| `All` | `Damageclass` | = 127 |
| `MaskFlamestrike` | `Damageclass` | = 5 |
| `MaskFroststrike` | `Damageclass` | = 17 |
| `MaskSpellstrike` | `Damageclass` | = 65 |
| `MaskShadowstrike` | `Damageclass` | = 33 |
| `MaskStormstrike` | `Damageclass` | = 9 |
| `MaskHolystrike` | `Damageclass` | = 3 |
| `MaskFrostfire` | `Damageclass` | = 20 |
| `MaskSpellfire` | `Damageclass` | = 68 |
| `MaskFirestorm` | `Damageclass` | = 12 |
| `MaskShadowflame` | `Damageclass` | = 36 |
| `MaskHolyfire` | `Damageclass` | = 6 |
| `MaskSpellfrost` | `Damageclass` | = 80 |
| `MaskFroststorm` | `Damageclass` | = 24 |
| `MaskShadowfrost` | `Damageclass` | = 48 |
| `MaskHolyfrost` | `Damageclass` | = 18 |
| `MaskSpellstorm` | `Damageclass` | = 72 |
| `MaskSpellshadow` | `Damageclass` | = 96 |
| `MaskDivine` | `Damageclass` | = 66 |
| `MaskShadowstorm` | `Damageclass` | = 40 |
| `MaskHolystorm` | `Damageclass` | = 10 |
| `MaskTwilight` | `Damageclass` | = 34 |
| `MaskElemental` | `Damageclass` | = 28 |
| `MaskChromatic` | `Damageclass` | = 62 |
| `MaskMagical` | `Damageclass` | = 126 |
| `MaskChaos` | `Damageclass` | = 124 |
| `MaskCosmic` | `Damageclass` | = 106 |

### DamageclassType

*Enumeration* · 2 values, 0..1

Access values as `Enum.DamageclassType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Physical` | `DamageclassType` | = 0 |
| `Magical` | `DamageclassType` | = 1 |

### EnvironmentalDamageFlags

*Enumeration* · 2 values, 1..2

Access values as `Enum.EnvironmentalDamageFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `OneTime` | `EnvironmentalDamageFlags` | = 1 |
| `DmgIsPct` | `EnvironmentalDamageFlags` | = 2 |

### Environmentaldamagetype

*Enumeration* · 6 values, 0..5

Access values as `Enum.Environmentaldamagetype.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Fatigue` | `Environmentaldamagetype` | = 0 |
| `Drowning` | `Environmentaldamagetype` | = 1 |
| `Falling` | `Environmentaldamagetype` | = 2 |
| `Lava` | `Environmentaldamagetype` | = 3 |
| `Slime` | `Environmentaldamagetype` | = 4 |
| `Fire` | `Environmentaldamagetype` | = 5 |
