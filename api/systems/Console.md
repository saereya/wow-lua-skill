# Console

Global functions · environment All · source `interface/addons/blizzard_apidocumentationgenerated/consoledocumentation.lua` (FileDataID 4637065)

## Functions

### CalculateStringEditDistance

```lua
CalculateStringEditDistance(firstString: stringView, secondString: stringView) -> distance: number
```

`SecretArguments=AllowedWhenUntainted`

### ConsoleEcho

```lua
ConsoleEcho(command: cstring, addToHistory: bool, prefix: cstring?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `command` | `cstring` |  |
| `addToHistory` | `bool` | default `false` |
| `prefix` | `cstring?` |  |

### ConsoleExec

```lua
ConsoleExec(command: cstring, addToHistory: bool) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `command` | `cstring` |  |
| `addToHistory` | `bool` | default `false` |

### ConsoleGetAllCommands

```lua
ConsoleGetAllCommands() -> commands: ConsoleCommandInfo[]
```

### ConsoleGetColorFromType

```lua
ConsoleGetColorFromType(colorType: ConsoleColorType) -> color: colorRGB
```

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `color` | `colorRGB` | `Mixin=ColorMixin` |

### ConsoleGetFontHeight

```lua
ConsoleGetFontHeight() -> fontHeightInPixels: number
```

### ConsoleIsActive

```lua
ConsoleIsActive() -> consoleIsActive: bool
```

### ConsolePrintAllMatchingCommands

```lua
ConsolePrintAllMatchingCommands(partialCommandText: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### ConsoleSetFontHeight

```lua
ConsoleSetFontHeight(fontHeightInPixels: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetConsoleKey

```lua
SetConsoleKey(keystring: cstring)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### CONSOLE_CLEAR

```lua
CONSOLE_CLEAR()
```

`UniqueEvent`

### CONSOLE_COLORS_CHANGED

```lua
CONSOLE_COLORS_CHANGED()
```

`UniqueEvent`

### CONSOLE_FONT_SIZE_CHANGED

```lua
CONSOLE_FONT_SIZE_CHANGED()
```

`UniqueEvent`

### CONSOLE_LOG

```lua
CONSOLE_LOG(message: cstring)
```

`SynchronousEvent`

### CONSOLE_MESSAGE

```lua
CONSOLE_MESSAGE(message: cstring, colorType: number)
```

`SynchronousEvent`

### CVAR_UPDATE

```lua
CVAR_UPDATE(eventName: cstring, value: cstring)
```

`SynchronousEvent`

### TOGGLE_CONSOLE

```lua
TOGGLE_CONSOLE(showConsole: bool?)
```

`SynchronousEvent`

## Types

### ConsoleCategory

*Enumeration* · 11 values, 0..10

Access values as `Enum.ConsoleCategory.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Debug` | `ConsoleCategory` | = 0 |
| `Graphics` | `ConsoleCategory` | = 1 |
| `Console` | `ConsoleCategory` | = 2 |
| `Combat` | `ConsoleCategory` | = 3 |
| `Game` | `ConsoleCategory` | = 4 |
| `Default` | `ConsoleCategory` | = 5 |
| `Net` | `ConsoleCategory` | = 6 |
| `Sound` | `ConsoleCategory` | = 7 |
| `Gm` | `ConsoleCategory` | = 8 |
| `Reveal` | `ConsoleCategory` | = 9 |
| `None` | `ConsoleCategory` | = 10 |

### ConsoleColorType

*Enumeration* · 12 values, 0..11

Access values as `Enum.ConsoleColorType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `DefaultColor` | `ConsoleColorType` | = 0 |
| `InputColor` | `ConsoleColorType` | = 1 |
| `EchoColor` | `ConsoleColorType` | = 2 |
| `ErrorColor` | `ConsoleColorType` | = 3 |
| `WarningColor` | `ConsoleColorType` | = 4 |
| `GlobalColor` | `ConsoleColorType` | = 5 |
| `AdminColor` | `ConsoleColorType` | = 6 |
| `HighlightColor` | `ConsoleColorType` | = 7 |
| `BackgroundColor` | `ConsoleColorType` | = 8 |
| `ClickbufferColor` | `ConsoleColorType` | = 9 |
| `PrivateColor` | `ConsoleColorType` | = 10 |
| `DefaultGreen` | `ConsoleColorType` | = 11 |

### ConsoleCommandType

*Enumeration* · 4 values, 0..3

Access values as `Enum.ConsoleCommandType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Cvar` | `ConsoleCommandType` | = 0 |
| `Command` | `ConsoleCommandType` | = 1 |
| `Macro` | `ConsoleCommandType` | = 2 |
| `Script` | `ConsoleCommandType` | = 3 |

### ConsoleCommandInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `command` | `cstring` |  |
| `help` | `cstring` |  |
| `category` | `ConsoleCategory` |  |
| `commandType` | `ConsoleCommandType` |  |
| `scriptContents` | `cstring` |  |
| `scriptParameters` | `cstring` |  |
