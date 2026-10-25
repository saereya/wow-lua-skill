# SecretUtil

Namespace `C_Secrets` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/secretpredicateapidocumentation.lua` (FileDataID 7644355)

'How is it a secret if we can C it?'

## Functions

### CanCompareUnitTokens

```lua
C_Secrets.CanCompareUnitTokens(unit1: UnitToken, unit2: UnitToken) -> isUnitComparisonPermitted: bool
```

Returns true if queries to compare two input unit tokens are permitted. If this returns false, APIs guarded by the RequiresComparableUnitTokens predicate will fail.

`SecretArguments=AllowedWhenUntainted`

### GetPowerTypeSecrecy

```lua
C_Secrets.GetPowerTypeSecrecy(powerType: PowerType) -> secrecy: SecrecyLevel
```

Queries the base secrecy for a power type.

`SecretArguments=AllowedWhenUntainted`

### GetSpellAuraSecrecy

```lua
C_Secrets.GetSpellAuraSecrecy(spellIdentifier: SpellIdentifier) -> secrecy: SecrecyLevel
```

Queries the base secrecy for a spell if queried as an aura.

`SecretArguments=AllowedWhenUntainted`

### GetSpellCastSecrecy

```lua
C_Secrets.GetSpellCastSecrecy(spellIdentifier: SpellIdentifier) -> secrecy: SecrecyLevel
```

Queries the base secrecy for a spell if queried as a cast.

`SecretArguments=AllowedWhenUntainted`

### GetSpellCooldownSecrecy

```lua
C_Secrets.GetSpellCooldownSecrecy(spellIdentifier: SpellIdentifier) -> secrecy: SecrecyLevel
```

Queries the base secrecy for a spell if queried as a cooldown.

`SecretArguments=AllowedWhenUntainted`

### HasSecretRestrictions

```lua
C_Secrets.HasSecretRestrictions() -> hasSecretRestrictions: bool
```

Returns true if this client build has secret value restrictions enabled. If false, all APIs that are tagged as potentially returning secrets will never do so.

### ShouldActionCooldownBeSecret

```lua
C_Secrets.ShouldActionCooldownBeSecret(actionID: luaIndex) -> isCooldownSecret: bool
```

Returns true if a given action bar slot ID will produce secret values for cooldowns if queried.

`SecretArguments=AllowedWhenUntainted`

### ShouldAurasBeSecret

```lua
C_Secrets.ShouldAurasBeSecret() -> hasSecretAuras: bool
```

Returns true if queries for aura data will generally produce secret values.

### ShouldCooldownsBeSecret

```lua
C_Secrets.ShouldCooldownsBeSecret() -> hasSecretCooldowns: bool
```

Returns true if queries for cooldown data will generally produce secret values.

### ShouldSpellAuraBeSecret

```lua
C_Secrets.ShouldSpellAuraBeSecret(spellIdentifier: SpellIdentifier) -> isAuraSecret: bool
```

Returns true if a given spell identifier would, if applied as an aura, produce secret values when queried.

`SecretArguments=AllowedWhenUntainted`

### ShouldSpellBookItemCooldownBeSecret

```lua
C_Secrets.ShouldSpellBookItemCooldownBeSecret(spellBookItemSlotIndex: luaIndex, spellBookItemSpellBank: SpellBookSpellBank) -> isCooldownSecret: bool
```

Returns true if a given spellbook item will produce secret values for cooldowns if queried.

`SecretArguments=AllowedWhenUntainted`

### ShouldSpellCooldownBeSecret

```lua
C_Secrets.ShouldSpellCooldownBeSecret(spellIdentifier: SpellIdentifier) -> isCooldownSecret: bool
```

Returns true if a given spell identifier will produce secret values for cooldowns if queried.

`SecretArguments=AllowedWhenUntainted`

### ShouldTotemSlotBeSecret

```lua
C_Secrets.ShouldTotemSlotBeSecret(slot: luaIndex) -> isTotemSecret: bool
```

Returns true if information about a totem slot will produce secret values if queried.

`SecretArguments=AllowedWhenUntainted`

### ShouldTotemSpellBeSecret

```lua
C_Secrets.ShouldTotemSpellBeSecret(spellID: number) -> isTotemSecret: bool
```

Returns true if information about a spell when associated with a totem slot will produce secret values if queried.

`SecretArguments=AllowedWhenUntainted`

### ShouldUnitAuraIndexBeSecret

```lua
C_Secrets.ShouldUnitAuraIndexBeSecret(unit: UnitToken, index: luaIndex, filter: AuraFilters?) -> isAuraSecret: bool
```

Returns true if a given aura index will produce secret values if queried.

`SecretArguments=AllowedWhenUntainted`

### ShouldUnitAuraInstanceBeSecret

```lua
C_Secrets.ShouldUnitAuraInstanceBeSecret(unit: UnitToken, auraInstanceID: number) -> isAuraSecret: bool
```

Returns true if a given aura instance ID will produce secret values if queried.

`SecretArguments=AllowedWhenUntainted`

### ShouldUnitAuraSlotBeSecret

```lua
C_Secrets.ShouldUnitAuraSlotBeSecret(unit: UnitToken, slot: number) -> isAuraSecret: bool
```

Returns true if a given aura slot ID will produce secret values if queried.

`SecretArguments=AllowedWhenUntainted`

### ShouldUnitComparisonBeSecret

```lua
C_Secrets.ShouldUnitComparisonBeSecret(unit1: UnitToken, unit2: UnitToken) -> isUnitComparisonSecret: bool
```

Returns true if queries that compare units will produce secret values.

`SecretArguments=AllowedWhenUntainted`

### ShouldUnitHealthMaxBeSecret

```lua
C_Secrets.ShouldUnitHealthMaxBeSecret(unit: UnitToken) -> isUnitHealthMaxSecret: bool
```

Returns true if queries for maximum unit health will produce secret values.

`SecretArguments=AllowedWhenUntainted`

### ShouldUnitIdentityBeSecret

```lua
C_Secrets.ShouldUnitIdentityBeSecret(unit: UnitToken) -> isUnitIdentitySecret: bool
```

Returns true if queries for unit identity (such as name or GUID) will produce secret values.

`SecretArguments=AllowedWhenUntainted`

### ShouldUnitPowerBeSecret

```lua
C_Secrets.ShouldUnitPowerBeSecret(unit: UnitToken, powerType: PowerType?) -> isUnitPowerSecret: bool
```

Returns true if queries for unit power will produce secret values.

`SecretArguments=AllowedWhenUntainted`

### ShouldUnitPowerMaxBeSecret

```lua
C_Secrets.ShouldUnitPowerMaxBeSecret(unit: UnitToken, powerType: PowerType?) -> isUnitPowerMaxSecret: bool
```

Returns true if queries for maximum unit power will produce secret values.

`SecretArguments=AllowedWhenUntainted`

### ShouldUnitSpellCastBeSecret

```lua
C_Secrets.ShouldUnitSpellCastBeSecret(unit: UnitToken, spellIdentifier: SpellIdentifier) -> isSpellCastSecret: bool
```

Returns true if queries for spell casting information for a unit would produce secret values when queried.

`SecretArguments=AllowedWhenUntainted`

### ShouldUnitSpellCastingBeSecret

```lua
C_Secrets.ShouldUnitSpellCastingBeSecret(unit: UnitToken) -> isSpellCastingSecret: bool
```

Returns true if queries for spell casting information for a specific unit will generally produce secret values.

`SecretArguments=AllowedWhenUntainted`

### ShouldUnitStatsBeSecret

```lua
C_Secrets.ShouldUnitStatsBeSecret() -> hasSecretStats: bool
```

Returns true if queries for unit statistics will produce secret values.

### ShouldUnitThreatStateBeSecret

```lua
C_Secrets.ShouldUnitThreatStateBeSecret(unit: UnitToken, mobUnit: UnitToken?) -> isUnitThreatSecret: bool
```

Returns true if queries for unit threat status will produce secret values.

`SecretArguments=AllowedWhenUntainted`

### ShouldUnitThreatValuesBeSecret

```lua
C_Secrets.ShouldUnitThreatValuesBeSecret(unit: UnitToken, mobUnit: UnitToken) -> isUnitThreatSecret: bool
```

Returns true if queries for unit threat values will produce secret values.

`SecretArguments=AllowedWhenUntainted`
