# SharedTraits

Namespace `C_Traits` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/sharedtraitsdocumentation.lua` (FileDataID 4637201)

## Functions

### CanEditConfig

```lua
C_Traits.CanEditConfig(configID: number) -> canEdit: bool, errorMessage: cstring
```

Returns whether the player can make changes to the specified talent config.

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `canEdit` | `bool` |  |
| `errorMessage` | `cstring` | If canEdit is false, this will be filled out with text explaining why the player can not make changes. |

### CanPurchaseRank

```lua
C_Traits.CanPurchaseRank(configID: number, nodeID: number, nodeEntryID: number) -> canPurchase: bool
```

`SecretArguments=AllowedWhenUntainted`

### CanRefundRank

```lua
C_Traits.CanRefundRank(configID: number, nodeID: number) -> canRefund: bool
```

`SecretArguments=AllowedWhenUntainted`

### CascadeRepurchaseRanks

```lua
C_Traits.CascadeRepurchaseRanks(configID: number, nodeID: number, entryID: number?) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### ClearCascadeRepurchaseHistory

```lua
C_Traits.ClearCascadeRepurchaseHistory(configID: number)
```

`SecretArguments=AllowedWhenUntainted`

### CloseTraitSystemInteraction

```lua
C_Traits.CloseTraitSystemInteraction()
```

### CommitConfig

```lua
C_Traits.CommitConfig(configID: number) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### ConfigHasStagedChanges

```lua
C_Traits.ConfigHasStagedChanges(configID: number) -> hasChanges: bool
```

`SecretArguments=AllowedWhenUntainted`

### GenerateImportString

```lua
C_Traits.GenerateImportString(configID: number) -> importString: string
```

`SecretArguments=AllowedWhenUntainted`

### GenerateInspectImportString

```lua
C_Traits.GenerateInspectImportString(target: cstring) -> importString: string
```

`SecretArguments=AllowedWhenUntainted`

### GetConditionInfo

```lua
C_Traits.GetConditionInfo(configID: number, condID: number) -> condInfo: TraitCondInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetConfigIDBySystemID

```lua
C_Traits.GetConfigIDBySystemID(systemID: number) -> configID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetConfigIDByTreeID

```lua
C_Traits.GetConfigIDByTreeID(treeID: number) -> configID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetConfigInfo

```lua
C_Traits.GetConfigInfo(configID: number) -> configInfo: TraitConfigInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetConfigsByType

```lua
C_Traits.GetConfigsByType(configType: TraitConfigType) -> configIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetConfigVariationID

```lua
C_Traits.GetConfigVariationID(systemID: number) -> variationID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetDefinitionInfo

```lua
C_Traits.GetDefinitionInfo(definitionID: number) -> definitionInfo: TraitDefinitionInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetEntryInfo

```lua
C_Traits.GetEntryInfo(configID: number, entryID: number) -> entryInfo: TraitEntryInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetGroupCurrencyInfo

```lua
C_Traits.GetGroupCurrencyInfo(configID: number, groupIDs: number[]) -> groupCurrencyInfos: GroupCurrencyInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetGroupDisplayInfoByTreeID

```lua
C_Traits.GetGroupDisplayInfoByTreeID(treeID: number) -> displayInfos: TraitGroupDisplayInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetIncreasedTraitData

```lua
C_Traits.GetIncreasedTraitData(nodeID: number, entryID: number) -> itemName: IncreasedTraitData[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetLoadoutSerializationVersion

```lua
C_Traits.GetLoadoutSerializationVersion() -> serializationVersion: number
```

### GetMaxAvailableTraitCurrency

```lua
C_Traits.GetMaxAvailableTraitCurrency(traitCurrencyID: number, limitBySourcedMax: bool) -> maxAvailable: number
```

`SecretArguments=AllowedWhenUntainted`

### GetNodeCost

```lua
C_Traits.GetNodeCost(configID: number, nodeID: number) -> costs: TraitCurrencyCost[]
```

`SecretArguments=AllowedWhenUntainted`

### GetNodeInfo

```lua
C_Traits.GetNodeInfo(configID: number, nodeID: number) -> nodeInfo: TraitNodeInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetStagedChanges

```lua
C_Traits.GetStagedChanges(configID: number) -> nodeIDsWithPurchases: number[], nodeIDsWithRefunds: number[], nodeIDsWithSelectionSwaps: number[]
```

Returns IDs of Trait Nodes with pending changes, grouped by the type of change; Returns nothing if there are no pending changes

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `nodeIDsWithPurchases` | `number[]` |  |
| `nodeIDsWithRefunds` | `number[]` |  |
| `nodeIDsWithSelectionSwaps` | `number[]` | Selection nodes that had a previously committed selected entry, and now have a different selected entry pending |

### GetStagedChangesCost

```lua
C_Traits.GetStagedChangesCost(configID: number) -> costs: TraitCurrencyCost[]
```

`SecretArguments=AllowedWhenUntainted`

### GetSubTreeInfo

```lua
C_Traits.GetSubTreeInfo(configID: number, subTreeID: number) -> subTreeInfo: TraitSubTreeInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSystemIDByTreeID

```lua
C_Traits.GetSystemIDByTreeID(treeID: number) -> systemID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetTraitCurrencyForAchievement

```lua
C_Traits.GetTraitCurrencyForAchievement(traitCurrencyID: number, achievementID: number) -> amount: number
```

`SecretArguments=AllowedWhenUntainted`

### GetTraitCurrencyInfo

```lua
C_Traits.GetTraitCurrencyInfo(traitCurrencyID: number) -> flags: number, type: number, currencyTypesID: number?, icon: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetTraitDescription

```lua
C_Traits.GetTraitDescription(entryID: number, rank: number) -> description: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetTraitSystemFlags

```lua
C_Traits.GetTraitSystemFlags(configID: number) -> flags: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetTraitSystemWidgetSetID

```lua
C_Traits.GetTraitSystemWidgetSetID(configID: number) -> uiWidgetSetID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetTreeCurrencyInfo

```lua
C_Traits.GetTreeCurrencyInfo(configID: number, treeID: number, excludeStagedChanges: bool) -> treeCurrencyInfo: TreeCurrencyInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetTreeHash

```lua
C_Traits.GetTreeHash(treeID: number) -> result: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetTreeInfo

```lua
C_Traits.GetTreeInfo(configID: number, treeID: number) -> treeInfo: TraitTreeInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetTreeNodes

```lua
C_Traits.GetTreeNodes(treeID: number) -> nodeIDs: number[]
```

Returns a list of nodeIDs, sorted ascending, for a given treeID. Contains nodes for all class specializations.

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### HasValidInspectData

```lua
C_Traits.HasValidInspectData() -> hasValidInspectData: bool
```

### IsReadyForCommit

```lua
C_Traits.IsReadyForCommit() -> isReadyForCommit: bool
```

### PurchaseAllRanks

```lua
C_Traits.PurchaseAllRanks(configID: number, nodeID: number, ignoreCost: bool) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### PurchaseRank

```lua
C_Traits.PurchaseRank(configID: number, nodeID: number) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### RefundAllRanks

```lua
C_Traits.RefundAllRanks(configID: number, nodeID: number) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### RefundRank

```lua
C_Traits.RefundRank(configID: number, nodeID: number, clearEdges: bool?) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### ResetTree

```lua
C_Traits.ResetTree(configID: number, treeID: number) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### ResetTreeByCurrency

```lua
C_Traits.ResetTreeByCurrency(configID: number, treeID: number, traitCurrencyID: number) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### RollbackConfig

```lua
C_Traits.RollbackConfig(configID: number) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetSelection

```lua
C_Traits.SetSelection(configID: number, nodeID: number, nodeEntryID: number?, clearEdges: bool?) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### StageConfig

```lua
C_Traits.StageConfig(configID: number) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### TalentTestUnlearnSpells

```lua
C_Traits.TalentTestUnlearnSpells()
```

### TryPurchaseAllRanks

```lua
C_Traits.TryPurchaseAllRanks(configID: number, nodeID: number) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### TryPurchaseToNode

```lua
C_Traits.TryPurchaseToNode(configID: number, nodeID: number) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### TryRefundToNode

```lua
C_Traits.TryRefundToNode(configID: number, nodeID: number, entryID: number) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

## Events

### CONFIG_COMMIT_FAILED

```lua
CONFIG_COMMIT_FAILED(configID: number)
```

`SynchronousEvent`

### TRAIT_COND_INFO_CHANGED

```lua
TRAIT_COND_INFO_CHANGED(condID: number)
```

`SynchronousEvent`

### TRAIT_CONFIG_CREATED

```lua
TRAIT_CONFIG_CREATED(configInfo: TraitConfigInfo)
```

`SynchronousEvent`

### TRAIT_CONFIG_DELETED

```lua
TRAIT_CONFIG_DELETED(configID: number)
```

`SynchronousEvent`

### TRAIT_CONFIG_LIST_UPDATED

```lua
TRAIT_CONFIG_LIST_UPDATED()
```

`SynchronousEvent`

### TRAIT_CONFIG_UPDATED

```lua
TRAIT_CONFIG_UPDATED(configID: number)
```

`SynchronousEvent`

### TRAIT_NODE_CHANGED

```lua
TRAIT_NODE_CHANGED(nodeID: number)
```

`SynchronousEvent`

### TRAIT_NODE_CHANGED_PARTIAL

```lua
TRAIT_NODE_CHANGED_PARTIAL(ID: number, info: TraitNodeInfoPartial)
```

`SynchronousEvent`

### TRAIT_NODE_ENTRY_UPDATED

```lua
TRAIT_NODE_ENTRY_UPDATED(nodeEntryID: number)
```

`SynchronousEvent`

### TRAIT_SUB_TREE_CHANGED

```lua
TRAIT_SUB_TREE_CHANGED(subTreeID: number)
```

`SynchronousEvent`

### TRAIT_SYSTEM_INTERACTION_STARTED

```lua
TRAIT_SYSTEM_INTERACTION_STARTED(treeID: number)
```

`SynchronousEvent`

### TRAIT_SYSTEM_NPC_CLOSED

```lua
TRAIT_SYSTEM_NPC_CLOSED()
```

`SynchronousEvent`

### TRAIT_TREE_CHANGED

```lua
TRAIT_TREE_CHANGED(treeID: number)
```

`SynchronousEvent`

### TRAIT_TREE_CURRENCY_INFO_UPDATED

```lua
TRAIT_TREE_CURRENCY_INFO_UPDATED(treeID: number)
```

`SynchronousEvent`

### TRY_PURCHASE_TO_NODE_PARTIAL_SUCCESS

```lua
TRY_PURCHASE_TO_NODE_PARTIAL_SUCCESS(nodeFinishedOn: number)
```

`SynchronousEvent`

## Types

### GroupCurrencyInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `traitNodeGroupID` | `number` |  |
| `currencyInfos` | `TreeCurrencyInfo[]` |  |

### IncreasedTraitData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `itemNameIncreasing` | `string` |  |
| `itemQualityIncreasing` | `ItemQuality` |  |
| `numPointsIncreased` | `number` |  |

### TraitCondInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `condID` | `number` |  |
| `ranksGranted` | `number?` |  |
| `isAlwaysMet` | `bool` |  |
| `isMet` | `bool` | True if the source for the condition has been fulfilled. |
| `isGate` | `bool` |  |
| `isSufficient` | `bool` | True if meeting the requirements for the condition means any nodes using this condition are considered fulfilled if the condition is met. |
| `type` | `number` | The value from the TraitConditionType enum the condition uses. |
| `questID` | `number?` |  |
| `achievementID` | `number?` |  |
| `specSetID` | `number?` |  |
| `playerLevel` | `number?` |  |
| `traitCurrencyID` | `number?` |  |
| `spentAmountRequired` | `number?` |  |
| `tooltipFormat` | `string?` |  |
| `traitCondAccountElementID` | `number?` |  |

### TraitConfigInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ID` | `number` |  |
| `type` | `TraitConfigType` |  |
| `name` | `string` |  |
| `treeIDs` | `number[]` |  |
| `usesSharedActionBars` | `bool` |  |

### TraitCurrencyCost

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ID` | `number` |  |
| `amount` | `number` |  |

### TraitDefinitionInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `number?` |  |
| `overrideName` | `string?` |  |
| `overrideSubtext` | `string?` |  |
| `overrideDescription` | `string?` |  |
| `overrideIcon` | `number?` |  |
| `overriddenSpellID` | `number?` |  |
| `subType` | `TraitDefinitionSubType?` |  |

### TraitEntryInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `definitionID` | `number?` | Nil on SubTreeSelection Node Entries |
| `subTreeID` | `number?` | Populated only on SubTreeSelection Node Entries; This is the SubTree that is activated if this Entry is chosen |
| `type` | `TraitNodeEntryType` |  |
| `maxRanks` | `number` |  |
| `isAvailable` | `bool` |  |
| `isDisplayError` | `bool` | True if this entry fails the TRAIT_CONDITION_TYPE_DISPLAY_ERROR condition check. Used to communicate a problem with the node to the player (e.g. A prerequisite node has not been purchased.) but will not prevent the player from spending points on the node. |
| `conditionIDs` | `number[]` |  |

### TraitEntryRankInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `entryID` | `number` |  |
| `rank` | `number` |  |

### TraitGateInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `topLeftNodeID` | `number` |  |
| `conditionID` | `number` |  |

### TraitGroupDisplayInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `groupID` | `number` |  |
| `treeID` | `number` |  |
| `skillLineID` | `number` |  |
| `orderIndex` | `number` |  |
| `displayName` | `cstring` |  |
| `icon` | `number` |  |

### TraitNodeInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ID` | `number` |  |
| `posX` | `number` |  |
| `posY` | `number` |  |
| `flags` | `number` |  |
| `entryIDs` | `number[]` |  |
| `entryIDsWithCommittedRanks` | `number[]` |  |
| `canPurchaseRank` | `bool` |  |
| `canRefundRank` | `bool` |  |
| `isAvailable` | `bool` |  |
| `isVisible` | `bool` |  |
| `isDisplayError` | `bool` | True if this node fails the TRAIT_CONDITION_TYPE_DISPLAY_ERROR condition check. Used to communicate a problem with the node to the player (e.g. A prerequisite node has not been purchased.) but will not prevent the player from spending points on the node. |
| `ranksPurchased` | `number` |  |
| `ranksIncreased` | `number` |  |
| `entryIDToRanksIncreased` | `LuaValueVariant` | A map of the entry IDs on this node to the number of ranks increased. This covers all entries on the node, which is important in the case of selection nodes where we have more than one option that could be increased. |
| `activeRank` | `number` |  |
| `currentRank` | `number` |  |
| `activeEntry` | `TraitEntryRankInfo?` |  |
| `nextEntry` | `TraitEntryRankInfo?` |  |
| `maxRanks` | `number` |  |
| `totalMaxRanks` | `number` |  |
| `type` | `TraitNodeType` |  |
| `visibleEdges` | `TraitOutEdgeInfo[]` |  |
| `meetsEdgeRequirements` | `bool` |  |
| `groupIDs` | `number[]` |  |
| `conditionIDs` | `number[]` |  |
| `isCascadeRepurchasable` | `bool` |  |
| `cascadeRepurchaseEntryID` | `number?` |  |
| `subTreeID` | `number?` | The SubTree this Node belongs to; Nil if it is not part of a SubTree |
| `subTreeActive` | `bool?` | True if this node has a SubTreeID, and the SubTree is chosen or staged; May be nil if not part of a SubTree at all |

### TraitNodeInfoPartial

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `canPurchaseRank` | `bool?` |  |
| `canRefundRank` | `bool?` |  |
| `isAvailable` | `bool?` |  |
| `isVisible` | `bool?` |  |
| `ranksPurchased` | `number?` |  |
| `activeRank` | `number?` |  |
| `currentRank` | `number?` |  |
| `meetsEdgeRequirements` | `bool?` |  |
| `isCascadeRepurchasable` | `bool?` |  |
| `activeEntryID` | `number?` |  |
| `subTreeActive` | `bool?` |  |

### TraitOutEdgeInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `targetNode` | `number` |  |
| `type` | `number` |  |
| `visualStyle` | `number` |  |
| `isActive` | `bool` |  |

### TraitSubTreeInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ID` | `number` |  |
| `name` | `string?` |  |
| `description` | `string?` |  |
| `iconElementID` | `textureAtlas?` |  |
| `traitCurrencyID` | `number?` |  |
| `isActive` | `bool` |  |
| `subTreeSelectionNodeIDs` | `number[]` | SubTreeSelectionNodes whose choice entries include this SubTree |
| `posX` | `number` | Center X node position calculated from the posX values of all of this subTree's nodes |
| `posY` | `number` | Topmost Y node position taken from the posY values of all of this subTree's nodes |

### TraitTreeInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ID` | `number` |  |
| `gates` | `TraitGateInfo[]` |  |
| `hideSingleRankNumbers` | `bool` |  |
| `cannotRefund` | `bool` |  |
| `rootNodeID` | `number?` |  |
| `uiTextureKit` | `textureKit` |  |
| `titleText` | `string?` |  |

### TreeCurrencyInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `traitCurrencyID` | `number` |  |
| `quantity` | `number` |  |
| `maxQuantity` | `number?` |  |
| `spent` | `number` |  |
| `spentInTree` | `number?` |  |
