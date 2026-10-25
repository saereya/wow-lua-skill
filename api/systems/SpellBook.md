# SpellBook

Namespace `C_SpellBook` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/spellbookdocumentation.lua` (FileDataID 4637245)

## Functions

### AbortSpellIntro

```lua
C_SpellBook.AbortSpellIntro(spellID: number)
```

`SecretArguments=AllowedWhenUntainted`

### CastSpellBookItem

```lua
C_SpellBook.CastSpellBookItem(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank, targetSelf: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellBookItemSlotIndex` | `luaIndex` |  |
| `spellBookItemSpellBank` | `SpellBookSpellBank` |  |
| `targetSelf` | `bool` | default `false`; If true, spell will target the current player; Otherwise, targets the player's current target |

### ContainsAnyDisenchantSpell

```lua
C_SpellBook.ContainsAnyDisenchantSpell() -> contains: bool
```

Returns true if player knows any Disenchant spells

### FindBaseSpellByID

```lua
C_SpellBook.FindBaseSpellByID(spellID: number) -> baseSpellID: number?
```

`SecretArguments=AllowedWhenUntainted`

### FindFlyoutSlotBySpellID

```lua
C_SpellBook.FindFlyoutSlotBySpellID(spellID: number) -> flyoutSlot: luaIndex
```

`SecretArguments=AllowedWhenUntainted`

### FindSpellBookSlotForSpell

```lua
C_SpellBook.FindSpellBookSlotForSpell(spellIdentifier: SpellIdentifier, includeHidden: bool, includeFlyouts: bool, includeFutureSpells: bool, includeOffSpec: bool) -> spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank
```

If found, returns the first slot position of a SpellBookItem matching the specified spell and criteria

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellIdentifier` | `SpellIdentifier` |  |
| `includeHidden` | `bool` | default `false`; If true, search includes SpellBookItems that are hidden from the SpellBook UI (ex: spells that have been replaced, are also in a Flyout, etc) |
| `includeFlyouts` | `bool` | default `true`; If true, search includes Flyout SpellBookItems containing the specified spell |
| `includeFutureSpells` | `bool` | default `false`; If true, search includes SpellBookItems for spells that have not yet been learned |
| `includeOffSpec` | `bool` | default `false`; If true, search includes SpellBookItems belonging to non-active specializations; If spell is in active and inactive spec, the active spec slot will always be returned |

### FindSpellOverrideByID

```lua
C_SpellBook.FindSpellOverrideByID(spellID: number) -> overrideSpellID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetClassSkillLineInfo

```lua
C_SpellBook.GetClassSkillLineInfo() -> skillLineInfo: SpellBookSkillLineInfo
```

`MayReturnNothing`

### GetCurrentLevelSpells

```lua
C_SpellBook.GetCurrentLevelSpells(level: number) -> spellIDs: number[]
```

Returns general, class, and active spec spells that are learned at the specified level

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetNumSpellBookSkillLines

```lua
C_SpellBook.GetNumSpellBookSkillLines() -> numSpellBookSkillLines: number
```

### GetSkillLineIndexByID

```lua
C_SpellBook.GetSkillLineIndexByID(skillLineID: number) -> skillIndex: luaIndex?
```

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `skillIndex` | `luaIndex?` | Will be nil if the specified SkillLine could not be found, or if it is not one of the player's tracked skill lines |

### GetSpellBookItemAutoCast

```lua
C_SpellBook.GetSpellBookItemAutoCast(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> autoCastAllowed: bool, autoCastEnabled: bool
```

Returns nothing if item doesn't exist or isn't a spell

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `autoCastAllowed` | `bool` | True if this spell is allowed to be auto-cast |
| `autoCastEnabled` | `bool` | True if auto-casting this spell is currently enabled (usually by the player) |

### GetSpellBookItemCastCount

```lua
C_SpellBook.GetSpellBookItemCastCount(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> castCount: number
```

Returns number of times a SpellBookItem can be cast, typically based on availability of things like required reagent items; Always returns 0 if item is not found or is not a spell

`SecretArguments=AllowedWhenUntainted` `SecretWhenCooldownsRestricted`

### GetSpellBookItemChargeDuration

```lua
C_SpellBook.GetSpellBookItemChargeDuration(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> duration: LuaDurationObject
```

Returns a duration object describing the active recharge time for a spellbook item.

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSpellBookItemCharges

```lua
C_SpellBook.GetSpellBookItemCharges(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> chargeInfo: SpellChargeInfo
```

Returns a table of info about the charges of a charge-accumulating SpellBookItem; May return nil if item is not found or is not charge-based

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretWhenCooldownsRestricted`

### GetSpellBookItemCooldown

```lua
C_SpellBook.GetSpellBookItemCooldown(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> spellCooldownInfo: SpellCooldownInfo
```

Returns nil if item doesn't exist or if this kind of item doesn't display cooldowns (ex: future or offspec spells)

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretWhenCooldownsRestricted`

### GetSpellBookItemCooldownDuration

```lua
C_SpellBook.GetSpellBookItemCooldownDuration(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank, ignoreGCD: bool) -> duration: LuaDurationObject
```

Returns a duration object describing the active cooldown duration for a spellbook item.

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellBookItemSlotIndex` | `luaIndex` |  |
| `spellBookItemSpellBank` | `SpellBookSpellBank` |  |
| `ignoreGCD` | `bool` | default `false` |

### GetSpellBookItemDescription

```lua
C_SpellBook.GetSpellBookItemDescription(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> description: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `description` | `string` | May be empty if spell's data isn't loaded yet; Listen for SPELL_TEXT_UPDATE event, or use SpellMixin to load asynchronously |

### GetSpellBookItemInfo

```lua
C_SpellBook.GetSpellBookItemInfo(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> spellBookItemInfo: SpellBookItemInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSpellBookItemLevelLearned

```lua
C_SpellBook.GetSpellBookItemLevelLearned(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> levelLearned: number
```

Returns the level the spell is learned at; May return a different value if the player is currently Level Linked with another player; Returns 0 if item is not a Spell

`SecretArguments=AllowedWhenUntainted`

### GetSpellBookItemLink

```lua
C_SpellBook.GetSpellBookItemLink(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank, glyphID: number?) -> spellLink: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSpellBookItemLossOfControlCooldownDuration

```lua
C_SpellBook.GetSpellBookItemLossOfControlCooldownDuration(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> duration: LuaDurationObject
```

Returns a duration object describing the active loss of control cooldown duration for a spellbook item.

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSpellBookItemLossOfControlCooldownInfo

```lua
C_SpellBook.GetSpellBookItemLossOfControlCooldownInfo(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> lossOfControlInfo: SpellLossOfControlInfo
```

Returns nil if item doesn't exist or if this kind of item doesn't display cooldowns (ex: future or offspec spells)

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretWhenCooldownsRestricted`

### GetSpellBookItemName

```lua
C_SpellBook.GetSpellBookItemName(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> name: string, subName: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `subName` | `string` | May be empty if spell's data isn't loaded yet; Listen for SPELL_TEXT_UPDATE event, or use SpellMixin to load asynchronously |

### GetSpellBookItemPowerCost

```lua
C_SpellBook.GetSpellBookItemPowerCost(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> powerCosts: SpellPowerCostInfo[]
```

Returns a table containing one or more SpellPowerCostInfos, one for each power type a SpellBookItem costs; May return nil if item is not found or has no resource costs

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSpellBookItemSkillLineIndex

```lua
C_SpellBook.GetSpellBookItemSkillLineIndex(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> skillLineIndex: luaIndex?
```

Get the index of the SkillLine this SpellBookItem is part of

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `skillLineIndex` | `luaIndex?` | Will be nil if the specified SpellBookItem doesn't exist or isn't part of a SkillLine |

### GetSpellBookItemTexture

```lua
C_SpellBook.GetSpellBookItemTexture(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> iconID: fileID
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSpellBookItemTradeSkillLink

```lua
C_SpellBook.GetSpellBookItemTradeSkillLink(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> spellLink: string
```

Returns nil if SpellBookItem is not associated with a trade skill

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSpellBookItemType

```lua
C_SpellBook.GetSpellBookItemType(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> itemType: SpellBookItemType, actionID: number, spellID: number?
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `itemType` | `SpellBookItemType` |  |
| `actionID` | `number` | Represents a base spellID for spells, flyoutID for flyouts, or petActionID for pet actions |
| `spellID` | `number?` | May be nil if item is not a spell; Will be the overriding spellID if spell is overriden, otherwise will match actionID |

### GetSpellBookSkillLineInfo

```lua
C_SpellBook.GetSpellBookSkillLineInfo(skillLineIndex: luaIndex) -> skillLineInfo: SpellBookSkillLineInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### HasPetSpells

```lua
C_SpellBook.HasPetSpells() -> numPetSpells: number, petNameToken: string
```

Returns nothing if player has no pet spells

`MayReturnNothing`

### IsAutoAttackSpellBookItem

```lua
C_SpellBook.IsAutoAttackSpellBookItem(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> isAutoAttack: bool
```

Returns true if the SpellBookItem is the player's melee Auto Attack spell

`SecretArguments=AllowedWhenUntainted`

### IsClassTalentSpellBookItem

```lua
C_SpellBook.IsClassTalentSpellBookItem(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> isClassTalent: bool
```

Returns true if the SpellBookItem comes from a Class Talent

`SecretArguments=AllowedWhenUntainted`

### IsPvPTalentSpellBookItem

```lua
C_SpellBook.IsPvPTalentSpellBookItem(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> isPvPTalent: bool
```

Returns true if the SpellBookItem comes from a PvP Talent

`SecretArguments=AllowedWhenUntainted`

### IsRangedAutoAttackSpellBookItem

```lua
C_SpellBook.IsRangedAutoAttackSpellBookItem(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> isRangedAutoAttack: bool
```

Returns true if the SpellBookItem is the player's ranged Auto Attack spell (ex: Shoot, Auto Shot, etc)

`SecretArguments=AllowedWhenUntainted`

### IsSpellBookItemHarmful

```lua
C_SpellBook.IsSpellBookItemHarmful(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> isHarmful: bool
```

Returns true if the SpellBookIem can be cast on hostile targets

`SecretArguments=AllowedWhenUntainted`

### IsSpellBookItemHelpful

```lua
C_SpellBook.IsSpellBookItemHelpful(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> isHelpful: bool
```

Returns true if the SpellBookIem can be cast on the player or other friendly targets

`SecretArguments=AllowedWhenUntainted`

### IsSpellBookItemInRange

```lua
C_SpellBook.IsSpellBookItemInRange(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank, targetUnit: UnitToken?) -> inRange: bool?
```

Returns true if the current target is within range of the SpellBookIem; False if out of range; Nil if range check was invalid

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellBookItemSlotIndex` | `luaIndex` |  |
| `spellBookItemSpellBank` | `SpellBookSpellBank` |  |
| `targetUnit` | `UnitToken?` | Optional specific target; If not supplied, player's current target (if any) will be used |

Returns:

| Name | Type | Notes |
|---|---|---|
| `inRange` | `bool?` | May be nil if the range check was invalid, ie due to unknown/invalid spell, missing/invalid target, etc |

### IsSpellBookItemLooseFlyoutMember

```lua
C_SpellBook.IsSpellBookItemLooseFlyoutMember(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> isFlyoutMember: bool
```

Returns true if the SpellBookItem is represented in a Flyout.

`SecretArguments=AllowedWhenUntainted`

### IsSpellBookItemLowRank

```lua
C_SpellBook.IsSpellBookItemLowRank(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> isLowRank: bool
```

Returns true if the SpellBookItem is a lower rank of a known higher rank spell.  Returns false if there is only a single rank or it is the highest rank known.

`SecretArguments=AllowedWhenUntainted`

### IsSpellBookItemOffSpec

```lua
C_SpellBook.IsSpellBookItemOffSpec(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> isOffSpec: bool
```

Returns true if the SpellBookItem belongs to a non-active class specialization

`SecretArguments=AllowedWhenUntainted`

### IsSpellBookItemPassive

```lua
C_SpellBook.IsSpellBookItemPassive(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> isPassive: bool
```

Returns true if the SpellBookItem is a passive spell; Will always return false if it is not a spell

`SecretArguments=AllowedWhenUntainted`

### IsSpellBookItemUsable

```lua
C_SpellBook.IsSpellBookItemUsable(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> isUsable: bool, insufficientPower: bool
```

Returns whether the SpellBookIem is currently castable; Typically based on things like learned status, required resources, etc

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `isUsable` | `bool` |  |
| `insufficientPower` | `bool` | True if SpellBookIem is specifically unusable due to insufficient power (ie MANA, RAGE, etc) |

### IsSpellInSpellBook

```lua
C_SpellBook.IsSpellInSpellBook(spellID: number, spellBank: SpellBookSpellBank, includeOverrides: bool) -> isInSpellBook: bool
```

Returns true if a spell should be found in the spellbook. This function can also return true for spells that aren't known, such as override spells granted by an aura linked to class talents

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `number` |  |
| `spellBank` | `SpellBookSpellBank` | default `"Player"` |
| `includeOverrides` | `bool` | default `true` |

### IsSpellKnown

```lua
C_SpellBook.IsSpellKnown(spellID: number, spellBank: SpellBookSpellBank) -> isKnown: bool
```

Returns true if a player knows a spell. This function can also return true for spells that aren't in the spellbook, such as temporarily-granted abilities

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `number` |  |
| `spellBank` | `SpellBookSpellBank` | default `"Player"` |

### IsSpellKnownOrInSpellBook

```lua
C_SpellBook.IsSpellKnownOrInSpellBook(spellID: number, spellBank: SpellBookSpellBank, includeOverrides: bool) -> isKnownOrInSpellBook: bool
```

Returns true if a spell is considered to be known or present in the spellbook

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `number` |  |
| `spellBank` | `SpellBookSpellBank` | default `"Player"` |
| `includeOverrides` | `bool` | default `true` |

### PickupSpellBookItem

```lua
C_SpellBook.PickupSpellBookItem(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank)
```

`SecretArguments=AllowedWhenUntainted`

### SetBarSlotFromIntro

```lua
C_SpellBook.SetBarSlotFromIntro(spellID: number, slotIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### SetSpellBookItemAutoCastEnabled

```lua
C_SpellBook.SetSpellBookItemAutoCastEnabled(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank, enabled: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SpellBookItemHasRange

```lua
C_SpellBook.SpellBookItemHasRange(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> hasRange: bool
```

Returns true if the SpellBookIem has a min and/or max range greater than 0; Will always return false if it is not a spell

`SecretArguments=AllowedWhenUntainted`

### ToggleSpellBookItemAutoCast

```lua
C_SpellBook.ToggleSpellBookItemAutoCast(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### CURRENT_SPELL_CAST_CHANGED

```lua
CURRENT_SPELL_CAST_CHANGED(cancelledCast: bool)
```

`SynchronousEvent`

### LEARNED_SPELL_IN_SKILL_LINE

```lua
LEARNED_SPELL_IN_SKILL_LINE(spellID: number, skillLineIndex: luaIndex, isGuildPerkSpell: bool)
```

`SynchronousEvent`

### MAX_SPELL_START_RECOVERY_OFFSET_CHANGED

```lua
MAX_SPELL_START_RECOVERY_OFFSET_CHANGED(clampedNewQueueWindowMs: number)
```

`SynchronousEvent`

### PLAYER_TOTEM_UPDATE

```lua
PLAYER_TOTEM_UPDATE(totemSlot: luaIndex)
```

`SynchronousEvent`

### SPELL_FLYOUT_UPDATE

```lua
SPELL_FLYOUT_UPDATE(flyoutID: number?, spellID: number?, isLearned: bool?)
```

`SynchronousEvent` `UniqueEvent`

### SPELL_PUSHED_TO_ACTIONBAR

```lua
SPELL_PUSHED_TO_ACTIONBAR(spellID: number, slot: luaIndex, page: luaIndex)
```

`SynchronousEvent`

### SPELL_PUSHED_TO_FLYOUT_ON_ACTIONBAR

```lua
SPELL_PUSHED_TO_FLYOUT_ON_ACTIONBAR(spellID: number, flyoutSlot: luaIndex, flyoutPage: luaIndex)
```

`SynchronousEvent`

### SPELLS_CHANGED

```lua
SPELLS_CHANGED()
```

`UniqueEvent`

### SPELL_UPDATE_CHARGES

```lua
SPELL_UPDATE_CHARGES()
```

`SynchronousEvent` `UniqueEvent`

### SPELL_UPDATE_COOLDOWN

```lua
SPELL_UPDATE_COOLDOWN(spellID: number?, baseSpellID: number?, category: number?, startRecoveryCategory: number?, itemID: number?)
```

`UniqueEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `number?` | Can be a base spell or an override spell. A nil value indicates that all cooldowns should be updated, rather than just a specific one. |
| `baseSpellID` | `number?` | Will be set to the base spell if the spellID parameter is an override spell. |
| `category` | `number?` | If the spellID parameter is set, the cooldown category of the spell. A nil value indicates the spell does not have a cooldown category. |
| `startRecoveryCategory` | `number?` | If the spellID parameter is set, the cooldown start recovery category of the spell. A nil value indicates the spell does not have a cooldown start recovery category. |
| `itemID` | `number?` | If the itemID parameter is set, it's the itemID associated with the cast of the spell. |

### SPELL_UPDATE_ICON

```lua
SPELL_UPDATE_ICON(spellID: number?)
```

`UniqueEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `number?` | Always refers to the base spell. A nil value indicates that all icons should be updated, rather than just a specific one. |

### SPELL_UPDATE_USABLE

```lua
SPELL_UPDATE_USABLE()
```

`UniqueEvent`

### SPELL_UPDATE_USES

```lua
SPELL_UPDATE_USES(spellID: number, baseSpellID: number?)
```

`UniqueEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `number` | Can be a base spell or override spell. |
| `baseSpellID` | `number?` | Will be set to the base spell if the spellID parameter is an override spell. |

### START_AUTOREPEAT_SPELL

```lua
START_AUTOREPEAT_SPELL()
```

`SynchronousEvent`

### STOP_AUTOREPEAT_SPELL

```lua
STOP_AUTOREPEAT_SPELL()
```

`SynchronousEvent`

### UPDATE_SHAPESHIFT_COOLDOWN

```lua
UPDATE_SHAPESHIFT_COOLDOWN()
```

`UniqueEvent`

### UPDATE_SHAPESHIFT_FORM

```lua
UPDATE_SHAPESHIFT_FORM()
```

`SynchronousEvent`

### UPDATE_SHAPESHIFT_FORMS

```lua
UPDATE_SHAPESHIFT_FORMS()
```

`UniqueEvent`

### UPDATE_SHAPESHIFT_USABLE

```lua
UPDATE_SHAPESHIFT_USABLE()
```

`UniqueEvent`

## Types

### SpellBookItemInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `actionID` | `number` | Represents a base spellID for spells, flyoutID for flyouts, or petActionID for pet actions |
| `spellID` | `number?` | May be nil if item is not a spell; Will be the overriding spellID if spell is overriden, otherwise will match actionID |
| `itemType` | `SpellBookItemType` |  |
| `name` | `string` |  |
| `subName` | `string` | May be empty if flyout, or if spell's data isn't loaded yet; Listen for SPELL_TEXT_UPDATE event, or use SpellMixin to load asynchronously |
| `iconID` | `fileID` |  |
| `isPassive` | `bool` | True if the item is a passive spell; Will always be false if it is not a spell |
| `isOffSpec` | `bool` | True if the item belongs to a non-active specialization |
| `skillLineIndex` | `luaIndex?` | Index of the SkillLine this SpellBookItem is part of; Nil this SpellBookItem isn't part of a SkillLine |

### SpellBookSkillLineInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `iconID` | `fileID` |  |
| `itemIndexOffset` | `number` | This value + 1 is the first Spell Book Item slotIndex within this skill line |
| `numSpellBookItems` | `number` |  |
| `isGuild` | `bool` |  |
| `shouldHide` | `bool` |  |
| `specID` | `number?` | Will be nil if this skill line is not associated with a specialization |
| `offSpecID` | `number?` | Will be nil if this skill line is not associated with a non-active specialization |
