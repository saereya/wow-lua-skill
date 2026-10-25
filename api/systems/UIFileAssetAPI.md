# UIFileAssetAPI

Namespace `C_UIFileAsset` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/uifileassetapidocumentation.lua` (FileDataID 7950562)

## Functions

### GetFileID

```lua
C_UIFileAsset.GetFileID(asset: FileAsset) -> assetFileID: fileID?
```

Returns the numeric file ID associated with a file asset.

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `assetFileID` | `fileID?` | The file ID corresponding to the given asset. If the asset is already a file ID, it is returned unchanged; otherwise returns nil if the file path is not known to the client. |

### IsKnownFile

```lua
C_UIFileAsset.IsKnownFile(asset: FileAsset) -> isValid: bool
```

Determines whether a file asset is known to the client, either as a shipped asset or a locally existing loose file.

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `isValid` | `bool` | True if the asset is shipped with the client or refers to a known loose file. Existence or openability of loose files is not verified. |

### IsLooseFile

```lua
C_UIFileAsset.IsLooseFile(asset: FileAsset) -> isLooseFile: bool
```

Determines whether a file asset refers to a known loose (local) file.

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `isLooseFile` | `bool` | True if the asset refers to a loose file known to the client. |
