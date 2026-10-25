# LuaTableExtensions

Namespace `table` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/luatableextensionsdocumentation.lua` (FileDataID 8293696)

## Functions

### contains

```lua
table.contains(table: table, value: any?) -> containsValue: bool
```

Returns true if any value in the table compares equal to the specified value.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `table` | `table` | The table to search. |
| `value` | `any?` | The value for which to search. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `containsValue` | `bool` | True if any entry in the table has the specified value. |

### count

```lua
table.count(table: table) -> count: number
```

Returns the number of entries in the table.

`SecretArguments=AllowedWhenUntainted` `SecretWhenLuaTableHasSecretKeys`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `table` | `table` | The table whose entries will be counted. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `count` | `number` | The number of entries in the table. |

### create

```lua
table.create(arraySizeHint: number, nodeSizeHint: number) -> table: table
```

Creates an empty table with storage preallocated for the specified number of array and non-array entries.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `arraySizeHint` | `number` | The number of array entries for which to preallocate storage. |
| `nodeSizeHint` | `number` | default `0`; The number of non-array entries for which to preallocate storage. |

### freeze

```lua
table.freeze(table: table) -> frozen: table
```

Marks a supplied table as frozen, preventing any modifications to its contents, or replacement of its metatable. If the table has a pre-existing metatable with a '__newindex' table or function, assignments will pass through without raising errors. For tainted code, only tables created by the same addon making this function call are permitted to be frozen.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `table` | `table` | The table to freeze. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `frozen` | `table` | The supplied table, passed through. |

### getcountinfo

```lua
table.getcountinfo(table: table) -> numEntries: number, numPositiveIntegerKeys: number, maxPositiveIntegerKey: number
```

Returns detailed information about the number and distribution of entries in the table.

`SecretArguments=AllowedWhenUntainted` `SecretWhenLuaTableHasSecretKeys`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `table` | `table` | The table to inspect. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `numEntries` | `number` | The total number of entries in the table. |
| `numPositiveIntegerKeys` | `number` | The number of entries with positive integral keys. |
| `maxPositiveIntegerKey` | `number` | The largest positive integral key in the table, or zero if no such keys were found. |

### indexof

```lua
table.indexof(table: table, value: any?) -> index: number?
```

Returns the first integer index whose value compares equal to the specified value, searching consecutively from index 1 until the first nil value.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `table` | `table` | The table to search. |
| `value` | `any?` | The value for which to search. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `index` | `number?` | The first matching index, or nil if no match is found. |

### isempty

```lua
table.isempty(table: table) -> empty: bool
```

Returns true if the table contains no entries.

`SecretArguments=AllowedWhenUntainted` `SecretWhenLuaTableHasSecretKeys`

Returns:

| Name | Type | Notes |
|---|---|---|
| `empty` | `bool` | True if the table contains no entries; otherwise false. |

### isfrozen

```lua
table.isfrozen(table: table) -> frozen: bool
```

Returns true if a table has been marked as frozen.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `table` | `table` | The table to inspect. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `frozen` | `bool` | True if the table has been made read-only; otherwise false. |

### keys

```lua
table.keys(table: table) -> keys: any
```

Returns an array containing the keys of the specified table.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `table` | `table` | The table whose keys will be returned. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `keys` | `any` | An array containing the table's keys. The order of the returned keys is unspecified. |

### removeunordered

```lua
table.removeunordered(table: table, index: number?) -> value: any?
```

Removes the value at the specified integer index by replacing it with the last value in the array and shortening the array by one element. The order of values in the array is not preserved.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `table` | `table` | The table from which to remove a value. |
| `index` | `number?` | The integer index of the value to remove. If omitted, the last value is removed. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `value` | `any?` | The removed value, or nil if the index is outside the array bounds. |

### removevalue

```lua
table.removevalue(table: table, value: any?) -> removedCount: number
```

Removes all values equal to the specified value from the array portion of a table.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `table` | `table` | The table from which to remove values. |
| `value` | `any?` | The value to remove. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `removedCount` | `number` | The number of values removed. |

### values

```lua
table.values(table: table) -> values: any
```

Returns an array containing the values of the specified table.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `table` | `table` | The table whose values will be returned. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `values` | `any` | An array containing the table's values. The order of the returned values is unspecified. |
