---
name: wow-addon-api-wowf
description: Exact Lua API reference for World of Warcraft wowf 1.60.1.70532 (build WOW-70532patch1.60.1_Retail), generated from the game client's own interface files. Use when writing, debugging or reviewing WoW addon code (Lua, XML, .toc files), when checking whether an API function, event, enum, widget method or FrameXML template exists in this game version, or when looking up arguments, return values, event payloads and combat or secret-value restrictions.
---

# World of Warcraft addon API (wowf 1.60.1.70532)

These files describe the Lua API of exactly this game build: 5,140 API functions,
1,477 widget methods, 1,814 events, 900 enums and
4,363 FrameXML templates. WoW's API changes a lot between expansions and client flavours.
Functions move into `C_` namespaces, get renamed or disappear. **When these files disagree with what you
remember, trust the files.** All paths below are relative to this skill's folder.

## Looking things up

1. **Search `signatures.txt` first.** It has one line per symbol, prefixed by its kind (`fn`, `method`,
   `event`, `enum`, `const`, `struct`, `callback`), followed by `# <doc file>`.

   For example, `grep -F 'fn C_Item.GetItemInfo(' signatures.txt` finds:

   ```
   fn C_Item.GetItemInfo(itemInfo: ItemInfo) -> itemName: cstring, itemLink: cstring, itemQuality: ItemQuality, itemLevel: number, itemMinLevel: number, itemType: cstring, itemSubType: cstring, itemStackCount: number, itemEquipLoc: cstring, itemTexture: fileID, sellPrice: number, classID: number, subclassID: number, bindType: number, expansionID: number, setID: number?, isCraftingReagent: bool, itemDescription: cstring  # api/systems/Item.md
   ```

2. **Open the doc file it names** (`api/systems/<System>.md` or `api/widgets/<Widget>.md`) for
   descriptions, default values and restriction flags.
3. **Resolve named types** with `grep -E '^(struct|enum Enum\.|callback) <Name>\b' signatures.txt`.
4. **Events:** `grep '^event <NAME>(' signatures.txt` shows the payload in the order `OnEvent` receives it.
   `api/events.md` lists them all by system.
5. **Blizzard UI code** (`framexml/templates.md`, `framexml/mixins.md`, `framexml/functions.md`) covers
   templates for `CreateFrame`, mixins such as `CallbackRegistryMixin`, and helper functions. Each entry
   gives `path:line` in the client's interface code. These exist only once that part of Blizzard's UI has
   loaded, and they change more often than the C API.
6. Search by keyword when you don't know the name: `grep -i 'mount' signatures.txt | grep '^fn'`.

Avoid reading `api.json` (10.7 MB) or `framexml/mixins.md` (2.3 MB) whole.
Grep them, or use `jq` on `api.json` for structured queries.

## Rules for writing addon code

- Only call functions, methods and events that appear in `signatures.txt` or `framexml/`. If something
  you expected is missing, say so and search for its replacement. Don't guess at an API.
- A `?` after a type means `nil` is possible: check before using the value. Functions flagged
  `MayReturnNothing` can return no values at all.
- `[protected]` in `signatures.txt` (`IsProtectedFunction` in the docs) marks functions that only secure
  code may call. Addon code reaches them through secure templates (search `framexml/templates.md` for
  `Secure`) activated by the player, such as a click on a secure button. Calling them directly fails.
  Don't modify protected frames while `InCombatLockdown()` returns true.
- Flags starting with `Secret` (such as `SecretWhenInCombat`) name the conditions under which values become
  *secret* to addon code. A secret value can be passed back to the API or displayed (for example with
  `FontString:SetText`), but not compared or used in arithmetic, so code must not branch on it.
- Use `Enum.<Name>.<Value>` instead of hard-coded numbers. Enum values are listed in `api/enums.md`.
- The game runs Lua 5.1: no `goto`, no integer division `//` and no bitwise operators (use the `bit`
  library, e.g. `bit.band`).
- Widget methods are inherited, so a `Button` also has every `Frame`, `ScriptRegion` and `Object` method.
  The documented types inherit from these parents:
  - `AnimatableObject`: ScriptRegion
  - `Animation`: Alpha, FlipBook, LineScale, LineTranslation, Path, Rotation, Scale, TextureCoordTranslation, Translation, VertexColor
  - `Button`: CheckButton
  - `FontInstance`: EditBox, FontString, MessageFrame, SimpleHTML
  - `Frame`: Browser, Button, ColorSelect, Cooldown, EditBox, GameTooltip, MessageFrame, Minimap, Model, ModelScene, MovieFrame, ScrollFrame, SimpleHTML, Slider, StatusBar
  - `FrameScriptObject`: Object
  - `Model`: PlayerModel
  - `ModelSceneActorBase`: ModelSceneActor
  - `Object`: Animation, AnimationGroup, ControlPoint, FontInstance, ScriptRegion
  - `PlayerModel`: CinematicModel, DressUpModel, TabardModelBase
  - `Region`: FontString, TextureBase
  - `ScriptRegion`: Frame, Region
  - `ScriptRegionResizing`: ScriptRegion
  - `TabardModelBase`: TabardModel
  - `TextureBase`: Line, MaskTexture, Texture

## Addon layout

```
Interface/AddOns/MyAddon/
  MyAddon.toc
  MyAddon.lua
```

```
## Interface: <number from /dump select(4, GetBuildInfo()) in game>
## Title: My Addon
## SavedVariables: MyAddonDB
MyAddon.lua
```

```lua
local addonName, ns = ...            -- every file of the addon receives the same private table ns

local frame = CreateFrame("Frame")
frame:RegisterEvent("ADDON_LOADED")
frame:SetScript("OnEvent", function(self, event, name)
  if name ~= addonName then return end
  MyAddonDB = MyAddonDB or {}       -- saved variables are loaded by now
  self:UnregisterEvent("ADDON_LOADED")
end)

SLASH_MYADDON1 = "/myaddon"
SlashCmdList.MYADDON = function(msg) print(addonName, msg) end
```

Check every event and function used in such code against `signatures.txt` for this build, including the
ones in this example.

## Editor support

`luals/` contains `---@meta` stubs for the Lua language server. Add the folder to `workspace.library` in
the addon's `.luarc.json` together with `"runtime.version": "Lua 5.1"`.

## Files

| File | Size | Contents |
|---|---|---|
| `signatures.txt` | 1.2 MB | every symbol, one per line |
| `api/systems/*.md` | 560 files | API systems: functions, events, types |
| `api/widgets/*.md` | 81 files | widget methods |
| `api/events.md` | 130 KB | events with payloads |
| `api/enums.md` | 244 KB | `Enum.*` and constants |
| `framexml/templates.md` | 654 KB | XML templates and intrinsic frames |
| `framexml/mixins.md` | 2.3 MB | mixins and utility tables with methods |
| `framexml/functions.md` | 814 KB | global Lua functions in Blizzard's UI |
| `luals/*.lua` | 1 MB | language server stubs |
| `api.json` | 10.7 MB | all of the above as data |
| `README.md` | 4 KB | overview for people |
