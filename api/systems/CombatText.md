# CombatText

Namespace `C_CombatText` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/combattextdocumentation.lua` (FileDataID 7036079)

## Functions

### GetActiveUnit

```lua
C_CombatText.GetActiveUnit() -> unitTarget: string
```

`MayReturnNothing`

### GetCurrentEventInfo

```lua
C_CombatText.GetCurrentEventInfo()
```

`SecretReturns`

### SetActiveUnit

```lua
C_CombatText.SetActiveUnit(unitToken: UnitToken)
```

`SecretArguments=AllowedWhenUntainted` `RequiresDeclassifiedUnitIdentity`

## Events

### COMBAT_TEXT_UPDATE

```lua
COMBAT_TEXT_UPDATE(combatTextType: cstring)
```

`SynchronousEvent`
