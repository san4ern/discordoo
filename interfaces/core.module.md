[discordoo](../README.md) / [Modules](../modules.md) / [core](../modules/core.md) / Module

# Interface: Module

[core](../modules/core.md).Module

Represents a module

## Implemented by

- [*ModuleHostModule*](../classes/wrapper.modulehostmodule.md)

## Table of contents

### Properties

- [destroyed](core.module.md#destroyed)
- [id](core.module.md#id)
- [init](core.module.md#init)
- [initialized](core.module.md#initialized)

## Properties

### destroyed

• `Optional` **destroyed**: () => *void* \| *Promise*<void\>

Function, which will be emitted once module is destroyed

#### Type declaration

▸ (): *void* \| *Promise*<void\>

**Returns:** *void* \| *Promise*<void\>

Defined in: [src/core/modules/Module.ts:13](https://github.com/Discordoo/discordoo/blob/8db69d8/src/core/modules/Module.ts#L13)

___

### id

• **id**: *string* \| *symbol*

Unique id for this module

Defined in: [src/core/modules/Module.ts:15](https://github.com/Discordoo/discordoo/blob/8db69d8/src/core/modules/Module.ts#L15)

___

### init

• `Optional` **init**: (`client`: [*Client*](../classes/core.client.md)<[*DefaultClientStack*](core.defaultclientstack.md)\>) => *void* \| *Promise*<void\>

Function, which will be emitted once module was initialized on client's startup

**`param`** client, the module will be bound to

#### Type declaration

▸ (`client`: [*Client*](../classes/core.client.md)<[*DefaultClientStack*](core.defaultclientstack.md)\>): *void* \| *Promise*<void\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `client` | [*Client*](../classes/core.client.md)<[*DefaultClientStack*](core.defaultclientstack.md)\> |

**Returns:** *void* \| *Promise*<void\>

Defined in: [src/core/modules/Module.ts:11](https://github.com/Discordoo/discordoo/blob/8db69d8/src/core/modules/Module.ts#L11)

___

### initialized

• **initialized**: *boolean*

Whether the module was initialized

Defined in: [src/core/modules/Module.ts:6](https://github.com/Discordoo/discordoo/blob/8db69d8/src/core/modules/Module.ts#L6)
