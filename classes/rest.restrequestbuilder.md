[discordoo](../README.md) / [Modules](../modules.md) / [rest](../modules/rest.md) / RESTRequestBuilder

# Class: RESTRequestBuilder

[rest](../modules/rest.md).RESTRequestBuilder

Create requests to Discord

**`internal`**

## Implements

- [*RequestBuilder*](../interfaces/core.requestbuilder.md)

## Table of contents

### Constructors

- [constructor](rest.restrequestbuilder.md#constructor)

### Properties

- [options](rest.restrequestbuilder.md#options)
- [queryStack](rest.restrequestbuilder.md#querystack)
- [retries](rest.restrequestbuilder.md#retries)
- [stack](rest.restrequestbuilder.md#stack)
- [token](rest.restrequestbuilder.md#token)

### Accessors

- [endpoint](rest.restrequestbuilder.md#endpoint)

### Methods

- [delete](rest.restrequestbuilder.md#delete)
- [get](rest.restrequestbuilder.md#get)
- [getHeaders](rest.restrequestbuilder.md#getheaders)
- [patch](rest.restrequestbuilder.md#patch)
- [post](rest.restrequestbuilder.md#post)
- [put](rest.restrequestbuilder.md#put)
- [query](rest.restrequestbuilder.md#query)
- [request](rest.restrequestbuilder.md#request)
- [url](rest.restrequestbuilder.md#url)

## Constructors

### constructor

\+ **new RESTRequestBuilder**(`token`: *string*, `options`: [*RESTOptions*](../interfaces/rest.restoptions.md)): [*RESTRequestBuilder*](rest.restrequestbuilder.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `token` | *string* | token to be used by this request |
| `options` | [*RESTOptions*](../interfaces/rest.restoptions.md) | request options |

**Returns:** [*RESTRequestBuilder*](rest.restrequestbuilder.md)

Defined in: [src/rest/RESTRequestBuilder.ts:21](https://github.com/Discordoo/discordoo/blob/8db69d8/src/rest/RESTRequestBuilder.ts#L21)

## Properties

### options

• **options**: [*RESTOptions*](../interfaces/rest.restoptions.md)

Tokens used by this request

Defined in: [src/rest/RESTRequestBuilder.ts:21](https://github.com/Discordoo/discordoo/blob/8db69d8/src/rest/RESTRequestBuilder.ts#L21)

___

### queryStack

• `Private` **queryStack**: *Record*<string, string\>

Query to be built

Defined in: [src/rest/RESTRequestBuilder.ts:14](https://github.com/Discordoo/discordoo/blob/8db69d8/src/rest/RESTRequestBuilder.ts#L14)

___

### retries

• `Private` **retries**: *number*= 0

Retries done

Defined in: [src/rest/RESTRequestBuilder.ts:16](https://github.com/Discordoo/discordoo/blob/8db69d8/src/rest/RESTRequestBuilder.ts#L16)

___

### stack

• `Private` **stack**: *string*[]

URI parts

Defined in: [src/rest/RESTRequestBuilder.ts:12](https://github.com/Discordoo/discordoo/blob/8db69d8/src/rest/RESTRequestBuilder.ts#L12)

___

### token

• **token**: *string*

Token of this request

Defined in: [src/rest/RESTRequestBuilder.ts:19](https://github.com/Discordoo/discordoo/blob/8db69d8/src/rest/RESTRequestBuilder.ts#L19)

## Accessors

### endpoint

• get **endpoint**(): *string*

URI request will be sent to

**Returns:** *string*

Defined in: [src/rest/RESTRequestBuilder.ts:64](https://github.com/Discordoo/discordoo/blob/8db69d8/src/rest/RESTRequestBuilder.ts#L64)

## Methods

### delete

▸ **delete**<T\>(`options?`: [*RequestOptions*](../interfaces/core.requestoptions.md)): *Promise*<[*RESTResponse*](../interfaces/core.restresponse.md)<T\>\>

Create DELETE request

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [*RequestOptions*](../interfaces/core.requestoptions.md) | options |

**Returns:** *Promise*<[*RESTResponse*](../interfaces/core.restresponse.md)<T\>\>

Implementation of: [RequestBuilder](../interfaces/core.requestbuilder.md)

Defined in: [src/rest/RESTRequestBuilder.ts:154](https://github.com/Discordoo/discordoo/blob/8db69d8/src/rest/RESTRequestBuilder.ts#L154)

___

### get

▸ **get**<T\>(`options?`: *Omit*<[*RequestOptions*](../interfaces/core.requestoptions.md), ``"body"``\>): *Promise*<[*RESTResponse*](../interfaces/core.restresponse.md)<T\>\>

Create GET request

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | *Omit*<[*RequestOptions*](../interfaces/core.requestoptions.md), ``"body"``\> | options |

**Returns:** *Promise*<[*RESTResponse*](../interfaces/core.restresponse.md)<T\>\>

Implementation of: [RequestBuilder](../interfaces/core.requestbuilder.md)

Defined in: [src/rest/RESTRequestBuilder.ts:122](https://github.com/Discordoo/discordoo/blob/8db69d8/src/rest/RESTRequestBuilder.ts#L122)

___

### getHeaders

▸ `Private` **getHeaders**(`headers?`: *Record*<any, any\>): *object*

Get headers

#### Parameters

| Name | Type |
| :------ | :------ |
| `headers?` | *Record*<any, any\> |

**Returns:** *object*

| Name | Type |
| :------ | :------ |
| `Authorization` | *string* |
| `Content-Type` | *string* |
| `User-Agent` | *string* |

Defined in: [src/rest/RESTRequestBuilder.ts:35](https://github.com/Discordoo/discordoo/blob/8db69d8/src/rest/RESTRequestBuilder.ts#L35)

___

### patch

▸ **patch**<T\>(`options?`: [*RequestOptions*](../interfaces/core.requestoptions.md)): *Promise*<[*RESTResponse*](../interfaces/core.restresponse.md)<T\>\>

Create PATCH request

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [*RequestOptions*](../interfaces/core.requestoptions.md) | options |

**Returns:** *Promise*<[*RESTResponse*](../interfaces/core.restresponse.md)<T\>\>

Implementation of: [RequestBuilder](../interfaces/core.requestbuilder.md)

Defined in: [src/rest/RESTRequestBuilder.ts:138](https://github.com/Discordoo/discordoo/blob/8db69d8/src/rest/RESTRequestBuilder.ts#L138)

___

### post

▸ **post**<T\>(`options?`: [*RequestOptions*](../interfaces/core.requestoptions.md)): *Promise*<[*RESTResponse*](../interfaces/core.restresponse.md)<T\>\>

Create POST request

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [*RequestOptions*](../interfaces/core.requestoptions.md) | options |

**Returns:** *Promise*<[*RESTResponse*](../interfaces/core.restresponse.md)<T\>\>

Implementation of: [RequestBuilder](../interfaces/core.requestbuilder.md)

Defined in: [src/rest/RESTRequestBuilder.ts:130](https://github.com/Discordoo/discordoo/blob/8db69d8/src/rest/RESTRequestBuilder.ts#L130)

___

### put

▸ **put**<T\>(`options?`: [*RequestOptions*](../interfaces/core.requestoptions.md)): *Promise*<[*RESTResponse*](../interfaces/core.restresponse.md)<T\>\>

Create PUT request

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [*RequestOptions*](../interfaces/core.requestoptions.md) | options |

**Returns:** *Promise*<[*RESTResponse*](../interfaces/core.restresponse.md)<T\>\>

Implementation of: [RequestBuilder](../interfaces/core.requestbuilder.md)

Defined in: [src/rest/RESTRequestBuilder.ts:146](https://github.com/Discordoo/discordoo/blob/8db69d8/src/rest/RESTRequestBuilder.ts#L146)

___

### query

▸ **query**(`k`: *string*, `v`: *any*): [*RequestBuilder*](../interfaces/core.requestbuilder.md)

Add query data

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `k` | *string* | key |
| `v` | *any* | value |

**Returns:** [*RequestBuilder*](../interfaces/core.requestbuilder.md)

Implementation of: [RequestBuilder](../interfaces/core.requestbuilder.md)

Defined in: [src/rest/RESTRequestBuilder.ts:49](https://github.com/Discordoo/discordoo/blob/8db69d8/src/rest/RESTRequestBuilder.ts#L49)

___

### request

▸ **request**<T\>(`method`: ``"GET"`` \| ``"POST"`` \| ``"PUT"`` \| ``"PATCH"`` \| ``"DELETE"``, `options?`: [*RequestOptions*](../interfaces/core.requestoptions.md)): *Promise*<[*RESTResponse*](../interfaces/core.restresponse.md)<T\>\>

Create a request

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `method` | ``"GET"`` \| ``"POST"`` \| ``"PUT"`` \| ``"PATCH"`` \| ``"DELETE"`` | method to be used |
| `options` | [*RequestOptions*](../interfaces/core.requestoptions.md) | options |

**Returns:** *Promise*<[*RESTResponse*](../interfaces/core.restresponse.md)<T\>\>

Defined in: [src/rest/RESTRequestBuilder.ts:77](https://github.com/Discordoo/discordoo/blob/8db69d8/src/rest/RESTRequestBuilder.ts#L77)

___

### url

▸ **url**(...`paths`: *string*[]): [*RequestBuilder*](../interfaces/core.requestbuilder.md)

Add part(s) to the URI

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...paths` | *string*[] | paths |

**Returns:** [*RequestBuilder*](../interfaces/core.requestbuilder.md)

Implementation of: [RequestBuilder](../interfaces/core.requestbuilder.md)

Defined in: [src/rest/RESTRequestBuilder.ts:58](https://github.com/Discordoo/discordoo/blob/8db69d8/src/rest/RESTRequestBuilder.ts#L58)
