[discordoo](../README.md) / [Modules](../modules.md) / [core](../modules/core.md) / Client

# Class: Client<ClientStack\>

[core](../modules/core.md).Client

Entry point for all of Discordoo. Manages modules and events

## Type parameters

| Name | Type | Default |
| :------ | :------ | :------ |
| `ClientStack` | [*DefaultClientStack*](../interfaces/core.defaultclientstack.md) | [*DefaultClientStack*](../interfaces/core.defaultclientstack.md) |

## Hierarchy

- *TypedEmitter*<ListenerSignature<ClientStack[``"events"``]\>\>

  ↳ **Client**

## Table of contents

### Constructors

- [constructor](core.client.md#constructor)

### Properties

- [cache](core.client.md#cache)
- [gateway](core.client.md#gateway)
- [modules](core.client.md#modules)
- [rest](core.client.md#rest)
- [token](core.client.md#token)
- [defaultMaxListeners](core.client.md#defaultmaxlisteners)

### Methods

- [addListener](core.client.md#addlistener)
- [emit](core.client.md#emit)
- [eventNames](core.client.md#eventnames)
- [getMaxListeners](core.client.md#getmaxlisteners)
- [listenerCount](core.client.md#listenercount)
- [listeners](core.client.md#listeners)
- [m](core.client.md#m)
- [module](core.client.md#module)
- [off](core.client.md#off)
- [on](core.client.md#on)
- [once](core.client.md#once)
- [prependListener](core.client.md#prependlistener)
- [prependOnceListener](core.client.md#prependoncelistener)
- [rawListeners](core.client.md#rawlisteners)
- [removeAllListeners](core.client.md#removealllisteners)
- [removeListener](core.client.md#removelistener)
- [setMaxListeners](core.client.md#setmaxlisteners)
- [use](core.client.md#use)
- [useCacheProvider](core.client.md#usecacheprovider)
- [useGatewayProvider](core.client.md#usegatewayprovider)
- [useRESTProvider](core.client.md#userestprovider)

## Constructors

### constructor

\+ **new Client**<ClientStack\>(`token`: *string*): [*Client*](core.client.md)<ClientStack\>

#### Type parameters

| Name | Type | Default |
| :------ | :------ | :------ |
| `ClientStack` | [*DefaultClientStack*](../interfaces/core.defaultclientstack.md) | [*DefaultClientStack*](../interfaces/core.defaultclientstack.md) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `token` | *string* |

**Returns:** [*Client*](core.client.md)<ClientStack\>

Overrides: TypedEmitter&lt;ListenerSignature&lt;ClientStack[&#x27;events&#x27;]\&gt;\&gt;.constructor

Defined in: [src/core/Client.ts:14](https://github.com/Discordoo/discordoo/blob/75592d0/src/core/Client.ts#L14)

## Properties

### cache

• **cache**: ``null`` \| [*CacheProvider*](../modules/core.md#cacheprovider)<ClientStack[``"cache"``]\>= null

CacheProvider used by this module

Defined in: [src/core/Client.ts:28](https://github.com/Discordoo/discordoo/blob/75592d0/src/core/Client.ts#L28)

___

### gateway

• **gateway**: ``null`` \| [*GatewayProvider*](../modules/core.md#gatewayprovider)<ClientStack[``"gateway"``]\>= null

GatewayProvider used by this module

Defined in: [src/core/Client.ts:31](https://github.com/Discordoo/discordoo/blob/75592d0/src/core/Client.ts#L31)

___

### modules

• **modules**: [*ModuleManager*](core.modulemanager.md)

Module manager of this client

Defined in: [src/core/Client.ts:22](https://github.com/Discordoo/discordoo/blob/75592d0/src/core/Client.ts#L22)

___

### rest

• **rest**: ``null`` \| [*RESTProvider*](../modules/core.md#restprovider)<ClientStack[``"rest"``]\>= null

RESTProvider used by this module

Defined in: [src/core/Client.ts:25](https://github.com/Discordoo/discordoo/blob/75592d0/src/core/Client.ts#L25)

___

### token

• **token**: *string*

Token used by this client

Defined in: [src/core/Client.ts:14](https://github.com/Discordoo/discordoo/blob/75592d0/src/core/Client.ts#L14)

___

### defaultMaxListeners

▪ `Static` **defaultMaxListeners**: *number*

Inherited from: TypedEmitter.defaultMaxListeners

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:10

## Methods

### addListener

▸ **addListener**<U\>(`event`: U, `listener`: *ListenerSignature*<ClientStack[``"events"``]\>[U]): [*Client*](core.client.md)<ClientStack\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | *string* \| *number* \| *symbol* |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | *ListenerSignature*<ClientStack[``"events"``]\>[U] |

**Returns:** [*Client*](core.client.md)<ClientStack\>

Inherited from: TypedEmitter.addListener

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:11

___

### emit

▸ **emit**<U\>(`event`: U, ...`args`: *Parameters*<*ListenerSignature*<ClientStack[``"events"``]\>[U]\>): *boolean*

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | *string* \| *number* \| *symbol* |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `...args` | *Parameters*<*ListenerSignature*<ClientStack[``"events"``]\>[U]\> |

**Returns:** *boolean*

Inherited from: TypedEmitter.emit

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:19

___

### eventNames

▸ **eventNames**<U\>(): U[]

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | *string* \| *number* \| *symbol* |

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

▸ **listenerCount**(`type`: keyof ClientStack[``"events"``]): *number*

#### Parameters

| Name | Type |
| :------ | :------ |
| `type` | keyof ClientStack[``"events"``] |

**Returns:** *number*

Inherited from: TypedEmitter.listenerCount

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:21

___

### listeners

▸ **listeners**<U\>(`type`: U): *ListenerSignature*<ClientStack[``"events"``]\>[U][]

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | *string* \| *number* \| *symbol* |

#### Parameters

| Name | Type |
| :------ | :------ |
| `type` | U |

**Returns:** *ListenerSignature*<ClientStack[``"events"``]\>[U][]

Inherited from: TypedEmitter.listeners

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:22

___

### m

▸ **m**(`id`: *string* \| *symbol*): ``null`` \| [*Module*](../interfaces/core.module.md)

Get a module. Alias for module(id).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | *string* \| *symbol* | module id |

**Returns:** ``null`` \| [*Module*](../interfaces/core.module.md)

Defined in: [src/core/Client.ts:37](https://github.com/Discordoo/discordoo/blob/75592d0/src/core/Client.ts#L37)

___

### module

▸ **module**(`id`: *string* \| *symbol*): ``null`` \| [*Module*](../interfaces/core.module.md)

Get a module

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | *string* \| *symbol* | module id |

**Returns:** ``null`` \| [*Module*](../interfaces/core.module.md)

Defined in: [src/core/Client.ts:45](https://github.com/Discordoo/discordoo/blob/75592d0/src/core/Client.ts#L45)

___

### off

▸ **off**<U\>(`event`: U, `listener`: *ListenerSignature*<ClientStack[``"events"``]\>[U]): [*Client*](core.client.md)<ClientStack\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | *string* \| *number* \| *symbol* |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | *ListenerSignature*<ClientStack[``"events"``]\>[U] |

**Returns:** [*Client*](core.client.md)<ClientStack\>

Inherited from: TypedEmitter.off

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:18

___

### on

▸ **on**<U\>(`event`: U, `listener`: *ListenerSignature*<ClientStack[``"events"``]\>[U]): [*Client*](core.client.md)<ClientStack\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | *string* \| *number* \| *symbol* |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | *ListenerSignature*<ClientStack[``"events"``]\>[U] |

**Returns:** [*Client*](core.client.md)<ClientStack\>

Inherited from: TypedEmitter.on

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:17

___

### once

▸ **once**<U\>(`event`: U, `listener`: *ListenerSignature*<ClientStack[``"events"``]\>[U]): [*Client*](core.client.md)<ClientStack\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | *string* \| *number* \| *symbol* |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | *ListenerSignature*<ClientStack[``"events"``]\>[U] |

**Returns:** [*Client*](core.client.md)<ClientStack\>

Inherited from: TypedEmitter.once

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:16

___

### prependListener

▸ **prependListener**<U\>(`event`: U, `listener`: *ListenerSignature*<ClientStack[``"events"``]\>[U]): [*Client*](core.client.md)<ClientStack\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | *string* \| *number* \| *symbol* |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | *ListenerSignature*<ClientStack[``"events"``]\>[U] |

**Returns:** [*Client*](core.client.md)<ClientStack\>

Inherited from: TypedEmitter.prependListener

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:12

___

### prependOnceListener

▸ **prependOnceListener**<U\>(`event`: U, `listener`: *ListenerSignature*<ClientStack[``"events"``]\>[U]): [*Client*](core.client.md)<ClientStack\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | *string* \| *number* \| *symbol* |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | *ListenerSignature*<ClientStack[``"events"``]\>[U] |

**Returns:** [*Client*](core.client.md)<ClientStack\>

Inherited from: TypedEmitter.prependOnceListener

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:13

___

### rawListeners

▸ **rawListeners**<U\>(`type`: U): *ListenerSignature*<ClientStack[``"events"``]\>[U][]

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | *string* \| *number* \| *symbol* |

#### Parameters

| Name | Type |
| :------ | :------ |
| `type` | U |

**Returns:** *ListenerSignature*<ClientStack[``"events"``]\>[U][]

Inherited from: TypedEmitter.rawListeners

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:23

___

### removeAllListeners

▸ **removeAllListeners**(`event?`: keyof ClientStack[``"events"``]): [*Client*](core.client.md)<ClientStack\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `event?` | keyof ClientStack[``"events"``] |

**Returns:** [*Client*](core.client.md)<ClientStack\>

Inherited from: TypedEmitter.removeAllListeners

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:15

___

### removeListener

▸ **removeListener**<U\>(`event`: U, `listener`: *ListenerSignature*<ClientStack[``"events"``]\>[U]): [*Client*](core.client.md)<ClientStack\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `U` | *string* \| *number* \| *symbol* |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | U |
| `listener` | *ListenerSignature*<ClientStack[``"events"``]\>[U] |

**Returns:** [*Client*](core.client.md)<ClientStack\>

Inherited from: TypedEmitter.removeListener

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:14

___

### setMaxListeners

▸ **setMaxListeners**(`n`: *number*): [*Client*](core.client.md)<ClientStack\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `n` | *number* |

**Returns:** [*Client*](core.client.md)<ClientStack\>

Inherited from: TypedEmitter.setMaxListeners

Defined in: node_modules/tiny-typed-emitter/lib/index.d.ts:25

___

### use

▸ **use**(...`modules`: [*Module*](../interfaces/core.module.md)[]): *void*

Create a new module load group

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...modules` | [*Module*](../interfaces/core.module.md)[] | modules in the group |

**Returns:** *void*

Defined in: [src/core/Client.ts:53](https://github.com/Discordoo/discordoo/blob/75592d0/src/core/Client.ts#L53)

___

### useCacheProvider

▸ **useCacheProvider**(`provider`: (`client`: [*Client*](core.client.md)<[*DefaultClientStack*](../interfaces/core.defaultclientstack.md)\>) => [*CacheProvider*](../modules/core.md#cacheprovider)<ClientStack[``"cache"``]\>): *void*

Set the [CacheProvider](../modules/core.md#cacheprovider) to be used by this client
Bounds it's context to [Client](core.client.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `provider` | (`client`: [*Client*](core.client.md)<[*DefaultClientStack*](../interfaces/core.defaultclientstack.md)\>) => [*CacheProvider*](../modules/core.md#cacheprovider)<ClientStack[``"cache"``]\> | function, that returns desired CacheProvider |

**Returns:** *void*

Defined in: [src/core/Client.ts:71](https://github.com/Discordoo/discordoo/blob/75592d0/src/core/Client.ts#L71)

___

### useGatewayProvider

▸ **useGatewayProvider**(`provider`: (`client`: [*Client*](core.client.md)<[*DefaultClientStack*](../interfaces/core.defaultclientstack.md)\>) => [*GatewayProvider*](../modules/core.md#gatewayprovider)<ClientStack[``"gateway"``]\>): *void*

Set the [CacheProvider](../modules/core.md#cacheprovider) to be used by this client
Bounds it's context to [Client](core.client.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `provider` | (`client`: [*Client*](core.client.md)<[*DefaultClientStack*](../interfaces/core.defaultclientstack.md)\>) => [*GatewayProvider*](../modules/core.md#gatewayprovider)<ClientStack[``"gateway"``]\> | function, that returns desired CacheProvider |

**Returns:** *void*

Defined in: [src/core/Client.ts:80](https://github.com/Discordoo/discordoo/blob/75592d0/src/core/Client.ts#L80)

___

### useRESTProvider

▸ **useRESTProvider**(`provider`: (`client`: [*Client*](core.client.md)<[*DefaultClientStack*](../interfaces/core.defaultclientstack.md)\>) => [*RESTProvider*](../modules/core.md#restprovider)<ClientStack[``"rest"``]\>): *void*

Set the [RESTProvider](../modules/core.md#restprovider) to be used by this client
Bounds it's context to [Client](core.client.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `provider` | (`client`: [*Client*](core.client.md)<[*DefaultClientStack*](../interfaces/core.defaultclientstack.md)\>) => [*RESTProvider*](../modules/core.md#restprovider)<ClientStack[``"rest"``]\> | function, that returns desired RESTProvider |

**Returns:** *void*

Defined in: [src/core/Client.ts:62](https://github.com/Discordoo/discordoo/blob/75592d0/src/core/Client.ts#L62)
