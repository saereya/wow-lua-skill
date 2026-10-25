# InstanceLeaverInfo

Namespace `C_InstanceLeaver` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/instanceleaverinfodocumentation.lua` (FileDataID 7260313)

## Functions

### IsPlayerLeaver

```lua
C_InstanceLeaver.IsPlayerLeaver() -> isLeaver: bool
```

Returns whether the player is considered a leaver for repeatedly abandoning mythic+ groups.

## Events

### INSTANCE_LEAVER_STATUS_CHANGED

```lua
INSTANCE_LEAVER_STATUS_CHANGED(isLeaver: bool)
```

`SynchronousEvent`
