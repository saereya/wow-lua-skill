# HousingBlueprintUI

Namespace `C_HousingBlueprint` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/housingblueprintuidocumentation.lua` (FileDataID 7889252)

## Functions

### CanExportRoom

```lua
C_HousingBlueprint.CanExportRoom(roomGUID: WOWGUID) -> canExport: bool
```

Returns true if the specific room is allowed to be exported

`SecretArguments=AllowedWhenUntainted`

### CanExportTypeFromCurrentLocation

```lua
C_HousingBlueprint.CanExportTypeFromCurrentLocation(type: HousingBlueprintType) -> locationValid: bool
```

Returns true if the player's current location is a valid place to attempt to export a specific kind of blueprint

`SecretArguments=AllowedWhenUntainted`

### CanImportTypeFromCurrentLocation

```lua
C_HousingBlueprint.CanImportTypeFromCurrentLocation(type: HousingBlueprintType) -> locationValid: bool
```

Returns true if the player's current location is a valid place to attempt to import a specific kind of blueprint

`SecretArguments=AllowedWhenUntainted`

### DeleteBlueprint

```lua
C_HousingBlueprint.DeleteBlueprint(blueprintID: BigUInteger)
```

Delete the specified owned blueprint; Listen for HousingBlueprintDeleteSuccess and HousingBlueprintDeleteFailure for results

`SecretArguments=AllowedWhenUntainted`

### ExportBlueprint

```lua
C_HousingBlueprint.ExportBlueprint(type: HousingBlueprintType, name: cstring)
```

Saves out a new Blueprint of the specified type, using the specified name, if available, based on where the player is currently standing (see GetExportAvailability); Listen for HousingBlueprintExportSuccess and HousingBlueprintExportFailure for results

`SecretArguments=AllowedWhenUntainted`

### ExportRoomBlueprint

```lua
C_HousingBlueprint.ExportRoomBlueprint(name: cstring, roomGUID: WOWGUID)
```

Saves out a new Blueprint of the specified room, using the specified name, if available (see GetExportAvailability); Listen for HousingBlueprintExportSuccess and HousingBlueprintExportFailure for results

`SecretArguments=AllowedWhenUntainted`

### GetBlueprintHyperlink

```lua
C_HousingBlueprint.GetBlueprintHyperlink(blueprintShareCode: cstring) -> hyperLink: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetBlueprintTypeForCode

```lua
C_HousingBlueprint.GetBlueprintTypeForCode(shareCode: cstring) -> type: HousingBlueprintType
```

Returns what type of Blueprint the specified code is for; Will return HousingBlueprintType.None if code is invalid; Does NOT check whether the shareCode actually matches up to a real valid Blueprint

`SecretArguments=AllowedWhenUntainted`

### GetExportAvailability

```lua
C_HousingBlueprint.GetExportAvailability() -> availability: HousingResult
```

Returns success if the player can currently export Blueprints, or a specific error type (ex: invalid location or permissions)

### GetFeatureAvailability

```lua
C_HousingBlueprint.GetFeatureAvailability() -> blueprintsAvailability: HousingResult
```

Returns success if Blueprints as a feature is currently enabled and available

### GetImportAvailability

```lua
C_HousingBlueprint.GetImportAvailability() -> availability: HousingResult
```

Returns success if the player can currently import Blueprints, or a specific error type (ex: invalid location or permissions)

### ImportBlueprint

```lua
C_HousingBlueprint.ImportBlueprint(shareCode: cstring)
```

Imports the specified blueprint, if available (see GetImportAvailability and CanImportTypeFromCurrentLocation); Listen for HousingBlueprintImportSuccess and HousingBlueprintImportFailure for results

`SecretArguments=AllowedWhenUntainted`

### IsShareCodeValid

```lua
C_HousingBlueprint.IsShareCodeValid(shareCode: cstring) -> isValid: bool
```

Returns true if the string matches the valid expected format for a Blueprint Share Code; Does NOT check whether the shareCode actually matches up to a real valid Blueprint

`SecretArguments=AllowedWhenUntainted`

### RenameBlueprint

```lua
C_HousingBlueprint.RenameBlueprint(blueprintID: BigUInteger, newName: cstring)
```

Rename the specified owned blueprint to the specified name; Listen for HousingBlueprintRenameSuccess and HousingBlueprintRenameFailure for results

`SecretArguments=AllowedWhenUntainted`

### RequestBlueprintCollection

```lua
C_HousingBlueprint.RequestBlueprintCollection()
```

Request the full list of all of the player's Blueprints; This is async, either the HOUSING_BLUEPRINT_COLLECTION_RECEIVED or HOUSING_BLUEPRINT_COLLECTION_FAILURE event will eventually be fired as a result

### RequestBlueprintContents

```lua
C_HousingBlueprint.RequestBlueprintContents(shareCode: cstring)
```

Request the full contents of a specific Blueprint, in context of the current owned plot or house (if any); This is async as content info includes dynamic data from the server, either the HOUSING_BLUEPRINT_CONTENTS_RECEIVED or HOUSING_BLUEPRINT_CONTENTS_FAILURE event will eventually be fired as a result; Calling this again before a prior request has finished will cancel the prior request

`SecretArguments=AllowedWhenUntainted`

### RequestBlueprintContentsForContext

```lua
C_HousingBlueprint.RequestBlueprintContentsForContext(shareCode: cstring, optionalHouseGUID: WOWGUID?)
```

Request the full contents of a specific Blueprint, either in context of a specific owned House or plot, or explicitly outside of any specific context; Typically used to update missing requirement info from previously-retrieved contents; See RequestBlueprintContents for other notes

`SecretArguments=AllowedWhenUntainted`

### StartImportRoomBlueprint

```lua
C_HousingBlueprint.StartImportRoomBlueprint(shareCode: cstring)
```

Start the process of importing a Room Blueprint. This will lead to Layout Mode being opened, so the player can then select an available door to attach the room to

`SecretArguments=AllowedWhenUntainted`

### UpdateBlueprintStringFromInput

```lua
C_HousingBlueprint.UpdateBlueprintStringFromInput(inputShareCode: cstring) -> updatedShareCode: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

## Events

### HOUSING_BLUEPRINT_COLLECTION_FAILURE

```lua
HOUSING_BLUEPRINT_COLLECTION_FAILURE(result: HousingResult)
```

`SynchronousEvent`

### HOUSING_BLUEPRINT_COLLECTION_RECEIVED

```lua
HOUSING_BLUEPRINT_COLLECTION_RECEIVED(collection: HousingBlueprintCollection)
```

`SynchronousEvent`

### HOUSING_BLUEPRINT_CONTENTS_FAILURE

```lua
HOUSING_BLUEPRINT_CONTENTS_FAILURE(blueprintShareCode: string, result: HousingResult)
```

`SynchronousEvent`

### HOUSING_BLUEPRINT_CONTENTS_RECEIVED

```lua
HOUSING_BLUEPRINT_CONTENTS_RECEIVED(contentInfo: HousingBlueprintContentInfo)
```

`SynchronousEvent`

### HOUSING_BLUEPRINT_DELETE_FAILURE

```lua
HOUSING_BLUEPRINT_DELETE_FAILURE(blueprintID: BigUInteger, result: HousingResult)
```

`SynchronousEvent`

### HOUSING_BLUEPRINT_DELETE_SUCCESS

```lua
HOUSING_BLUEPRINT_DELETE_SUCCESS(blueprintID: BigUInteger)
```

`SynchronousEvent`

### HOUSING_BLUEPRINT_EXPORT_FAILURE

```lua
HOUSING_BLUEPRINT_EXPORT_FAILURE(result: HousingResult)
```

`SynchronousEvent`

### HOUSING_BLUEPRINT_EXPORT_SUCCESS

```lua
HOUSING_BLUEPRINT_EXPORT_SUCCESS(blueprintShareCode: string)
```

`SynchronousEvent`

### HOUSING_BLUEPRINT_IMPORT_FAILURE

```lua
HOUSING_BLUEPRINT_IMPORT_FAILURE(result: HousingResult)
```

`SynchronousEvent`

### HOUSING_BLUEPRINT_IMPORT_STARTED

```lua
HOUSING_BLUEPRINT_IMPORT_STARTED()
```

`SynchronousEvent`

### HOUSING_BLUEPRINT_IMPORT_SUCCESS

```lua
HOUSING_BLUEPRINT_IMPORT_SUCCESS()
```

`SynchronousEvent`

### HOUSING_BLUEPRINT_RENAME_FAILURE

```lua
HOUSING_BLUEPRINT_RENAME_FAILURE(blueprintID: BigUInteger, result: HousingResult)
```

`SynchronousEvent`

### HOUSING_BLUEPRINT_RENAME_SUCCESS

```lua
HOUSING_BLUEPRINT_RENAME_SUCCESS(blueprintID: BigUInteger, name: string)
```

`SynchronousEvent`

### HOUSING_BLUEPRINTS_AVAILABILITY_CHANGED

```lua
HOUSING_BLUEPRINTS_AVAILABILITY_CHANGED()
```

`SynchronousEvent`
