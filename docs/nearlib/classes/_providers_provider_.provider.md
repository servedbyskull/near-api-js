---
id: "_providers_provider_.provider"
title: "Provider"
sidebar_label: "Provider"
---

## Hierarchy

* **Provider**

  ↳ [JsonRpcProvider](_providers_json_rpc_provider_.jsonrpcprovider.md)

## Index

### Methods

* [block](_providers_provider_.provider.md#abstract-block)
* [getNetwork](_providers_provider_.provider.md#abstract-getnetwork)
* [query](_providers_provider_.provider.md#abstract-query)
* [sendTransaction](_providers_provider_.provider.md#abstract-sendtransaction)
* [status](_providers_provider_.provider.md#abstract-status)
* [txStatus](_providers_provider_.provider.md#abstract-txstatus)

## Methods

### `Abstract` block

▸ **block**(`height`: number): *Promise‹[BlockResult](../interfaces/_providers_provider_.blockresult.md)›*

*Defined in [providers/provider.ts:95](https://github.com/nearprotocol/nearlib/blob/f222a4e/src.ts/providers/provider.ts#L95)*

**Parameters:**

Name | Type |
------ | ------ |
`height` | number |

**Returns:** *Promise‹[BlockResult](../interfaces/_providers_provider_.blockresult.md)›*

___

### `Abstract` getNetwork

▸ **getNetwork**(): *Promise‹[Network](../interfaces/_utils_network_.network.md)›*

*Defined in [providers/provider.ts:89](https://github.com/nearprotocol/nearlib/blob/f222a4e/src.ts/providers/provider.ts#L89)*

**Returns:** *Promise‹[Network](../interfaces/_utils_network_.network.md)›*

___

### `Abstract` query

▸ **query**(`path`: string, `data`: string): *Promise‹any›*

*Defined in [providers/provider.ts:94](https://github.com/nearprotocol/nearlib/blob/f222a4e/src.ts/providers/provider.ts#L94)*

**Parameters:**

Name | Type |
------ | ------ |
`path` | string |
`data` | string |

**Returns:** *Promise‹any›*

___

### `Abstract` sendTransaction

▸ **sendTransaction**(`signedTransaction`: [SignedTransaction](_transaction_.signedtransaction.md)): *Promise‹[FinalExecutionOutcome](../interfaces/_providers_provider_.finalexecutionoutcome.md)›*

*Defined in [providers/provider.ts:92](https://github.com/nearprotocol/nearlib/blob/f222a4e/src.ts/providers/provider.ts#L92)*

**Parameters:**

Name | Type |
------ | ------ |
`signedTransaction` | [SignedTransaction](_transaction_.signedtransaction.md) |

**Returns:** *Promise‹[FinalExecutionOutcome](../interfaces/_providers_provider_.finalexecutionoutcome.md)›*

___

### `Abstract` status

▸ **status**(): *Promise‹[NodeStatusResult](../interfaces/_providers_provider_.nodestatusresult.md)›*

*Defined in [providers/provider.ts:90](https://github.com/nearprotocol/nearlib/blob/f222a4e/src.ts/providers/provider.ts#L90)*

**Returns:** *Promise‹[NodeStatusResult](../interfaces/_providers_provider_.nodestatusresult.md)›*

___

### `Abstract` txStatus

▸ **txStatus**(`txHash`: Uint8Array): *Promise‹[FinalExecutionOutcome](../interfaces/_providers_provider_.finalexecutionoutcome.md)›*

*Defined in [providers/provider.ts:93](https://github.com/nearprotocol/nearlib/blob/f222a4e/src.ts/providers/provider.ts#L93)*

**Parameters:**

Name | Type |
------ | ------ |
`txHash` | Uint8Array |

**Returns:** *Promise‹[FinalExecutionOutcome](../interfaces/_providers_provider_.finalexecutionoutcome.md)›*