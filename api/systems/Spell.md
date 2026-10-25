# Spell

Namespace `C_Spell` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/spelldocumentation.lua` (FileDataID 4637244)

## Functions

### CancelAutoRepeatSpell

```lua
C_Spell.CancelAutoRepeatSpell() -> wasCancelled: bool
```

Cancels the player's active auto repeat spell, if any

`HasRestrictions`

### CancelItemTempEnchantment

```lua
C_Spell.CancelItemTempEnchantment(weaponSlot: WeaponSlot, enchantmentType: ItemEnchantType)
```

Cancel a temporary enchantment on an item

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### CancelSpellByID

```lua
C_Spell.CancelSpellByID(spellID: number)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### DoesSpellExist

```lua
C_Spell.DoesSpellExist(spellIdentifier: SpellIdentifier) -> spellExists: bool
```

Returns true if the spell exists, regardless of whether the player has learned it

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellIdentifier` | `SpellIdentifier` | Spell ID, name, name(subtext), or link; Using name will always check for an override on that spell |

### EnableSpellRangeCheck

```lua
C_Spell.EnableSpellRangeCheck(spellIdentifier: SpellIdentifier, enable: bool)
```

Used in conjunction with SpellRangeCheckUpdate to inform the UI when a spell goes in or out of range with the current target.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellIdentifier` | `SpellIdentifier` |  |
| `enable` | `bool` | True if changes in range for the spell should dispatch SpellRangeCheckUpdate. False if the spell no longer needs the event. |

### GetAuraStatChanges

```lua
C_Spell.GetAuraStatChanges(spellID: number) -> healthChange: number, powerTypeChanges: PowerTypeChange[]
```

`SecretArguments=AllowedWhenUntainted`

### GetBaseSpell

```lua
C_Spell.GetBaseSpell(spellIdentifier: SpellIdentifier, spec: number) -> baseSpellID: number
```

`SecretArguments=AllowedWhenTainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellIdentifier` | `SpellIdentifier` |  |
| `spec` | `number` | default `0`; Which Class Specialization to consider, as overrides may vary by Spec; Defaults to player's current Spec; `NeverSecret` |

Returns:

| Name | Type | Notes |
|---|---|---|
| `baseSpellID` | `number` | Returns the spellID passed in if there is no override |

### GetDeadlyDebuffInfo

```lua
C_Spell.GetDeadlyDebuffInfo(spellIdentifier: SpellIdentifier) -> deadlyDebuffInfo: DeadlyDebuffInfo
```

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

### GetItemCooldown

```lua
C_Spell.GetItemCooldown(itemID: number) -> spellCooldownInfo: SpellCooldownInfo
```

Returns nil if the item is not found or on cooldown

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

### GetItemModifiedAppearancesApplied

```lua
C_Spell.GetItemModifiedAppearancesApplied(spellID: number) -> itemModifiedAppearanceIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetLastCategoryCooldownSource

```lua
C_Spell.GetLastCategoryCooldownSource(spellCategory: number) -> spellID: number?, itemID: number?
```

Searches for the most recent spellID and itemID that started a cooldown in this category

`SecretArguments=AllowedWhenTainted` `MayReturnNothing` `SecretWhenCooldownsRestricted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `number?` | The most recent spell associated with the category |
| `itemID` | `number?` | The item used to trigger this spell |

### GetMawPowerLinkBySpellID

```lua
C_Spell.GetMawPowerLinkBySpellID(spellID: SpellIdentifier) -> link: cstring
```

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

### GetMawPowerRarityInfoBySpellID

```lua
C_Spell.GetMawPowerRarityInfoBySpellID(spellID: SpellIdentifier) -> rarityID: number, rarityBorderAtlas: textureAtlas
```

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

### GetOverrideSpell

```lua
C_Spell.GetOverrideSpell(spellIdentifier: SpellIdentifier, spec: number, onlyKnown: bool, ignoreOverrideSpellID: number) -> overrideSpellID: number
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellIdentifier` | `SpellIdentifier` |  |
| `spec` | `number` | default `0`; Which Class Specialization to consider, as overrides may vary by Spec; Defaults to player's current Spec |
| `onlyKnown` | `bool` | default `true` |
| `ignoreOverrideSpellID` | `number` | default `0` |

Returns:

| Name | Type | Notes |
|---|---|---|
| `overrideSpellID` | `number` | Returns the spellID passed in if there is no override |

### GetSchoolString

```lua
C_Spell.GetSchoolString(schoolMask: number) -> result: cstring
```

`SecretArguments=AllowedWhenTainted`

### GetSpellAutoCast

```lua
C_Spell.GetSpellAutoCast(spellIdentifier: SpellIdentifier) -> autoCastAllowed: bool, autoCastEnabled: bool
```

Returns nil if spell is not found

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

### GetSpellCastCount

```lua
C_Spell.GetSpellCastCount(spellIdentifier: SpellIdentifier) -> castCount: number
```

Returns number of times a spell can be cast, typically based on availability of things like required reagent items; Returns 0 if spell is not found

`SecretArguments=AllowedWhenTainted` `SecretWhenCooldownsRestricted`

### GetSpellChargeDuration

```lua
C_Spell.GetSpellChargeDuration(spellIdentifier: SpellIdentifier) -> duration: LuaDurationObject
```

Returns a duration object describing the active recharge time for a spell.

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

### GetSpellCharges

```lua
C_Spell.GetSpellCharges(spellIdentifier: SpellIdentifier) -> chargeInfo: SpellChargeInfo
```

Returns a table of info about the charges of a charge-accumulating spell; May return nil if spell is not found or is not charge-based

`SecretArguments=AllowedWhenTainted` `MayReturnNothing` `SecretWhenCooldownsRestricted`

### GetSpellCooldown

```lua
C_Spell.GetSpellCooldown(spellIdentifier: SpellIdentifier) -> spellCooldownInfo: SpellCooldownInfo
```

Returns nil if spell is not found

`SecretArguments=AllowedWhenTainted` `MayReturnNothing` `SecretWhenCooldownsRestricted`

### GetSpellCooldownDuration

```lua
C_Spell.GetSpellCooldownDuration(spellIdentifier: SpellIdentifier, ignoreGCD: bool) -> duration: LuaDurationObject
```

Returns a duration object describing the active cooldown duration for a spell.

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellIdentifier` | `SpellIdentifier` |  |
| `ignoreGCD` | `bool` | default `false` |

### GetSpellDescription

```lua
C_Spell.GetSpellDescription(spellIdentifier: SpellIdentifier) -> description: string
```

Returns nil if spell is not found

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `description` | `string` | May be empty if spell's data isn't loaded yet; Listen for SPELL_TEXT_UPDATE event, or use SpellMixin to load asynchronously |

### GetSpellDescriptionForItemLocation

```lua
C_Spell.GetSpellDescriptionForItemLocation(spellIdentifier: SpellIdentifier, itemLocation: ItemLocation) -> description: string
```

Returns nil if spell is not found

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellIdentifier` | `SpellIdentifier` |  |
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

Returns:

| Name | Type | Notes |
|---|---|---|
| `description` | `string` | May be empty if spell's data isn't loaded yet; Listen for SPELL_TEXT_UPDATE event, or use SpellMixin to load asynchronously |

### GetSpellDisplayCount

```lua
C_Spell.GetSpellDisplayCount(spellIdentifier: SpellIdentifier, maxDisplayCount: number, replacementString: cstring) -> displayCount: string
```

Depending on the spell, return a string that is either the use count or number of charges. If value is beyond the display count parameter, returns the replacementString (defaults to '*').

`SecretArguments=AllowedWhenUntainted` `SecretWhenCooldownsRestricted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellIdentifier` | `SpellIdentifier` |  |
| `maxDisplayCount` | `number` | default `9999` |
| `replacementString` | `cstring` | default `"*"` |

### GetSpellIDForSpellIdentifier

```lua
C_Spell.GetSpellIDForSpellIdentifier(spellIdentifier: SpellIdentifier) -> spellID: number
```

Meant primarily for getting a spell id from a spell name or link; Returns nothing if spell does not exist

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellIdentifier` | `SpellIdentifier` | Spell ID, name, name(subtext), or link; Using name will always check for an override on that spell; If passed a spell ID, will return same id as was passed |

### GetSpellInfo

```lua
C_Spell.GetSpellInfo(spellIdentifier: SpellIdentifier) -> spellInfo: SpellInfo
```

Returns nil if spell is not found

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellIdentifier` | `SpellIdentifier` | Spell ID, name, name(subtext), or link; Using name will always check for an override on that spell |

### GetSpellLevelLearned

```lua
C_Spell.GetSpellLevelLearned(spellIdentifier: SpellIdentifier) -> levelLearned: number
```

Returns the level the spell is learned at; May return a different value if the player is currently Level Linked with another player

`SecretArguments=AllowedWhenTainted`

### GetSpellLink

```lua
C_Spell.GetSpellLink(spellIdentifier: SpellIdentifier, glyphID: number?) -> spellLink: string
```

Returns nil if spell is not found

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellIdentifier` | `SpellIdentifier` |  |
| `glyphID` | `number?` | `NeverSecret` |

### GetSpellLossOfControlCooldownDuration

```lua
C_Spell.GetSpellLossOfControlCooldownDuration(spellIdentifier: SpellIdentifier) -> duration: LuaDurationObject
```

Returns a duration object describing the active loss of control cooldown duration for a spell.

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

### GetSpellLossOfControlCooldownInfo

```lua
C_Spell.GetSpellLossOfControlCooldownInfo(spellIdentifier: SpellIdentifier) -> lossOfControlInfo: SpellLossOfControlInfo
```

Returns nil if spell is not found

`SecretArguments=AllowedWhenTainted` `MayReturnNothing` `SecretWhenCooldownsRestricted`

### GetSpellMaxCumulativeAuraApplications

```lua
C_Spell.GetSpellMaxCumulativeAuraApplications(spellID: SpellIdentifier) -> cumulativeAura: number
```

`SecretArguments=AllowedWhenTainted` `SecretWhenUnitAuraRestricted`

### GetSpellName

```lua
C_Spell.GetSpellName(spellIdentifier: SpellIdentifier) -> name: cstring
```

Returns nil if spell is not found

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

### GetSpellPowerCost

```lua
C_Spell.GetSpellPowerCost(spellIdentifier: SpellIdentifier) -> powerCosts: SpellPowerCostInfo[]
```

Returns a table containing one or more SpellPowerCostInfos, one for each power type this spell costs; May return nil if spell is not found or has no resource costs

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

### GetSpellQueueWindow

```lua
C_Spell.GetSpellQueueWindow() -> result: number
```

### GetSpellSkillLineAbilityRank

```lua
C_Spell.GetSpellSkillLineAbilityRank(spellIdentifier: SpellIdentifier) -> rank: number
```

Returns the rank of a spell that corresponds to an ability within a ranked SkillLine (ex: a crafting Recipe); Returns nil if spell is not found, or isn't part of a ranked SkillLine

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

### GetSpellSubtext

```lua
C_Spell.GetSpellSubtext(spellIdentifier: SpellIdentifier) -> subtext: string
```

Returns nil if spell is not found

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `subtext` | `string` | May be empty if spell's data isn't loaded yet; Listen for SPELL_TEXT_UPDATE event, or use SpellMixin to load asynchronously |

### GetSpellTexture

```lua
C_Spell.GetSpellTexture(spellIdentifier: SpellIdentifier) -> iconID: fileID, originalIconID: fileID, conditionalIconID: fileID?
```

Returns nothing if spell is not found

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

### GetSpellTradeSkillLink

```lua
C_Spell.GetSpellTradeSkillLink(spellIdentifier: SpellIdentifier) -> spellLink: string
```

Returns nil if spell is not associated with a trade skill

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

### GetTargetSpellID

```lua
C_Spell.GetTargetSpellID() -> spellID: number
```

### GetVisibilityInfo

```lua
C_Spell.GetVisibilityInfo(spellID: number, visibilityType: SpellAuraVisibilityType) -> hasCustom: bool, alwaysShowMine: bool, showForMySpec: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### IsActiveSpell

```lua
C_Spell.IsActiveSpell(spellIdentifier: SpellIdentifier, targetUnit: UnitToken?) -> isActiveSpell: bool
```

Returns true if the spell is a currently active toggled spell

`SecretArguments=AllowedWhenTainted` `SecretWhenUnitAuraRestricted` `SecretWhenUnitIdentityRestricted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellIdentifier` | `SpellIdentifier` |  |
| `targetUnit` | `UnitToken?` | Optional specific target; If not supplied, the player will be used, or their pet if the spell is a pet spell |

### IsAutoAttackSpell

```lua
C_Spell.IsAutoAttackSpell(spellIdentifier: SpellIdentifier) -> isAutoAttack: bool
```

Returns true if the spell is the player's melee Auto Attack spell

`SecretArguments=AllowedWhenTainted`

### IsAutoRepeatSpell

```lua
C_Spell.IsAutoRepeatSpell(spellIdentifier: SpellIdentifier) -> isAutoRepeat: bool
```

Returns true if the spell is an auto repeat player spell

`SecretArguments=AllowedWhenTainted`

### IsClassTalentSpell

```lua
C_Spell.IsClassTalentSpell(spellIdentifier: SpellIdentifier) -> isAutoRepeat: bool
```

Returns true if the spell comes from a Class Talent

`SecretArguments=AllowedWhenTainted`

### IsConsumableSpell

```lua
C_Spell.IsConsumableSpell(spellIdentifier: SpellIdentifier) -> consumable: bool
```

`SecretArguments=AllowedWhenTainted`

### IsCurrentSpell

```lua
C_Spell.IsCurrentSpell(spellIdentifier: SpellIdentifier) -> isCurrentSpell: bool
```

Returns true if the spell is currently being cast or is queued to be cast

`SecretArguments=AllowedWhenTainted`

### IsExternalDefensive

```lua
C_Spell.IsExternalDefensive(spellID: number) -> isExternalDefensive: bool
```

Returns true if an aura is considered an external defensive.

`SecretArguments=AllowedWhenUntainted`

### IsPressHoldReleaseSpell

```lua
C_Spell.IsPressHoldReleaseSpell(spellIdentifier: SpellIdentifier) -> isPressHoldRelease: bool
```

Returns true if the spell is an 'empower' type spell that is cast by pressing and holding, with the on-release cast typically being affected by time held

`SecretArguments=AllowedWhenTainted`

### IsPriorityAura

```lua
C_Spell.IsPriorityAura(spellID: number) -> isHighPriority: bool
```

Returns true if an aura is considered high priority and should be ordered ahead of other auras in the UI.

`SecretArguments=AllowedWhenUntainted`

### IsPvPTalentSpell

```lua
C_Spell.IsPvPTalentSpell(spellIdentifier: SpellIdentifier) -> isAutoRepeat: bool
```

Returns true if the spell comes from a PvP Talent

`SecretArguments=AllowedWhenTainted`

### IsRangedAutoAttackSpell

```lua
C_Spell.IsRangedAutoAttackSpell(spellIdentifier: SpellIdentifier) -> isRangedAutoAttack: bool
```

Returns true if the spell is the player's ranged Auto Attack spell (ex: Shoot, Auto Shot, etc)

`SecretArguments=AllowedWhenTainted`

### IsSelfBuff

```lua
C_Spell.IsSelfBuff(spellID: number) -> hasSelfEffectsOnly: bool
```

Returns true if an aura only applies effects to the player, and no other units.

`SecretArguments=AllowedWhenUntainted`

### IsSpellCrowdControl

```lua
C_Spell.IsSpellCrowdControl(spellIdentifier: SpellIdentifier) -> isCrowdControl: bool
```

Returns true if the spell causes a crowd control effect when cast on a valid target.

`SecretArguments=AllowedWhenTainted`

### IsSpellDataCached

```lua
C_Spell.IsSpellDataCached(spellIdentifier: SpellIdentifier) -> isCached: bool
```

Returns true if data for the spell has already been loaded and cached this session

`SecretArguments=AllowedWhenUntainted`

### IsSpellDisabled

```lua
C_Spell.IsSpellDisabled(spellIdentifier: SpellIdentifier) -> disabled: bool
```

`SecretArguments=AllowedWhenTainted`

### IsSpellHarmful

```lua
C_Spell.IsSpellHarmful(spellIdentifier: SpellIdentifier) -> isHarmful: bool
```

Returns true if the spell can be cast on hostile targets

`SecretArguments=AllowedWhenTainted`

### IsSpellHelpful

```lua
C_Spell.IsSpellHelpful(spellIdentifier: SpellIdentifier) -> isHelpful: bool
```

Returns true if the spell can be cast on the player or other friendly targets

`SecretArguments=AllowedWhenTainted`

### IsSpellImportant

```lua
C_Spell.IsSpellImportant(spellIdentifier: SpellIdentifier) -> isImportant: bool
```

Returns true if the spell is considered important. For example a spell that's lethal if not interrupted would be considered important.

`SecretArguments=AllowedWhenTainted`

### IsSpellInRange

```lua
C_Spell.IsSpellInRange(spellIdentifier: SpellIdentifier, targetUnit: UnitToken?) -> inRange: bool?
```

Returns true if the current target is within range of the spell; False if out of range; Nil if range check was invalid

`SecretArguments=AllowedWhenTainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellIdentifier` | `SpellIdentifier` |  |
| `targetUnit` | `UnitToken?` | Optional specific target; If not supplied, player's current target (if any) will be used |

Returns:

| Name | Type | Notes |
|---|---|---|
| `inRange` | `bool?` | May be nil if the range check was invalid, ie due to unknown/invalid spell, missing/invalid target, etc |

### IsSpellPassive

```lua
C_Spell.IsSpellPassive(spellIdentifier: SpellIdentifier) -> isPassive: bool
```

`SecretArguments=AllowedWhenTainted`

### IsSpellUsable

```lua
C_Spell.IsSpellUsable(spellIdentifier: SpellIdentifier) -> isUsable: bool, insufficientPower: bool
```

Returns whether the spell is currently castable; Typically based on things like learned status, required resources, etc

`SecretArguments=AllowedWhenTainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `isUsable` | `bool` |  |
| `insufficientPower` | `bool` | True if spell is specifically unusable due to insufficient power (ie MANA, RAGE, etc) |

### PickupSpell

```lua
C_Spell.PickupSpell(spellIdentifier: SpellIdentifier)
```

`SecretArguments=AllowedWhenUntainted`

### PlaceTargetingSpellAtCursor

```lua
C_Spell.PlaceTargetingSpellAtCursor()
```

`HasRestrictions`

### RequestLoadSpellData

```lua
C_Spell.RequestLoadSpellData(spellIdentifier: SpellIdentifier)
```

Requests data for the spell be loaded; Listen for SPELL_DATA_LOAD_RESULT to be notified when load is finished

`SecretArguments=AllowedWhenUntainted`

### SetSpellAutoCastEnabled

```lua
C_Spell.SetSpellAutoCastEnabled(spellIdentifier: SpellIdentifier, enabled: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SpellHasRange

```lua
C_Spell.SpellHasRange(spellIdentifier: SpellIdentifier) -> hasRange: bool
```

Returns true if the spell has a min and/or max range greater than 0

`SecretArguments=AllowedWhenTainted`

### TargetSpellChecksItemCondition

```lua
C_Spell.TargetSpellChecksItemCondition() -> result: bool
```

### TargetSpellIsEnchanting

```lua
C_Spell.TargetSpellIsEnchanting() -> isEnchanting: bool
```

### TargetSpellJumpsUpgradeTrack

```lua
C_Spell.TargetSpellJumpsUpgradeTrack() -> jumpsUpgradeTrack: bool
```

### TargetSpellReplacesBonusTree

```lua
C_Spell.TargetSpellReplacesBonusTree() -> result: bool
```

### ToggleSpellAutoCast

```lua
C_Spell.ToggleSpellAutoCast(spellIdentifier: SpellIdentifier)
```

Toggles whether spell's autoCast is enabled

`SecretArguments=AllowedWhenUntainted`

## Events

### ENCHANT_SPELL_COMPLETED

```lua
ENCHANT_SPELL_COMPLETED(successful: bool, enchantedItem: ItemLocation?)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `successful` | `bool` |  |
| `enchantedItem` | `ItemLocation?` | `Mixin=ItemLocationMixin` |

### ENCHANT_SPELL_SELECTED

```lua
ENCHANT_SPELL_SELECTED()
```

`SynchronousEvent`

### SPELL_DATA_LOAD_RESULT

```lua
SPELL_DATA_LOAD_RESULT(spellID: number, success: bool)
```

`SynchronousEvent`

### SPELL_RANGE_CHECK_UPDATE

```lua
SPELL_RANGE_CHECK_UPDATE(spellIdentifier: SpellIdentifier, isInRange: bool, checksRange: bool)
```

Used in conjunction with EnableSpellRangeCheck to inform the UI when a spell goes in or out of range with the current target.

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `spellIdentifier` | `SpellIdentifier` |  |
| `isInRange` | `bool` | Whether or not the current target is in range of the spell. Should not be used if the 'checksRange' parameter is false. |
| `checksRange` | `bool` | Can be false if a range check was not made for any reason, for example there is not a current target. |

### SPELL_TEXT_UPDATE

```lua
SPELL_TEXT_UPDATE(spellID: number)
```

`SynchronousEvent`

### UPDATE_SPELL_TARGET_ITEM_CONTEXT

```lua
UPDATE_SPELL_TARGET_ITEM_CONTEXT()
```

`SynchronousEvent`

## Types

### DeadlyDebuffInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `criticalTimeRemainingMs` | `number?` |  |
| `criticalStacks` | `number?` |  |
| `priority` | `number` |  |
| `warningText` | `string` |  |
| `soundKitID` | `number?` |  |

### PowerTypeChange

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `powerType` | `PowerType` |  |
| `amount` | `number` |  |

### SpellInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `iconID` | `fileID` | Icon for this spell; If spell has been overriden, this may be the icon for the overriding spell; See originalIconID for spell's non-overriden icon |
| `originalIconID` | `fileID` |  |
| `castTime` | `number` |  |
| `minRange` | `number` |  |
| `maxRange` | `number` |  |
| `spellID` | `number` |  |
