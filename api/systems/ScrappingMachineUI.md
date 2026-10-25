# ScrappingMachineUI

Namespace `C_ScrappingMachineUI` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/scrappingmachineuidocumentation.lua` (FileDataID 4637193)

## Functions

### CloseScrappingMachine

```lua
C_ScrappingMachineUI.CloseScrappingMachine()
```

### DropPendingScrapItemFromCursor

```lua
C_ScrappingMachineUI.DropPendingScrapItemFromCursor(index: number)
```

`SecretArguments=AllowedWhenUntainted`

### GetCurrentPendingScrapItemLocationByIndex

```lua
C_ScrappingMachineUI.GetCurrentPendingScrapItemLocationByIndex(index: number) -> itemLoc: ItemLocation
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `itemLoc` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### GetScrappingMachineName

```lua
C_ScrappingMachineUI.GetScrappingMachineName() -> name: string
```

`MayReturnNothing`

### GetScrapSpellID

```lua
C_ScrappingMachineUI.GetScrapSpellID() -> spellID: number
```

### HasScrappableItems

```lua
C_ScrappingMachineUI.HasScrappableItems() -> hasScrappableItems: bool
```

### RemoveAllScrapItems

```lua
C_ScrappingMachineUI.RemoveAllScrapItems()
```

### RemoveCurrentScrappingItem

```lua
C_ScrappingMachineUI.RemoveCurrentScrappingItem()
```

### RemoveItemToScrap

```lua
C_ScrappingMachineUI.RemoveItemToScrap(index: number)
```

`SecretArguments=AllowedWhenUntainted`

### ScrapItems

```lua
C_ScrappingMachineUI.ScrapItems()
```

### ValidateScrappingList

```lua
C_ScrappingMachineUI.ValidateScrappingList()
```

## Events

### SCRAPPING_MACHINE_ITEM_ADDED

```lua
SCRAPPING_MACHINE_ITEM_ADDED(index: number)
```

`SynchronousEvent`

### SCRAPPING_MACHINE_ITEM_REMOVED

```lua
SCRAPPING_MACHINE_ITEM_REMOVED(index: number)
```

`SynchronousEvent`

### SCRAPPING_MACHINE_PENDING_ITEM_CHANGED

```lua
SCRAPPING_MACHINE_PENDING_ITEM_CHANGED()
```

`SynchronousEvent`

### SCRAPPING_MACHINE_SCRAPPING_FINISHED

```lua
SCRAPPING_MACHINE_SCRAPPING_FINISHED()
```

`SynchronousEvent`
