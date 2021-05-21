[discordoo](../README.md) / [Modules](../modules.md) / [core](../modules/core.md) / RequestBuilder

# Interface: RequestBuilder

[core](../modules/core.md).RequestBuilder

Represents a request builder

## Implemented by

- [*RESTRequestBuilder*](../classes/rest.restrequestbuilder.md)

## Table of contents

### Methods

- [delete](core.requestbuilder.md#delete)
- [get](core.requestbuilder.md#get)
- [patch](core.requestbuilder.md#patch)
- [post](core.requestbuilder.md#post)
- [put](core.requestbuilder.md#put)
- [query](core.requestbuilder.md#query)
- [url](core.requestbuilder.md#url)

## Methods

### delete

▸ **delete**<T\>(`options?`: [*RequestOptions*](core.requestoptions.md)): *Promise*<[*RESTResponse*](core.restresponse.md)<T\>\>

Create DELETE request

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options?` | [*RequestOptions*](core.requestoptions.md) | options |

**Returns:** *Promise*<[*RESTResponse*](core.restresponse.md)<T\>\>

Defined in: [src/core/providers/rest/RequestBuilder.ts:35](https://github.com/Discordoo/discordoo/blob/8db69d8/src/core/providers/rest/RequestBuilder.ts#L35)

___

### get

▸ **get**<T\>(`options?`: [*RequestOptions*](core.requestoptions.md)): *Promise*<[*RESTResponse*](core.restresponse.md)<T\>\>

Create GET request

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options?` | [*RequestOptions*](core.requestoptions.md) | options |

**Returns:** *Promise*<[*RESTResponse*](core.restresponse.md)<T\>\>

Defined in: [src/core/providers/rest/RequestBuilder.ts:23](https://github.com/Discordoo/discordoo/blob/8db69d8/src/core/providers/rest/RequestBuilder.ts#L23)

___

### patch

▸ **patch**<T\>(`options?`: [*RequestOptions*](core.requestoptions.md)): *Promise*<[*RESTResponse*](core.restresponse.md)<T\>\>

Create PATCH request

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options?` | [*RequestOptions*](core.requestoptions.md) | options |

**Returns:** *Promise*<[*RESTResponse*](core.restresponse.md)<T\>\>

Defined in: [src/core/providers/rest/RequestBuilder.ts:47](https://github.com/Discordoo/discordoo/blob/8db69d8/src/core/providers/rest/RequestBuilder.ts#L47)

___

### post

▸ **post**<T\>(`options?`: [*RequestOptions*](core.requestoptions.md)): *Promise*<[*RESTResponse*](core.restresponse.md)<T\>\>

Create POST request

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options?` | [*RequestOptions*](core.requestoptions.md) | options |

**Returns:** *Promise*<[*RESTResponse*](core.restresponse.md)<T\>\>

Defined in: [src/core/providers/rest/RequestBuilder.ts:29](https://github.com/Discordoo/discordoo/blob/8db69d8/src/core/providers/rest/RequestBuilder.ts#L29)

___

### put

▸ **put**<T\>(`options?`: [*RequestOptions*](core.requestoptions.md)): *Promise*<[*RESTResponse*](core.restresponse.md)<T\>\>

Create PUT request

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options?` | [*RequestOptions*](core.requestoptions.md) | options |

**Returns:** *Promise*<[*RESTResponse*](core.restresponse.md)<T\>\>

Defined in: [src/core/providers/rest/RequestBuilder.ts:41](https://github.com/Discordoo/discordoo/blob/8db69d8/src/core/providers/rest/RequestBuilder.ts#L41)

___

### query

▸ **query**(`k`: *string*, `v`: *string*): [*RequestBuilder*](core.requestbuilder.md)

Add query data

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `k` | *string* | key |
| `v` | *string* | value |

**Returns:** [*RequestBuilder*](core.requestbuilder.md)

Defined in: [src/core/providers/rest/RequestBuilder.ts:17](https://github.com/Discordoo/discordoo/blob/8db69d8/src/core/providers/rest/RequestBuilder.ts#L17)

___

### url

▸ **url**(...`paths`: *string*[]): [*RequestBuilder*](core.requestbuilder.md)

Add part(s) to the URI

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...paths` | *string*[] | paths |

**Returns:** [*RequestBuilder*](core.requestbuilder.md)

Defined in: [src/core/providers/rest/RequestBuilder.ts:10](https://github.com/Discordoo/discordoo/blob/8db69d8/src/core/providers/rest/RequestBuilder.ts#L10)
