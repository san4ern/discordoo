[discordoo](../README.md) / [Modules](../modules.md) / [wrapper](../modules/wrapper.md) / ModuleHostModule

# Class: ModuleHostModule

[wrapper](../modules/wrapper.md).ModuleHostModule

Module which is capable of loading other modules

## Implements

- [*Module*](../interfaces/core.module.md)

## Table of contents

### Constructors

- [constructor](wrapper.modulehostmodule.md#constructor)

### Properties

- [id](wrapper.modulehostmodule.md#id)
- [initialized](wrapper.modulehostmodule.md#initialized)
- [modules](wrapper.modulehostmodule.md#modules)

### Methods

- [init](wrapper.modulehostmodule.md#init)

## Constructors

### constructor

\+ **new ModuleHostModule**(`modules`: [*Module*](../interfaces/core.module.md)[]): [*ModuleHostModule*](wrapper.modulehostmodule.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `modules` | [*Module*](../interfaces/core.module.md)[] | modules to load |

**Returns:** [*ModuleHostModule*](wrapper.modulehostmodule.md)

Defined in: [src/wrapper/ModuleHostModule.ts:9](https://github.com/Discordoo/discordoo/blob/8db69d8/src/wrapper/ModuleHostModule.ts#L9)

## Properties

### id

• **id**: *string* \| *symbol*= 'host-module'

Unique id for this module

Implementation of: [Module](../interfaces/core.module.md).[id](../interfaces/core.module.md#id)

Defined in: [src/wrapper/ModuleHostModule.ts:5](https://github.com/Discordoo/discordoo/blob/8db69d8/src/wrapper/ModuleHostModule.ts#L5)

___

### initialized

• **initialized**: *boolean*= false

Whether the module was initialized

Implementation of: [Module](../interfaces/core.module.md).[initialized](../interfaces/core.module.md#initialized)

Defined in: [src/wrapper/ModuleHostModule.ts:6](https://github.com/Discordoo/discordoo/blob/8db69d8/src/wrapper/ModuleHostModule.ts#L6)

___

### modules

• **modules**: [*Module*](../interfaces/core.module.md)[]

Modules which will be loaded by this module

Defined in: [src/wrapper/ModuleHostModule.ts:9](https://github.com/Discordoo/discordoo/blob/8db69d8/src/wrapper/ModuleHostModule.ts#L9)

## Methods

### init

▸ **init**(`client`: [*Client*](core.client.md)<[*DefaultClientStack*](../interfaces/core.defaultclientstack.md)\>): *void*

Function, which will be emitted once module was initialized on client's startup

#### Parameters

| Name | Type |
| :------ | :------ |
| `client` | [*Client*](core.client.md)<[*DefaultClientStack*](../interfaces/core.defaultclientstack.md)\> |

**Returns:** *void*

Implementation of: Module.init

Defined in: [src/wrapper/ModuleHostModule.ts:18](https://github.com/Discordoo/discordoo/blob/8db69d8/src/wrapper/ModuleHostModule.ts#L18)
