[discordoo](../README.md) / [Modules](../modules.md) / [core](../modules/core.md) / CacheNamespace

# Interface: CacheNamespace<K, V\>

[core](../modules/core.md).CacheNamespace

Represents a cache namespace. Custom caching modules must implement it

**`note`** Some implementations may use remote cache, e.g. Redis, so all the methods are async

## Type parameters

| Name | Default |
| :------ | :------ |
| `K` | *unknown* |
| `V` | *unknown* |

## Implemented by

- [*CollectionCacheNamespace*](../classes/cache.collectioncachenamespace.md)

## Table of contents

### Methods

- [delete](core.cachenamespace.md#delete)
- [get](core.cachenamespace.md#get)
- [has](core.cachenamespace.md#has)
- [set](core.cachenamespace.md#set)
- [size](core.cachenamespace.md#size)

## Methods

### delete

▸ **delete**(`key`: K): *Promise*<boolean\>

Delete a key from cache

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | K | cache to delete |

**Returns:** *Promise*<boolean\>

Defined in: [src/core/providers/cache/CacheNamespace.ts:23](https://github.com/Discordoo/discordoo/blob/75592d0/src/core/providers/cache/CacheNamespace.ts#L23)

___

### get

▸ **get**(`key`: K): *Promise*<``null`` \| V\>

Get value from key

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | K | key to get |

**Returns:** *Promise*<``null`` \| V\>

Defined in: [src/core/providers/cache/CacheNamespace.ts:10](https://github.com/Discordoo/discordoo/blob/75592d0/src/core/providers/cache/CacheNamespace.ts#L10)

___

### has

▸ **has**(`key`: K): *Promise*<boolean\>

Check if key exists in cache

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | K | key to check |

**Returns:** *Promise*<boolean\>

Defined in: [src/core/providers/cache/CacheNamespace.ts:29](https://github.com/Discordoo/discordoo/blob/75592d0/src/core/providers/cache/CacheNamespace.ts#L29)

___

### set

▸ **set**(`key`: K, `value`: V): *Promise*<boolean\>

Set a key to given value

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | K | key to set |
| `value` | V | value to be set |

**Returns:** *Promise*<boolean\>

Defined in: [src/core/providers/cache/CacheNamespace.ts:17](https://github.com/Discordoo/discordoo/blob/75592d0/src/core/providers/cache/CacheNamespace.ts#L17)

___

### size

▸ **size**(): *Promise*<number\>

Get size of cache

**Returns:** *Promise*<number\>

Defined in: [src/core/providers/cache/CacheNamespace.ts:32](https://github.com/Discordoo/discordoo/blob/75592d0/src/core/providers/cache/CacheNamespace.ts#L32)
