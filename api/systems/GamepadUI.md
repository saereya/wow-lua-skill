# GamepadUI

Namespace `C_GamepadUI` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/gamepaduidocumentation.lua` (FileDataID 6651412)

## Functions

### GetFirstGamepadActionBarStorageSlotIndexForActiveStance

```lua
C_GamepadUI.GetFirstGamepadActionBarStorageSlotIndexForActiveStance() -> activeStanceFirstGamepadStorageSlotIndex: luaIndex?
```

### GetFirstGamepadActionStorageSlotIndex

```lua
C_GamepadUI.GetFirstGamepadActionStorageSlotIndex() -> firstGamepadActionStorageSlotIndex: luaIndex
```

### GetFirstGamepadPetActionStorageSlotIndex

```lua
C_GamepadUI.GetFirstGamepadPetActionStorageSlotIndex() -> firstGamepadPetActionStorageSlotID: luaIndex
```

### IsValidGamepadActionStorageSlotIndex

```lua
C_GamepadUI.IsValidGamepadActionStorageSlotIndex(gamepadActionStorageSlotIndex: luaIndex) -> isValid: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsValidGamepadPossessBarStorageSlotIndex

```lua
C_GamepadUI.IsValidGamepadPossessBarStorageSlotIndex(gamepadPossessBarStorageSlotIndex: luaIndex) -> isValid: bool
```

`SecretArguments=AllowedWhenUntainted`

## Events

### GAMEPAD_POSSESS_BAR_OVERRIDE_CHANGED

```lua
GAMEPAD_POSSESS_BAR_OVERRIDE_CHANGED(oldOverride: GamepadPossessBarOverride, newOverride: GamepadPossessBarOverride)
```

`UniqueEvent`

### GAMEPAD_STANCE_BAR_OVERRIDE_CHANGED

```lua
GAMEPAD_STANCE_BAR_OVERRIDE_CHANGED(oldOverride: GamepadStanceBarOverride, newOverride: GamepadStanceBarOverride)
```

`UniqueEvent`

## Types

### GamepadPossessBarOverride

*Enumeration* · 12 values, 1..12

Access values as `Enum.GamepadPossessBarOverride.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `SpecialPageTopBar` | `GamepadPossessBarOverride` | = 1 |
| `Page1LeftBar` | `GamepadPossessBarOverride` | = 2 |
| `Page1RightBar` | `GamepadPossessBarOverride` | = 3 |
| `Page1BottomBar` | `GamepadPossessBarOverride` | = 4 |
| `Page2TopBar` | `GamepadPossessBarOverride` | = 5 |
| `Page2LeftBar` | `GamepadPossessBarOverride` | = 6 |
| `Page2RightBar` | `GamepadPossessBarOverride` | = 7 |
| `Page2BottomBar` | `GamepadPossessBarOverride` | = 8 |
| `Page3TopBar` | `GamepadPossessBarOverride` | = 9 |
| `Page3LeftBar` | `GamepadPossessBarOverride` | = 10 |
| `Page3RightBar` | `GamepadPossessBarOverride` | = 11 |
| `Page3BottomBar` | `GamepadPossessBarOverride` | = 12 |

### GamepadStanceBarOverride

*Enumeration* · 12 values, 1..12

Access values as `Enum.GamepadStanceBarOverride.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `GamepadStanceBarOverride` | = 1 |
| `Page1LeftBar` | `GamepadStanceBarOverride` | = 2 |
| `Page1RightBar` | `GamepadStanceBarOverride` | = 3 |
| `Page1BottomBar` | `GamepadStanceBarOverride` | = 4 |
| `Page2TopBar` | `GamepadStanceBarOverride` | = 5 |
| `Page2LeftBar` | `GamepadStanceBarOverride` | = 6 |
| `Page2RightBar` | `GamepadStanceBarOverride` | = 7 |
| `Page2BottomBar` | `GamepadStanceBarOverride` | = 8 |
| `Page3TopBar` | `GamepadStanceBarOverride` | = 9 |
| `Page3LeftBar` | `GamepadStanceBarOverride` | = 10 |
| `Page3RightBar` | `GamepadStanceBarOverride` | = 11 |
| `Page3BottomBar` | `GamepadStanceBarOverride` | = 12 |

### GamepadActionBarConstants

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `NUM_SLOTS_PER_GAMEPAD_ACTION_BAR_GROUP` | `number` | = `4` |
| `NUM_GROUPS_PER_GAMEPAD_ACTION_BAR` | `number` | = `2` |
| `NUM_SLOTS_PER_GAMEPAD_ACTION_BAR` | `number` | = `Constants.GamepadActionBarConstants.NUM_SLOTS_PER_GAMEPAD_ACTION_BAR_GROUP * Constants.GamepadActionBarConstants.NUM_GROUPS_PER_GAMEPAD_ACTION_BAR` |
| `NUM_PAGEABLE_BARS_IN_GAMEPAD_ACTION_BAR_PAGE_UNIT` | `number` | = `4` |
| `NUM_PAGEABLE_SLOTS_PER_GAMEPAD_ACTION_BAR_PAGE_UNIT_STANDARD_PAGE` | `number` | = `Constants.GamepadActionBarConstants.NUM_PAGEABLE_BARS_IN_GAMEPAD_ACTION_BAR_PAGE_UNIT * Constants.GamepadActionBarConstants.NUM_SLOTS_PER_GAMEPAD_ACTION_BAR` |
| `NUM_RESERVED_SLOTS_PER_GAMEPAD_ACTION_BAR_PAGE_UNIT` | `number` | = `4` |
| `NUM_PAGES_PER_GAMEPAD_ACTION_BAR_PAGE_UNIT` | `number` | = `4` |
| `NUM_STANDARD_PAGES_PER_GAMEPAD_ACTION_BAR_PAGE_UNIT` | `number` | = `3` |
| `GAMEPAD_ACTION_BAR_PAGE_UNIT_SPECIAL_PAGE_INDEX` | `number` | = `4` |
| `NUM_PAGEABLE_SLOTS_PER_GAMEPAD_ACTION_BAR_PAGE_UNIT` | `number` | = `Constants.GamepadActionBarConstants.NUM_PAGEABLE_SLOTS_PER_GAMEPAD_ACTION_BAR_PAGE_UNIT_STANDARD_PAGE * Constants.GamepadActionBarConstants.NUM_STANDARD_PAGES_PER_GAMEPAD_ACTION_BAR_PAGE_UNIT` |
| `NUM_GAMEPAD_STANCE_ACTION_BARS` | `number` | = `5` |
