# BattlePet

Namespace `C_BattlePet` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/battlepetdocumentation.lua` (FileDataID 4637034)

## Events

### PET_BATTLE_ABILITY_CHANGED

```lua
PET_BATTLE_ABILITY_CHANGED(owner: number, petIndex: number, abilityID: number)
```

`SynchronousEvent`

### PET_BATTLE_ACTION_SELECTED

```lua
PET_BATTLE_ACTION_SELECTED()
```

`SynchronousEvent`

### PET_BATTLE_AURA_APPLIED

```lua
PET_BATTLE_AURA_APPLIED(owner: number, petIndex: number, auraInstanceID: number)
```

`SynchronousEvent`

### PET_BATTLE_AURA_CANCELED

```lua
PET_BATTLE_AURA_CANCELED(owner: number, petIndex: number, auraInstanceID: number)
```

`SynchronousEvent`

### PET_BATTLE_AURA_CHANGED

```lua
PET_BATTLE_AURA_CHANGED(owner: number, petIndex: number, auraInstanceID: number)
```

`SynchronousEvent`

### PET_BATTLE_CAPTURED

```lua
PET_BATTLE_CAPTURED(owner: number, petIndex: number)
```

`SynchronousEvent`

### PET_BATTLE_CLOSE

```lua
PET_BATTLE_CLOSE()
```

`SynchronousEvent`

### PET_BATTLE_FINAL_ROUND

```lua
PET_BATTLE_FINAL_ROUND(owner: number)
```

`SynchronousEvent`

### PET_BATTLE_HEALTH_CHANGED

```lua
PET_BATTLE_HEALTH_CHANGED(owner: number, petIndex: number, healthChange: number)
```

`SynchronousEvent`

### PET_BATTLE_LEVEL_CHANGED

```lua
PET_BATTLE_LEVEL_CHANGED(owner: number, petIndex: number, newLevel: number)
```

`SynchronousEvent`

### PET_BATTLE_MAX_HEALTH_CHANGED

```lua
PET_BATTLE_MAX_HEALTH_CHANGED(owner: number, petIndex: number, healthChange: number)
```

`SynchronousEvent`

### PET_BATTLE_OPENING_DONE

```lua
PET_BATTLE_OPENING_DONE()
```

`SynchronousEvent`

### PET_BATTLE_OPENING_START

```lua
PET_BATTLE_OPENING_START()
```

`SynchronousEvent`

### PET_BATTLE_OVER

```lua
PET_BATTLE_OVER()
```

`SynchronousEvent`

### PET_BATTLE_OVERRIDE_ABILITY

```lua
PET_BATTLE_OVERRIDE_ABILITY(abilityIndex: number)
```

`SynchronousEvent`

### PET_BATTLE_PET_CHANGED

```lua
PET_BATTLE_PET_CHANGED(owner: number)
```

`SynchronousEvent`

### PET_BATTLE_PET_ROUND_PLAYBACK_COMPLETE

```lua
PET_BATTLE_PET_ROUND_PLAYBACK_COMPLETE(roundNumber: number)
```

`SynchronousEvent`

### PET_BATTLE_PET_ROUND_RESULTS

```lua
PET_BATTLE_PET_ROUND_RESULTS(roundNumber: number)
```

`SynchronousEvent`

### PET_BATTLE_PET_TYPE_CHANGED

```lua
PET_BATTLE_PET_TYPE_CHANGED(owner: number, petIndex: number, stateValue: number)
```

`SynchronousEvent`

### PET_BATTLE_PVP_DUEL_REQUEST_CANCEL

```lua
PET_BATTLE_PVP_DUEL_REQUEST_CANCEL()
```

`SynchronousEvent`

### PET_BATTLE_PVP_DUEL_REQUESTED

```lua
PET_BATTLE_PVP_DUEL_REQUESTED(fullName: cstring)
```

`SynchronousEvent`

### PET_BATTLE_QUEUE_PROPOSAL_ACCEPTED

```lua
PET_BATTLE_QUEUE_PROPOSAL_ACCEPTED()
```

`SynchronousEvent`

### PET_BATTLE_QUEUE_PROPOSAL_DECLINED

```lua
PET_BATTLE_QUEUE_PROPOSAL_DECLINED()
```

`SynchronousEvent`

### PET_BATTLE_QUEUE_PROPOSE_MATCH

```lua
PET_BATTLE_QUEUE_PROPOSE_MATCH()
```

`SynchronousEvent`

### PET_BATTLE_QUEUE_STATUS

```lua
PET_BATTLE_QUEUE_STATUS()
```

`SynchronousEvent`

### PET_BATTLE_XP_CHANGED

```lua
PET_BATTLE_XP_CHANGED(owner: number, petIndex: number, xpChange: number)
```

`SynchronousEvent`
