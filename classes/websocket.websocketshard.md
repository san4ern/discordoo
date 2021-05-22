[discordoo](../README.md) / [Modules](../modules.md) / [websocket](../modules/websocket.md) / WebSocketShard

# Class: WebSocketShard

[websocket](../modules/websocket.md).WebSocketShard

## Hierarchy

- *TypedEmitter*<[*WebSocketShardEvents*](../interfaces/websocket.websocketshardevents.md)\>

  ↳ **WebSocketShard**

## Table of contents

### Constructors

- [constructor](websocket.websocketshard.md#constructor)

### Properties

- [connection](websocket.websocketshard.md#connection)
- [heartbeatInterval](websocket.websocketshard.md#heartbeatinterval)
- [id](websocket.websocketshard.md#id)
- [lastHeartbeatAcked](websocket.websocketshard.md#lastheartbeatacked)
- [lastPingTimestamp](websocket.websocketshard.md#lastpingtimestamp)
- [manager](websocket.websocketshard.md#manager)
- [pendingGuilds](websocket.websocketshard.md#pendingguilds)
- [ping](websocket.websocketshard.md#ping)
- [sequence](websocket.websocketshard.md#sequence)
- [sessionID](websocket.websocketshard.md#sessionid)
- [defaultMaxListeners](websocket.websocketshard.md#defaultmaxlisteners)

### Methods

- [ackHeartbeat](websocket.websocketshard.md#ackheartbeat)
- [addListener](websocket.websocketshard.md#addlistener)
- [connect](websocket.websocketshard.md#connect)
- [createIdentify](websocket.websocketshard.md#createidentify)
- [destroy](websocket.websocketshard.md#destroy)
- [emit](websocket.websocketshard.md#emit)
- [eventNames](websocket.websocketshard.md#eventnames)
- [getMaxListeners](websocket.websocketshard.md#getmaxlisteners)
- [handlePacket](websocket.websocketshard.md#handlepacket)
- [heartbeat](websocket.websocketshard.md#heartbeat)
- [identify](websocket.websocketshard.md#identify)
- [listenerCount](websocket.websocketshard.md#listenercount)
- [listeners](websocket.websocketshard.md#listeners)
- [off](websocket.websocketshard.md#off)
- [on](websocket.websocketshard.md#on)
- [onClose](websocket.websocketshard.md#onclose)
- [onMessage](websocket.websocketshard.md#onmessage)
- [once](websocket.websocketshard.md#once)
- [prependListener](websocket.websocketshard.md#prependlistener)
- [prependOnceListener](websocket.websocketshard.md#prependoncelistener)
- [rawListeners](websocket.websocketshard.md#rawlisteners)
- [removeAllListeners](websocket.websocketshard.md#removealllisteners)
- [removeListener](websocket.websocketshard.md#removelistener)
- [removeListeners](websocket.websocketshard.md#removelisteners)
- [resumeIdentify](websocket.websocketshard.md#resumeidentify)
- [send](websocket.websocketshard.md#send)
- [setMaxListeners](websocket.websocketshard.md#setmaxlisteners)
- [setupHeartbeatInterval](websocket.websocketshard.md#setupheartbeatinterval)

## Constructors

### constructor

\+ **new WebSocketShard**(`manager`: [*WebSocketManager*](websocket.websocketmanager.md), `id`: *number*): [*WebSocketShard*](websocket.websocketshard.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `manager` | [*WebSocketManager*](websocket.websocketmanager.md) |
| `id` | *number* |

**Returns:** [*WebSocketShard*](websocket.websocketshard.md)

Overrides: TypedEmitter&lt;WebSocketShardEvents\&gt;.constructor

Defined in: [src/websocket/WebSocketShard.ts:20](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketShard.ts#L20)

## Properties

### connection

• `Private` `Optional` **connection**: *WebSocket*

Defined in: [src/websocket/WebSocketShard.ts:15](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketShard.ts#L15)

___

### heartbeatInterval

• `Private` `Optional` **heartbeatInterval**: *any*

Defined in: [src/websocket/WebSocketShard.ts:19](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketShard.ts#L19)

___

### id

• **id**: *number*

Defined in: [src/websocket/WebSocketShard.ts:10](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketShard.ts#L10)

___

### lastHeartbeatAcked

• `Private` **lastHeartbeatAcked**: *boolean*= true

Defined in: [src/websocket/WebSocketShard.ts:20](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketShard.ts#L20)

___

### lastPingTimestamp

• **lastPingTimestamp**: *number*= 0

Defined in: [src/websocket/WebSocketShard.ts:12](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketShard.ts#L12)

___

### manager

• **manager**: [*WebSocketManager*](websocket.websocketmanager.md)

Defined in: [src/websocket/WebSocketShard.ts:9](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketShard.ts#L9)

___

### pendingGuilds

• `Private` **pendingGuilds**: *string*[]

Defined in: [src/websocket/WebSocketShard.ts:18](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketShard.ts#L18)

___

### ping

• **ping**: *number*= -1

Defined in: [src/websocket/WebSocketShard.ts:13](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketShard.ts#L13)

___

### sequence

• `Private` **sequence**: *number*= -1

Defined in: [src/websocket/WebSocketShard.ts:17](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketShard.ts#L17)

___

### sessionID

• `Private` `Optional` **sessionID**: *string*

Defined in: [src/websocket/WebSocketShard.ts:16](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketShard.ts#L16)

___

### defaultMaxListeners

▪ `Static` **defaultMaxListeners**: *number*

Inherited from: TypedEmitter.defaultMaxListeners

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:10

## Methods

### ackHeartbeat

▸ `Private` **ackHeartbeat**(): *void*

**Returns:** *void*

Defined in: [src/websocket/WebSocketShard.ts:151](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketShard.ts#L151)

___

### addListener

▸ **addListener**<U\>(`event`: U, `listener`: [*WebSocketShardEvents*](../interfaces/websocket.websocketshardevents.md)[U]): [*WebSocketShard*](websocket.websocketshard.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | ``"message"`` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | [*WebSocketShardEvents*](../interfaces/websocket.websocketshardevents.md)[U] |

**Returns:** [*WebSocketShard*](websocket.websocketshard.md)

Inherited from: TypedEmitter.addListener

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:11

___

### connect

▸ **connect**(): *Promise*<undefined \| ``false``\>

**Returns:** *Promise*<undefined \| ``false``\>

Defined in: [src/websocket/WebSocketShard.ts:29](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketShard.ts#L29)

___

### createIdentify

▸ `Private` **createIdentify**(): *void*

**Returns:** *void*

Defined in: [src/websocket/WebSocketShard.ts:44](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketShard.ts#L44)

___

### destroy

▸ **destroy**(`__namedParameters?`: { `code`:  ; `reconnect`:  ; `reset`:   }): *void*

#### Parameters

| Name | Type |
| :------ | :------ |
| `__namedParameters` | *object* |
| `__namedParameters.code` | - |
| `__namedParameters.reconnect` | - |
| `__namedParameters.reset` | - |

**Returns:** *void*

Defined in: [src/websocket/WebSocketShard.ts:166](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketShard.ts#L166)

___

### emit

▸ **emit**<U\>(`event`: U, ...`args`: *Parameters*<[*WebSocketShardEvents*](../interfaces/websocket.websocketshardevents.md)[U]\>): *boolean*

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | ``"message"`` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `...args` | *Parameters*<[*WebSocketShardEvents*](../interfaces/websocket.websocketshardevents.md)[U]\> |

**Returns:** *boolean*

Inherited from: TypedEmitter.emit

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:19

___

### eventNames

▸ **eventNames**<U\>(): U[]

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | ``"message"`` |

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

### handlePacket

▸ `Private` **handlePacket**(`packet?`: *Record*<any, any\>): *void*

#### Parameters

| Name | Type |
| :------ | :------ |
| `packet?` | *Record*<any, any\> |

**Returns:** *void*

Defined in: [src/websocket/WebSocketShard.ts:95](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketShard.ts#L95)

___

### heartbeat

▸ `Private` **heartbeat**(): *void*

**Returns:** *void*

Defined in: [src/websocket/WebSocketShard.ts:139](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketShard.ts#L139)

___

### identify

▸ `Private` **identify**(): *any*

**Returns:** *any*

Defined in: [src/websocket/WebSocketShard.ts:40](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketShard.ts#L40)

___

### listenerCount

▸ **listenerCount**(`type`: ``"message"``): *number*

#### Parameters

| Name | Type |
| :------ | :------ |
| `type` | ``"message"`` |

**Returns:** *number*

Inherited from: TypedEmitter.listenerCount

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:21

___

### listeners

▸ **listeners**<U\>(`type`: U): [*WebSocketShardEvents*](../interfaces/websocket.websocketshardevents.md)[U][]

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | ``"message"`` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `type` | U |

**Returns:** [*WebSocketShardEvents*](../interfaces/websocket.websocketshardevents.md)[U][]

Inherited from: TypedEmitter.listeners

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:22

___

### off

▸ **off**<U\>(`event`: U, `listener`: [*WebSocketShardEvents*](../interfaces/websocket.websocketshardevents.md)[U]): [*WebSocketShard*](websocket.websocketshard.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | ``"message"`` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | [*WebSocketShardEvents*](../interfaces/websocket.websocketshardevents.md)[U] |

**Returns:** [*WebSocketShard*](websocket.websocketshard.md)

Inherited from: TypedEmitter.off

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:18

___

### on

▸ **on**<U\>(`event`: U, `listener`: [*WebSocketShardEvents*](../interfaces/websocket.websocketshardevents.md)[U]): [*WebSocketShard*](websocket.websocketshard.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | ``"message"`` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | [*WebSocketShardEvents*](../interfaces/websocket.websocketshardevents.md)[U] |

**Returns:** [*WebSocketShard*](websocket.websocketshard.md)

Inherited from: TypedEmitter.on

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:17

___

### onClose

▸ `Private` **onClose**(`event`: CloseEvent): *void*

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | CloseEvent |

**Returns:** *void*

Defined in: [src/websocket/WebSocketShard.ts:73](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketShard.ts#L73)

___

### onMessage

▸ `Private` **onMessage**(`event`: MessageEvent): *void*

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | MessageEvent |

**Returns:** *void*

Defined in: [src/websocket/WebSocketShard.ts:77](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketShard.ts#L77)

___

### once

▸ **once**<U\>(`event`: U, `listener`: [*WebSocketShardEvents*](../interfaces/websocket.websocketshardevents.md)[U]): [*WebSocketShard*](websocket.websocketshard.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | ``"message"`` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | [*WebSocketShardEvents*](../interfaces/websocket.websocketshardevents.md)[U] |

**Returns:** [*WebSocketShard*](websocket.websocketshard.md)

Inherited from: TypedEmitter.once

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:16

___

### prependListener

▸ **prependListener**<U\>(`event`: U, `listener`: [*WebSocketShardEvents*](../interfaces/websocket.websocketshardevents.md)[U]): [*WebSocketShard*](websocket.websocketshard.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | ``"message"`` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | [*WebSocketShardEvents*](../interfaces/websocket.websocketshardevents.md)[U] |

**Returns:** [*WebSocketShard*](websocket.websocketshard.md)

Inherited from: TypedEmitter.prependListener

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:12

___

### prependOnceListener

▸ **prependOnceListener**<U\>(`event`: U, `listener`: [*WebSocketShardEvents*](../interfaces/websocket.websocketshardevents.md)[U]): [*WebSocketShard*](websocket.websocketshard.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | ``"message"`` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | [*WebSocketShardEvents*](../interfaces/websocket.websocketshardevents.md)[U] |

**Returns:** [*WebSocketShard*](websocket.websocketshard.md)

Inherited from: TypedEmitter.prependOnceListener

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:13

___

### rawListeners

▸ **rawListeners**<U\>(`type`: U): [*WebSocketShardEvents*](../interfaces/websocket.websocketshardevents.md)[U][]

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | ``"message"`` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `type` | U |

**Returns:** [*WebSocketShardEvents*](../interfaces/websocket.websocketshardevents.md)[U][]

Inherited from: TypedEmitter.rawListeners

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:23

___

### removeAllListeners

▸ **removeAllListeners**(`event?`: ``"message"``): [*WebSocketShard*](websocket.websocketshard.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `event?` | ``"message"`` |

**Returns:** [*WebSocketShard*](websocket.websocketshard.md)

Inherited from: TypedEmitter.removeAllListeners

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:15

___

### removeListener

▸ **removeListener**<U\>(`event`: U, `listener`: [*WebSocketShardEvents*](../interfaces/websocket.websocketshardevents.md)[U]): [*WebSocketShard*](websocket.websocketshard.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | ``"message"`` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | [*WebSocketShardEvents*](../interfaces/websocket.websocketshardevents.md)[U] |

**Returns:** [*WebSocketShard*](websocket.websocketshard.md)

Inherited from: TypedEmitter.removeListener

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:14

___

### removeListeners

▸ `Private` **removeListeners**(): *void*

**Returns:** *void*

Defined in: [src/websocket/WebSocketShard.ts:191](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketShard.ts#L191)

___

### resumeIdentify

▸ `Private` **resumeIdentify**(): *any*

**Returns:** *any*

Defined in: [src/websocket/WebSocketShard.ts:61](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketShard.ts#L61)

___

### send

▸ `Private` **send**(`data`: *any*): *void*

#### Parameters

| Name | Type |
| :------ | :------ |
| `data` | *any* |

**Returns:** *void*

Defined in: [src/websocket/WebSocketShard.ts:131](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketShard.ts#L131)

___

### setMaxListeners

▸ **setMaxListeners**(`n`: *number*): [*WebSocketShard*](websocket.websocketshard.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `n` | *number* |

**Returns:** [*WebSocketShard*](websocket.websocketshard.md)

Inherited from: TypedEmitter.setMaxListeners

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:25

___

### setupHeartbeatInterval

▸ `Private` **setupHeartbeatInterval**(`interval`: *number*): *void*

#### Parameters

| Name | Type |
| :------ | :------ |
| `interval` | *number* |

**Returns:** *void*

Defined in: [src/websocket/WebSocketShard.ts:157](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketShard.ts#L157)
