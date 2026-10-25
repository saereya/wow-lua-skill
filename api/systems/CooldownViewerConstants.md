# CooldownViewerConstants

source `interface/addons/blizzard_apidocumentationgenerated/cooldownviewerconstantsdocumentation.lua` (FileDataID 6438301)

## Types

### CooldownSetLinkedSpellFlags

*Enumeration* · 1 values, 1..1

Access values as `Enum.CooldownSetLinkedSpellFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `UseAsTooltip` | `CooldownSetLinkedSpellFlags` | = 1 |

### CooldownSetSpellFlags

*Enumeration* · 3 values, 1..4

Access values as `Enum.CooldownSetSpellFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `HideAura` | `CooldownSetSpellFlags` | = 1 |
| `HideByDefault` | `CooldownSetSpellFlags` | = 2 |
| `SelectHighestLevelLinkedSpell` | `CooldownSetSpellFlags` | = 4 |

### CooldownViewerAddAlertStatus

*Enumeration* · 4 values, 0..3

Access values as `Enum.CooldownViewerAddAlertStatus.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Success` | `CooldownViewerAddAlertStatus` | = 0 |
| `InvalidAlertType` | `CooldownViewerAddAlertStatus` | = 1 |
| `InvalidEventType` | `CooldownViewerAddAlertStatus` | = 2 |
| `DuplicateAlert` | `CooldownViewerAddAlertStatus` | = 3 |

### CooldownViewerAlertEventType

*Enumeration* · 6 values, 1..6

Access values as `Enum.CooldownViewerAlertEventType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Available` | `CooldownViewerAlertEventType` | = 1 |
| `PandemicTime` | `CooldownViewerAlertEventType` | = 2 |
| `OnCooldown` | `CooldownViewerAlertEventType` | = 3 |
| `ChargeGained` | `CooldownViewerAlertEventType` | = 4 |
| `OnAuraApplied` | `CooldownViewerAlertEventType` | = 5 |
| `OnAuraRemoved` | `CooldownViewerAlertEventType` | = 6 |

### CooldownViewerAlertType

*Enumeration* · 2 values, 1..2

Access values as `Enum.CooldownViewerAlertType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Sound` | `CooldownViewerAlertType` | = 1 |
| `Visual` | `CooldownViewerAlertType` | = 2 |

### CooldownViewerCategory

*Enumeration* · 9 values, 0..8

Access values as `Enum.CooldownViewerCategory.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Essential` | `CooldownViewerCategory` | = 0 |
| `Utility` | `CooldownViewerCategory` | = 1 |
| `TrackedBuff` | `CooldownViewerCategory` | = 2 |
| `TrackedBar` | `CooldownViewerCategory` | = 3 |
| `GroupBuff` | `CooldownViewerCategory` | = 4 |
| `SpecAgnosticEssential` | `CooldownViewerCategory` | = 5 |
| `SpecAgnosticTracked` | `CooldownViewerCategory` | = 6 |
| `EquipSlotEssential` | `CooldownViewerCategory` | = 7 |
| `EquipSlotTracked` | `CooldownViewerCategory` | = 8 |

### CooldownViewerSound

*Enumeration* · 94 values, 0..93

Access values as `Enum.CooldownViewerSound.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `TextToSpeech` | `CooldownViewerSound` | = 0 |
| `AnimalsCat` | `CooldownViewerSound` | = 1 |
| `AnimalsChicken` | `CooldownViewerSound` | = 2 |
| `AnimalsCow` | `CooldownViewerSound` | = 3 |
| `AnimalsGnoll` | `CooldownViewerSound` | = 4 |
| `AnimalsGoat` | `CooldownViewerSound` | = 5 |
| `AnimalsLion` | `CooldownViewerSound` | = 6 |
| `AnimalsPanther` | `CooldownViewerSound` | = 7 |
| `AnimalsRattlesnake` | `CooldownViewerSound` | = 8 |
| `AnimalsSheep` | `CooldownViewerSound` | = 9 |
| `AnimalsWolf` | `CooldownViewerSound` | = 10 |
| `DevicesBoatHorn` | `CooldownViewerSound` | = 11 |
| `DevicesAirHorn` | `CooldownViewerSound` | = 12 |
| `DevicesBikeHorn` | `CooldownViewerSound` | = 13 |
| `DevicesCashRegister` | `CooldownViewerSound` | = 14 |
| `DevicesJackpotBell` | `CooldownViewerSound` | = 15 |
| `DevicesJackpotCoins` | `CooldownViewerSound` | = 16 |
| `DevicesJackpotFail` | `CooldownViewerSound` | = 17 |
| `DevicesRotaryPhoneDial` | `CooldownViewerSound` | = 18 |
| `DevicesRotaryPhoneRing` | `CooldownViewerSound` | = 19 |
| `DevicesStovePipe` | `CooldownViewerSound` | = 20 |
| `DevicesTrashcanLid` | `CooldownViewerSound` | = 21 |
| `ImpactsAnvilStrike` | `CooldownViewerSound` | = 22 |
| `ImpactsBubbleSmash` | `CooldownViewerSound` | = 23 |
| `ImpactsLowThud` | `CooldownViewerSound` | = 24 |
| `ImpactsMetalClanks` | `CooldownViewerSound` | = 25 |
| `ImpactsMetalRattle` | `CooldownViewerSound` | = 26 |
| `ImpactsMetalScrape` | `CooldownViewerSound` | = 27 |
| `ImpactsMetalWarble` | `CooldownViewerSound` | = 28 |
| `ImpactsPopClick` | `CooldownViewerSound` | = 29 |
| `ImpactsStrangeClang` | `CooldownViewerSound` | = 30 |
| `ImpactsSwordScrape` | `CooldownViewerSound` | = 31 |
| `InstrumentsBellRing` | `CooldownViewerSound` | = 32 |
| `InstrumentsBellTrill` | `CooldownViewerSound` | = 33 |
| `InstrumentsBrass` | `CooldownViewerSound` | = 34 |
| `InstrumentsChimeAscending` | `CooldownViewerSound` | = 35 |
| `InstrumentsGuitarChug` | `CooldownViewerSound` | = 36 |
| `InstrumentsGuitarPinch` | `CooldownViewerSound` | = 37 |
| `InstrumentsPitchPipeDistressed` | `CooldownViewerSound` | = 38 |
| `InstrumentsPitchPipeNote` | `CooldownViewerSound` | = 39 |
| `InstrumentsSynthBig` | `CooldownViewerSound` | = 40 |
| `InstrumentsSynthBuzz` | `CooldownViewerSound` | = 41 |
| `InstrumentsSynthHigh` | `CooldownViewerSound` | = 42 |
| `InstrumentsWarhorn` | `CooldownViewerSound` | = 43 |
| `War2AbstractWhoosh` | `CooldownViewerSound` | = 44 |
| `War2Choir` | `CooldownViewerSound` | = 45 |
| `War2Construction` | `CooldownViewerSound` | = 46 |
| `War2MagicChimes` | `CooldownViewerSound` | = 47 |
| `War2PigSqueal` | `CooldownViewerSound` | = 48 |
| `War2Saws` | `CooldownViewerSound` | = 49 |
| `War2Seal` | `CooldownViewerSound` | = 50 |
| `War2Slow` | `CooldownViewerSound` | = 51 |
| `War2Smith` | `CooldownViewerSound` | = 52 |
| `War2SynthStinger` | `CooldownViewerSound` | = 53 |
| `War2TrumpetRally` | `CooldownViewerSound` | = 54 |
| `War2ZippyMagic` | `CooldownViewerSound` | = 55 |
| `War3Bell` | `CooldownViewerSound` | = 56 |
| `War3CrunchyBell` | `CooldownViewerSound` | = 57 |
| `War3DrumSplash` | `CooldownViewerSound` | = 58 |
| `War3Error` | `CooldownViewerSound` | = 59 |
| `War3Fanfare` | `CooldownViewerSound` | = 60 |
| `War3GateOpen` | `CooldownViewerSound` | = 61 |
| `War3Gold` | `CooldownViewerSound` | = 62 |
| `War3MagicShimmer` | `CooldownViewerSound` | = 63 |
| `War3Ringout` | `CooldownViewerSound` | = 64 |
| `War3Rooster` | `CooldownViewerSound` | = 65 |
| `War3ShimmerBell` | `CooldownViewerSound` | = 66 |
| `War3WolfHowl` | `CooldownViewerSound` | = 67 |
| `ShortBellStrike` | `CooldownViewerSound` | = 68 |
| `ShortBellTree` | `CooldownViewerSound` | = 69 |
| `ShortBigPot` | `CooldownViewerSound` | = 70 |
| `ShortBlades` | `CooldownViewerSound` | = 71 |
| `ShortCoffeeMug` | `CooldownViewerSound` | = 72 |
| `ShortCowBell` | `CooldownViewerSound` | = 73 |
| `ShortFingerSnap` | `CooldownViewerSound` | = 74 |
| `ShortGuitar` | `CooldownViewerSound` | = 75 |
| `ShortKalimba` | `CooldownViewerSound` | = 76 |
| `ShortMetalBladeDrop` | `CooldownViewerSound` | = 77 |
| `ShortMetalBladeOnRod` | `CooldownViewerSound` | = 78 |
| `ShortMetalImpact` | `CooldownViewerSound` | = 79 |
| `ShortMiniWoodXylophone` | `CooldownViewerSound` | = 80 |
| `ShortPaperCup` | `CooldownViewerSound` | = 81 |
| `ShortSheetMetal` | `CooldownViewerSound` | = 82 |
| `ShortStovePipe` | `CooldownViewerSound` | = 83 |
| `ShortStovePipeBlade` | `CooldownViewerSound` | = 84 |
| `ShortSwordShing` | `CooldownViewerSound` | = 85 |
| `ShortSynthBleep` | `CooldownViewerSound` | = 86 |
| `ShortSynthBlurp` | `CooldownViewerSound` | = 87 |
| `ShortSynthError` | `CooldownViewerSound` | = 88 |
| `ShortSynthHigh` | `CooldownViewerSound` | = 89 |
| `ShortTriangle` | `CooldownViewerSound` | = 90 |
| `ShortWaterDrop` | `CooldownViewerSound` | = 91 |
| `ShortWineBottle` | `CooldownViewerSound` | = 92 |
| `ShortWoodXylophone` | `CooldownViewerSound` | = 93 |

### GroupBuffItemFlags

*Enumeration* · 1 values, 1..1

Access values as `Enum.GroupBuffItemFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `HideByDefault` | `GroupBuffItemFlags` | = 1 |

### CooldownViewerUIConstants

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `COOLDOWN_VIEWER_LINKED_SPELLS_SIZE` | `number` | = `4` |
| `COOLDOWN_VIEWER_CATEGORY_SET_SIZE` | `number` | = `16` |
| `COOLDOWN_VIEWER_SPEC_AGNOSTIC_PARENT_ID` | `number` | = `0` |
| `COOLDOWN_VIEWER_COMBAT_POTION_ICON_FID` | `number` | = `134737` |
| `COOLDOWN_VIEWER_HEALTH_POTION_ICON_FID` | `number` | = `134834` |
| `COOLDOWN_VIEWER_HEALTHSTONE_ICON_FID` | `number` | = `538745` |

### GroupBuffUIConstants

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `GROUP_BUFF_ITEM_LIST_SIZE` | `number` | = `16` |
