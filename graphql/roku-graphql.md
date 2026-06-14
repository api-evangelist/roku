# Roku GraphQL Schema

This document describes a conceptual GraphQL schema for the Roku streaming platform, covering the Roku Pay Web Services (billing, subscriptions, transaction validation), External Control Protocol (ECP) for device control, content catalog (Direct Publisher and Search Feed), channel and media modeling, developer account management, and SceneGraph component concepts.

## Schema Source

The schema is derived from the following Roku developer resources:

- Roku Developer Program: https://developer.roku.com/en-gb/docs/developer-program/getting-started/roku-dev-prog.md
- Roku Pay Web Services: https://developer.roku.com/docs/developer-program/roku-pay/overview.md
- External Control Protocol: https://developer.roku.com/docs/developer-program/dev-tools/external-control-api.md
- Direct Publisher Feed: https://github.com/rokudev/feed-specifications
- Search Feed: https://github.com/rokudev/search-feed-json
- Nabu Cloud: https://github.com/rokudev/dev-doc
- GitHub Organization: https://github.com/rokudev

## Top-Level Types

### Content Catalog

- **Channel** — a Roku channel application installed on a device or available in the Channel Store.
- **ChannelItem** — an individual item within a channel's content listing.
- **ChannelCategory** — a grouping of content within a channel (e.g., genre, collection).
- **ChannelContent** — content metadata associated with a channel, referencing movies, series, and live feeds.
- **Media** — abstract base type for all playable media on the Roku platform.
- **Movie** — a long-form film with metadata such as title, description, ratings, availability windows, and content URLs.
- **Series** — a TV series with one or more seasons.
- **Season** — a season of a series containing ordered episodes.
- **Episode** — a single episode within a season, with its own content URLs and metadata.
- **Clip** — a short-form video clip or promotional excerpt.
- **Live** — a live-streaming feed with a real-time content URL.
- **LinearChannel** — a 24/7 linear programming channel with an EPG feed.

### Feed Content

- **FeedContent** — the root object for a Direct Publisher or Search Feed JSON payload.
- **ContentItem** — a polymorphic content entry within a feed (movie, series, live, etc.).
- **ContentCategory** — a category label used to group content items within a feed.
- **ContentDetail** — extended metadata for a content item including genres, tags, and localized titles.

### People and Credits

- **Actor** — a cast member associated with a content item.
- **Director** — a director credit associated with a content item.

### Ratings and Availability

- **Rating** — a content rating (e.g., TV-MA, PG-13) attached to a media item.
- **RatingType** — the rating authority or system (e.g., MPAA, TV Parental Guidelines).
- **AvailabilityWindow** — a time window during which a content item is available for streaming.

### Billing and Payments

- **Price** — a monetary amount associated with a purchase or subscription.
- **PriceType** — the pricing model (one-time purchase, monthly subscription, annual subscription).
- **EntitlementGrant** — a record of a subscription or purchase entitlement granted to a user.
- **EntitlementRevoke** — a record of an entitlement revocation or cancellation.
- **Purchase** — a transactional purchase of content or a subscription product.
- **PurchaseItem** — an individual line item within a purchase (product ID, quantity, price).
- **BillingRecord** — a Roku Pay billing transaction record with status and timestamp.

### TRS (Transactional/Recurring Subscriptions)

- **TRSContent** — content metadata for a transactional or recurring subscription product.
- **TRSChannel** — a Roku channel configured with TRS monetization.

### Player and Device

- **Player** — the media player state of a Roku device (current content, playback position, status).
- **PlayerSettings** — configurable playback preferences on a Roku device.
- **Device** — a Roku device on the local network, identified by serial number and model.
- **DeviceModel** — the hardware model specification for a Roku device.
- **DeviceSettings** — user-configurable settings on a Roku device (audio, display, network).
- **NetworkInfo** — network configuration details for a Roku device (IP, MAC, WiFi SSID).
- **DisplayType** — the display capability of a Roku device (HD, 4K, HDR).
- **AudioType** — the audio output capability of a Roku device (stereo, Dolby Atmos, DTS).

### Applications and SceneGraph

- **AppInfo** — metadata about an installed Roku channel application (ID, name, version, type).
- **SceneGraphComponent** — a SceneGraph UI node component with type, fields, and child nodes.
- **SubscribeButton** — a SceneGraph component for triggering subscription purchases.
- **SignInScreen** — a SceneGraph component for implementing user sign-in UI.
- **Signup** — a representation of a new user signup event within a Roku channel.

### External Control Protocol (ECP)

- **ECP** — the root object for External Control Protocol interactions with a local Roku device.
- **ECPControl** — an ECP command issued to a Roku device (launch app, set channel, etc.).
- **ECPInput** — an ECP deep-link input payload for passing parameters to an app at launch.
- **ECPKeyPress** — a simulated remote-control key press event sent via ECP.

### Developer and Authentication

- **APIKey** — an API key credential for authenticating with Roku Pay Web Services.
- **APISession** — an active authenticated session with a Roku developer API.
- **DeveloperAccount** — a Roku developer account with associated channels, API keys, and billing.
- **TestUser** — a test user account used in Roku Pay sandbox testing.

### Channel Store

- **ChannelStore** — the Roku Channel Store, providing discovery and installation of channels.

## Queries

- `channel(id: ID!)` — fetch a channel by ID.
- `channels(filter: ChannelFilter)` — list channels matching filter criteria.
- `device(serialNumber: String!)` — fetch a Roku device by serial number.
- `devices` — list all Roku devices on the local network (via ECP discovery).
- `movie(id: ID!)` — fetch a movie by ID.
- `series(id: ID!)` — fetch a series by ID.
- `episode(id: ID!)` — fetch an episode by ID.
- `purchase(transactionId: String!)` — fetch a purchase record by transaction ID.
- `entitlement(customerId: String!, channelId: String!)` — check entitlement for a customer.
- `billingRecord(transactionId: String!)` — fetch a billing record.
- `appInfo(deviceId: ID!)` — fetch the active app on a device.
- `installedApps(deviceId: ID!)` — list all installed apps on a device.
- `feedContent(feedUrl: String!)` — fetch and parse a Direct Publisher or Search Feed.
- `developerAccount(id: ID!)` — fetch a developer account by ID.
- `channelStore(query: String)` — search the Roku Channel Store.

## Mutations

- `launchApp(deviceId: ID!, appId: String!, input: ECPInputInput)` — launch a Roku app via ECP.
- `sendKeyPress(deviceId: ID!, key: KeyType!)` — send a key press via ECP.
- `validateTransaction(transactionId: String!, apiKey: String!)` — validate a Roku Pay transaction.
- `cancelSubscription(customerId: String!, channelId: String!, apiKey: String!)` — cancel a subscription.
- `refundTransaction(transactionId: String!, amount: Float, apiKey: String!)` — refund a transaction.
- `updateBillCycle(customerId: String!, channelId: String!, newDate: String!, apiKey: String!)` — update billing cycle date.
- `issueCredit(customerId: String!, channelId: String!, amount: Float!, apiKey: String!)` — issue a service credit.
- `grantEntitlement(customerId: String!, channelId: String!, productId: String!, apiKey: String!)` — grant an entitlement.
- `revokeEntitlement(customerId: String!, channelId: String!, productId: String!, apiKey: String!)` — revoke an entitlement.

## Subscriptions

- `deviceStatus(deviceId: ID!)` — stream real-time player and network status updates from a Roku device.
- `billingEvents(channelId: String!, apiKey: String!)` — stream billing events for a channel.
