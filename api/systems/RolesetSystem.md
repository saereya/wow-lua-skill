# RolesetSystem

Namespace `C_Roleset` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/rolesetsystemdocumentation.lua` (FileDataID 7967272)

## Functions

### ApplyRolesetFilters

```lua
C_Roleset.ApplyRolesetFilters(blockedRolesets: string[], allowedRolesets: string[])
```

Sets or clears both blocklist and allowlist filters atomically with a single visibility reevaluation. Pass an empty table to clear the corresponding filter.

`SecretArguments=AllowedWhenUntainted`

### GetActiveAllowedRolesets

```lua
C_Roleset.GetActiveAllowedRolesets() -> allowedRolesets: string[]
```

Returns the rolesets in the currently active allowlist.

### GetActiveBlockedRolesets

```lua
C_Roleset.GetActiveBlockedRolesets() -> blockedRolesets: string[]
```

Returns the rolesets in the currently active blocklist.
