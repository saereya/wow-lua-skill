# ActionBar

Namespace `C_ActionBar` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/actionbarframedocumentation.lua` (FileDataID 4637017)

## Functions

### EnableActionRangeCheck

```lua
C_ActionBar.EnableActionRangeCheck(actionID: luaIndex, enable: bool)
```

Used in conjunction with ActionRangeCheckUpdate to inform the UI when an action goes in or out of range with its current target.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `actionID` | `luaIndex` |  |
| `enable` | `bool` | True if changes in range for the action should dispatch ActionRangeCheckUpdate. False if the action no longer needs the event. |

### FindAssistedCombatActionButtons

```lua
C_ActionBar.FindAssistedCombatActionButtons(setToSearch: ActionBarSet) -> slots: luaIndex[]
```

Returns the list of action bar slots that contain the Assisted Combat action spell.

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `setToSearch` | `ActionBarSet` | default `"All"` |

### FindFlyoutActionButtons

```lua
C_ActionBar.FindFlyoutActionButtons(flyoutID: number, setToSearch: ActionBarSet) -> slots: luaIndex[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `flyoutID` | `number` |  |
| `setToSearch` | `ActionBarSet` | default `"All"` |

### FindPetActionButtons

```lua
C_ActionBar.FindPetActionButtons(petActionID: number, setToSearch: ActionBarSet) -> slots: luaIndex[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `petActionID` | `number` |  |
| `setToSearch` | `ActionBarSet` | default `"All"` |

### FindSpellActionButtons

```lua
C_ActionBar.FindSpellActionButtons(spellID: SpellIdentifier, setToSearch: ActionBarSet) -> slots: luaIndex[]
```

Returns the list of action bar slots that contain a specified spell.

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `SpellIdentifier` | Expects a base spell, so if a spell is overridden the base ID should be provided. |
| `setToSearch` | `ActionBarSet` | default `"All"`; `NeverSecret` |

### ForceUpdateAction

```lua
C_ActionBar.ForceUpdateAction(slotID: luaIndex, suppressEvents: bool)
```

Force updates some internals for an action button slot.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `slotID` | `luaIndex` |  |
| `suppressEvents` | `bool` | default `false` |

### GetActionAutocast

```lua
C_ActionBar.GetActionAutocast(actionID: luaIndex) -> autocastAllowed: bool, autocastEnabled: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresValidActionSlot`

### GetActionBarPage

```lua
C_ActionBar.GetActionBarPage() -> currentPage: luaIndex
```

### GetActionChargeDuration

```lua
C_ActionBar.GetActionChargeDuration(actionID: luaIndex) -> duration: LuaDurationObject
```

Returns a duration object describing the active recharge time for an action.

`SecretArguments=AllowedWhenUntainted` `RequiresValidActionSlot`

### GetActionCharges

```lua
C_ActionBar.GetActionCharges(actionID: luaIndex) -> chargeInfo: SpellChargeInfo
```

`SecretArguments=AllowedWhenUntainted` `RequiresValidActionSlot` `SecretWhenCooldownsRestricted`

### GetActionCooldown

```lua
C_ActionBar.GetActionCooldown(actionID: luaIndex) -> cooldownInfo: SpellCooldownInfo
```

`SecretArguments=AllowedWhenUntainted` `RequiresValidActionSlot` `SecretWhenCooldownsRestricted`

### GetActionCooldownDuration

```lua
C_ActionBar.GetActionCooldownDuration(actionID: luaIndex, ignoreGCD: bool) -> duration: LuaDurationObject
```

Returns a duration object describing the active cooldown duration for an action.

`SecretArguments=AllowedWhenUntainted` `RequiresValidActionSlot`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `actionID` | `luaIndex` |  |
| `ignoreGCD` | `bool` | default `false` |

### GetActionDisplayCount

```lua
C_ActionBar.GetActionDisplayCount(actionID: luaIndex, maxDisplayCount: number, replacementString: cstring) -> displayCount: string
```

Depending on the action type, return a string that is either the use count or number of charges. If value is beyond the display count parameter, returns the replacementString (defaults to '*').

`SecretArguments=AllowedWhenUntainted` `RequiresValidActionSlot` `SecretWhenCooldownsRestricted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `actionID` | `luaIndex` |  |
| `maxDisplayCount` | `number` | default `9999` |
| `replacementString` | `cstring` | default `"*"` |

### GetActionLossOfControlCooldownDuration

```lua
C_ActionBar.GetActionLossOfControlCooldownDuration(actionID: luaIndex) -> duration: LuaDurationObject
```

Returns a duration object describing the active loss of control cooldown duration for an action.

`SecretArguments=AllowedWhenUntainted` `RequiresValidActionSlot`

### GetActionLossOfControlCooldownInfo

```lua
C_ActionBar.GetActionLossOfControlCooldownInfo(actionID: luaIndex) -> lossOfControlInfo: SpellLossOfControlInfo
```

`SecretArguments=AllowedWhenUntainted` `RequiresValidActionSlot` `SecretWhenCooldownsRestricted`

### GetActionText

```lua
C_ActionBar.GetActionText(actionID: luaIndex) -> text: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresValidActionSlot`

### GetActionTexture

```lua
C_ActionBar.GetActionTexture(actionID: luaIndex) -> textureFileID: fileID
```

`SecretArguments=AllowedWhenUntainted` `RequiresValidActionSlot`

### GetActionUseCount

```lua
C_ActionBar.GetActionUseCount(actionID: luaIndex) -> count: number
```

`SecretArguments=AllowedWhenUntainted` `RequiresValidActionSlot` `SecretWhenCooldownsRestricted`

### GetBonusBarIndex

```lua
C_ActionBar.GetBonusBarIndex() -> bonusBarIndex: luaIndex
```

### GetBonusBarIndexForSlot

```lua
C_ActionBar.GetBonusBarIndexForSlot(slotID: luaIndex) -> bonusBarIndex: luaIndex?
```

`SecretArguments=AllowedWhenUntainted`

### GetBonusBarOffset

```lua
C_ActionBar.GetBonusBarOffset() -> bonusBarOffset: number
```

### GetExtraBarIndex

```lua
C_ActionBar.GetExtraBarIndex() -> extraBarIndex: luaIndex
```

### GetItemActionOnEquipSpellID

```lua
C_ActionBar.GetItemActionOnEquipSpellID(actionID: luaIndex) -> onEquipSpellID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetMultiCastBarIndex

```lua
C_ActionBar.GetMultiCastBarIndex() -> multiCastBarIndex: luaIndex
```

### GetOverrideBarIndex

```lua
C_ActionBar.GetOverrideBarIndex() -> overrideBarIndex: luaIndex
```

### GetOverrideBarSkin

```lua
C_ActionBar.GetOverrideBarSkin() -> textureFileID: fileID?
```

### GetPetActionPetBarIndices

```lua
C_ActionBar.GetPetActionPetBarIndices(petActionID: number, setToSearch: ActionBarSet) -> slots: luaIndex[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `petActionID` | `number` |  |
| `setToSearch` | `ActionBarSet` | default `"All"` |

### GetProfessionQuality

```lua
C_ActionBar.GetProfessionQuality(actionID: luaIndex) -> quality: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetProfessionQualityInfo

```lua
C_ActionBar.GetProfessionQualityInfo(actionID: luaIndex) -> info: CraftingQualityInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetSpell

```lua
C_ActionBar.GetSpell(actionID: luaIndex) -> spellID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetTempShapeshiftBarIndex

```lua
C_ActionBar.GetTempShapeshiftBarIndex() -> tempShapeshiftBarIndex: luaIndex
```

### GetVehicleBarIndex

```lua
C_ActionBar.GetVehicleBarIndex() -> vehicleBarIndex: luaIndex
```

### HasAction

```lua
C_ActionBar.HasAction(actionID: luaIndex) -> hasAction: bool
```

Returns true if an actionbar slot is populated with an action.

`SecretArguments=AllowedWhenUntainted` `RequiresValidActionSlot`

### HasAssistedCombatActionButtons

```lua
C_ActionBar.HasAssistedCombatActionButtons(setToSearch: ActionBarSet) -> hasButtons: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `setToSearch` | `ActionBarSet` | default `"All"` |

### HasBonusActionBar

```lua
C_ActionBar.HasBonusActionBar() -> hasBonusActionBar: bool
```

### HasExtraActionBar

```lua
C_ActionBar.HasExtraActionBar() -> hasExtraActionBar: bool
```

### HasFlyoutActionButtons

```lua
C_ActionBar.HasFlyoutActionButtons(flyoutID: number, setToSearch: ActionBarSet) -> hasFlyoutActionButtons: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `flyoutID` | `number` |  |
| `setToSearch` | `ActionBarSet` | default `"All"` |

### HasOverrideActionBar

```lua
C_ActionBar.HasOverrideActionBar() -> hasOverrideActionBar: bool
```

### HasPetActionButtons

```lua
C_ActionBar.HasPetActionButtons(petActionID: number, setToSearch: ActionBarSet) -> hasPetActionButtons: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `petActionID` | `number` |  |
| `setToSearch` | `ActionBarSet` | default `"All"` |

### HasPetActionPetBarIndices

```lua
C_ActionBar.HasPetActionPetBarIndices(petActionID: number, setToSearch: ActionBarSet) -> hasPetActionPetBarIndices: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `petActionID` | `number` |  |
| `setToSearch` | `ActionBarSet` | default `"All"` |

### HasRangeRequirements

```lua
C_ActionBar.HasRangeRequirements(actionID: luaIndex) -> hasRangeRequirements: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresValidActionSlot`

### HasSpellActionButtons

```lua
C_ActionBar.HasSpellActionButtons(spellID: SpellIdentifier, setToSearch: ActionBarSet) -> hasSpellActionButtons: bool
```

`SecretArguments=AllowedWhenTainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `SpellIdentifier` |  |
| `setToSearch` | `ActionBarSet` | default `"All"`; `NeverSecret` |

### HasTempShapeshiftActionBar

```lua
C_ActionBar.HasTempShapeshiftActionBar() -> hasTempShapeshiftActionBar: bool
```

### HasVehicleActionBar

```lua
C_ActionBar.HasVehicleActionBar() -> hasVehicleActionBar: bool
```

### IsActionInRange

```lua
C_ActionBar.IsActionInRange(actionID: luaIndex, target: UnitToken?) -> isInRange: bool?
```

`SecretArguments=AllowedWhenUntainted` `RequiresValidActionSlot`

Returns:

| Name | Type | Notes |
|---|---|---|
| `isInRange` | `bool?` | If nil, range cannot be determined (eg. no target is available). |

### IsAssistedCombatAction

```lua
C_ActionBar.IsAssistedCombatAction(slotID: luaIndex) -> isAssistedCombatAction: bool
```

Returns whether the given action button contains the Assisted Combat action spell.

`SecretArguments=AllowedWhenUntainted`

### IsAttackAction

```lua
C_ActionBar.IsAttackAction(actionID: luaIndex) -> isAttackAction: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresValidActionSlot`

### IsAutoCastPetAction

```lua
C_ActionBar.IsAutoCastPetAction(slotID: luaIndex) -> isAutoCastPetAction: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsAutoRepeatAction

```lua
C_ActionBar.IsAutoRepeatAction(actionID: luaIndex) -> isAutoRepeatAction: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresValidActionSlot`

### IsConsumableAction

```lua
C_ActionBar.IsConsumableAction(actionID: luaIndex) -> isConsumableAction: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresValidActionSlot`

### IsCurrentAction

```lua
C_ActionBar.IsCurrentAction(actionID: luaIndex) -> isCurrentAction: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresValidActionSlot`

### IsEnabledAutoCastPetAction

```lua
C_ActionBar.IsEnabledAutoCastPetAction(slotID: luaIndex) -> isEnabledAutoCastPetAction: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsEquippedAction

```lua
C_ActionBar.IsEquippedAction(actionID: luaIndex) -> isEquippedAction: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresValidActionSlot`

### IsEquippedGearOutfitAction

```lua
C_ActionBar.IsEquippedGearOutfitAction(slotID: luaIndex) -> isEquippedGearOutfitAction: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsHarmfulAction

```lua
C_ActionBar.IsHarmfulAction(actionID: luaIndex, useNeutral: bool) -> isHarmful: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsHelpfulAction

```lua
C_ActionBar.IsHelpfulAction(actionID: luaIndex, useNeutral: bool) -> isHelpful: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsInterruptAction

```lua
C_ActionBar.IsInterruptAction(slotID: luaIndex) -> isInterruptAction: bool
```

Returns whether the given action button contains a spell that can interrupt spellcasting.

`SecretArguments=AllowedWhenUntainted`

### IsItemAction

```lua
C_ActionBar.IsItemAction(actionID: luaIndex) -> isItemAction: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresValidActionSlot`

### IsMacroActionWithShowTooltip

```lua
C_ActionBar.IsMacroActionWithShowTooltip(actionID: luaIndex) -> isMacroActionWithShowTooltip: bool
```

Returns whether the given action button contains a macro with an explicit #showtooltip directive.

`SecretArguments=AllowedWhenUntainted` `RequiresValidActionSlot`

### IsOnBarOrSpecialBar

```lua
C_ActionBar.IsOnBarOrSpecialBar(spellID: SpellIdentifier, setToSearch: ActionBarSet) -> isOnBarOrSpecialBar: bool
```

`SecretArguments=AllowedWhenTainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `SpellIdentifier` |  |
| `setToSearch` | `ActionBarSet` | default `"All"`; `NeverSecret` |

### IsPossessBarVisible

```lua
C_ActionBar.IsPossessBarVisible() -> isPossessBarVisible: bool
```

### IsStackableAction

```lua
C_ActionBar.IsStackableAction(actionID: luaIndex) -> isStackableAction: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresValidActionSlot`

### IsUsableAction

```lua
C_ActionBar.IsUsableAction(actionID: luaIndex) -> isUsable: bool, isLackingResources: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresValidActionSlot`

### PutActionInSlot

```lua
C_ActionBar.PutActionInSlot(slotID: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### RegisterActionUIButton

```lua
C_ActionBar.RegisterActionUIButton(checkboxFrame: SimpleCheckbox, actionID: luaIndex, cooldownFrame: CooldownFrame)
```

`SecretArguments=AllowedWhenUntainted` `RequiresValidActionSlot`

### SetActionBarPage

```lua
C_ActionBar.SetActionBarPage(pageIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### ShouldOverrideBarShowHealthBar

```lua
C_ActionBar.ShouldOverrideBarShowHealthBar() -> showHealthBar: bool
```

### ShouldOverrideBarShowManaBar

```lua
C_ActionBar.ShouldOverrideBarShowManaBar() -> showManaBar: bool
```

### ShouldShowKeyring

```lua
C_ActionBar.ShouldShowKeyring() -> isKeyringEnabled: bool
```

### ToggleAutoCastPetAction

```lua
C_ActionBar.ToggleAutoCastPetAction(slotID: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### UnregisterActionUIButton

```lua
C_ActionBar.UnregisterActionUIButton(checkboxFrame: SimpleCheckbox)
```

`SecretArguments=AllowedWhenUntainted`

### UsesActionText

```lua
C_ActionBar.UsesActionText(actionID: luaIndex) -> usesActionText: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresValidActionSlot`

## Events

### ACTIONBAR_HIDEGRID

```lua
ACTIONBAR_HIDEGRID()
```

`SynchronousEvent`

### ACTIONBAR_PAGE_CHANGED

```lua
ACTIONBAR_PAGE_CHANGED()
```

`SynchronousEvent`

### ACTIONBAR_SHOW_BOTTOMLEFT

```lua
ACTIONBAR_SHOW_BOTTOMLEFT()
```

`SynchronousEvent`

### ACTIONBAR_SHOWGRID

```lua
ACTIONBAR_SHOWGRID()
```

`SynchronousEvent`

### ACTIONBAR_SLOT_CHANGED

```lua
ACTIONBAR_SLOT_CHANGED(slot: number)
```

`SynchronousEvent`

### ACTIONBAR_UPDATE_COOLDOWN

```lua
ACTIONBAR_UPDATE_COOLDOWN()
```

`UniqueEvent`

### ACTIONBAR_UPDATE_STATE

```lua
ACTIONBAR_UPDATE_STATE()
```

`UniqueEvent`

### ACTIONBAR_UPDATE_USABLE

```lua
ACTIONBAR_UPDATE_USABLE()
```

`UniqueEvent`

### ACTION_RANGE_CHECK_UPDATE

```lua
ACTION_RANGE_CHECK_UPDATE(slot: luaIndex, isInRange: bool, checksRange: bool)
```

Used in conjunction with EnableActionRangeCheck to inform the UI when an action goes in or out of range with its current target.

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `slot` | `luaIndex` |  |
| `isInRange` | `bool` | Whether or not the current target is in range of the action. Should not be used if the 'checksRange' parameter is false. |
| `checksRange` | `bool` | Can be false if a range check was not made for any reason, for example there is not a current target. |

### ACTION_USABLE_CHANGED

```lua
ACTION_USABLE_CHANGED(changes: ActionUsableState[])
```

`SynchronousEvent`

### PET_BAR_UPDATE

```lua
PET_BAR_UPDATE()
```

`SynchronousEvent`

### UPDATE_BONUS_ACTIONBAR

```lua
UPDATE_BONUS_ACTIONBAR()
```

`SynchronousEvent` `UniqueEvent`

### UPDATE_EXTRA_ACTIONBAR

```lua
UPDATE_EXTRA_ACTIONBAR()
```

`UniqueEvent`

### UPDATE_MULTI_CAST_ACTIONBAR

```lua
UPDATE_MULTI_CAST_ACTIONBAR()
```

`UniqueEvent`

### UPDATE_OVERRIDE_ACTIONBAR

```lua
UPDATE_OVERRIDE_ACTIONBAR()
```

`UniqueEvent`

## Types

### ActionBarSet

*Enumeration* · 4 values, 0..3

Access values as `Enum.ActionBarSet.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `ActionBarSet` | = 0 |
| `Mkb` | `ActionBarSet` | = 1 |
| `Gamepad` | `ActionBarSet` | = 2 |
| `All` | `ActionBarSet` | = 3 |
