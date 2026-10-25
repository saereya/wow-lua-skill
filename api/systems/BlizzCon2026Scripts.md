# BlizzCon2026Scripts

Namespace `C_BlizzCon2026` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/blizzcon2026documentation.lua` (FileDataID 8202188)

## Functions

### GetExperience

```lua
C_BlizzCon2026.GetExperience() -> experience: Bc26Experience
```

### IsActive

```lua
C_BlizzCon2026.IsActive() -> isActive: bool
```

### IsColdSwapFeatureEnabled

```lua
C_BlizzCon2026.IsColdSwapFeatureEnabled() -> isEnabled: bool
```

### SetExperience

```lua
C_BlizzCon2026.SetExperience(experience: Bc26Experience)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### BC_26_COLD_SWAP_FEATURE_ENABLED_CHANGED

```lua
BC_26_COLD_SWAP_FEATURE_ENABLED_CHANGED(newEnabled: bool, oldEnabled: bool)
```

`UniqueEvent`

### BC_26_EXPERIENCE_CHANGED

```lua
BC_26_EXPERIENCE_CHANGED(newExperience: Bc26Experience, oldExperience: Bc26Experience)
```

`UniqueEvent`

## Types

### Bc26Experience

*Enumeration* · 2 values, 0..1

Access values as `Enum.Bc26Experience.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Skyborne` | `Bc26Experience` | = 0 |
| `Dungeon` | `Bc26Experience` | = 1 |
