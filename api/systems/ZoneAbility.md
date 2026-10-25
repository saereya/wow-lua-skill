# ZoneAbility

Namespace `C_ZoneAbility` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/zoneabilitydocumentation.lua` (FileDataID 4637309)

## Functions

### GetActiveAbilities

```lua
C_ZoneAbility.GetActiveAbilities() -> zoneAbilities: ZoneAbilityInfo[]
```

### GetZoneAbilityIcon

```lua
C_ZoneAbility.GetZoneAbilityIcon(zoneAbilitySpellID: number) -> zoneAbilityIconID: number?
```

`SecretArguments=AllowedWhenUntainted`

## Types

### ZoneAbilityInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `zoneAbilityID` | `number` |  |
| `uiPriority` | `number` |  |
| `spellID` | `number` |  |
| `textureKit` | `textureKit` |  |
| `tutorialText` | `cstring?` |  |
