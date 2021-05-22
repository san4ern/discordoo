[discordoo](../README.md) / [Modules](../modules.md) / [rest](../modules/rest.md) / RESTOptions

# Interface: RESTOptions

[rest](../modules/rest.md).RESTOptions

Options for rest

## Table of contents

### Properties

- [maxRetries](rest.restoptions.md#maxretries)
- [useragent](rest.restoptions.md#useragent)
- [v](rest.restoptions.md#v)

## Properties

### maxRetries

• **maxRetries**: *number*

Times, REST will try to perform the request with 5xx error code

Defined in: [src/rest/RESTOptions.ts:11](https://github.com/Discordoo/discordoo/blob/75592d0/src/rest/RESTOptions.ts#L11)

___

### useragent

• **useragent**: *string*

UserAgent to use
Shouldn't be used, since Discord requires it to contain library name and it's version

Defined in: [src/rest/RESTOptions.ts:9](https://github.com/Discordoo/discordoo/blob/75592d0/src/rest/RESTOptions.ts#L9)

___

### v

• **v**: *number*

API version to use

Defined in: [src/rest/RESTOptions.ts:4](https://github.com/Discordoo/discordoo/blob/75592d0/src/rest/RESTOptions.ts#L4)
