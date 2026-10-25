# DyeColorInfo

Namespace `C_DyeColor` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/dyecolorinfodocumentation.lua` (FileDataID 6637346)

## Functions

### GetAllDyeColorCategories

```lua
C_DyeColor.GetAllDyeColorCategories() -> dyeColorCategoryIDs: number[]
```

### GetAllDyeColors

```lua
C_DyeColor.GetAllDyeColors(ownedColorsOnly: bool) -> dyeColorIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `ownedColorsOnly` | `bool` | default `false` |

### GetDyeColorCategoryInfo

```lua
C_DyeColor.GetDyeColorCategoryInfo(dyeColorCategoryID: number) -> dyeColorCategoryInfo: DyeColorCategoryDisplayInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetDyeColorInfo

```lua
C_DyeColor.GetDyeColorInfo(dyeColorID: number) -> dyeColorInfo: DyeColorDisplayInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetDyeColorsForItem

```lua
C_DyeColor.GetDyeColorsForItem(itemLinkOrID: ItemInfo) -> dyeColorIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetDyeColorsForItemLocation

```lua
C_DyeColor.GetDyeColorsForItemLocation(itemLocation: ItemLocation) -> dyeColorIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### GetDyeColorsInCategory

```lua
C_DyeColor.GetDyeColorsInCategory(dyeColorCategory: number, ownedColorsOnly: bool) -> dyeColorIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `dyeColorCategory` | `number` |  |
| `ownedColorsOnly` | `bool` | default `false` |

### IsDyeColorOwned

```lua
C_DyeColor.IsDyeColorOwned(dyeColorID: number) -> isOwned: bool
```

True if the player owns any of the consumable item used to apply the specified dye

`SecretArguments=AllowedWhenUntainted`

## Events

### DYE_COLOR_CATEGORY_UPDATED

```lua
DYE_COLOR_CATEGORY_UPDATED(dyeColorCategoryID: number)
```

`SynchronousEvent`

### DYE_COLOR_UPDATED

```lua
DYE_COLOR_UPDATED(dyeColorID: number)
```

`SynchronousEvent`
