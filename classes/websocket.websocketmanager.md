[discordoo](../README.md) / [Modules](../modules.md) / [websocket](../modules/websocket.md) / WebSocketManager

# Class: WebSocketManager

[websocket](../modules/websocket.md).WebSocketManager

## Hierarchy

- *TypedEmitter*<[*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md)\>

  ↳ **WebSocketManager**

## Table of contents

### Constructors

- [constructor](websocket.websocketmanager.md#constructor)

### Properties

- [gateway](websocket.websocketmanager.md#gateway)
- [options](websocket.websocketmanager.md#options)
- [shardQueue](websocket.websocketmanager.md#shardqueue)
- [shards](websocket.websocketmanager.md#shards)
- [totalShards](websocket.websocketmanager.md#totalshards)
- [defaultMaxListeners](websocket.websocketmanager.md#defaultmaxlisteners)

### Methods

- [addListener](websocket.websocketmanager.md#addlistener)
- [connect](websocket.websocketmanager.md#connect)
- [createShards](websocket.websocketmanager.md#createshards)
- [emit](websocket.websocketmanager.md#emit)
- [eventNames](websocket.websocketmanager.md#eventnames)
- [getMaxListeners](websocket.websocketmanager.md#getmaxlisteners)
- [listenerCount](websocket.websocketmanager.md#listenercount)
- [listeners](websocket.websocketmanager.md#listeners)
- [off](websocket.websocketmanager.md#off)
- [on](websocket.websocketmanager.md#on)
- [once](websocket.websocketmanager.md#once)
- [prependListener](websocket.websocketmanager.md#prependlistener)
- [prependOnceListener](websocket.websocketmanager.md#prependoncelistener)
- [rawListeners](websocket.websocketmanager.md#rawlisteners)
- [removeAllListeners](websocket.websocketmanager.md#removealllisteners)
- [removeListener](websocket.websocketmanager.md#removelistener)
- [setMaxListeners](websocket.websocketmanager.md#setmaxlisteners)

## Constructors

### constructor

\+ **new WebSocketManager**(`token`: *string*, `options`: *Omit*<[*GatewayOptions*](../interfaces/websocket.gatewayoptions.md), ``"token"``\>): [*WebSocketManager*](websocket.websocketmanager.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `token` | *string* |
| `options` | *Omit*<[*GatewayOptions*](../interfaces/websocket.gatewayoptions.md), ``"token"``\> |

**Returns:** [*WebSocketManager*](websocket.websocketmanager.md)

Overrides: TypedEmitter&lt;WebSocketManagerEvents\&gt;.constructor

Defined in: [src/websocket/WebSocketManager.ts:27](https://github.com/Discordoo/discordoo/blob/8db69d8/src/websocket/WebSocketManager.ts#L27)

## Properties

### gateway

• `Private` `Optional` **gateway**: APIGatewayBotInfo

Defined in: [src/websocket/WebSocketManager.ts:22](https://github.com/Discordoo/discordoo/blob/8db69d8/src/websocket/WebSocketManager.ts#L22)

___

### options

• `Readonly` **options**: [*GatewayOptions*](../interfaces/websocket.gatewayoptions.md)

Defined in: [src/websocket/WebSocketManager.ts:21](https://github.com/Discordoo/discordoo/blob/8db69d8/src/websocket/WebSocketManager.ts#L21)

___

### shardQueue

• `Private` **shardQueue**: *Set*<[*WebSocketShard*](websocket.websocketshard.md)\>

Defined in: [src/websocket/WebSocketManager.ts:24](https://github.com/Discordoo/discordoo/blob/8db69d8/src/websocket/WebSocketManager.ts#L24)

___

### shards

• **shards**: [*Collection*](collection.collection-1.md)<number, [*WebSocketShard*](websocket.websocketshard.md)\>

Defined in: [src/websocket/WebSocketManager.ts:27](https://github.com/Discordoo/discordoo/blob/8db69d8/src/websocket/WebSocketManager.ts#L27)

___

### totalShards

• **totalShards**: *number*= 1

Defined in: [src/websocket/WebSocketManager.ts:26](https://github.com/Discordoo/discordoo/blob/8db69d8/src/websocket/WebSocketManager.ts#L26)

___

### defaultMaxListeners

▪ `Static` **defaultMaxListeners**: *number*

Inherited from: TypedEmitter.defaultMaxListeners

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:10

## Methods

### addListener

▸ **addListener**<U\>(`event`: U, `listener`: [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md)[U]): [*WebSocketManager*](websocket.websocketmanager.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | keyof [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md)[U] |

**Returns:** [*WebSocketManager*](websocket.websocketmanager.md)

Inherited from: TypedEmitter.addListener

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:11

___

### connect

▸ **connect**(): *Promise*<any\>

**Returns:** *Promise*<any\>

Defined in: [src/websocket/WebSocketManager.ts:48](https://github.com/Discordoo/discordoo/blob/8db69d8/src/websocket/WebSocketManager.ts#L48)

___

### createShards

▸ `Private` **createShards**(): *any*

**Returns:** *any*

Defined in: [src/websocket/WebSocketManager.ts:105](https://github.com/Discordoo/discordoo/blob/8db69d8/src/websocket/WebSocketManager.ts#L105)

___

### emit

▸ **emit**<U\>(`event`: U, ...`args`: *Parameters*<[*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md)[U]\>): *boolean*

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | keyof [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `...args` | *Parameters*<[*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md)[U]\> |

**Returns:** *boolean*

Inherited from: TypedEmitter.emit

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:19

___

### eventNames

▸ **eventNames**<U\>(): U[]

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | keyof [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md) |

**Returns:** U[]

Inherited from: TypedEmitter.eventNames

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:20

___

### getMaxListeners

▸ **getMaxListeners**(): *number*

**Returns:** *number*

Inherited from: TypedEmitter.getMaxListeners

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:24

___

### listenerCount

▸ **listenerCount**(`type`: keyof [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md)): *number*

#### Parameters

| Name | Type |
| :------ | :------ |
| `type` | keyof [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md) |

**Returns:** *number*

Inherited from: TypedEmitter.listenerCount

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:21

___

### listeners

▸ **listeners**<U\>(`type`: U): [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md)[U][]

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | keyof [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `type` | U |

**Returns:** [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md)[U][]

Inherited from: TypedEmitter.listeners

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:22

___

### off

▸ **off**<U\>(`event`: U, `listener`: [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md)[U]): [*WebSocketManager*](websocket.websocketmanager.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | keyof [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md)[U] |

**Returns:** [*WebSocketManager*](websocket.websocketmanager.md)

Inherited from: TypedEmitter.off

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:18

___

### on

▸ **on**<U\>(`event`: U, `listener`: [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md)[U]): [*WebSocketManager*](websocket.websocketmanager.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | keyof [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md)[U] |

**Returns:** [*WebSocketManager*](websocket.websocketmanager.md)

Inherited from: TypedEmitter.on

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:17

___

### once

▸ **once**<U\>(`event`: U, `listener`: [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md)[U]): [*WebSocketManager*](websocket.websocketmanager.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | keyof [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md)[U] |

**Returns:** [*WebSocketManager*](websocket.websocketmanager.md)

Inherited from: TypedEmitter.once

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:16

___

### prependListener

▸ **prependListener**<U\>(`event`: U, `listener`: [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md)[U]): [*WebSocketManager*](websocket.websocketmanager.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | keyof [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md)[U] |

**Returns:** [*WebSocketManager*](websocket.websocketmanager.md)

Inherited from: TypedEmitter.prependListener

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:12

___

### prependOnceListener

▸ **prependOnceListener**<U\>(`event`: U, `listener`: [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md)[U]): [*WebSocketManager*](websocket.websocketmanager.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | keyof [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md)[U] |

**Returns:** [*WebSocketManager*](websocket.websocketmanager.md)

Inherited from: TypedEmitter.prependOnceListener

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:13

___

### rawListeners

▸ **rawListeners**<U\>(`type`: U): [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md)[U][]

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | keyof [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `type` | U |

**Returns:** [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md)[U][]

Inherited from: TypedEmitter.rawListeners

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:23

___

### removeAllListeners

▸ **removeAllListeners**(`event?`: keyof [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md)): [*WebSocketManager*](websocket.websocketmanager.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `event?` | keyof [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md) |

**Returns:** [*WebSocketManager*](websocket.websocketmanager.md)

Inherited from: TypedEmitter.removeAllListeners

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:15

___

### removeListener

▸ **removeListener**<U\>(`event`: U, `listener`: [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md)[U]): [*WebSocketManager*](websocket.websocketmanager.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | keyof [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | [*WebSocketManagerEvents*](../interfaces/websocket.websocketmanagerevents.md)[U] |

**Returns:** [*WebSocketManager*](websocket.websocketmanager.md)

Inherited from: TypedEmitter.removeListener

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:14

___

### setMaxListeners

▸ **setMaxListeners**(`n`: *number*): [*WebSocketManager*](websocket.websocketmanager.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `n` | *number* |

**Returns:** [*WebSocketManager*](websocket.websocketmanager.md)

Inherited from: TypedEmitter.setMaxListeners

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:25
