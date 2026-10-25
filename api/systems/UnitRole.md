# UnitRole

Global functions · environment All · source `interface/addons/blizzard_apidocumentationgenerated/unitroledocumentation.lua` (FileDataID 6344473)

## Functions

### AreClassRolesSoftSuggestions

```lua
AreClassRolesSoftSuggestions() -> result: bool
```

If true, UnitGetAvailableRoles results should be treated as suggested role, not hard limits on what role the current player can display as.

### CanShowSetRoleButton

```lua
CanShowSetRoleButton() -> result: bool
```

### InitiateRolePoll

```lua
InitiateRolePoll() -> result: bool
```

### UnitGetAvailableRoles

```lua
UnitGetAvailableRoles(unit: UnitToken) -> tank: bool, healer: bool, dps: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretWhenUnitIdentityRestricted`

### UnitSetRole

```lua
UnitSetRole(unit: UnitToken, roleStr: cstring?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### UnitSetRoleEnum

```lua
UnitSetRoleEnum(unit: UnitToken, role: LFGRole?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

## Events

### ROLE_CHANGED_INFORM

```lua
ROLE_CHANGED_INFORM(changedName: cstring, fromName: cstring, oldRole: cstring, newRole: cstring)
```

`SynchronousEvent`

### ROLE_POLL_BEGIN

```lua
ROLE_POLL_BEGIN(fromName: cstring)
```

`SynchronousEvent`
