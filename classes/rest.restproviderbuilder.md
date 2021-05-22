[discordoo](../README.md) / [Modules](../modules.md) / [rest](../modules/rest.md) / RESTProviderBuilder

# Class: RESTProviderBuilder

[rest](../modules/rest.md).RESTProviderBuilder

Builds a RestProvider for [Client](core.client.md)

## Table of contents

### Constructors

- [constructor](rest.restproviderbuilder.md#constructor)

### Properties

- [client](rest.restproviderbuilder.md#client)

### Methods

- [getRestProvider](rest.restproviderbuilder.md#getrestprovider)

## Constructors

### constructor

\+ **new RESTProviderBuilder**(`options?`: [*RESTOptions*](../interfaces/rest.restoptions.md)): [*RESTProviderBuilder*](rest.restproviderbuilder.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [*RESTOptions*](../interfaces/rest.restoptions.md) | builder's options |

**Returns:** [*RESTProviderBuilder*](rest.restproviderbuilder.md)

Defined in: [src/rest/RESTProviderBuilder.ts:9](https://github.com/Discordoo/discordoo/blob/75592d0/src/rest/RESTProviderBuilder.ts#L9)

## Properties

### client

• **client**: [*RESTClient*](rest.restclient.md)

[RESTClient](rest.restclient.md) used by this builder

Defined in: [src/rest/RESTProviderBuilder.ts:9](https://github.com/Discordoo/discordoo/blob/75592d0/src/rest/RESTProviderBuilder.ts#L9)

## Methods

### getRestProvider

▸ **getRestProvider**(): *function*

Get rest provider

**Returns:** (`client`: [*Client*](core.client.md)<[*DefaultClientStack*](../interfaces/core.defaultclientstack.md)\>) => [*RESTProvider*](../modules/core.md#restprovider)<[*RequestBuilder*](../interfaces/core.requestbuilder.md)\>

Defined in: [src/rest/RESTProviderBuilder.ts:21](https://github.com/Discordoo/discordoo/blob/75592d0/src/rest/RESTProviderBuilder.ts#L21)
