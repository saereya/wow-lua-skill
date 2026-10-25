# Soulbinds

Namespace `C_Soulbinds` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/soulbindsdocumentation.lua` (FileDataID 4637246)

## Functions

### ActivateSoulbind

```lua
C_Soulbinds.ActivateSoulbind(soulbindID: number)
```

`SecretArguments=AllowedWhenUntainted`

### CanActivateSoulbind

```lua
C_Soulbinds.CanActivateSoulbind(soulbindID: number) -> result: bool, errorDescription: cstring?
```

`SecretArguments=AllowedWhenUntainted`

### CanModifySoulbind

```lua
C_Soulbinds.CanModifySoulbind() -> result: bool
```

### CanResetConduitsInSoulbind

```lua
C_Soulbinds.CanResetConduitsInSoulbind(soulbindID: number) -> result: bool, errorDescription: cstring?
```

`SecretArguments=AllowedWhenUntainted`

### CanSwitchActiveSoulbindTreeBranch

```lua
C_Soulbinds.CanSwitchActiveSoulbindTreeBranch() -> result: bool
```

### CloseUI

```lua
C_Soulbinds.CloseUI()
```

### CommitPendingConduitsInSoulbind

```lua
C_Soulbinds.CommitPendingConduitsInSoulbind(soulbindID: number)
```

`SecretArguments=AllowedWhenUntainted`

### FindNodeIDActuallyInstalled

```lua
C_Soulbinds.FindNodeIDActuallyInstalled(soulbindID: number, conduitID: number) -> nodeID: number
```

`SecretArguments=AllowedWhenUntainted`

### FindNodeIDAppearingInstalled

```lua
C_Soulbinds.FindNodeIDAppearingInstalled(soulbindID: number, conduitID: number) -> nodeID: number
```

`SecretArguments=AllowedWhenUntainted`

### FindNodeIDPendingInstall

```lua
C_Soulbinds.FindNodeIDPendingInstall(soulbindID: number, conduitID: number) -> nodeID: number
```

`SecretArguments=AllowedWhenUntainted`

### FindNodeIDPendingUninstall

```lua
C_Soulbinds.FindNodeIDPendingUninstall(soulbindID: number, conduitID: number) -> nodeID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetActiveSoulbindID

```lua
C_Soulbinds.GetActiveSoulbindID() -> soulbindID: number
```

### GetConduitCollection

```lua
C_Soulbinds.GetConduitCollection(conduitType: SoulbindConduitType) -> collectionData: ConduitCollectionData[]
```

`SecretArguments=AllowedWhenUntainted`

### GetConduitCollectionCount

```lua
C_Soulbinds.GetConduitCollectionCount() -> count: number
```

### GetConduitCollectionData

```lua
C_Soulbinds.GetConduitCollectionData(conduitID: number) -> collectionData: ConduitCollectionData?
```

`SecretArguments=AllowedWhenUntainted`

### GetConduitCollectionDataAtCursor

```lua
C_Soulbinds.GetConduitCollectionDataAtCursor() -> collectionData: ConduitCollectionData?
```

### GetConduitCollectionDataByVirtualID

```lua
C_Soulbinds.GetConduitCollectionDataByVirtualID(virtualID: number) -> collectionData: ConduitCollectionData?
```

`SecretArguments=AllowedWhenUntainted`

### GetConduitDisplayed

```lua
C_Soulbinds.GetConduitDisplayed(nodeID: number) -> conduitID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetConduitHyperlink

```lua
C_Soulbinds.GetConduitHyperlink(conduitID: number, rank: number) -> link: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetConduitIDPendingInstall

```lua
C_Soulbinds.GetConduitIDPendingInstall(nodeID: number) -> conduitID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetConduitQuality

```lua
C_Soulbinds.GetConduitQuality(conduitID: number, rank: number) -> quality: number
```

`SecretArguments=AllowedWhenUntainted`

### GetConduitRank

```lua
C_Soulbinds.GetConduitRank(conduitID: number) -> conduitRank: number
```

`SecretArguments=AllowedWhenUntainted`

### GetConduitSpellID

```lua
C_Soulbinds.GetConduitSpellID(conduitID: number, conduitRank: number) -> spellID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetInstalledConduitID

```lua
C_Soulbinds.GetInstalledConduitID(nodeID: number) -> conduitID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetNode

```lua
C_Soulbinds.GetNode(nodeID: number) -> node: SoulbindNode
```

`SecretArguments=AllowedWhenUntainted`

### GetSoulbindData

```lua
C_Soulbinds.GetSoulbindData(soulbindID: number) -> data: SoulbindData
```

`SecretArguments=AllowedWhenUntainted`

### GetSpecsAssignedToSoulbind

```lua
C_Soulbinds.GetSpecsAssignedToSoulbind(soulbindID: number) -> specIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetTree

```lua
C_Soulbinds.GetTree(treeID: number) -> tree: SoulbindTree
```

`SecretArguments=AllowedWhenUntainted`

### HasAnyInstalledConduitInSoulbind

```lua
C_Soulbinds.HasAnyInstalledConduitInSoulbind(soulbindID: number) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### HasAnyPendingConduits

```lua
C_Soulbinds.HasAnyPendingConduits() -> result: bool
```

### HasPendingConduitsInSoulbind

```lua
C_Soulbinds.HasPendingConduitsInSoulbind(soulbindID: number) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsConduitInstalled

```lua
C_Soulbinds.IsConduitInstalled(nodeID: number) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsConduitInstalledInSoulbind

```lua
C_Soulbinds.IsConduitInstalledInSoulbind(soulbindID: number, conduitID: number) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsItemConduitByItemInfo

```lua
C_Soulbinds.IsItemConduitByItemInfo(itemInfo: ItemInfo) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsNodePendingModify

```lua
C_Soulbinds.IsNodePendingModify(nodeID: number) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsUnselectedConduitPendingInSoulbind

```lua
C_Soulbinds.IsUnselectedConduitPendingInSoulbind(soulbindID: number) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### ModifyNode

```lua
C_Soulbinds.ModifyNode(nodeID: number, conduitID: number, type: SoulbindConduitTransactionType)
```

`SecretArguments=AllowedWhenUntainted`

### SelectNode

```lua
C_Soulbinds.SelectNode(nodeID: number)
```

`SecretArguments=AllowedWhenUntainted`

### UnmodifyNode

```lua
C_Soulbinds.UnmodifyNode(nodeID: number)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### SOULBIND_ACTIVATED

```lua
SOULBIND_ACTIVATED(soulbindID: number)
```

`SynchronousEvent`

### SOULBIND_CONDUIT_COLLECTION_CLEARED

```lua
SOULBIND_CONDUIT_COLLECTION_CLEARED()
```

`SynchronousEvent`

### SOULBIND_CONDUIT_COLLECTION_REMOVED

```lua
SOULBIND_CONDUIT_COLLECTION_REMOVED(conduitID: number)
```

`SynchronousEvent`

### SOULBIND_CONDUIT_COLLECTION_UPDATED

```lua
SOULBIND_CONDUIT_COLLECTION_UPDATED(collectionData: ConduitCollectionData)
```

`SynchronousEvent`

### SOULBIND_CONDUIT_INSTALLED

```lua
SOULBIND_CONDUIT_INSTALLED(nodeID: number, data: SoulbindConduitData)
```

`SynchronousEvent`

### SOULBIND_CONDUIT_UNINSTALLED

```lua
SOULBIND_CONDUIT_UNINSTALLED(nodeID: number, data: SoulbindConduitData)
```

`SynchronousEvent`

### SOULBIND_FORGE_INTERACTION_ENDED

```lua
SOULBIND_FORGE_INTERACTION_ENDED()
```

`SynchronousEvent`

### SOULBIND_FORGE_INTERACTION_STARTED

```lua
SOULBIND_FORGE_INTERACTION_STARTED()
```

`SynchronousEvent`

### SOULBIND_NODE_LEARNED

```lua
SOULBIND_NODE_LEARNED(nodeID: number)
```

`SynchronousEvent`

### SOULBIND_NODE_UNLEARNED

```lua
SOULBIND_NODE_UNLEARNED(nodeID: number)
```

`SynchronousEvent`

### SOULBIND_NODE_UPDATED

```lua
SOULBIND_NODE_UPDATED(nodeID: number)
```

`SynchronousEvent`

### SOULBIND_PATH_CHANGED

```lua
SOULBIND_PATH_CHANGED()
```

`SynchronousEvent`

### SOULBIND_PENDING_CONDUIT_CHANGED

```lua
SOULBIND_PENDING_CONDUIT_CHANGED(nodeID: number, conduitID: number)
```

`SynchronousEvent`

## Types

### ConduitCollectionData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `conduitID` | `number` |  |
| `conduitRank` | `number` |  |
| `conduitItemLevel` | `number` |  |
| `conduitType` | `SoulbindConduitType` |  |
| `conduitSpecSetID` | `number` |  |
| `conduitSpecIDs` | `number[]` |  |
| `conduitSpecName` | `cstring?` |  |
| `covenantID` | `number?` |  |
| `conduitItemID` | `number` |  |

### SoulbindConduitData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `conduitID` | `number` |  |
| `conduitRank` | `number` |  |

### SoulbindData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ID` | `number` |  |
| `covenantID` | `number` |  |
| `name` | `cstring` |  |
| `description` | `cstring` |  |
| `textureKit` | `textureKit` |  |
| `unlocked` | `bool` |  |
| `cvarIndex` | `luaIndex` |  |
| `tree` | `SoulbindTree` |  |
| `modelSceneData` | `SoulbindModelSceneData` |  |
| `activationSoundKitID` | `number` |  |
| `playerConditionReason` | `cstring?` |  |

### SoulbindModelSceneData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `creatureDisplayInfoID` | `number` |  |
| `modelSceneActorID` | `number` |  |

### SoulbindNode

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ID` | `number` |  |
| `row` | `number` |  |
| `column` | `number` |  |
| `icon` | `fileID` |  |
| `spellID` | `number` |  |
| `playerConditionReason` | `cstring?` |  |
| `conduitID` | `number` |  |
| `conduitRank` | `number` |  |
| `state` | `SoulbindNodeState` |  |
| `conduitType` | `SoulbindConduitType?` |  |
| `parentNodeIDs` | `number[]` |  |
| `failureRenownRequirement` | `number?` |  |
| `socketEnhanced` | `bool?` |  |

### SoulbindTree

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `editable` | `bool` |  |
| `nodes` | `SoulbindNode[]` |  |
