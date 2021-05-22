[discordoo](../README.md) / [Modules](../modules.md) / [wrapper](../modules/wrapper.md) / ClientBuilder

# Class: ClientBuilder<Stack\>

[wrapper](../modules/wrapper.md).ClientBuilder

## Type parameters

| Name | Type | Default |
| :------ | :------ | :------ |
| `Stack` | [*DefaultClientStack*](../interfaces/core.defaultclientstack.md) | [*DefaultClientStack*](../interfaces/core.defaultclientstack.md) |

## Table of contents

### Constructors

- [constructor](wrapper.clientbuilder.md#constructor)

### Properties

- [client](wrapper.clientbuilder.md#client)

### Methods

- [build](wrapper.clientbuilder.md#build)
- [cache](wrapper.clientbuilder.md#cache)
- [rest](wrapper.clientbuilder.md#rest)

## Constructors

### constructor

\+ **new ClientBuilder**<Stack\>(`token`: *string*, `root`: [*ModuleHostModule*](wrapper.modulehostmodule.md)): [*ClientBuilder*](wrapper.clientbuilder.md)<Stack\>

#### Type parameters

| Name | Type | Default |
| :------ | :------ | :------ |
| `Stack` | [*DefaultClientStack*](../interfaces/core.defaultclientstack.md) | [*DefaultClientStack*](../interfaces/core.defaultclientstack.md) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `token` | *string* |
| `root` | [*ModuleHostModule*](wrapper.modulehostmodule.md) |

**Returns:** [*ClientBuilder*](wrapper.clientbuilder.md)<Stack\>

Defined in: [src/wrapper/ClientBuilder.ts:7](https://github.com/Discordoo/discordoo/blob/75592d0/src/wrapper/ClientBuilder.ts#L7)

## Properties

### client

• **client**: [*Client*](core.client.md)<Stack\>

Defined in: [src/wrapper/ClientBuilder.ts:7](https://github.com/Discordoo/discordoo/blob/75592d0/src/wrapper/ClientBuilder.ts#L7)

## Methods

### build

▸ **build**(): [*Client*](core.client.md)<Stack\>

**Returns:** [*Client*](core.client.md)<Stack\>

Defined in: [src/wrapper/ClientBuilder.ts:26](https://github.com/Discordoo/discordoo/blob/75592d0/src/wrapper/ClientBuilder.ts#L26)

___

### cache

▸ **cache**(`provider`: (`client`: [*Client*](core.client.md)<[*DefaultClientStack*](../interfaces/core.defaultclientstack.md)\>) => [*CacheProvider*](../modules/core.md#cacheprovider)<[*CacheNamespace*](../interfaces/core.cachenamespace.md)<unknown, unknown\>\>): [*ClientBuilder*](wrapper.clientbuilder.md)<Stack\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `provider` | (`client`: [*Client*](core.client.md)<[*DefaultClientStack*](../interfaces/core.defaultclientstack.md)\>) => [*CacheProvider*](../modules/core.md#cacheprovider)<[*CacheNamespace*](../interfaces/core.cachenamespace.md)<unknown, unknown\>\> |

**Returns:** [*ClientBuilder*](wrapper.clientbuilder.md)<Stack\>

Defined in: [src/wrapper/ClientBuilder.ts:21](https://github.com/Discordoo/discordoo/blob/75592d0/src/wrapper/ClientBuilder.ts#L21)

___

### rest

▸ **rest**(`provider`: (`client`: [*Client*](core.client.md)<[*DefaultClientStack*](../interfaces/core.defaultclientstack.md)\>) => [*RESTProvider*](../modules/core.md#restprovider)<[*RequestBuilder*](../interfaces/core.requestbuilder.md)\>): [*ClientBuilder*](wrapper.clientbuilder.md)<Stack\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `provider` | (`client`: [*Client*](core.client.md)<[*DefaultClientStack*](../interfaces/core.defaultclientstack.md)\>) => [*RESTProvider*](../modules/core.md#restprovider)<[*RequestBuilder*](../interfaces/core.requestbuilder.md)\> |

**Returns:** [*ClientBuilder*](wrapper.clientbuilder.md)<Stack\>

Defined in: [src/wrapper/ClientBuilder.ts:16](https://github.com/Discordoo/discordoo/blob/75592d0/src/wrapper/ClientBuilder.ts#L16)
