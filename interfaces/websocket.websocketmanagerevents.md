[discordoo](../README.md) / [Modules](../modules.md) / [websocket](../modules/websocket.md) / WebSocketManagerEvents

# Interface: WebSocketManagerEvents

[websocket](../modules/websocket.md).WebSocketManagerEvents

## Table of contents

### Properties

- [connected](websocket.websocketmanagerevents.md#connected)
- [disconnected](websocket.websocketmanagerevents.md#disconnected)
- [message](websocket.websocketmanagerevents.md#message)
- [shardSpawn](websocket.websocketmanagerevents.md#shardspawn)

## Properties

### connected

• **connected**: (`id`: *number*) => *void*

#### Type declaration

▸ (`id`: *number*): *void*

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | *number* |

**Returns:** *void*

Defined in: [src/websocket/WebSocketManagerEvents.ts:5](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketManagerEvents.ts#L5)

___

### disconnected

• **disconnected**: (`id`: *number*) => *void*

#### Type declaration

▸ (`id`: *number*): *void*

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | *number* |

**Returns:** *void*

Defined in: [src/websocket/WebSocketManagerEvents.ts:6](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketManagerEvents.ts#L6)

___

### message

• **message**: (`msg`: *GatewayHello* \| *GatewayHeartbeatRequest* \| *GatewayHeartbeatAck* \| *GatewayInvalidSession* \| *GatewayReconnect* \| GatewayDispatchPayload, `id`: *number*) => *void*

#### Type declaration

▸ (`msg`: *GatewayHello* \| *GatewayHeartbeatRequest* \| *GatewayHeartbeatAck* \| *GatewayInvalidSession* \| *GatewayReconnect* \| GatewayDispatchPayload, `id`: *number*): *void*

#### Parameters

| Name | Type |
| :------ | :------ |
| `msg` | *GatewayHello* \| *GatewayHeartbeatRequest* \| *GatewayHeartbeatAck* \| *GatewayInvalidSession* \| *GatewayReconnect* \| GatewayDispatchPayload |
| `id` | *number* |

**Returns:** *void*

Defined in: [src/websocket/WebSocketManagerEvents.ts:4](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketManagerEvents.ts#L4)

___

### shardSpawn

• **shardSpawn**: (`id`: *number*) => *void*

#### Type declaration

▸ (`id`: *number*): *void*

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | *number* |

**Returns:** *void*

Defined in: [src/websocket/WebSocketManagerEvents.ts:7](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/WebSocketManagerEvents.ts#L7)
