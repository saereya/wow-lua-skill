# LuaDurationManualClock

Widget methods (`LuaDurationManualClockAPI`) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/luadurationmanualclockapidocumentation.lua` (FileDataID 7937109)

## Methods

### AdvanceTime

```lua
LuaDurationManualClock:AdvanceTime(delta: Seconds)
```

Advances the clock by a specified number of seconds.

`SecretArguments=AllowedWhenUntainted`

### ResetTime

```lua
LuaDurationManualClock:ResetTime()
```

Resets the clock to a zero time value.

### RewindTime

```lua
LuaDurationManualClock:RewindTime(delta: Seconds)
```

Rewinds the clock by a specified number of seconds.

`SecretArguments=AllowedWhenUntainted`

### SetTime

```lua
LuaDurationManualClock:SetTime(time: FrameTime)
```

Sets the current clock timestamp to a given value.

`SecretArguments=AllowedWhenUntainted`
