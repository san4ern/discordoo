[discordoo](../README.md) / [Modules](../modules.md) / core

# Module: core

## Table of contents

### Classes

- [Base](../classes/core.base.md)
- [Client](../classes/core.client.md)
- [Constants](../classes/core.constants.md)
- [ModuleManager](../classes/core.modulemanager.md)

### Interfaces

- [CacheNamespace](../interfaces/core.cachenamespace.md)
- [ClientEventsHandlers](../interfaces/core.clienteventshandlers.md)
- [DefaultClientStack](../interfaces/core.defaultclientstack.md)
- [GatewayProviderAPI](../interfaces/core.gatewayproviderapi.md)
- [Module](../interfaces/core.module.md)
- [RESTResponse](../interfaces/core.restresponse.md)
- [RequestBuilder](../interfaces/core.requestbuilder.md)
- [RequestOptions](../interfaces/core.requestoptions.md)

### Type aliases

- [CacheProvider](core.md#cacheprovider)
- [GatewayProvider](core.md#gatewayprovider)
- [RESTProvider](core.md#restprovider)

## Type aliases

### CacheProvider

Ƭ **CacheProvider**<T\>: (`namespace`: *string*) => T

Represents a CacheProvider. Bound to Client context

#### Type parameters

| Name | Type | Default |
| :------ | :------ | :------ |
| `T` | [*CacheNamespace*](../interfaces/core.cachenamespace.md) | [*CacheNamespace*](../interfaces/core.cachenamespace.md) |

#### Type declaration

▸ (`namespace`: *string*): T

#### Parameters

| Name | Type |
| :------ | :------ |
| `namespace` | *string* |

**Returns:** T

Defined in: [src/core/providers/cache/CacheProvider.ts:4](https://github.com/Discordoo/discordoo/blob/75592d0/src/core/providers/cache/CacheProvider.ts#L4)

___

### GatewayProvider

Ƭ **GatewayProvider**<T\>: () => T

#### Type parameters

| Name | Type | Default |
| :------ | :------ | :------ |
| `T` | [*GatewayProviderAPI*](../interfaces/core.gatewayproviderapi.md) | [*GatewayProviderAPI*](../interfaces/core.gatewayproviderapi.md) |

#### Type declaration

▸ (): T

**Returns:** T

Defined in: [src/core/providers/gateway/GatewayProvider.ts:12](https://github.com/Discordoo/discordoo/blob/75592d0/src/core/providers/gateway/GatewayProvider.ts#L12)

___

### RESTProvider

Ƭ **RESTProvider**<T\>: () => T

Represents a RESTProvider. Bound to Client context

#### Type parameters

| Name | Type | Default |
| :------ | :------ | :------ |
| `T` | [*RequestBuilder*](../interfaces/core.requestbuilder.md) | [*RequestBuilder*](../interfaces/core.requestbuilder.md) |

#### Type declaration

▸ (): T

**Returns:** T

Defined in: [src/core/providers/rest/RESTProvider.ts:4](https://github.com/Discordoo/discordoo/blob/75592d0/src/core/providers/rest/RESTProvider.ts#L4)
