# SpellActivationOverlay

Namespace `C_SpellActivationOverlay` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/spellactivationoverlaydocumentation.lua` (FileDataID 4637243)

## Functions

### IsSpellOverlayed

```lua
C_SpellActivationOverlay.IsSpellOverlayed(spellID: number) -> isSpellOverlayed: bool
```

`SecretArguments=AllowedWhenUntainted`

## Events

### SPELL_ACTIVATION_OVERLAY_GLOW_HIDE

```lua
SPELL_ACTIVATION_OVERLAY_GLOW_HIDE(spellID: number)
```

`SynchronousEvent`

### SPELL_ACTIVATION_OVERLAY_GLOW_SHOW

```lua
SPELL_ACTIVATION_OVERLAY_GLOW_SHOW(spellID: number)
```

`SynchronousEvent`

### SPELL_ACTIVATION_OVERLAY_HIDE

```lua
SPELL_ACTIVATION_OVERLAY_HIDE(spellID: number?)
```

`SynchronousEvent`

### SPELL_ACTIVATION_OVERLAY_SHOW

```lua
SPELL_ACTIVATION_OVERLAY_SHOW(spellID: number, overlayFileDataID: number, locationType: ScreenLocationType, scale: number, r: number, g: number, b: number)
```

`SynchronousEvent`
