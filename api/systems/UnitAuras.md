# UnitAuras

Namespace `C_UnitAuras` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/unitauradocumentation.lua` (FileDataID 4637290)

## Functions

### AddAuraSound

```lua
C_UnitAuras.AddAuraSound(trigger: UnitAuraSoundTrigger, sound: UnitAuraSoundInfo) -> auraSoundID: number?
```

Registers a sound for an aura event. The sound is stopped after five seconds of playback. The throttleSeconds value must be between 0 and 5 seconds, inclusive.

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### AddBlockedAura

```lua
C_UnitAuras.AddBlockedAura(unit: UnitTokenRestrictedForAddOns, auraInstanceID: number)
```

`SecretArguments=AllowedWhenUntainted`

### AddPrivateAuraAnchor

```lua
C_UnitAuras.AddPrivateAuraAnchor(args: AddPrivateAuraAnchorArgs) -> anchorID: number?
```

`SecretArguments=AllowedWhenUntainted`

### AuraIsBigDefensive

```lua
C_UnitAuras.AuraIsBigDefensive(spellID: SpellIdentifier) -> isBigDefensive: bool
```

`SecretArguments=AllowedWhenTainted`

### AuraIsPrivate

```lua
C_UnitAuras.AuraIsPrivate(spellID: SpellIdentifier) -> isPrivate: bool
```

`SecretArguments=AllowedWhenTainted`

### CancelAuraByInstanceID

```lua
C_UnitAuras.CancelAuraByInstanceID(unit: UnitTokenRestrictedForAddOns, auraInstanceID: number)
```

`SecretArguments=AllowedWhenUntainted` `RequiresUnitAuraAccess` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unit` | `UnitTokenRestrictedForAddOns` | `NeverSecret` |
| `auraInstanceID` | `number` |  |

### ClearBlockedAuras

```lua
C_UnitAuras.ClearBlockedAuras(unit: UnitTokenRestrictedForAddOns)
```

`SecretArguments=AllowedWhenUntainted`

### DoesAuraHaveExpirationTime

```lua
C_UnitAuras.DoesAuraHaveExpirationTime(auraInstanceUnit: UnitToken, auraInstanceID: number) -> hasExpirationTime: bool
```

Returns true if an aura instance will expire after a certain amount of time.

`SecretArguments=AllowedWhenUntainted` `RequiresUnitAuraAccess` `RequiresValidUnitAuraInstance` `SecretWhenUnitAuraRestricted`

### GetAuraApplicationDisplayCount

```lua
C_UnitAuras.GetAuraApplicationDisplayCount(auraInstanceUnit: UnitToken, auraInstanceID: number, minDisplayCount: number, maxDisplayCount: number?) -> count: string
```

Formats a string for displaying the number of applications an aura has present.

`SecretArguments=AllowedWhenUntainted` `RequiresUnitAuraAccess` `RequiresValidUnitAuraInstance` `SecretWhenUnitAuraRestricted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `auraInstanceUnit` | `UnitToken` |  |
| `auraInstanceID` | `number` |  |
| `minDisplayCount` | `number` | default `2`; Minimum number of applications required; if the application count is below this figure an empty string will be returned.; `NeverSecret` |
| `maxDisplayCount` | `number?` | Maximum number of applications allowed; if the application count is above this figure then the string '*' will be returned.; `NeverSecret` |

### GetAuraBaseDuration

```lua
C_UnitAuras.GetAuraBaseDuration(auraInstanceUnit: UnitToken, auraInstanceID: number, spellID: SpellIdentifier?) -> newDuration: number?
```

Returns the base duration of the given spell (or aura). Takes an optional spellID to use as the new duration if that cannot be derived from the aura, if that value isn't supplied the aura's spellID will be used

`SecretArguments=AllowedWhenTainted` `RequiresUnitAuraAccess` `RequiresValidUnitAuraInstance` `SecretWhenUnitAuraRestricted`

### GetAuraCasterGUID

```lua
C_UnitAuras.GetAuraCasterGUID(auraInstanceUnit: UnitToken, auraInstanceID: number) -> casterGUID: WOWGUID?
```

`SecretArguments=AllowedWhenTainted` `RequiresUnitAuraAccess` `RequiresValidUnitAuraInstance` `SecretWhenUnitAuraRestricted`

### GetAuraDataByAuraInstanceID

```lua
C_UnitAuras.GetAuraDataByAuraInstanceID(unit: UnitTokenRestrictedForAddOns, auraInstanceID: number) -> aura: AuraData?
```

`SecretArguments=AllowedWhenUntainted` `RequiresUnitAuraAccess` `SecretWhenUnitAuraRestricted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unit` | `UnitTokenRestrictedForAddOns` | `NeverSecret` |
| `auraInstanceID` | `number` |  |

### GetAuraDataByIndex

```lua
C_UnitAuras.GetAuraDataByIndex(unit: UnitTokenRestrictedForAddOns, index: luaIndex, filter: AuraFilters?) -> aura: AuraData?
```

`SecretArguments=AllowedWhenUntainted` `RequiresUnitAuraAccess` `SecretWhenUnitAuraRestricted`

### GetAuraDataBySlot

```lua
C_UnitAuras.GetAuraDataBySlot(unit: UnitTokenRestrictedForAddOns, slot: number) -> aura: AuraData?
```

`SecretArguments=AllowedWhenUntainted` `RequiresUnitAuraAccess` `SecretWhenUnitAuraRestricted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unit` | `UnitTokenRestrictedForAddOns` | `NeverSecret` |
| `slot` | `number` |  |

### GetAuraDataBySpellName

```lua
C_UnitAuras.GetAuraDataBySpellName(unit: UnitTokenRestrictedForAddOns, spellName: cstring, filter: AuraFilters?) -> aura: AuraData?
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitAuraRestricted` `RequiresNonSecretAura`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unit` | `UnitTokenRestrictedForAddOns` | `NeverSecret` |
| `spellName` | `cstring` |  |
| `filter` | `AuraFilters?` |  |

### GetAuraDispelTypeColor

```lua
C_UnitAuras.GetAuraDispelTypeColor(auraInstanceUnit: UnitToken, auraInstanceID: number, curve: LuaColorCurveObject) -> dispelTypeColor: colorRGBA
```

Queries the dispel type associated with an aura instance and remaps it to a color via a curve, with the dispel type ID used as the 'x' value.

`SecretArguments=AllowedWhenUntainted` `RequiresUnitAuraAccess` `RequiresValidUnitAuraInstance` `SecretWhenUnitAuraRestricted` `SecretWhenCurveSecret`

Returns:

| Name | Type | Notes |
|---|---|---|
| `dispelTypeColor` | `colorRGBA` | `Mixin=ColorMixin` |

### GetAuraDuration

```lua
C_UnitAuras.GetAuraDuration(auraInstanceUnit: UnitToken, auraInstanceID: number) -> duration: LuaDurationObject
```

`SecretArguments=AllowedWhenUntainted` `RequiresUnitAuraAccess` `RequiresValidUnitAuraInstance`

### GetAuraSlots

```lua
C_UnitAuras.GetAuraSlots(unit: UnitTokenRestrictedForAddOns, filter: AuraFilters?, maxSlots: number?, continuationToken: number?) -> outContinuationToken: number?, slots: number
```

`SecretArguments=AllowedWhenUntainted` `RequiresUnitAuraAccess`

Returns:

| Name | Type | Notes |
|---|---|---|
| `outContinuationToken` | `number?` |  |
| `slots` | `number` | `StrideIndex=1` |

### GetBuffDataByIndex

```lua
C_UnitAuras.GetBuffDataByIndex(unit: UnitTokenRestrictedForAddOns, index: luaIndex, filter: AuraFilters?) -> aura: AuraData?
```

`SecretArguments=AllowedWhenUntainted` `RequiresUnitAuraAccess` `SecretWhenUnitAuraRestricted`

### GetCooldownAuraBySpellID

```lua
C_UnitAuras.GetCooldownAuraBySpellID(spellID: SpellIdentifier) -> cooldownSpellID: number?
```

`SecretArguments=AllowedWhenTainted`

### GetDebuffDataByIndex

```lua
C_UnitAuras.GetDebuffDataByIndex(unit: UnitTokenRestrictedForAddOns, index: luaIndex, filter: AuraFilters?) -> aura: AuraData?
```

`SecretArguments=AllowedWhenUntainted` `RequiresUnitAuraAccess` `SecretWhenUnitAuraRestricted`

### GetGroupBuffVisualAlerts

```lua
C_UnitAuras.GetGroupBuffVisualAlerts() -> visualAlerts: GroupBuffVisualAlertInfo[]
```

Returns the alerts passed to SetGroupBuffVisualAlerts plus an entry for every linked rank spell of those group buffs.

### GetHiddenGroupBuffs

```lua
C_UnitAuras.GetHiddenGroupBuffs() -> spellIDs: number[]
```

Returns the spell IDs passed to SetHiddenGroupBuffs plus every linked rank spell of those group buffs.

### GetPlayerAuraBySpellID

```lua
C_UnitAuras.GetPlayerAuraBySpellID(spellID: SpellIdentifier) -> aura: AuraData?
```

`SecretArguments=AllowedWhenTainted` `SecretWhenUnitAuraRestricted` `RequiresNonSecretAura`

### GetRefreshCarryOverDuration

```lua
C_UnitAuras.GetRefreshCarryOverDuration(auraInstanceUnit: UnitToken, auraInstanceID: number, spellID: SpellIdentifier?) -> newDuration: number?
```

Returns the client-predicted amount of time that a new spellcast of the same spell would carry over to the new application of that aura. Takes an optional spellID to use as the new duration if that cannot be derived from the aura, if that value isn't supplied the aura's spellID will be used

`SecretArguments=AllowedWhenTainted` `RequiresUnitAuraAccess` `RequiresValidUnitAuraInstance` `SecretWhenUnitAuraRestricted`

### GetRefreshExtendedDuration

```lua
C_UnitAuras.GetRefreshExtendedDuration(auraInstanceUnit: UnitToken, auraInstanceID: number, spellID: SpellIdentifier?) -> newDuration: number?
```

Returns the client-predicted new duration of this aura if it were cast again right now. Takes an optional spellID to use as the new duration if that cannot be derived from the aura, if that value isn't supplied the aura's spellID will be used

`SecretArguments=AllowedWhenTainted` `RequiresUnitAuraAccess` `RequiresValidUnitAuraInstance` `SecretWhenUnitAuraRestricted`

### GetUnitAuraBySpellID

```lua
C_UnitAuras.GetUnitAuraBySpellID(unit: UnitTokenRestrictedForAddOns, spellID: SpellIdentifier) -> aura: AuraData?
```

Returns the first instance of an aura on a unit matching a given spell ID. Returns nil if no such aura is found. Additionally can return nil if querying a unit that is not visible (eg. party members on other maps).

`SecretArguments=AllowedWhenTainted` `SecretWhenUnitAuraRestricted` `RequiresNonSecretAura`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unit` | `UnitTokenRestrictedForAddOns` | `NeverSecret` |
| `spellID` | `SpellIdentifier` |  |

### GetUnitAuraInstanceIDs

```lua
C_UnitAuras.GetUnitAuraInstanceIDs(unit: UnitTokenRestrictedForAddOns, filter: AuraFilters, maxCount: number?, sortRule: UnitAuraSortRule, sortDirection: UnitAuraSortDirection) -> auraInstanceIDs: number[]
```

`SecretArguments=AllowedWhenUntainted` `RequiresUnitAuraAccess`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unit` | `UnitTokenRestrictedForAddOns` | `NeverSecret` |
| `filter` | `AuraFilters` |  |
| `maxCount` | `number?` |  |
| `sortRule` | `UnitAuraSortRule` | default `"Unsorted"` |
| `sortDirection` | `UnitAuraSortDirection` | default `"Normal"` |

### GetUnitAuras

```lua
C_UnitAuras.GetUnitAuras(unit: UnitTokenRestrictedForAddOns, filter: AuraFilters, maxCount: number?, sortRule: UnitAuraSortRule, sortDirection: UnitAuraSortDirection) -> auras: AuraData[]
```

`SecretArguments=AllowedWhenUntainted` `RequiresUnitAuraAccess`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unit` | `UnitTokenRestrictedForAddOns` | `NeverSecret` |
| `filter` | `AuraFilters` |  |
| `maxCount` | `number?` |  |
| `sortRule` | `UnitAuraSortRule` | default `"Unsorted"` |
| `sortDirection` | `UnitAuraSortDirection` | default `"Normal"` |

Returns:

| Name | Type | Notes |
|---|---|---|
| `auras` | `AuraData[]` | `ConditionalSecretContents` |

### IsAuraFilteredOutByInstanceID

```lua
C_UnitAuras.IsAuraFilteredOutByInstanceID(unit: UnitTokenRestrictedForAddOns, auraInstanceID: number, filter: AuraFilters) -> isFiltered: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresUnitAuraAccess`

### RemoveAuraSound

```lua
C_UnitAuras.RemoveAuraSound(auraSoundID: number)
```

`SecretArguments=AllowedWhenUntainted`

### RemovePrivateAuraAnchor

```lua
C_UnitAuras.RemovePrivateAuraAnchor(anchorID: number)
```

`SecretArguments=AllowedWhenUntainted`

### ResetAuraDataProvider

```lua
C_UnitAuras.ResetAuraDataProvider()
```

### SetGroupBuffVisualAlerts

```lua
C_UnitAuras.SetGroupBuffVisualAlerts(visualAlerts: GroupBuffVisualAlertInfo[])
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `visualAlerts` | `GroupBuffVisualAlertInfo[]` | `NeverSecretContents` |

### SetHiddenGroupBuffs

```lua
C_UnitAuras.SetHiddenGroupBuffs(spellIDs: number[])
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellIDs` | `number[]` | `NeverSecretContents` |

### SetPrivateWarningTextAnchor

```lua
C_UnitAuras.SetPrivateWarningTextAnchor(parent: SimpleFrame, anchor: AnchorBinding?)
```

`SecretArguments=AllowedWhenUntainted`

### SwitchAuraDataProvider

```lua
C_UnitAuras.SwitchAuraDataProvider()
```

### WantsAlteredForm

```lua
C_UnitAuras.WantsAlteredForm(unit: UnitToken) -> wantsAlteredForm: bool
```

`SecretArguments=AllowedWhenUntainted`

## Events

### AURA_DATA_PROVIDER_SWITCH

```lua
AURA_DATA_PROVIDER_SWITCH(useRealDataProvider: bool)
```

`SynchronousEvent`

### GROUP_BUFF_VISUAL_ALERTS_CHANGED

```lua
GROUP_BUFF_VISUAL_ALERTS_CHANGED(visualAlerts: GroupBuffVisualAlertInfo[])
```

The payload matches GetGroupBuffVisualAlerts, including linked rank spells.

`SynchronousEvent`

### HIDDEN_GROUP_BUFFS_CHANGED

```lua
HIDDEN_GROUP_BUFFS_CHANGED(spellIDs: number[])
```

The payload matches GetHiddenGroupBuffs, including linked rank spells.

`SynchronousEvent`

### UNIT_AURA

```lua
UNIT_AURA(unitTarget: UnitTokenVariant, updateInfo: UnitAuraUpdateInfo)
```

`SecretWhenAurasRestricted` `SynchronousEvent`

### UNIT_AURA_BLOCKED

```lua
UNIT_AURA_BLOCKED(unitTarget: UnitTokenVariant, auraInstanceID: number)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `unitTarget` | `UnitTokenVariant` |  |
| `auraInstanceID` | `number` | `SecretValue` |

### UNIT_AURA_BLOCK_LIST_CLEARED

```lua
UNIT_AURA_BLOCK_LIST_CLEARED(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`
