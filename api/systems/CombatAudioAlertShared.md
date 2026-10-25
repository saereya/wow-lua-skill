# CombatAudioAlertShared

source `interface/addons/blizzard_apidocumentationgenerated/combataudioalertshareddocumentation.lua` (FileDataID 7697796)

## Types

### CombatAudioAlertCastState

*Enumeration* · 3 values, 0..2

Access values as `Enum.CombatAudioAlertCastState.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Off` | `CombatAudioAlertCastState` | = 0 |
| `OnCastStart` | `CombatAudioAlertCastState` | = 1 |
| `OnCastEnd` | `CombatAudioAlertCastState` | = 2 |

### CombatAudioAlertCategory

*Enumeration* · 10 values, 0..9

Access values as `Enum.CombatAudioAlertCategory.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `General` | `CombatAudioAlertCategory` | = 0 |
| `PlayerHealth` | `CombatAudioAlertCategory` | = 1 |
| `TargetHealth` | `CombatAudioAlertCategory` | = 2 |
| `PlayerCast` | `CombatAudioAlertCategory` | = 3 |
| `TargetCast` | `CombatAudioAlertCategory` | = 4 |
| `PlayerResource1` | `CombatAudioAlertCategory` | = 5 |
| `PlayerResource2` | `CombatAudioAlertCategory` | = 6 |
| `PartyHealth` | `CombatAudioAlertCategory` | = 7 |
| `PlayerDebuffs` | `CombatAudioAlertCategory` | = 8 |
| `PlayerHealthPulse` | `CombatAudioAlertCategory` | = 9 |

### CombatAudioAlertDebuffSelfAlertValues

*Enumeration* · 2 values, 0..1

Access values as `Enum.CombatAudioAlertDebuffSelfAlertValues.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Off` | `CombatAudioAlertDebuffSelfAlertValues` | = 0 |
| `DispelType` | `CombatAudioAlertDebuffSelfAlertValues` | = 1 |

### CombatAudioAlertPartyPercentValues

*Enumeration* · 11 values, 0..10

Access values as `Enum.CombatAudioAlertPartyPercentValues.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Off` | `CombatAudioAlertPartyPercentValues` | = 0 |
| `Under100Percent` | `CombatAudioAlertPartyPercentValues` | = 1 |
| `Under90Percent` | `CombatAudioAlertPartyPercentValues` | = 2 |
| `Under80Percent` | `CombatAudioAlertPartyPercentValues` | = 3 |
| `Under70Percent` | `CombatAudioAlertPartyPercentValues` | = 4 |
| `Under60Percent` | `CombatAudioAlertPartyPercentValues` | = 5 |
| `Under50Percent` | `CombatAudioAlertPartyPercentValues` | = 6 |
| `Under40Percent` | `CombatAudioAlertPartyPercentValues` | = 7 |
| `Under30Percent` | `CombatAudioAlertPartyPercentValues` | = 8 |
| `Under20Percent` | `CombatAudioAlertPartyPercentValues` | = 9 |
| `Under10Percent` | `CombatAudioAlertPartyPercentValues` | = 10 |

### CombatAudioAlertPercentValues

*Enumeration* · 6 values, 0..5

Access values as `Enum.CombatAudioAlertPercentValues.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Off` | `CombatAudioAlertPercentValues` | = 0 |
| `Every10Percent` | `CombatAudioAlertPercentValues` | = 1 |
| `Every20Percent` | `CombatAudioAlertPercentValues` | = 2 |
| `Every30Percent` | `CombatAudioAlertPercentValues` | = 3 |
| `Every40Percent` | `CombatAudioAlertPercentValues` | = 4 |
| `Every50Percent` | `CombatAudioAlertPercentValues` | = 5 |

### CombatAudioAlertPlayerCastFormatValues

*Enumeration* · 5 values, 0..4

Access values as `Enum.CombatAudioAlertPlayerCastFormatValues.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `CastingSpellname` | `CombatAudioAlertPlayerCastFormatValues` | = 0 |
| `CastSpellname` | `CombatAudioAlertPlayerCastFormatValues` | = 1 |
| `Casting` | `CombatAudioAlertPlayerCastFormatValues` | = 2 |
| `Cast` | `CombatAudioAlertPlayerCastFormatValues` | = 3 |
| `Spellname` | `CombatAudioAlertPlayerCastFormatValues` | = 4 |

### CombatAudioAlertPlayerDebuffFormatValues

*Enumeration* · 2 values, 0..1

Access values as `Enum.CombatAudioAlertPlayerDebuffFormatValues.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Full` | `CombatAudioAlertPlayerDebuffFormatValues` | = 0 |
| `NoSpellname` | `CombatAudioAlertPlayerDebuffFormatValues` | = 1 |

### CombatAudioAlertPlayerHealthFormatValues

*Enumeration* · 6 values, 0..5

Access values as `Enum.CombatAudioAlertPlayerHealthFormatValues.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `HealthFull` | `CombatAudioAlertPlayerHealthFormatValues` | = 0 |
| `HealthNoPercent` | `CombatAudioAlertPlayerHealthFormatValues` | = 1 |
| `HealthNoPercentDiv10` | `CombatAudioAlertPlayerHealthFormatValues` | = 2 |
| `NoHealthFull` | `CombatAudioAlertPlayerHealthFormatValues` | = 3 |
| `NoHealthNoPercent` | `CombatAudioAlertPlayerHealthFormatValues` | = 4 |
| `NoHealthNoPercentDiv10` | `CombatAudioAlertPlayerHealthFormatValues` | = 5 |

### CombatAudioAlertPlayerResourceFormatValues

*Enumeration* · 6 values, 0..5

Access values as `Enum.CombatAudioAlertPlayerResourceFormatValues.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `ResourceFull` | `CombatAudioAlertPlayerResourceFormatValues` | = 0 |
| `ResourceNoPercent` | `CombatAudioAlertPlayerResourceFormatValues` | = 1 |
| `ResourceNoPercentDiv10` | `CombatAudioAlertPlayerResourceFormatValues` | = 2 |
| `NoResourceFull` | `CombatAudioAlertPlayerResourceFormatValues` | = 3 |
| `NoResourceNoPercent` | `CombatAudioAlertPlayerResourceFormatValues` | = 4 |
| `NoResourceNoPercentDiv10` | `CombatAudioAlertPlayerResourceFormatValues` | = 5 |

### CombatAudioAlertPulsePercentValues

*Enumeration* · 10 values, 0..9

Access values as `Enum.CombatAudioAlertPulsePercentValues.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Off` | `CombatAudioAlertPulsePercentValues` | = 0 |
| `Under90Percent` | `CombatAudioAlertPulsePercentValues` | = 1 |
| `Under80Percent` | `CombatAudioAlertPulsePercentValues` | = 2 |
| `Under70Percent` | `CombatAudioAlertPulsePercentValues` | = 3 |
| `Under60Percent` | `CombatAudioAlertPulsePercentValues` | = 4 |
| `Under50Percent` | `CombatAudioAlertPulsePercentValues` | = 5 |
| `Under40Percent` | `CombatAudioAlertPulsePercentValues` | = 6 |
| `Under30Percent` | `CombatAudioAlertPulsePercentValues` | = 7 |
| `Under20Percent` | `CombatAudioAlertPulsePercentValues` | = 8 |
| `Under10Percent` | `CombatAudioAlertPulsePercentValues` | = 9 |

### CombatAudioAlertSayIfTargetedType

*Enumeration* · 4 values, 0..3

Access values as `Enum.CombatAudioAlertSayIfTargetedType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `CombatAudioAlertSayIfTargetedType` | = 0 |
| `Aggro` | `CombatAudioAlertSayIfTargetedType` | = 1 |
| `Targeted` | `CombatAudioAlertSayIfTargetedType` | = 2 |
| `TargetedBy` | `CombatAudioAlertSayIfTargetedType` | = 3 |

### CombatAudioAlertSpecSetting

*Enumeration* · 9 values, 0..8

Access values as `Enum.CombatAudioAlertSpecSetting.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Resource1Percent` | `CombatAudioAlertSpecSetting` | = 0 |
| `Resource1Format` | `CombatAudioAlertSpecSetting` | = 1 |
| `Resource1Voice` | `CombatAudioAlertSpecSetting` | = 2 |
| `Resource1Volume` | `CombatAudioAlertSpecSetting` | = 3 |
| `Resource2Percent` | `CombatAudioAlertSpecSetting` | = 4 |
| `Resource2Format` | `CombatAudioAlertSpecSetting` | = 5 |
| `Resource2Voice` | `CombatAudioAlertSpecSetting` | = 6 |
| `Resource2Volume` | `CombatAudioAlertSpecSetting` | = 7 |
| `SayIfTargeted` | `CombatAudioAlertSpecSetting` | = 8 |

### CombatAudioAlertTargetCastFormatValues

*Enumeration* · 7 values, 0..6

Access values as `Enum.CombatAudioAlertTargetCastFormatValues.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `TargetCastingSpellname` | `CombatAudioAlertTargetCastFormatValues` | = 0 |
| `TargetCastSpellname` | `CombatAudioAlertTargetCastFormatValues` | = 1 |
| `CastingSpellname` | `CombatAudioAlertTargetCastFormatValues` | = 2 |
| `CastSpellname` | `CombatAudioAlertTargetCastFormatValues` | = 3 |
| `Casting` | `CombatAudioAlertTargetCastFormatValues` | = 4 |
| `Cast` | `CombatAudioAlertTargetCastFormatValues` | = 5 |
| `Spellname` | `CombatAudioAlertTargetCastFormatValues` | = 6 |

### CombatAudioAlertTargetDeathBehavior

*Enumeration* · 2 values, 0..1

Access values as `Enum.CombatAudioAlertTargetDeathBehavior.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Default` | `CombatAudioAlertTargetDeathBehavior` | = 0 |
| `SayTargetDead` | `CombatAudioAlertTargetDeathBehavior` | = 1 |

### CombatAudioAlertTargetHealthFormatValues

*Enumeration* · 9 values, 0..8

Access values as `Enum.CombatAudioAlertTargetHealthFormatValues.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `NoHealthFull` | `CombatAudioAlertTargetHealthFormatValues` | = 0 |
| `NoHealthNoPercent` | `CombatAudioAlertTargetHealthFormatValues` | = 1 |
| `NoHealthNoPercentDiv10` | `CombatAudioAlertTargetHealthFormatValues` | = 2 |
| `HealthFull` | `CombatAudioAlertTargetHealthFormatValues` | = 3 |
| `HealthNoPercent` | `CombatAudioAlertTargetHealthFormatValues` | = 4 |
| `HealthNoPercentDiv10` | `CombatAudioAlertTargetHealthFormatValues` | = 5 |
| `TargetFull` | `CombatAudioAlertTargetHealthFormatValues` | = 6 |
| `TargetNoPercent` | `CombatAudioAlertTargetHealthFormatValues` | = 7 |
| `TargetNoPercentDiv10` | `CombatAudioAlertTargetHealthFormatValues` | = 8 |

### CombatAudioAlertThrottle

*Enumeration* · 11 values, 0..10

Access values as `Enum.CombatAudioAlertThrottle.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Sample` | `CombatAudioAlertThrottle` | = 0 |
| `PlayerHealth` | `CombatAudioAlertThrottle` | = 1 |
| `TargetHealth` | `CombatAudioAlertThrottle` | = 2 |
| `PlayerCast` | `CombatAudioAlertThrottle` | = 3 |
| `TargetCast` | `CombatAudioAlertThrottle` | = 4 |
| `PlayerResource1` | `CombatAudioAlertThrottle` | = 5 |
| `PlayerResource2` | `CombatAudioAlertThrottle` | = 6 |
| `PlayerHealthSamePercent` | `CombatAudioAlertThrottle` | = 7 |
| `TargetHealthSamePercent` | `CombatAudioAlertThrottle` | = 8 |
| `PlayerResource1SamePercent` | `CombatAudioAlertThrottle` | = 9 |
| `PlayerResource2SamePercent` | `CombatAudioAlertThrottle` | = 10 |

### CombatAudioAlertType

*Enumeration* · 2 values, 0..1

Access values as `Enum.CombatAudioAlertType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Health` | `CombatAudioAlertType` | = 0 |
| `Cast` | `CombatAudioAlertType` | = 1 |

### CombatAudioAlertUnit

*Enumeration* · 2 values, 0..1

Access values as `Enum.CombatAudioAlertUnit.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Player` | `CombatAudioAlertUnit` | = 0 |
| `Target` | `CombatAudioAlertUnit` | = 1 |
