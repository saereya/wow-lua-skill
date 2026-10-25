# GameRules

Namespace `C_GameRules` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/gamerulesdocumentation.lua` (FileDataID 5096353)

## Functions

### AccountHasSDEnabled

```lua
C_GameRules.AccountHasSDEnabled() -> isSDEnabled: bool
```

### AutoConnectToGameModeRealm

```lua
C_GameRules.AutoConnectToGameModeRealm(gameModeRecordID: number)
```

`SecretArguments=AllowedWhenUntainted`

### DoesGameModeHavePromo

```lua
C_GameRules.DoesGameModeHavePromo(gameModeRecordID: number) -> hasPromo: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetActiveGameMode

```lua
C_GameRules.GetActiveGameMode() -> gameMode: GameMode
```

### GetCurrentEventRealmQueues

```lua
C_GameRules.GetCurrentEventRealmQueues() -> eventRealmQueues: EventRealmQueues
```

### GetCurrentGameModeDisplayInfo

```lua
C_GameRules.GetCurrentGameModeDisplayInfo() -> info: GameModeDisplayInfo?
```

### GetCurrentGameModeRecordID

```lua
C_GameRules.GetCurrentGameModeRecordID() -> gameModeRecordID: number
```

### GetDisplayedGameModeRecordIDAtIndex

```lua
C_GameRules.GetDisplayedGameModeRecordIDAtIndex(displayIndex: luaIndex) -> gameModeRecordID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetForeverExperiencePreset

```lua
C_GameRules.GetForeverExperiencePreset() -> preset: ForeverExperiencePreset?
```

### GetGameModeDisplayInfoByRecordID

```lua
C_GameRules.GetGameModeDisplayInfoByRecordID(gameModeRecordID: number) -> info: GameModeDisplayInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetGameModeGlueScreenName

```lua
C_GameRules.GetGameModeGlueScreenName() -> screenName: cstring
```

### GetGameModePromoGlobalString

```lua
C_GameRules.GetGameModePromoGlobalString(gameModeRecordID: number) -> promoGlobalString: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetGameRuleAsFloat

```lua
C_GameRules.GetGameRuleAsFloat(gameRule: GameRule, decimalPlaces: number) -> value: number
```

Returns the numeric value specified in the Game Rule, multiplied by 0.1 for every decimal place requested

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `gameRule` | `GameRule` |  |
| `decimalPlaces` | `number` | default `0` |

### GetGameRuleAsFrameStrata

```lua
C_GameRules.GetGameRuleAsFrameStrata(gameRule: GameRule) -> frameStrata: cstring
```

Returns the value specified in the Game Rule converted to a frame strata

`SecretArguments=AllowedWhenUntainted`

### GetNumDisplayedGameModes

```lua
C_GameRules.GetNumDisplayedGameModes() -> numDisplayedGameModes: number
```

### IsCharacterlessLoginActive

```lua
C_GameRules.IsCharacterlessLoginActive() -> active: bool
```

### IsClassAllowedForGameMode

```lua
C_GameRules.IsClassAllowedForGameMode(classID: number) -> valid: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsGameModeEnabled

```lua
C_GameRules.IsGameModeEnabled(gameModeRecordID: number) -> enabled: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsGameRuleActive

```lua
C_GameRules.IsGameRuleActive(gameRule: GameRule) -> isActive: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsHardcoreActive

```lua
C_GameRules.IsHardcoreActive() -> active: bool
```

### IsMultiActionBarVisibilityForced

```lua
C_GameRules.IsMultiActionBarVisibilityForced() -> valid: bool
```

### IsPersonalResourceDisplayEnabled

```lua
C_GameRules.IsPersonalResourceDisplayEnabled() -> isPersonalResourceDisplayEnabled: bool
```

Checks the game rule as well as nameplateShowSelf

### IsPlunderstorm

```lua
C_GameRules.IsPlunderstorm() -> active: bool
```

### IsSDHDToggleEnabled

```lua
C_GameRules.IsSDHDToggleEnabled() -> isEnabled: bool
```

### IsSelfFoundAllowed

```lua
C_GameRules.IsSelfFoundAllowed() -> active: bool
```

### IsStandard

```lua
C_GameRules.IsStandard() -> active: bool
```

### IsWoWHack

```lua
C_GameRules.IsWoWHack() -> active: bool
```

### SetForeverExperiencePreset

```lua
C_GameRules.SetForeverExperiencePreset(preset: ForeverExperiencePreset)
```

`SecretArguments=AllowedWhenUntainted`

### SetSDHDToggleValue

```lua
C_GameRules.SetSDHDToggleValue(setToSD: bool, usageLocation: SdToggleUsageLocationUI)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### ACTIVE_GAME_MODE_UPDATED

```lua
ACTIVE_GAME_MODE_UPDATED(gameMode: GameMode)
```

`SynchronousEvent`

### AVAILABLE_GAME_MODES_UPDATED

```lua
AVAILABLE_GAME_MODES_UPDATED()
```

`SynchronousEvent`

### EVENT_REALM_QUEUES_UPDATED

```lua
EVENT_REALM_QUEUES_UPDATED(eventRealmQueues: EventRealmQueues)
```

`SynchronousEvent`

### GAME_MODE_DISPLAY_INFO_UPDATED

```lua
GAME_MODE_DISPLAY_INFO_UPDATED()
```

`SynchronousEvent`

### GAME_MODE_DISPLAY_MODE_TOGGLE_DISABLED

```lua
GAME_MODE_DISPLAY_MODE_TOGGLE_DISABLED(gameModeRecordID: number, disabled: bool)
```

`SynchronousEvent`

### GAME_RULES_CHANGED

```lua
GAME_RULES_CHANGED()
```

`SynchronousEvent`

## Types

### ForeverExperiencePreset

*Enumeration* · 2 values, 0..1

Access values as `Enum.ForeverExperiencePreset.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Classic` | `ForeverExperiencePreset` | = 0 |
| `Modern` | `ForeverExperiencePreset` | = 1 |

### SdToggleUsageLocationUI

*Enumeration* · 4 values, 0..3

Access values as `Enum.SdToggleUsageLocationUI.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `BeforeLogin` | `SdToggleUsageLocationUI` | = 0 |
| `CharacterCreation` | `SdToggleUsageLocationUI` | = 1 |
| `BarberShop` | `SdToggleUsageLocationUI` | = 2 |
| `OptionsMenu` | `SdToggleUsageLocationUI` | = 3 |

### GameModeDisplayInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `logo` | `fileID` |  |
| `logoHeight` | `number` |  |
| `logoVerticalOffset` | `number` |  |
| `logoShrunkenHeight` | `number` |  |
| `logoUsesDarkBackdrop` | `bool` |  |
| `characterCreateExtraHeight` | `number` |  |
| `characterCreateOuterBorder` | `fileID` |  |
