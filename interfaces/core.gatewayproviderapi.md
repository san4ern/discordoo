[discordoo](../README.md) / [Modules](../modules.md) / [core](../modules/core.md) / GatewayProviderAPI

# Interface: GatewayProviderAPI

[core](../modules/core.md).GatewayProviderAPI

## Hierarchy

- *TypedEmitter*<GatewayProviderEvents\>

  ↳ **GatewayProviderAPI**

## Table of contents

### Properties

- [send](core.gatewayproviderapi.md#send)
- [start](core.gatewayproviderapi.md#start)
- [status](core.gatewayproviderapi.md#status)

### Methods

- [addListener](core.gatewayproviderapi.md#addlistener)
- [emit](core.gatewayproviderapi.md#emit)
- [eventNames](core.gatewayproviderapi.md#eventnames)
- [getMaxListeners](core.gatewayproviderapi.md#getmaxlisteners)
- [listenerCount](core.gatewayproviderapi.md#listenercount)
- [listeners](core.gatewayproviderapi.md#listeners)
- [off](core.gatewayproviderapi.md#off)
- [on](core.gatewayproviderapi.md#on)
- [once](core.gatewayproviderapi.md#once)
- [prependListener](core.gatewayproviderapi.md#prependlistener)
- [prependOnceListener](core.gatewayproviderapi.md#prependoncelistener)
- [rawListeners](core.gatewayproviderapi.md#rawlisteners)
- [removeAllListeners](core.gatewayproviderapi.md#removealllisteners)
- [removeListener](core.gatewayproviderapi.md#removelistener)
- [setMaxListeners](core.gatewayproviderapi.md#setmaxlisteners)

## Properties

### send

• **send**: (`msg`: GatewaySendPayload) => *Promise*<void\>

#### Type declaration

▸ (`msg`: GatewaySendPayload): *Promise*<void\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `msg` | GatewaySendPayload |

**Returns:** *Promise*<void\>

Defined in: [src/core/providers/gateway/GatewayProvider.ts:7](https://github.com/Discordoo/discordoo/blob/8db69d8/src/core/providers/gateway/GatewayProvider.ts#L7)

___

### start

• **start**: (`token`: *string*) => *Promise*<void\>

#### Type declaration

▸ (`token`: *string*): *Promise*<void\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `token` | *string* |

**Returns:** *Promise*<void\>

Defined in: [src/core/providers/gateway/GatewayProvider.ts:9](https://github.com/Discordoo/discordoo/blob/8db69d8/src/core/providers/gateway/GatewayProvider.ts#L9)

___

### status

• **status**: GatewayStatus

Defined in: [src/core/providers/gateway/GatewayProvider.ts:8](https://github.com/Discordoo/discordoo/blob/8db69d8/src/core/providers/gateway/GatewayProvider.ts#L8)

## Methods

### addListener

▸ **addListener**<U\>(`event`: U, `listener`: default[U]): [*GatewayProviderAPI*](core.gatewayproviderapi.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | keyof default |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | default[U] |

**Returns:** [*GatewayProviderAPI*](core.gatewayproviderapi.md)

Inherited from: TypedEmitter.addListener

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:11

___

### emit

▸ **emit**<U\>(`event`: U, ...`args`: *Parameters*<default[U]\>): *boolean*

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | keyof default |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `...args` | *Parameters*<default[U]\> |

**Returns:** *boolean*

Inherited from: TypedEmitter.emit

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:19

___

### eventNames

▸ **eventNames**<U\>(): U[]

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | keyof default |

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

▸ **listenerCount**(`type`: keyof default): *number*

#### Parameters

| Name | Type |
| :------ | :------ |
| `type` | keyof default |

**Returns:** *number*

Inherited from: TypedEmitter.listenerCount

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:21

___

### listeners

▸ **listeners**<U\>(`type`: U): default[U][]

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | keyof default |

#### Parameters

| Name | Type |
| :------ | :------ |
| `type` | U |

**Returns:** default[U][]

Inherited from: TypedEmitter.listeners

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:22

___

### off

▸ **off**<U\>(`event`: U, `listener`: default[U]): [*GatewayProviderAPI*](core.gatewayproviderapi.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | keyof default |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | default[U] |

**Returns:** [*GatewayProviderAPI*](core.gatewayproviderapi.md)

Inherited from: TypedEmitter.off

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:18

___

### on

▸ **on**<U\>(`event`: U, `listener`: default[U]): [*GatewayProviderAPI*](core.gatewayproviderapi.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | keyof default |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | default[U] |

**Returns:** [*GatewayProviderAPI*](core.gatewayproviderapi.md)

Inherited from: TypedEmitter.on

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:17

___

### once

▸ **once**<U\>(`event`: U, `listener`: default[U]): [*GatewayProviderAPI*](core.gatewayproviderapi.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | keyof default |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | default[U] |

**Returns:** [*GatewayProviderAPI*](core.gatewayproviderapi.md)

Inherited from: TypedEmitter.once

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:16

___

### prependListener

▸ **prependListener**<U\>(`event`: U, `listener`: default[U]): [*GatewayProviderAPI*](core.gatewayproviderapi.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | keyof default |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | default[U] |

**Returns:** [*GatewayProviderAPI*](core.gatewayproviderapi.md)

Inherited from: TypedEmitter.prependListener

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:12

___

### prependOnceListener

▸ **prependOnceListener**<U\>(`event`: U, `listener`: default[U]): [*GatewayProviderAPI*](core.gatewayproviderapi.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | keyof default |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | default[U] |

**Returns:** [*GatewayProviderAPI*](core.gatewayproviderapi.md)

Inherited from: TypedEmitter.prependOnceListener

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:13

___

### rawListeners

▸ **rawListeners**<U\>(`type`: U): default[U][]

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | keyof default |

#### Parameters

| Name | Type |
| :------ | :------ |
| `type` | U |

**Returns:** default[U][]

Inherited from: TypedEmitter.rawListeners

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:23

___

### removeAllListeners

▸ **removeAllListeners**(`event?`: keyof default): [*GatewayProviderAPI*](core.gatewayproviderapi.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `event?` | keyof default |

**Returns:** [*GatewayProviderAPI*](core.gatewayproviderapi.md)

Inherited from: TypedEmitter.removeAllListeners

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:15

___

### removeListener

▸ **removeListener**<U\>(`event`: U, `listener`: default[U]): [*GatewayProviderAPI*](core.gatewayproviderapi.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | keyof default |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | default[U] |

**Returns:** [*GatewayProviderAPI*](core.gatewayproviderapi.md)

Inherited from: TypedEmitter.removeListener

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:14

___

### setMaxListeners

▸ **setMaxListeners**(`n`: *number*): [*GatewayProviderAPI*](core.gatewayproviderapi.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `n` | *number* |

**Returns:** [*GatewayProviderAPI*](core.gatewayproviderapi.md)

Inherited from: TypedEmitter.setMaxListeners

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:25
