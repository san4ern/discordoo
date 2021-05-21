[discordoo](../README.md) / [Modules](../modules.md) / [core](../modules/core.md) / Base

# Class: Base

[core](../modules/core.md).Base

Base structure for everything which has snowflake

## Table of contents

### Constructors

- [constructor](core.base.md#constructor)

### Properties

- [id](core.base.md#id)

### Accessors

- [createdAt](core.base.md#createdat)
- [createdTimestamp](core.base.md#createdtimestamp)

### Methods

- [equal](core.base.md#equal)

## Constructors

### constructor

\+ **new Base**(`id`: *string*): [*Base*](core.base.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | *string* | id |

**Returns:** [*Base*](core.base.md)

Defined in: [src/core/structures/Base.ts:6](https://github.com/Discordoo/discordoo/blob/8db69d8/src/core/structures/Base.ts#L6)

## Properties

### id

• **id**: *string*

Unique id

Defined in: [src/core/structures/Base.ts:6](https://github.com/Discordoo/discordoo/blob/8db69d8/src/core/structures/Base.ts#L6)

## Accessors

### createdAt

• get **createdAt**(): Date

Get creation date

**Returns:** Date

Defined in: [src/core/structures/Base.ts:24](https://github.com/Discordoo/discordoo/blob/8db69d8/src/core/structures/Base.ts#L24)

___

### createdTimestamp

• get **createdTimestamp**(): *number*

Unix timestamp

**Returns:** *number*

Defined in: [src/core/structures/Base.ts:29](https://github.com/Discordoo/discordoo/blob/8db69d8/src/core/structures/Base.ts#L29)

## Methods

### equal

▸ **equal**(`compareTo`: [*Base*](core.base.md)): *boolean*

Check, if two entities are equal

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `compareTo` | [*Base*](core.base.md) | entity to compare to |

**Returns:** *boolean*

Defined in: [src/core/structures/Base.ts:19](https://github.com/Discordoo/discordoo/blob/8db69d8/src/core/structures/Base.ts#L19)
