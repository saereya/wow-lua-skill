# AddOns

Namespace `C_AddOns` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/addonsdocumentation.lua` (FileDataID 4637015)

## Functions

### DisableAddOn

```lua
C_AddOns.DisableAddOn(name: uiAddon, character: cstring)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `name` | `uiAddon` |  |
| `character` | `cstring` | default `"0"` |

### DisableAllAddOns

```lua
C_AddOns.DisableAllAddOns(character: cstring?)
```

`SecretArguments=AllowedWhenUntainted`

### DoesAddOnExist

```lua
C_AddOns.DoesAddOnExist(name: uiAddon) -> exists: bool
```

`SecretArguments=AllowedWhenUntainted`

### DoesAddOnHaveLoadError

```lua
C_AddOns.DoesAddOnHaveLoadError(name: uiAddon) -> hadError: bool
```

`SecretArguments=AllowedWhenUntainted`

### EnableAddOn

```lua
C_AddOns.EnableAddOn(name: uiAddon, character: cstring)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `name` | `uiAddon` |  |
| `character` | `cstring` | default `"0"` |

### EnableAllAddOns

```lua
C_AddOns.EnableAllAddOns(character: cstring?)
```

`SecretArguments=AllowedWhenUntainted`

### GetAddOnDependencies

```lua
C_AddOns.GetAddOnDependencies(name: uiAddon) -> deps: cstring
```

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `deps` | `cstring` | `StrideIndex=1` |

### GetAddOnEnableState

```lua
C_AddOns.GetAddOnEnableState(name: uiAddon, character: cstring) -> state: AddOnEnableState
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `name` | `uiAddon` |  |
| `character` | `cstring` | default `"0"` |

### GetAddOnInfo

```lua
C_AddOns.GetAddOnInfo(name: uiAddon) -> name: cstring, title: cstring, notes: cstring, loadable: bool, reason: cstring, security: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetAddOnInterfaceVersion

```lua
C_AddOns.GetAddOnInterfaceVersion(name: uiAddon) -> interfaceVersion: number
```

`SecretArguments=AllowedWhenUntainted`

### GetAddOnLocalTable

```lua
C_AddOns.GetAddOnLocalTable(name: uiAddon) -> table: LuaValueVariant
```

Returns the addon table (passed as the second argument of ... to files) for any addon that opts in through setting AllowAddOnTableAccess: 1 in the toc file. Insecure code cannot query addon tables from Blizzard addons.

`SecretArguments=AllowedWhenUntainted`

### GetAddOnMetadata

```lua
C_AddOns.GetAddOnMetadata(name: uiAddon, variable: cstring) -> value: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetAddOnName

```lua
C_AddOns.GetAddOnName(index: uiAddon) -> name: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetAddOnNotes

```lua
C_AddOns.GetAddOnNotes(name: uiAddon) -> notes: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetAddOnOptionalDependencies

```lua
C_AddOns.GetAddOnOptionalDependencies(name: uiAddon) -> deps: cstring
```

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `deps` | `cstring` | `StrideIndex=1` |

### GetAddOnSecurity

```lua
C_AddOns.GetAddOnSecurity(name: uiAddon) -> security: AddOnSecurityStatus
```

`SecretArguments=AllowedWhenUntainted`

### GetAddOnTitle

```lua
C_AddOns.GetAddOnTitle(name: uiAddon) -> title: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetNumAddOns

```lua
C_AddOns.GetNumAddOns() -> numAddOns: number
```

### GetScriptsDisallowedForBeta

```lua
C_AddOns.GetScriptsDisallowedForBeta() -> disallowed: bool
```

### IsAddOnDefaultEnabled

```lua
C_AddOns.IsAddOnDefaultEnabled(name: uiAddon) -> defaultEnabled: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsAddOnLoadable

```lua
C_AddOns.IsAddOnLoadable(name: uiAddon, character: cstring, demandLoaded: bool) -> loadable: bool, reason: cstring
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `name` | `uiAddon` |  |
| `character` | `cstring` | default `"0"` |
| `demandLoaded` | `bool` | default `false` |

### IsAddOnLoaded

```lua
C_AddOns.IsAddOnLoaded(name: uiAddon) -> loadedOrLoading: bool, loaded: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsAddOnLoadOnDemand

```lua
C_AddOns.IsAddOnLoadOnDemand(name: uiAddon) -> loadOnDemand: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsAddonVersionCheckEnabled

```lua
C_AddOns.IsAddonVersionCheckEnabled() -> isEnabled: bool
```

### LoadAddOn

```lua
C_AddOns.LoadAddOn(name: uiAddon) -> loaded: bool?, value: string?
```

`SecretArguments=AllowedWhenUntainted`

### ResetAddOns

```lua
C_AddOns.ResetAddOns()
```

### ResetDisabledAddOns

```lua
C_AddOns.ResetDisabledAddOns()
```

### SaveAddOns

```lua
C_AddOns.SaveAddOns()
```

### SetAddonVersionCheck

```lua
C_AddOns.SetAddonVersionCheck(enabled: bool)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### ADDON_LOADED

```lua
ADDON_LOADED(addOnName: cstring, containsBindings: bool)
```

`SynchronousEvent`

### ADDONS_UNLOADING

```lua
ADDONS_UNLOADING(closingClient: bool)
```

`SynchronousEvent`

### SAVED_VARIABLES_TOO_LARGE

```lua
SAVED_VARIABLES_TOO_LARGE(addOnName: cstring)
```

`SynchronousEvent`

## Types

### AddOnInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `title` | `cstring` |  |
| `notes` | `cstring` |  |
| `loadable` | `bool` |  |
| `reason` | `cstring` |  |
| `security` | `cstring` |  |

### AddOnLoadableInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `loadable` | `bool` |  |
| `reason` | `cstring` |  |
