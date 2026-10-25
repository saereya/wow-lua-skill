# EncodingUtil

Namespace `C_EncodingUtil` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/encodingutildocumentation.lua` (FileDataID 6718792)

## Functions

### CompressString

```lua
C_EncodingUtil.CompressString(source: stringView, method: CompressionMethod, level: CompressionLevel) -> output: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `source` | `stringView` |  |
| `method` | `CompressionMethod` | default `"Deflate"` |
| `level` | `CompressionLevel` | default `"Default"` |

### DecodeBase64

```lua
C_EncodingUtil.DecodeBase64(source: stringView, variant: Base64Variant) -> output: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `source` | `stringView` |  |
| `variant` | `Base64Variant` | default `"Standard"` |

### DecodeHex

```lua
C_EncodingUtil.DecodeHex(source: string) -> output: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### DecompressString

```lua
C_EncodingUtil.DecompressString(source: stringView, method: CompressionMethod) -> output: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `source` | `stringView` |  |
| `method` | `CompressionMethod` | default `"Deflate"` |

### DeserializeCBOR

```lua
C_EncodingUtil.DeserializeCBOR(source: stringView) -> value: LuaValueVariant?
```

`SecretArguments=AllowedWhenUntainted`

### DeserializeJSON

```lua
C_EncodingUtil.DeserializeJSON(source: string) -> value: LuaValueVariant?
```

`SecretArguments=AllowedWhenUntainted`

### EncodeBase64

```lua
C_EncodingUtil.EncodeBase64(source: stringView, variant: Base64Variant) -> output: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `source` | `stringView` |  |
| `variant` | `Base64Variant` | default `"Standard"` |

### EncodeHex

```lua
C_EncodingUtil.EncodeHex(source: stringView) -> output: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### SerializeCBOR

```lua
C_EncodingUtil.SerializeCBOR(value: LuaValueVariant?, options: CBORSerializationOptions?) -> output: string
```

`SecretArguments=AllowedWhenUntainted`

### SerializeJSON

```lua
C_EncodingUtil.SerializeJSON(value: LuaValueVariant?, options: JSONSerializationOptions?) -> output: string
```

`SecretArguments=AllowedWhenUntainted`

## Types

### Base64Variant

*Enumeration* · 2 values, 0..1

Access values as `Enum.Base64Variant.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Standard` | `Base64Variant` | = 0; Encodes with the alphabet defined in RFC 4648 (with potential padding bytes) |
| `StandardUrlSafe` | `Base64Variant` | = 1; Encodes with the 'URL and Filename Safe' alphabet from RFC 4648 (with potential padding bytes) |

### CompressionLevel

*Enumeration* · 3 values, 0..2

Access values as `Enum.CompressionLevel.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Default` | `CompressionLevel` | = 0 |
| `OptimizeForSpeed` | `CompressionLevel` | = 1 |
| `OptimizeForSize` | `CompressionLevel` | = 2 |

### CompressionMethod

*Enumeration* · 3 values, 0..2

Access values as `Enum.CompressionMethod.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Deflate` | `CompressionMethod` | = 0 |
| `Zlib` | `CompressionMethod` | = 1 |
| `Gzip` | `CompressionMethod` | = 2 |

### CBORSerializationOptions

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ignoreSerializationErrors` | `bool` | default `false`; If true, attempt to ignore errors from unsupported values and instead replace them where applicable with 'undefined' CBOR items. |

### JSONSerializationOptions

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ignoreSerializationErrors` | `bool` | default `false`; If true, attempt to ignore errors from unsupported values and instead replace them where applicable with 'null' JSON values. |
