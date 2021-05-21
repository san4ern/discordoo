[discordoo](../README.md) / [Modules](../modules.md) / [rest](../modules/rest.md) / RESTClient

# Class: RESTClient

[rest](../modules/rest.md).RESTClient

Helps to send requests to Discord

## Table of contents

### Constructors

- [constructor](rest.restclient.md#constructor)

### Properties

- [options](rest.restclient.md#options)
- [token](rest.restclient.md#token)

### Methods

- [request](rest.restclient.md#request)

## Constructors

### constructor

\+ **new RESTClient**(`token`: *string*, `options?`: [*RESTOptions*](../interfaces/rest.restoptions.md)): [*RESTClient*](rest.restclient.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `token` | *string* | token to use in requests |
| `options` | [*RESTOptions*](../interfaces/rest.restoptions.md) | options |

**Returns:** [*RESTClient*](rest.restclient.md)

Defined in: [src/rest/RESTClient.ts:6](https://github.com/Discordoo/discordoo/blob/8db69d8/src/rest/RESTClient.ts#L6)

## Properties

### options

• **options**: [*RESTOptions*](../interfaces/rest.restoptions.md)

___

### token

• **token**: *string*

## Methods

### request

▸ **request**(`tokenOverride?`: *string*): [*RESTRequestBuilder*](rest.restrequestbuilder.md)

Create a request

#### Parameters

| Name | Type |
| :------ | :------ |
| `tokenOverride?` | *string* |

**Returns:** [*RESTRequestBuilder*](rest.restrequestbuilder.md)

Defined in: [src/rest/RESTClient.ts:14](https://github.com/Discordoo/discordoo/blob/8db69d8/src/rest/RESTClient.ts#L14)
