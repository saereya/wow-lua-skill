# Tutorial

Namespace `C_Tutorial` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/tutorialdocumentation.lua` (FileDataID 4637276)

## Functions

### AbandonTutorialArea

```lua
C_Tutorial.AbandonTutorialArea()
```

### GetCombatEventInfo

```lua
C_Tutorial.GetCombatEventInfo()
```

`RequireNPERestricted`

### ReturnToTutorialArea

```lua
C_Tutorial.ReturnToTutorialArea()
```

### SendTutorialStartButtonTelem

```lua
C_Tutorial.SendTutorialStartButtonTelem(skipTutorial: bool)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

## Events

### LEAVING_TUTORIAL_AREA

```lua
LEAVING_TUTORIAL_AREA()
```

`SynchronousEvent`

### NPE_TUTORIAL_UPDATE

```lua
NPE_TUTORIAL_UPDATE()
```

`SynchronousEvent`

### TUTORIAL_COMBAT_EVENT

```lua
TUTORIAL_COMBAT_EVENT()
```

`RequireNPERestricted` `SynchronousEvent`

### TUTORIAL_HIGHLIGHT_SPELL

```lua
TUTORIAL_HIGHLIGHT_SPELL(spellID: number, tutorialGlobalStringTag: cstring)
```

`SynchronousEvent`

### TUTORIAL_TRIGGER

```lua
TUTORIAL_TRIGGER(tutorialIndex: number, forceShow: bool)
```

`SynchronousEvent`

### TUTORIAL_UNHIGHLIGHT_SPELL

```lua
TUTORIAL_UNHIGHLIGHT_SPELL()
```

`SynchronousEvent`

## Types

### FrameTutorialAccount

*Enumeration* · 51 values, 1..51

Access values as `Enum.FrameTutorialAccount.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `HudRevampBagChanges` | `FrameTutorialAccount` | = 1 |
| `PerksProgramActivitiesIntro` | `FrameTutorialAccount` | = 2 |
| `EditModeManager` | `FrameTutorialAccount` | = 3 |
| `TransmogSetsTab` | `FrameTutorialAccount` | = 4 |
| `MountCollectionDragonriding` | `FrameTutorialAccount` | = 5 |
| `LFGList` | `FrameTutorialAccount` | = 6 |
| `HeirloomJournalLevel` | `FrameTutorialAccount` | = 7 |
| `TimerunnersAdvantage` | `FrameTutorialAccount` | = 8 |
| `AccountWideReputation` | `FrameTutorialAccount` | = 9 |
| `TransferableCurrencies` | `FrameTutorialAccount` | = 10 |
| `BindToAccountUntilEquip` | `FrameTutorialAccount` | = 11 |
| `CompletedQuestsFilter` | `FrameTutorialAccount` | = 12 |
| `CompletedQuestsFilterSeen` | `FrameTutorialAccount` | = 13 |
| `ConcentrationCurrency` | `FrameTutorialAccount` | = 14 |
| `MapLegendOpened` | `FrameTutorialAccount` | = 15 |
| `NpcCraftingOrders` | `FrameTutorialAccount` | = 16 |
| `NpcCraftingOrderCreateButton` | `FrameTutorialAccount` | = 17 |
| `NpcCraftingOrderTabNew` | `FrameTutorialAccount` | = 18 |
| `LocalStoriesFilterSeen` | `FrameTutorialAccount` | = 19 |
| `EventSchedulerTabSeen` | `FrameTutorialAccount` | = 20 |
| `AssistedCombatRotationDragSpell` | `FrameTutorialAccount` | = 21 |
| `AssistedCombatRotationActionButton` | `FrameTutorialAccount` | = 22 |
| `HousingDecorCleanup` | `FrameTutorialAccount` | = 23 |
| `HousingDecorPlace` | `FrameTutorialAccount` | = 24 |
| `HousingDecorClippingGrid` | `FrameTutorialAccount` | = 25 |
| `HousingDecorCustomization` | `FrameTutorialAccount` | = 26 |
| `HousingDecorLayout` | `FrameTutorialAccount` | = 27 |
| `HousingHouseFinderMap` | `FrameTutorialAccount` | = 28 |
| `HousingHouseFinderVisitHouse` | `FrameTutorialAccount` | = 29 |
| `HousingItemAcquisition` | `FrameTutorialAccount` | = 30 |
| `HousingNewPip` | `FrameTutorialAccount` | = 31 |
| `PerksProgramActivitiesOpen` | `FrameTutorialAccount` | = 32 |
| `EnconterJournalTutorialsTabSeen` | `FrameTutorialAccount` | = 33 |
| `HousingMarketTab` | `FrameTutorialAccount` | = 34 |
| `HousingTeleportButton` | `FrameTutorialAccount` | = 35 |
| `RPETalentStarterBuild` | `FrameTutorialAccount` | = 36 |
| `HousingInvalidCollision` | `FrameTutorialAccount` | = 37 |
| `HousingModesUnlocked` | `FrameTutorialAccount` | = 38 |
| `HousingExpertMode` | `FrameTutorialAccount` | = 39 |
| `HousingCleanupMode` | `FrameTutorialAccount` | = 40 |
| `TransmogOutfits` | `FrameTutorialAccount` | = 41 |
| `TransmogSets` | `FrameTutorialAccount` | = 42 |
| `TransmogCustomSets` | `FrameTutorialAccount` | = 43 |
| `TransmogSituations` | `FrameTutorialAccount` | = 44 |
| `TransmogWeaponOptions` | `FrameTutorialAccount` | = 45 |
| `TransmogTrialOfStyle` | `FrameTutorialAccount` | = 46 |
| `TransmogCustomSetsMigration` | `FrameTutorialAccount` | = 47 |
| `HousingEndeavorsTabSeen` | `FrameTutorialAccount` | = 48 |
| `RunesOfPower` | `FrameTutorialAccount` | = 49 |
| `HousingPetBeds` | `FrameTutorialAccount` | = 50 |
| `Reserved1` | `FrameTutorialAccount` | = 51 |

## Predicates

Conditions referenced by the flags above.

- `RequireNPERestricted` *Precondition* (failure mode: ReturnNothing)
