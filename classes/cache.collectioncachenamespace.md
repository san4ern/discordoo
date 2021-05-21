[discordoo](../README.md) / [Modules](../modules.md) / [cache](../modules/cache.md) / CollectionCacheNamespace

# Class: CollectionCacheNamespace<K, V\>

[cache](../modules/cache.md).CollectionCacheNamespace

Represents a cache namespace

## Type parameters

| Name | Default |
| :------ | :------ |
| `K` | *unknown* |
| `V` | *unknown* |

## Implements

- [*CacheNamespace*](../interfaces/core.cachenamespace.md)<K, V\>

## Table of contents

### Constructors

- [constructor](cache.collectioncachenamespace.md#constructor)

### Properties

- [#data](cache.collectioncachenamespace.md##data)

### Methods

- [delete](cache.collectioncachenamespace.md#delete)
- [filter](cache.collectioncachenamespace.md#filter)
- [forEach](cache.collectioncachenamespace.md#foreach)
- [get](cache.collectioncachenamespace.md#get)
- [has](cache.collectioncachenamespace.md#has)
- [random](cache.collectioncachenamespace.md#random)
- [set](cache.collectioncachenamespace.md#set)
- [size](cache.collectioncachenamespace.md#size)

## Constructors

### constructor

\+ **new CollectionCacheNamespace**<K, V\>(): [*CollectionCacheNamespace*](cache.collectioncachenamespace.md)<K, V\>

#### Type parameters

| Name | Default |
| :------ | :------ |
| `K` | *unknown* |
| `V` | *unknown* |

**Returns:** [*CollectionCacheNamespace*](cache.collectioncachenamespace.md)<K, V\>

## Properties

### #data

• `Private` **#data**: [*Collection*](collection.collection-1.md)<K, V\>

Collection used by this cache namespace

Defined in: [src/cache/CollectionCacheNamespace.ts:7](https://github.com/Discordoo/discordoo/blob/8db69d8/src/cache/CollectionCacheNamespace.ts#L7)

## Methods

### delete

▸ **delete**(`key`: K): *Promise*<boolean\>

Delete a key from collection

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | K | key to delete |

**Returns:** *Promise*<boolean\>

Implementation of: [CacheNamespace](../interfaces/core.cachenamespace.md)

Defined in: [src/cache/CollectionCacheNamespace.ts:13](https://github.com/Discordoo/discordoo/blob/8db69d8/src/cache/CollectionCacheNamespace.ts#L13)

___

### filter

▸ **filter**(`predicate`: (`value`: V, `key`: K, `collection`: [*Collection*](collection.collection-1.md)<K, V\>) => *boolean*): *Promise*<[*Collection*](collection.collection-1.md)<K, V\>\>

The same as {@link Collection#filter}

#### Parameters

| Name | Type |
| :------ | :------ |
| `predicate` | (`value`: V, `key`: K, `collection`: [*Collection*](collection.collection-1.md)<K, V\>) => *boolean* |

**Returns:** *Promise*<[*Collection*](collection.collection-1.md)<K, V\>\>

Defined in: [src/cache/CollectionCacheNamespace.ts:49](https://github.com/Discordoo/discordoo/blob/8db69d8/src/cache/CollectionCacheNamespace.ts#L49)

___

### forEach

▸ **forEach**(`predicate`: (`value`: V, `key`: K, `collection`: [*Collection*](collection.collection-1.md)<K, V\>) => *boolean*): *Promise*<void\>

The same as {@link Collection#forEach}

#### Parameters

| Name | Type |
| :------ | :------ |
| `predicate` | (`value`: V, `key`: K, `collection`: [*Collection*](collection.collection-1.md)<K, V\>) => *boolean* |

**Returns:** *Promise*<void\>

Defined in: [src/cache/CollectionCacheNamespace.ts:59](https://github.com/Discordoo/discordoo/blob/8db69d8/src/cache/CollectionCacheNamespace.ts#L59)

___

### get

▸ **get**(`key`: K): *Promise*<``null`` \| V\>

Get a key from collection

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | K | key to get |

**Returns:** *Promise*<``null`` \| V\>

Implementation of: [CacheNamespace](../interfaces/core.cachenamespace.md)

Defined in: [src/cache/CollectionCacheNamespace.ts:21](https://github.com/Discordoo/discordoo/blob/8db69d8/src/cache/CollectionCacheNamespace.ts#L21)

___

### has

▸ **has**(`key`: K): *Promise*<boolean\>

Check if collection has a key

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | K | ket to check |

**Returns:** *Promise*<boolean\>

Implementation of: [CacheNamespace](../interfaces/core.cachenamespace.md)

Defined in: [src/cache/CollectionCacheNamespace.ts:29](https://github.com/Discordoo/discordoo/blob/8db69d8/src/cache/CollectionCacheNamespace.ts#L29)

___

### random

▸ **random**(`amount?`: *number*): *Promise*<V \| V[]\>

The same as {@link Collection#random}

#### Parameters

| Name | Type |
| :------ | :------ |
| `amount?` | *number* |

**Returns:** *Promise*<V \| V[]\>

Defined in: [src/cache/CollectionCacheNamespace.ts:54](https://github.com/Discordoo/discordoo/blob/8db69d8/src/cache/CollectionCacheNamespace.ts#L54)

___

### set

▸ **set**(`key`: K, `value`: V): *Promise*<boolean\>

Change key's value

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | K | key to set |
| `value` | V | value to set |

**Returns:** *Promise*<boolean\>

Implementation of: [CacheNamespace](../interfaces/core.cachenamespace.md)

Defined in: [src/cache/CollectionCacheNamespace.ts:38](https://github.com/Discordoo/discordoo/blob/8db69d8/src/cache/CollectionCacheNamespace.ts#L38)

___

### size

▸ **size**(): *Promise*<number\>

Get total elements in the collection

**Returns:** *Promise*<number\>

Implementation of: [CacheNamespace](../interfaces/core.cachenamespace.md)

Defined in: [src/cache/CollectionCacheNamespace.ts:44](https://github.com/Discordoo/discordoo/blob/8db69d8/src/cache/CollectionCacheNamespace.ts#L44)
