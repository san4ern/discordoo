[discordoo](../README.md) / [Modules](../modules.md) / [cache](../modules/cache.md) / CacheProviderBuilder

# Class: CacheProviderBuilder

[cache](../modules/cache.md).CacheProviderBuilder

An adapter of [CacheManager](cache.cachemanager.md) for [Client](core.client.md)

## Table of contents

### Constructors

- [constructor](cache.cacheproviderbuilder.md#constructor)

### Properties

- [manager](cache.cacheproviderbuilder.md#manager)

### Methods

- [getCacheProvider](cache.cacheproviderbuilder.md#getcacheprovider)

## Constructors

### constructor

\+ **new CacheProviderBuilder**(): [*CacheProviderBuilder*](cache.cacheproviderbuilder.md)

**Returns:** [*CacheProviderBuilder*](cache.cacheproviderbuilder.md)

## Properties

### manager

• **manager**: [*CacheManager*](cache.cachemanager.md)

Cache manager, adapted by this adapter

Defined in: [src/cache/CacheProviderBuilder.ts:7](https://github.com/Discordoo/discordoo/blob/8db69d8/src/cache/CacheProviderBuilder.ts#L7)

## Methods

### getCacheProvider

▸ **getCacheProvider**(): *function*

Get a cache provider

**Returns:** (`client`: [*Client*](core.client.md)<[*DefaultClientStack*](../interfaces/core.defaultclientstack.md)\>) => [*CacheProvider*](../modules/core.md#cacheprovider)<[*CacheNamespace*](../interfaces/core.cachenamespace.md)<unknown, unknown\>\>

Defined in: [src/cache/CacheProviderBuilder.ts:10](https://github.com/Discordoo/discordoo/blob/8db69d8/src/cache/CacheProviderBuilder.ts#L10)
