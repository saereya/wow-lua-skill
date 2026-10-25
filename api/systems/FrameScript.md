# FrameScript

Global functions · environment All · source `interface/addons/blizzard_apidocumentationgenerated/framescriptdocumentation.lua` (FileDataID 5243958)

## Functions

### AddSourceLocationExclude

```lua
AddSourceLocationExclude(fileName: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### canaccessallvalues

```lua
canaccessallvalues(values: LuaValueReference) -> canAccessAllValues: bool
```

Returns true if the immediate calling function has appropriate permissions to access and operate on all supplied values.

`SecretArguments=AllowedWhenUntainted` `SecureHooksAllowed=False`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `values` | `LuaValueReference` | `StrideIndex=1` |

### canaccesssecrets

```lua
canaccesssecrets() -> canAccessSecrets: bool
```

Returns true if the immediate calling function has appropriate permissions to access or operate on secret values.

`SecureHooksAllowed=False`

### canaccesstable

```lua
canaccesstable(table: LuaValueReference) -> canAccessTable: bool
```

Returns true if the immediate calling function has appropriate permissions to index secret tables. This will return false if the caller cannot access the table value itself, or if access to the table contents is disallowed by taint.

`SecretArguments=AllowedWhenUntainted` `SecureHooksAllowed=False`

### canaccessvalue

```lua
canaccessvalue(value: LuaValueReference) -> canAccessValue: bool
```

Returns true if the immediate calling function has appropriate permissions to access and operate on a specific value.

`SecretArguments=AllowedWhenUntainted` `SecureHooksAllowed=False`

### CreateFrameWithOptions

```lua
CreateFrameWithOptions(options: CreateFrameOptions) -> frame: SimpleFrame
```

`SecretArguments=AllowedWhenUntainted`

### CreateFromMixins

```lua
CreateFromMixins(mixins: LuaValueVariant) -> object: LuaValueVariant
```

`SecretArguments=AllowedWhenUntainted` `SecureHooksAllowed=False`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `mixins` | `LuaValueVariant` | `StrideIndex=1` |

### CreateSecureDelegate

```lua
CreateSecureDelegate(luaFunction: LuaValueReference, options: SecureDelegateOptions?) -> secureDelegateFunction: LuaValueReference
```

Creates a secure delegate closure for a Lua function. The delegate invokes the original function in a protected call context with secure execution taint, and supports passing and returning values directly.

`SecretArguments=AllowedWhenUntainted` `SecureHooksAllowed=False` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `luaFunction` | `LuaValueReference` | The Lua function to invoke through the secure delegate. |
| `options` | `SecureDelegateOptions?` | Optional settings controlling secure delegate behavior. If omitted, default options are used. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `secureDelegateFunction` | `LuaValueReference` | A secure delegate function that calls through to the original Lua function. |

### CreateWindow

```lua
CreateWindow(popupStyle: bool, topMost: bool) -> window: SimpleWindow?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `popupStyle` | `bool` | default `true` |
| `topMost` | `bool` | default `false` |

### debugprofilestart

```lua
debugprofilestart()
```

Starts a timer for profiling. The final time can be obtained by calling debugprofilestop.

### debugprofilestop

```lua
debugprofilestop() -> elapsedMilliseconds: number
```

Returns the time in milliseconds since the last debugprofilestart call.

### dropsecretaccess

```lua
dropsecretaccess()
```

Removes the ability for the immediate calling function to access secret values.

`SecureHooksAllowed=False`

### dumpobject

```lua
dumpobject(value: LuaValueReference?) -> result: LuaValueReference?
```

Invokes the '__dump' metamethod on any value (if present), returning its result.

`SecretArguments=AllowedWhenUntainted` `SecureHooksAllowed=False`

### GetCallstackHeight

```lua
GetCallstackHeight() -> height: number
```

### GetCurrentEventID

```lua
GetCurrentEventID() -> eventID: number?
```

### GetErrorCallstackHeight

```lua
GetErrorCallstackHeight() -> height: number?
```

### GetEventTime

```lua
GetEventTime(eventProfileIndex: number) -> totalElapsedTime: number, numExecutedHandlers: number, slowestHandlerName: cstring, slowestHandlerTime: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetForbiddenObjectTable

```lua
GetForbiddenObjectTable(object: FrameScriptObject) -> forbiddenTable: FrameScriptObject
```

`SecretArguments=AllowedWhenUntainted` `Environment=SecureOnly` `SecureHooksAllowed=False`

### GetScriptBucketThrottleLimits

```lua
GetScriptBucketThrottleLimits() -> limits: ScriptBucketThrottleLimits
```

### GetSourceLocation

```lua
GetSourceLocation() -> location: string
```

`MayReturnNothing`

### hasanysecretvalues

```lua
hasanysecretvalues(values: LuaValueReference) -> isAnyValueSecret: bool
```

Returns true if a supplied value is a secret value.

`SecretArguments=AllowedWhenUntainted` `SecureHooksAllowed=False`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `values` | `LuaValueReference` | `StrideIndex=1` |

### issecrettable

```lua
issecrettable(table: LuaValueReference) -> isSecretOrContentsSecret: bool
```

Returns true if a supplied value is a secret table. This function will return true if the table value itself is secret, or if flags on the table are set such that accesses of the table would produce secrets.

`SecretArguments=AllowedWhenUntainted` `SecureHooksAllowed=False`

### issecretvalue

```lua
issecretvalue(value: LuaValueReference) -> isSecret: bool
```

Returns true if a supplied value is a secret value.

`SecretArguments=AllowedWhenUntainted` `SecureHooksAllowed=False`

### mapvalues

```lua
mapvalues(func: LuaValueReference, values: LuaValueReference) -> mapped: LuaValueReference
```

Applies a given function over all supplied values individually, replacing the value with the result of the call.

`SecretArguments=AllowedWhenUntainted` `SecureHooksAllowed=False`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `func` | `LuaValueReference` |  |
| `values` | `LuaValueReference` | `StrideIndex=1` |

Returns:

| Name | Type | Notes |
|---|---|---|
| `mapped` | `LuaValueReference` | `StrideIndex=1` |

### Mixin

```lua
Mixin(object: LuaValueVariant, mixins: LuaValueVariant) -> outObject: LuaValueVariant
```

`SecretArguments=AllowedWhenUntainted` `SecureHooksAllowed=False`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `object` | `LuaValueVariant` |  |
| `mixins` | `LuaValueVariant` | `StrideIndex=1` |

### RegisterEventCallback

```lua
RegisterEventCallback(eventName: cstring, callback: EventCallbackType)
```

`SecretArguments=AllowedWhenUntainted` `SecureHooksAllowed=False`

### RegisterUnitEventCallback

```lua
RegisterUnitEventCallback(eventName: cstring, callback: EventCallbackType, unit: UnitToken)
```

`SecretArguments=AllowedWhenUntainted` `SecureHooksAllowed=False`

### RunScript

```lua
RunScript(text: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### scrub

```lua
scrub(values: LuaValueReference) -> scrubbed: LuaValueReference
```

Returns a transformed list of values with inputs that are either secret or are not string, number, or boolean type replaced by nil values.

`SecretArguments=AllowedWhenUntainted` `SecureHooksAllowed=False`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `values` | `LuaValueReference` | `StrideIndex=1` |

Returns:

| Name | Type | Notes |
|---|---|---|
| `scrubbed` | `LuaValueReference` | `StrideIndex=1` |

### scrubsecretvalues

```lua
scrubsecretvalues(values: LuaValueReference) -> scrubbed: LuaValueReference
```

Returns a transformed list of values with inputs that are secret values replaced by nil values.

`SecretArguments=AllowedWhenUntainted` `SecureHooksAllowed=False`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `values` | `LuaValueReference` | `StrideIndex=1` |

Returns:

| Name | Type | Notes |
|---|---|---|
| `scrubbed` | `LuaValueReference` | `StrideIndex=1` |

### secretunwrap

```lua
secretunwrap(values: LuaValueReference) -> unwrapped: LuaValueReference
```

Unwraps all supplied secrets, converting them back to regular values.

`SecretArguments=AllowedWhenUntainted` `SecureHooksAllowed=False` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `values` | `LuaValueReference` | `StrideIndex=1` |

Returns:

| Name | Type | Notes |
|---|---|---|
| `unwrapped` | `LuaValueReference` | `StrideIndex=1` |

### secretwrap

```lua
secretwrap(values: LuaValueReference) -> wrapped: LuaValueReference
```

Converts all supplied values to secret values, preventing most operations on them from occurring on tainted code paths.

`SecretArguments=AllowedWhenUntainted` `SecureHooksAllowed=False`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `values` | `LuaValueReference` | `StrideIndex=1` |

Returns:

| Name | Type | Notes |
|---|---|---|
| `wrapped` | `LuaValueReference` | `StrideIndex=1` |

### securecallmethod

```lua
securecallmethod(object: LuaValueReference, method: cstring, arguments: LuaValueReference) -> results: LuaValueReference
```

Invokes a named method on an object with a secure call barrier that prevents errors or taint from function lookup and execution from propagating to the caller.

`SecretArguments=AllowedWhenUntainted` `SecureHooksAllowed=False`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `object` | `LuaValueReference` | The table on which to look up the named method from. Lookup of the method uses raw access and ignores any associated metatable. |
| `method` | `cstring` | The name of a method to retrieve. |
| `arguments` | `LuaValueReference` | Arguments to supply to the method. The initial 'object' parameter is always supplied as the first argument, followed by these values.; `StrideIndex=1` |

Returns:

| Name | Type | Notes |
|---|---|---|
| `results` | `LuaValueReference` | Results from the executed function. If an error occurred, this result list will be empty.; `StrideIndex=1` |

### securecopy

```lua
securecopy(value: LuaValueReference?, options: SecureCopyOptions?) -> copy: LuaValueReference
```

Securely copies a Lua value. Tables are deep-copied with recursive and shared references preserved. Copied values receive the current execution taint.

`SecretArguments=AllowedWhenUntainted` `SecureHooksAllowed=False`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `value` | `LuaValueReference?` | The Lua value to copy. |
| `options` | `SecureCopyOptions?` | Optional settings controlling value copying behavior. If omitted, default secure copy options are used. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `copy` | `LuaValueReference` | The copied value. For tables, recursive and shared references within the copied graph are preserved. |

### SetErrorCallstackHeight

```lua
SetErrorCallstackHeight(height: number?)
```

`SecretArguments=AllowedWhenUntainted`

### settablesecurity

```lua
settablesecurity(table: LuaValueVariant, option: TableSecurityOption)
```

`SecretArguments=AllowedWhenUntainted` `SecureHooksAllowed=False` `HasRestrictions`

### UnregisterEventCallback

```lua
UnregisterEventCallback(eventName: cstring, callback: EventCallbackType)
```

`SecretArguments=AllowedWhenUntainted` `SecureHooksAllowed=False`

### UnregisterUnitEventCallback

```lua
UnregisterUnitEventCallback(eventName: cstring, callback: EventCallbackType, unit: UnitToken)
```

`SecretArguments=AllowedWhenUntainted` `SecureHooksAllowed=False`

## Types

### TableSecurityOption

*Enumeration* · 3 values, 0..2

Access values as `Enum.TableSecurityOption.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `DisallowTaintedAccess` | `TableSecurityOption` | = 0 |
| `DisallowSecretKeys` | `TableSecurityOption` | = 1 |
| `SecretWrapContents` | `TableSecurityOption` | = 2 |

### CreateFrameOptions

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `frameType` | `cstring` |  |
| `name` | `cstring?` |  |
| `parent` | `SimpleFrame?` |  |
| `inherits` | `cstring[]?` |  |
| `id` | `number?` |  |
| `forbidden` | `bool` | default `false` |
| `hidden` | `bool` | default `false` |

### ScriptBucketThrottleLimits

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `luaScriptBucketThrottleMaxMsPerSecondNormal` | `number` |  |
| `luaScriptBucketThrottleMaxMsPerSecondRestricted` | `number` |  |
| `luaScriptBucketThrottleMaxMsBurstNormal` | `number` |  |
| `luaScriptBucketThrottleMaxMsBurstRestricted` | `number` |  |

### SecureCopyOptions

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `maxTraversalDepth` | `number` | default `100`; Maximum table nesting depth allowed during recursive copying. |
| `wrapUntrustedFunctions` | `bool` | default `true`; Wrap function values in secure closures that call through using the original function taint. |
| `permitScriptObjects` | `bool` | default `false`; If true, preserve references to script objects in the copied output. By default, script objects will raise an error. |

### SecureDelegateOptions

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `wrapUntrustedFunctions` | `bool` | default `true`; Wrap function arguments in secure closures that call through using the original function taint. |

### EventCallbackType

*CallbackType*
