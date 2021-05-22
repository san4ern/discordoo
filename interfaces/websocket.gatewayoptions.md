[discordoo](../README.md) / [Modules](../modules.md) / [websocket](../modules/websocket.md) / GatewayOptions

# Interface: GatewayOptions

[websocket](../modules/websocket.md).GatewayOptions

## Hierarchy

- *GatewayIdentifyData*

  ↳ **GatewayOptions**

## Table of contents

### Properties

- [compress](websocket.gatewayoptions.md#compress)
- [guild\_subscriptions](websocket.gatewayoptions.md#guild_subscriptions)
- [intents](websocket.gatewayoptions.md#intents)
- [large\_threshold](websocket.gatewayoptions.md#large_threshold)
- [maxShards](websocket.gatewayoptions.md#maxshards)
- [presence](websocket.gatewayoptions.md#presence)
- [properties](websocket.gatewayoptions.md#properties)
- [shard](websocket.gatewayoptions.md#shard)
- [shards](websocket.gatewayoptions.md#shards)
- [spawnDelay](websocket.gatewayoptions.md#spawndelay)
- [token](websocket.gatewayoptions.md#token)
- [url](websocket.gatewayoptions.md#url)
- [version](websocket.gatewayoptions.md#version)

## Properties

### compress

• `Optional` **compress**: *boolean*

Whether this connection supports compression of packets

**`default`** false

Inherited from: GatewayIdentifyData.compress

Defined in: node_modules/discord-api-types/v8/gateway/index.d.ts:1030

___

### guild\_subscriptions

• `Optional` **guild\_subscriptions**: *boolean*

Enables dispatching of guild subscription events (presence and typing events)

**`default`** true

**`deprecated`** Use `intents` instead

Inherited from: GatewayIdentifyData.guild\_subscriptions

Defined in: node_modules/discord-api-types/v8/gateway/index.d.ts:1056

___

### intents

• **intents**: *number*

The Gateway Intents you wish to receive

See https://discord.com/developers/docs/topics/gateway#gateway-intents

Inherited from: GatewayIdentifyData.intents

Defined in: node_modules/discord-api-types/v8/gateway/index.d.ts:1062

___

### large\_threshold

• `Optional` **large\_threshold**: *number*

Value between 50 and 250, total number of members where the gateway will stop sending
offline members in the guild member list

**`default`** 50

Inherited from: GatewayIdentifyData.large\_threshold

Defined in: node_modules/discord-api-types/v8/gateway/index.d.ts:1037

___

### maxShards

• `Optional` **maxShards**: *number*

Maximum amount of shards that can be spawned by the [WebSocketManager](../classes/websocket.websocketmanager.md)

Defined in: [src/websocket/GatewayOptions.ts:13](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/GatewayOptions.ts#L13)

___

### presence

• `Optional` **presence**: GatewayPresenceUpdateData

Presence structure for initial presence information

See https://discord.com/developers/docs/topics/gateway#update-status

Inherited from: GatewayIdentifyData.presence

Defined in: node_modules/discord-api-types/v8/gateway/index.d.ts:1049

___

### properties

• **properties**: GatewayIdentifyProperties

Connection properties

See https://discord.com/developers/docs/topics/gateway#identify-identify-connection-properties

Inherited from: GatewayIdentifyData.properties

Defined in: node_modules/discord-api-types/v8/gateway/index.d.ts:1024

___

### shard

• `Optional` **shard**: [shard\_id: number, shard\_count: number]

Used for Guild Sharding

See https://discord.com/developers/docs/topics/gateway#sharding

Inherited from: GatewayIdentifyData.shard

Defined in: node_modules/discord-api-types/v8/gateway/index.d.ts:1043

___

### shards

• `Optional` **shards**: *number* \| *number*[] \| ``"auto"``

If number is provided - WS will create X shards
If auto is provided, shards amount will be fetched from Discord
If array of numbers is provided, the library will interpret it as IDs of shards to be spawned

Defined in: [src/websocket/GatewayOptions.ts:9](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/GatewayOptions.ts#L9)

___

### spawnDelay

• `Optional` **spawnDelay**: *number*

Waiting time between shards launches, in ms

Defined in: [src/websocket/GatewayOptions.ts:24](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/GatewayOptions.ts#L24)

___

### token

• **token**: *string*

Authentication token

Inherited from: GatewayIdentifyData.token

Defined in: node_modules/discord-api-types/v8/gateway/index.d.ts:1018

___

### url

• `Optional` **url**: *string*

Gateway URL

Defined in: [src/websocket/GatewayOptions.ts:21](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/GatewayOptions.ts#L21)

___

### version

• `Optional` **version**: ``9``

Version of gateway to use

Defined in: [src/websocket/GatewayOptions.ts:18](https://github.com/Discordoo/discordoo/blob/75592d0/src/websocket/GatewayOptions.ts#L18)
