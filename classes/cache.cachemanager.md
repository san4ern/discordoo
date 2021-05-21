[discordoo](../README.md) / [Modules](../modules.md) / [cache](../modules/cache.md) / CacheManager

# Class: CacheManager

[cache](../modules/cache.md).CacheManager

Represents a cache manager

Used for cache namespaces fetching

## Table of contents

### Constructors

- [constructor](cache.cachemanager.md#constructor)

### Properties

- [caches](cache.cachemanager.md#caches)

### Methods

- [getCache](cache.cachemanager.md#getcache)

## Constructors

### constructor

\+ **new CacheManager**(): [*CacheManager*](cache.cachemanager.md)

**Returns:** [*CacheManager*](cache.cachemanager.md)

## Properties

### caches

• **caches**: [*Collection*](collection.collection-1.md)<string, [*CollectionCacheNamespace*](cache.collectioncachenamespace.md)<unknown, unknown\>\>

Namespaces controlled by this manager

Defined in: [src/cache/CacheManager.ts:11](https://github.com/Discordoo/discordoo/blob/8db69d8/src/cache/CacheManager.ts#L11)

## Methods

### getCache

▸ **getCache**<K, V\>(`id`: *string*): [*CollectionCacheNamespace*](cache.collectioncachenamespace.md)<K, V\>

Get a cache namespace

#### Type parameters

| Name | Default |
| :------ | :------ |
| `K` | *unknown* |
| `V` | *unknown* |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | *string* | id of cache namespace |

**Returns:** [*CollectionCacheNamespace*](cache.collectioncachenamespace.md)<K, V\>

Defined in: [src/cache/CacheManager.ts:17](https://github.com/Discordoo/discordoo/blob/8db69d8/src/cache/CacheManager.ts#L17)
