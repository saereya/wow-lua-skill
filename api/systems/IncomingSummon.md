# IncomingSummon

Namespace `C_IncomingSummon` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/incomingsummondocumentation.lua` (FileDataID 4637100)

## Functions

### HasIncomingSummon

```lua
C_IncomingSummon.HasIncomingSummon(unit: UnitToken) -> summon: bool
```

`SecretArguments=AllowedWhenUntainted`

### IncomingSummonStatus

```lua
C_IncomingSummon.IncomingSummonStatus(unit: UnitToken) -> status: SummonStatus
```

`SecretArguments=AllowedWhenUntainted`

## Types

### SummonStatus

*Enumeration* · 4 values, 0..3

Access values as `Enum.SummonStatus.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `SummonStatus` | = 0 |
| `Pending` | `SummonStatus` | = 1 |
| `Accepted` | `SummonStatus` | = 2 |
| `Declined` | `SummonStatus` | = 3 |
