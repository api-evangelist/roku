# Roku (roku)
Roku is the leading TV streaming platform in the U.S., Canada, and Mexico, offering a comprehensive operating system that powers smart TVs, streaming players, and audio devices. Roku provides a robust developer program for building channel apps, monetizing through Roku Pay, integrating analytics, and controlling devices via the External Control Protocol. The platform supports both BrightScript and SceneGraph frameworks for app development, and the Nabu Cloud developer cloud for managing remote test devices and channel builds.

**URL:** [Visit APIs.json URL](https://github.com/api-evangelist/roku)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Streaming, Television, Media, Entertainment, Connected TV, Consumer Electronics

## Timestamps

- **Created:** 2026-05-04
- **Modified:** 2026-05-05

## APIs

### Roku BrightScript SDK
BrightScript is Roku's scripting language used to build apps for the Roku platform. The SDK provides a comprehensive component library with over 100 built-in objects covering UI, networking, media playback, and device interaction. BrightScript is a programming language and on-device runtime, not a network API.

**Human URL:** [https://developer.roku.com/docs/references/brightscript/component-reference.md](https://developer.roku.com/docs/references/brightscript/component-reference.md)

#### Tags:

 - SDK, BrightScript, Channel Development

#### Properties

- [Documentation](https://developer.roku.com/docs/references/brightscript/component-reference.md)
- [APIReference](https://developer.roku.com/docs/references/brightscript/component-reference.md)

### Roku SceneGraph
SceneGraph is Roku's XML-based declarative UI framework for building rich, performant channel applications. It provides node components, animations, and a scene-based architecture. SceneGraph is an on-device UI framework, not a network API.

**Human URL:** [https://developer.roku.com/docs/developer-program/core-concepts/scenegraph-overview.md](https://developer.roku.com/docs/developer-program/core-concepts/scenegraph-overview.md)

#### Tags:

 - UI Framework, SceneGraph, Channel Development

#### Properties

- [Documentation](https://developer.roku.com/docs/developer-program/core-concepts/scenegraph-overview.md)
- [APIReference](https://developer.roku.com/docs/references/scenegraph/component-reference.md)

### Roku External Control Protocol (ECP)
The External Control Protocol (ECP) is an HTTP-based API exposed on port 8060 of every Roku device on the local network. It enables third-party applications, mobile remote-control apps, automated test systems, and home-automation hubs to discover devices via SSDP, inject simulated remote-control key presses, launch installed apps with deep-link parameters, query device state, and retrieve developer-mode diagnostics.

**Human URL:** [https://developer.roku.com/docs/developer-program/dev-tools/external-control-api.md](https://developer.roku.com/docs/developer-program/dev-tools/external-control-api.md)

#### Tags:

 - REST, HTTP, Device Control, LAN

#### Properties

- [Documentation](https://developer.roku.com/docs/developer-program/dev-tools/external-control-api.md)
- [APIReference](https://developer.roku.com/docs/developer-program/dev-tools/external-control-api.md)
- [OpenAPI](openapi/roku-external-control-protocol.yaml)
- [JSONSchema (Active App Schema)](json-schema/external-control-protocol-active-app-schema.json)
- [JSONSchema (App List Schema)](json-schema/external-control-protocol-app-list-schema.json)
- [JSONSchema (App Schema)](json-schema/external-control-protocol-app-schema.json)
- [JSONSchema (Device Info Schema)](json-schema/external-control-protocol-device-info-schema.json)
- [JSONSchema (Media Player Schema)](json-schema/external-control-protocol-media-player-schema.json)
- [JSONStructure (Device Info Structure)](json-structure/external-control-protocol-device-info-structure.json)
- [JSONStructure (App Structure)](json-structure/external-control-protocol-app-structure.json)
- [JSONStructure (App List Structure)](json-structure/external-control-protocol-app-list-structure.json)
- [JSONStructure (Active App Structure)](json-structure/external-control-protocol-active-app-structure.json)
- [JSONStructure (Media Player Structure)](json-structure/external-control-protocol-media-player-structure.json)
- [JSON-LD](json-ld/roku-external-control-protocol-context.jsonld)
- [Example (Query Device Info Example)](examples/external-control-protocol-query-device-info-example.json)
- [Example (Query Apps Example)](examples/external-control-protocol-query-apps-example.json)
- [Example (Launch App Example)](examples/external-control-protocol-launch-app-example.json)

### Roku Pay Web Services
Roku Pay Web Services provide server-to-server APIs for billing, subscription management, transaction validation, and entitlement checks for monetized Roku channels. Channels query these endpoints from their authentication backends to verify entitlements, issue refunds, adjust billing cycles, and grant service credits.

**Human URL:** [https://developer.roku.com/docs/developer-program/roku-pay/overview.md](https://developer.roku.com/docs/developer-program/roku-pay/overview.md)

#### Tags:

 - Billing, Payments, Subscriptions, Monetization

#### Properties

- [Documentation](https://developer.roku.com/docs/developer-program/roku-pay/overview.md)
- [APIReference](https://developer.roku.com/dev/docs/roku-web-service)
- [OpenAPI](openapi/roku-pay-web-services.yaml)
- [JSONSchema (Transaction Validation Schema)](json-schema/pay-web-services-transaction-validation-schema.json)
- [JSONSchema (Refund Validation Schema)](json-schema/pay-web-services-refund-validation-schema.json)
- [JSONSchema (Cancel Subscription Request Schema)](json-schema/pay-web-services-cancel-subscription-request-schema.json)
- [JSONSchema (Refund Subscription Request Schema)](json-schema/pay-web-services-refund-subscription-request-schema.json)
- [JSONSchema (Update Bill Cycle Request Schema)](json-schema/pay-web-services-update-bill-cycle-request-schema.json)
- [JSONSchema (Issue Credit Request Schema)](json-schema/pay-web-services-issue-credit-request-schema.json)
- [JSONSchema (Subscription Result Schema)](json-schema/pay-web-services-subscription-result-schema.json)
- [JSONStructure (Transaction Validation Structure)](json-structure/pay-web-services-transaction-validation-structure.json)
- [JSONStructure (Refund Validation Structure)](json-structure/pay-web-services-refund-validation-structure.json)
- [JSONStructure (Subscription Result Structure)](json-structure/pay-web-services-subscription-result-structure.json)
- [JSON-LD](json-ld/roku-pay-web-services-context.jsonld)
- [Example (Validate Transaction Example)](examples/pay-web-services-validate-transaction-example.json)
- [Example (Cancel Subscription Example)](examples/pay-web-services-cancel-subscription-example.json)

### Roku Nabu Cloud
Nabu Cloud is Roku's developer cloud platform for managing remote test devices, snapshots, builds, projects, organisations, groups, and personal access tokens. It provides REST APIs (and an AsyncAPI streaming endpoint) for orchestrating remote Roku test devices and CI/CD workflows. The OpenAPI specification is published in the Roku dev-doc repository.

**Human URL:** [https://github.com/rokudev/dev-doc/tree/v2.0/reference/nabu_cloud](https://github.com/rokudev/dev-doc/tree/v2.0/reference/nabu_cloud)

#### Tags:

 - REST, Developer Cloud, Test Devices, CI CD

#### Properties

- [Documentation](https://github.com/rokudev/dev-doc/tree/v2.0/reference/nabu_cloud)
- [OpenAPI](openapi/roku-nabu-cloud.yaml)
- [JSON-LD](json-ld/roku-nabu-cloud-context.jsonld)
- [Example (List Devices Example)](examples/nabu-cloud-list-devices-example.json)
- [Example (Create Device Example)](examples/nabu-cloud-create-device-example.json)

### Roku Search Feed
Roku Search Feed is a JSON feed format that publishers ingest to expose their catalog to Roku Search. The feed provides movies, series, episodes, short-form videos, TV specials, and live feeds with localized titles, descriptions, ratings, content links, and external IDs.

**Human URL:** [https://github.com/rokudev/search-feed-json](https://github.com/rokudev/search-feed-json)

#### Tags:

 - Feed, Search, Content Catalog

#### Properties

- [Documentation](https://github.com/rokudev/search-feed-json)
- [JSONSchema (Search Feed Schema)](json-schema/search-feed-schema.json)
- [JSON-LD](json-ld/roku-search-feed-context.jsonld)
- [Example (Simple Search Feed Example)](examples/roku-search-feed-simple-example.json)
- [Example (Advanced Search Feed Example)](examples/roku-search-feed-advanced-example.json)

### Roku Direct Publisher Feed
Roku Direct Publisher (RDP) feed is a JSON feed specification that allows non-technical publishers to populate channels by hosting a structured catalog of short-form videos, movies, series, episodes, and live feeds. Roku ingests the feed on a schedule and renders the channel UI automatically.

**Human URL:** [https://github.com/rokudev/feed-specifications](https://github.com/rokudev/feed-specifications)

#### Tags:

 - Feed, Direct Publisher, Content Catalog

#### Properties

- [Documentation](https://github.com/rokudev/feed-specifications/blob/master/direct-publisher-feed-specification.md)
- [APIReference](https://github.com/rokudev/feed-specifications)
- [Example (Direct Publisher Feed Example)](examples/roku-direct-publisher-feed-example.json)

### Roku Analytics
Roku Analytics provides performance reporting, audience metrics, and engagement data for Roku channel publishers. Reports are accessed through the Roku Developer Dashboard rather than a public REST API.

**Human URL:** [https://developer.roku.com/docs/developer-program/marketing/roku-analytics.md](https://developer.roku.com/docs/developer-program/marketing/roku-analytics.md)

#### Tags:

 - Analytics, Reporting

#### Properties

- [Documentation](https://developer.roku.com/docs/developer-program/marketing/roku-analytics.md)

### Roku Authentication Framework
APIs and patterns for implementing user sign-in and authentication within Roku channels, including device-linking ("on-device authentication") and OAuth-style flows. The framework is implemented in BrightScript on the device; the publisher's authentication backend is custom-built.

**Human URL:** [https://developer.roku.com/docs/developer-program/authentication/authentication-overview.md](https://developer.roku.com/docs/developer-program/authentication/authentication-overview.md)

#### Tags:

 - Authentication, OAuth

#### Properties

- [Documentation](https://developer.roku.com/docs/developer-program/authentication/authentication-overview.md)
- [CodeExamples (On-Device Authentication Sample)](https://github.com/rokudev/on-device-authentication)

## Common Properties

- [Website](https://www.roku.com)
- [DeveloperPortal](https://developer.roku.com)
- [Documentation](https://developer.roku.com/docs)
- [GettingStarted](https://developer.roku.com/en-gb/docs/get-started/getting-started.md)
- [Courses](https://developer.roku.com/en-gb/videos/courses)
- [SDK](https://developer.roku.com/en-gb/docs/developer-program/dev-tools/dev-tools-overview.md)
- [Support](https://developer.roku.com/en-gb/support)
- [Blog](https://blog.roku.com)
- [GitHubOrganization](https://github.com/rokudev)
- [GitHubRepository (Roku Developer Documentation)](https://github.com/rokudev/dev-doc)
- [GitHubRepository (Roku Channel Samples)](https://github.com/rokudev/samples)
- [GitHubRepository (roku-deploy npm Package)](https://github.com/rokudev/roku-deploy)
- [GitHubRepository (BrightScript Debug Protocol Wrapper)](https://github.com/rokudev/roku-debug)
- [GitHubRepository (VSCode BrightScript Extension)](https://github.com/rokudev/vscode-brightscript-language)
- [Tools (BrightScript VSCode Extension)](https://github.com/rokudev/vscode-brightscript-language)
- [Tools (roku-deploy CLI (npm))](https://github.com/rokudev/roku-deploy)
- [Tools (Roku Automated Channel Testing (Selenium WebDriver))](https://github.com/rokudev/automated-channel-testing)
- [Tools (Roku Unit Testing Framework)](https://github.com/rokudev/unit-testing-framework)
- [Tools (Python BrightScript Remote Debugger)](https://github.com/rokudev/remote-debugger)
- [CodeExamples (Roku Sample Channels)](https://github.com/rokudev/samples)
- [CodeExamples (Hello World Channel)](https://github.com/rokudev/hello-world)
- [CodeExamples (SceneGraph Master Sample)](https://github.com/rokudev/scenegraph-master-sample)
- [CodeExamples (Hero Grid Channel Sample)](https://github.com/rokudev/hero-grid-channel)
- [CodeExamples (Standard Dialog Framework Sample)](https://github.com/rokudev/standard-dialog-framework)
- [SpectralRules](rules/roku-spectral-rules.yml)
- [NaftikoCapability (Roku Channel Operations Workflow)](capabilities/channel-operations.yaml)
- [NaftikoCapability (ECP Shared Capability)](capabilities/shared/external-control-protocol.yaml)
- [NaftikoCapability (Roku Pay Shared Capability)](capabilities/shared/pay-web-services.yaml)
- [NaftikoCapability (Nabu Cloud Shared Capability)](capabilities/shared/nabu-cloud.yaml)
- [Vocabulary](vocabulary/roku-vocabulary.yaml)
- [TermsOfService](https://developer.roku.com/en-gb/docs/developer-program/agreements/registered-developer-agreement.md)
- [PrivacyPolicy](https://docs.roku.com/published/userprivacypolicy/en/us)

## Features

| Name | Description |
|------|-------------|
| Channel Development | BrightScript and SceneGraph frameworks for building Roku TV streaming channel applications. |
| Device Control | Local-network HTTP API (ECP) for discovery, key injection, app launching, and diagnostics. |
| Roku Pay | Server-to-server billing APIs for transaction validation, refunds, and subscription management. |
| Direct Publisher | JSON feed ingestion path for non-technical publishers to populate Roku channels. |
| Search Feed | Catalog feed ingestion that surfaces publisher content in Roku Search. |
| Nabu Cloud | Roku's developer cloud for managing remote test devices, snapshots, and builds. |
| Channel Store Monetization | Transactional and subscription monetization through ChannelStore and roChannelStore components. |
| Advertising Framework | Roku Advertising Framework (RAF) for monetizing video content with ads. |

## Use Cases

| Name | Description |
|------|-------------|
| Streaming Channel Development | Build full-screen TV streaming channels with BrightScript/SceneGraph and ship to the Roku Channel Store. |
| Subscription Video On Demand | Monetize video content with recurring subscriptions managed by Roku Pay. |
| Transactional Video On Demand | Monetize individual movie/episode purchases via the Channel Store and Roku Pay. |
| Free Ad-Supported Streaming TV | Free streaming with the Roku Advertising Framework. |
| TV Remote and Home Automation | Build mobile or hub-based remote-control apps that drive Roku devices via ECP. |
| Automated Channel Testing | Run channel certification tests on remote Roku test devices in Nabu Cloud. |

## Integrations

| Name | Description |
|------|-------------|
| Visual Studio Code | BrightScript language extension for VSCode with debugging and side-loading. |
| Selenium WebDriver | WebDriver-based automated channel testing. |
| npm | roku-deploy and roku-debug published as npm packages. |
| Sublime Text | BrightScript syntax-highlighting package. |
| GitHub | Source-of-truth for Roku-published samples, tooling, and the dev-doc OpenAPI spec. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Roku External Control Protocol](openapi/roku-external-control-protocol.yaml)
- [Roku Nabu Cloud](openapi/roku-nabu-cloud.yaml)
- [Roku Pay Web Services](openapi/roku-pay-web-services.yaml)

### JSON Schema

- [external-control-protocol-active-app-schema](json-schema/external-control-protocol-active-app-schema.json)
- [external-control-protocol-app-list-schema](json-schema/external-control-protocol-app-list-schema.json)
- [external-control-protocol-app-schema](json-schema/external-control-protocol-app-schema.json)
- [external-control-protocol-device-info-schema](json-schema/external-control-protocol-device-info-schema.json)
- [external-control-protocol-media-player-schema](json-schema/external-control-protocol-media-player-schema.json)
- [nabu-cloud-agent-stream-option-schema](json-schema/nabu-cloud-agent-stream-option-schema.json)
- [nabu-cloud-awsregion-schema](json-schema/nabu-cloud-awsregion-schema.json)
- [nabu-cloud-body-serviceaccounts-login-token-schema](json-schema/nabu-cloud-body-serviceaccounts-login-token-schema.json)
- [nabu-cloud-build-out-schema](json-schema/nabu-cloud-build-out-schema.json)
- [nabu-cloud-build-source-schema](json-schema/nabu-cloud-build-source-schema.json)
- [nabu-cloud-device-create-schema](json-schema/nabu-cloud-device-create-schema.json)
- [nabu-cloud-device-history-out-schema](json-schema/nabu-cloud-device-history-out-schema.json)
- [nabu-cloud-device-instance-info-schema](json-schema/nabu-cloud-device-instance-info-schema.json)
- [nabu-cloud-device-out-schema](json-schema/nabu-cloud-device-out-schema.json)
- [nabu-cloud-device-start-schema](json-schema/nabu-cloud-device-start-schema.json)
- [nabu-cloud-device-status-schema](json-schema/nabu-cloud-device-status-schema.json)
- [nabu-cloud-device-type-schema](json-schema/nabu-cloud-device-type-schema.json)
- [nabu-cloud-device-update-schema](json-schema/nabu-cloud-device-update-schema.json)
- [nabu-cloud-group-add-member-schema](json-schema/nabu-cloud-group-add-member-schema.json)
- [nabu-cloud-group-create-schema](json-schema/nabu-cloud-group-create-schema.json)
- [nabu-cloud-group-member-out-schema](json-schema/nabu-cloud-group-member-out-schema.json)
- [nabu-cloud-group-out-schema](json-schema/nabu-cloud-group-out-schema.json)
- [nabu-cloud-group-role-out-schema](json-schema/nabu-cloud-group-role-out-schema.json)
- [nabu-cloud-group-update-schema](json-schema/nabu-cloud-group-update-schema.json)
- [nabu-cloud-ice-server-schema](json-schema/nabu-cloud-ice-server-schema.json)
- [nabu-cloud-kubernetes-status-schema](json-schema/nabu-cloud-kubernetes-status-schema.json)
- [nabu-cloud-oidctoken-response-model-schema](json-schema/nabu-cloud-oidctoken-response-model-schema.json)
- [nabu-cloud-organisation-member-out-schema](json-schema/nabu-cloud-organisation-member-out-schema.json)
- [nabu-cloud-organisation-out-schema](json-schema/nabu-cloud-organisation-out-schema.json)
- [nabu-cloud-organisation-region-out-schema](json-schema/nabu-cloud-organisation-region-out-schema.json)
- [nabu-cloud-organisation-role-out-schema](json-schema/nabu-cloud-organisation-role-out-schema.json)
- [nabu-cloud-personal-access-token-create-schema](json-schema/nabu-cloud-personal-access-token-create-schema.json)
- [nabu-cloud-personal-access-token-created-schema](json-schema/nabu-cloud-personal-access-token-created-schema.json)
- [nabu-cloud-personal-access-token-out-schema](json-schema/nabu-cloud-personal-access-token-out-schema.json)
- [nabu-cloud-personal-access-token-refresh-schema](json-schema/nabu-cloud-personal-access-token-refresh-schema.json)
- [nabu-cloud-personal-access-token-status-schema](json-schema/nabu-cloud-personal-access-token-status-schema.json)
- [nabu-cloud-project-create-schema](json-schema/nabu-cloud-project-create-schema.json)
- [nabu-cloud-project-group-add-schema](json-schema/nabu-cloud-project-group-add-schema.json)
- [nabu-cloud-project-group-out-schema](json-schema/nabu-cloud-project-group-out-schema.json)
- [nabu-cloud-project-group-update-schema](json-schema/nabu-cloud-project-group-update-schema.json)
- [nabu-cloud-project-member-add-schema](json-schema/nabu-cloud-project-member-add-schema.json)
- [nabu-cloud-project-member-out-schema](json-schema/nabu-cloud-project-member-out-schema.json)
- [nabu-cloud-project-out-schema](json-schema/nabu-cloud-project-out-schema.json)
- [nabu-cloud-project-role-out-schema](json-schema/nabu-cloud-project-role-out-schema.json)
- [nabu-cloud-project-update-schema](json-schema/nabu-cloud-project-update-schema.json)
- [nabu-cloud-scope-out-schema](json-schema/nabu-cloud-scope-out-schema.json)
- [nabu-cloud-snapshot-create-schema](json-schema/nabu-cloud-snapshot-create-schema.json)
- [nabu-cloud-snapshot-out-schema](json-schema/nabu-cloud-snapshot-out-schema.json)
- [nabu-cloud-snapshot-update-schema](json-schema/nabu-cloud-snapshot-update-schema.json)
- [nabu-cloud-user-out-schema](json-schema/nabu-cloud-user-out-schema.json)
- [pay-web-services-cancel-subscription-request-schema](json-schema/pay-web-services-cancel-subscription-request-schema.json)
- [pay-web-services-issue-credit-request-schema](json-schema/pay-web-services-issue-credit-request-schema.json)
- [pay-web-services-refund-subscription-request-schema](json-schema/pay-web-services-refund-subscription-request-schema.json)
- [pay-web-services-refund-validation-schema](json-schema/pay-web-services-refund-validation-schema.json)
- [pay-web-services-subscription-result-schema](json-schema/pay-web-services-subscription-result-schema.json)
- [pay-web-services-transaction-validation-schema](json-schema/pay-web-services-transaction-validation-schema.json)
- [pay-web-services-update-bill-cycle-request-schema](json-schema/pay-web-services-update-bill-cycle-request-schema.json)
- [search-feed-schema](json-schema/search-feed-schema.json)

### JSON Structure

- [external-control-protocol-active-app-structure](json-structure/external-control-protocol-active-app-structure.json)
- [external-control-protocol-app-list-structure](json-structure/external-control-protocol-app-list-structure.json)
- [external-control-protocol-app-structure](json-structure/external-control-protocol-app-structure.json)
- [external-control-protocol-device-info-structure](json-structure/external-control-protocol-device-info-structure.json)
- [external-control-protocol-media-player-structure](json-structure/external-control-protocol-media-player-structure.json)
- [nabu-cloud-agent-stream-option-structure](json-structure/nabu-cloud-agent-stream-option-structure.json)
- [nabu-cloud-awsregion-structure](json-structure/nabu-cloud-awsregion-structure.json)
- [nabu-cloud-body-serviceaccounts-login-token-structure](json-structure/nabu-cloud-body-serviceaccounts-login-token-structure.json)
- [nabu-cloud-build-out-structure](json-structure/nabu-cloud-build-out-structure.json)
- [nabu-cloud-build-source-structure](json-structure/nabu-cloud-build-source-structure.json)
- [nabu-cloud-device-create-structure](json-structure/nabu-cloud-device-create-structure.json)
- [nabu-cloud-device-history-out-structure](json-structure/nabu-cloud-device-history-out-structure.json)
- [nabu-cloud-device-instance-info-structure](json-structure/nabu-cloud-device-instance-info-structure.json)
- [nabu-cloud-device-out-structure](json-structure/nabu-cloud-device-out-structure.json)
- [nabu-cloud-device-start-structure](json-structure/nabu-cloud-device-start-structure.json)
- [nabu-cloud-device-status-structure](json-structure/nabu-cloud-device-status-structure.json)
- [nabu-cloud-device-type-structure](json-structure/nabu-cloud-device-type-structure.json)
- [nabu-cloud-device-update-structure](json-structure/nabu-cloud-device-update-structure.json)
- [nabu-cloud-group-add-member-structure](json-structure/nabu-cloud-group-add-member-structure.json)
- [nabu-cloud-group-create-structure](json-structure/nabu-cloud-group-create-structure.json)
- [nabu-cloud-group-member-out-structure](json-structure/nabu-cloud-group-member-out-structure.json)
- [nabu-cloud-group-out-structure](json-structure/nabu-cloud-group-out-structure.json)
- [nabu-cloud-group-role-out-structure](json-structure/nabu-cloud-group-role-out-structure.json)
- [nabu-cloud-group-update-structure](json-structure/nabu-cloud-group-update-structure.json)
- [nabu-cloud-ice-server-structure](json-structure/nabu-cloud-ice-server-structure.json)
- [nabu-cloud-kubernetes-status-structure](json-structure/nabu-cloud-kubernetes-status-structure.json)
- [nabu-cloud-oidctoken-response-model-structure](json-structure/nabu-cloud-oidctoken-response-model-structure.json)
- [nabu-cloud-organisation-member-out-structure](json-structure/nabu-cloud-organisation-member-out-structure.json)
- [nabu-cloud-organisation-out-structure](json-structure/nabu-cloud-organisation-out-structure.json)
- [nabu-cloud-organisation-region-out-structure](json-structure/nabu-cloud-organisation-region-out-structure.json)
- [nabu-cloud-organisation-role-out-structure](json-structure/nabu-cloud-organisation-role-out-structure.json)
- [nabu-cloud-personal-access-token-create-structure](json-structure/nabu-cloud-personal-access-token-create-structure.json)
- [nabu-cloud-personal-access-token-created-structure](json-structure/nabu-cloud-personal-access-token-created-structure.json)
- [nabu-cloud-personal-access-token-out-structure](json-structure/nabu-cloud-personal-access-token-out-structure.json)
- [nabu-cloud-personal-access-token-refresh-structure](json-structure/nabu-cloud-personal-access-token-refresh-structure.json)
- [nabu-cloud-personal-access-token-status-structure](json-structure/nabu-cloud-personal-access-token-status-structure.json)
- [nabu-cloud-project-create-structure](json-structure/nabu-cloud-project-create-structure.json)
- [nabu-cloud-project-group-add-structure](json-structure/nabu-cloud-project-group-add-structure.json)
- [nabu-cloud-project-group-out-structure](json-structure/nabu-cloud-project-group-out-structure.json)
- [nabu-cloud-project-group-update-structure](json-structure/nabu-cloud-project-group-update-structure.json)
- [nabu-cloud-project-member-add-structure](json-structure/nabu-cloud-project-member-add-structure.json)
- [nabu-cloud-project-member-out-structure](json-structure/nabu-cloud-project-member-out-structure.json)
- [nabu-cloud-project-out-structure](json-structure/nabu-cloud-project-out-structure.json)
- [nabu-cloud-project-role-out-structure](json-structure/nabu-cloud-project-role-out-structure.json)
- [nabu-cloud-project-update-structure](json-structure/nabu-cloud-project-update-structure.json)
- [nabu-cloud-scope-out-structure](json-structure/nabu-cloud-scope-out-structure.json)
- [nabu-cloud-snapshot-create-structure](json-structure/nabu-cloud-snapshot-create-structure.json)
- [nabu-cloud-snapshot-out-structure](json-structure/nabu-cloud-snapshot-out-structure.json)
- [nabu-cloud-snapshot-update-structure](json-structure/nabu-cloud-snapshot-update-structure.json)
- [nabu-cloud-user-out-structure](json-structure/nabu-cloud-user-out-structure.json)
- [pay-web-services-cancel-subscription-request-structure](json-structure/pay-web-services-cancel-subscription-request-structure.json)
- [pay-web-services-issue-credit-request-structure](json-structure/pay-web-services-issue-credit-request-structure.json)
- [pay-web-services-refund-subscription-request-structure](json-structure/pay-web-services-refund-subscription-request-structure.json)
- [pay-web-services-refund-validation-structure](json-structure/pay-web-services-refund-validation-structure.json)
- [pay-web-services-subscription-result-structure](json-structure/pay-web-services-subscription-result-structure.json)
- [pay-web-services-transaction-validation-structure](json-structure/pay-web-services-transaction-validation-structure.json)
- [pay-web-services-update-bill-cycle-request-structure](json-structure/pay-web-services-update-bill-cycle-request-structure.json)
- [roku-search-feed-structure](json-structure/roku-search-feed-structure.json)

### JSON-LD

- [roku-external-control-protocol-context](json-ld/roku-external-control-protocol-context.jsonld)
- [roku-nabu-cloud-context](json-ld/roku-nabu-cloud-context.jsonld)
- [roku-pay-web-services-context](json-ld/roku-pay-web-services-context.jsonld)
- [roku-search-feed-context](json-ld/roku-search-feed-context.jsonld)

### Examples

- [external-control-protocol-launch-app-example](examples/external-control-protocol-launch-app-example.json)
- [external-control-protocol-query-apps-example](examples/external-control-protocol-query-apps-example.json)
- [external-control-protocol-query-device-info-example](examples/external-control-protocol-query-device-info-example.json)
- [nabu-cloud-create-device-example](examples/nabu-cloud-create-device-example.json)
- [nabu-cloud-list-devices-example](examples/nabu-cloud-list-devices-example.json)
- [pay-web-services-cancel-subscription-example](examples/pay-web-services-cancel-subscription-example.json)
- [pay-web-services-validate-transaction-example](examples/pay-web-services-validate-transaction-example.json)
- [roku-direct-publisher-feed-example](examples/roku-direct-publisher-feed-example.json)
- [roku-search-feed-advanced-example](examples/roku-search-feed-advanced-example.json)
- [roku-search-feed-simple-example](examples/roku-search-feed-simple-example.json)

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [Roku External Control Protocol](capabilities/shared/external-control-protocol.yaml) — 15 operations
- [Roku Nabu Cloud](capabilities/shared/nabu-cloud.yaml) — 24 operations
- [Roku Pay Web Services](capabilities/shared/pay-web-services.yaml) — 6 operations

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|---------------|-------|---------|
| [Roku Channel Operations](capabilities/channel-operations.yaml) | ECP, Pay, Nabu Cloud | 21 | Channel Developer, QA Engineer, Billing Operator |

## Vocabulary

- [Roku Vocabulary](vocabulary/roku-vocabulary.yaml) — Unified taxonomy mapping 17 resources, 15 actions, 1 workflow, and 3 personas across operational (OpenAPI) and capability (Naftiko) dimensions

## Rules

- [Roku Spectral Rules](rules/roku-spectral-rules.yml) — 27 rules across 12 categories enforcing Roku API conventions

## Maintainers

**FN:** API Evangelist

**URL:** https://apievangelist.com