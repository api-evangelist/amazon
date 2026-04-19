# Amazon (amazon)

Amazon is a global technology and e-commerce company offering a wide range of consumer and developer APIs including the Selling Partner API for marketplace sellers, Advertising API for campaign management, Amazon Pay for payments, Alexa Skills Kit for voice experiences, Amazon Appstore for mobile applications, and the Creators API for affiliate publishers. These APIs power Amazon's ecosystem of sellers, developers, advertisers, and content creators.

**URL:** [https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/apis.yml)

## Tags

- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice

## Timestamps

- **Created:** 2024-01-15
- **Modified:** 2026-04-19

## APIs

### Amazon Selling Partner API

The Amazon Selling Partner API (SP-API) is a RESTful API that enables Amazon sellers and vendors to programmatically manage their marketplace operations including listings, orders, payments, reports, and fulfillment. It replaces the deprecated Amazon Marketplace Web Service (MWS) and provides access to region-specific endpoints for North America, Europe, and Far East marketplaces.

**Human URL:** [https://developer-docs.amazon.com/sp-api](https://developer-docs.amazon.com/sp-api)

**Base URL:** https://sellingpartnerapi-na.amazon.com

#### Tags

- E-Commerce
- Fulfillment
- Marketplace
- Orders
- Sellers

#### Properties

- [Documentation](https://developer-docs.amazon.com/sp-api)
- [OpenAPI](openapi/amazon-selling-partner-api-openapi.yml)
- [JSONSchema](json-schema/selling-partner-order-schema.json)

### Amazon Advertising API

The Amazon Advertising API enables programmatic management of advertising campaigns on Amazon including Sponsored Products, Sponsored Brands, and Sponsored Display campaigns across various marketplaces. Developers can create, manage, and optimize campaigns, access reporting data, and manage budgets and targeting.

**Human URL:** [https://advertising.amazon.com/API/docs/en-us/reference/api-overview](https://advertising.amazon.com/API/docs/en-us/reference/api-overview)

**Base URL:** https://advertising-api.amazon.com

#### Tags

- Advertising
- Campaigns
- Marketing
- Sponsored Products

#### Properties

- [Documentation](https://advertising.amazon.com/API/docs/en-us/reference/api-overview)
- [OpenAPI](openapi/amazon-advertising-api-openapi.yml)

### Amazon Creators API

The Amazon Creators API provides programmatic access to Amazon product data for publishers, influencers, and affiliate partners. It is the recommended replacement for the Product Advertising API and requires Amazon Associates membership with qualifying sales history.

**Human URL:** [https://affiliate-program.amazon.com/creatorsapi/docs/en-us/introduction](https://affiliate-program.amazon.com/creatorsapi/docs/en-us/introduction)

**Base URL:** https://affiliate-program.amazon.com/creatorsapi

#### Tags

- Affiliates
- Content Creators
- E-Commerce
- Products

#### Properties

- [Documentation](https://affiliate-program.amazon.com/creatorsapi/docs/en-us/introduction)

### Amazon Pay API

The Amazon Pay API enables merchants to integrate Amazon Pay for payment processing on their websites and mobile applications. It supports one-time purchases, subscriptions, and recurring payments with checkout session management, charge operations, and refund capabilities.

**Human URL:** [https://developer.amazon.com/docs/amazon-pay-api-v2/introduction.html](https://developer.amazon.com/docs/amazon-pay-api-v2/introduction.html)

**Base URL:** https://pay-api.amazon.com

#### Tags

- Checkout
- E-Commerce
- Payments
- Subscriptions

#### Properties

- [Documentation](https://developer.amazon.com/docs/amazon-pay-api-v2/introduction.html)
- [OpenAPI](openapi/amazon-pay-api-openapi.yml)

### Amazon Alexa Skills Kit API

The Alexa Skills Kit (ASK) REST APIs enable developers to create, manage, test, and deploy custom voice skills for Alexa-enabled devices including skill manifest management, interaction model building, and hosted skill management for voice experiences and smart home integrations.

**Human URL:** [https://developer.amazon.com/en-US/docs/alexa/rest-apis/rest-apis.html](https://developer.amazon.com/en-US/docs/alexa/rest-apis/rest-apis.html)

**Base URL:** https://api.amazonalexa.com

#### Tags

- Alexa
- Skills
- Smart Home
- Voice

#### Properties

- [Documentation](https://developer.amazon.com/en-US/docs/alexa/rest-apis/rest-apis.html)

### Amazon Appstore API

The Amazon Appstore Developer APIs provide tools for managing app submissions, testing, and monetization through in-app purchases on the Amazon Appstore for Android and Fire OS applications.

**Human URL:** [https://www.developer.amazon.com/docs/apps-and-games/documentation.html](https://www.developer.amazon.com/docs/apps-and-games/documentation.html)

**Base URL:** https://developer.amazon.com/api/appstore

#### Tags

- App Store
- Apps
- In-App Purchases
- Mobile

#### Properties

- [Documentation](https://www.developer.amazon.com/docs/apps-and-games/documentation.html)

## Common Properties

- [Portal](https://developer.amazon.com/)
- [Website](https://www.amazon.com/)
- [Documentation](https://developer.amazon.com/docs/)
- [TermsOfService](https://developer.amazon.com/support/legal/da)
- [PrivacyPolicy](https://www.amazon.com/gp/help/customer/display.html?nodeId=468496)
- [Support](https://developer.amazon.com/support)
- [GitHubOrganization](https://github.com/amzn)
- [Console](https://developer.amazon.com/dashboard)
- [SignUp](https://www.amazon.com/ap/register?openid.assoc_handle=aws)
- [Login](https://developer.amazon.com/login)
- [Blog](https://developer.amazon.com/blogs/)
- [YouTube](https://www.youtube.com/c/AmazonDeveloper)
- [Contact](https://www.amazon.com/gp/help/customer/contact-us)
- [JSON-LD](json-ld/amazon-context.jsonld)
- [SpectralRules](rules/amazon-spectral-rules.yml)
- [Vocabulary](vocabulary/amazon-vocabulary.yaml)
- [NaftikoCapability](capabilities/amazon-seller-and-commerce.yaml)

## Features

- **Marketplace Seller Operations** — Full lifecycle management of Amazon marketplace seller operations including catalog, inventory, orders, shipping, and financial reporting.
- **Programmatic Advertising** — Create and optimize Sponsored Products, Sponsored Brands, and Sponsored Display advertising campaigns with granular targeting and reporting.
- **Amazon Pay Integration** — Enable Amazon Pay on external websites and mobile apps with checkout session management, one-time charges, subscriptions, and refunds.
- **Voice Experience Development** — Build Alexa voice skills for Echo devices, Fire TV, and third-party Alexa-enabled hardware with the Alexa Skills Kit.
- **Affiliate and Creator Commerce** — Access Amazon product data for affiliate marketing and content creation through the Creators API with product search and deep linking.
- **Mobile App Monetization** — Publish and monetize apps on the Amazon Appstore with in-app purchasing for digital goods, subscriptions, and consumables.
- **Multi-Region Marketplace Support** — Access North America, Europe, and Far East marketplaces through region-specific SP-API endpoints.
- **Developer Console and Testing Tools** — Sandbox environments, developer consoles, and testing tools for building and validating Amazon integrations before going live.

## Use Cases

- **Marketplace Seller Automation** — Automate product listing creation, price updates, inventory management, and order fulfillment for Amazon marketplace sellers.
- **Advertising Campaign Optimization** — Build automated bid management and campaign optimization tools using the Amazon Advertising API and performance reporting.
- **E-Commerce Payment Integration** — Add Amazon Pay as a payment option for external e-commerce sites to reduce checkout friction and increase conversion rates.
- **Voice Commerce and Smart Home** — Create Alexa skills for voice-driven shopping, home automation, and customer service interactions.
- **Affiliate Content Monetization** — Build product recommendation engines and affiliate content sites using the Creators API for real-time Amazon product data.

## Integrations

- **Amazon MWS Legacy Migration** — SP-API is the modern replacement for the deprecated Amazon Marketplace Web Service (MWS) for all seller operations.
- **Alexa Smart Home** — Integrate smart home devices and services with Alexa voice control using the Smart Home Skill API.
- **Login with Amazon** — OAuth 2.0 authentication for all Amazon developer APIs including SP-API, Advertising API, and ASK via Login with Amazon (LWA).
- **Amazon Associates Program** — Affiliate program integration for the Creators API and Product Advertising API for commission-based product promotion.
- **Fire OS and Android** — Amazon Appstore SDK for Fire OS and Android apps with in-app purchasing and device targeting capabilities.

## Artifacts

### OpenAPI Specifications

- [Amazon Selling Partner API OpenAPI](openapi/amazon-selling-partner-api-openapi.yml)
- [Amazon Advertising API OpenAPI](openapi/amazon-advertising-api-openapi.yml)
- [Amazon Pay API OpenAPI](openapi/amazon-pay-api-openapi.yml)

### JSON Schema

- [Selling Partner Order Schema](json-schema/selling-partner-order-schema.json)
- [Advertising Campaign Schema](json-schema/advertising-campaign-schema.json)
- [Pay Checkout Session Schema](json-schema/pay-checkout-session-schema.json)

### JSON Structure

- [Selling Partner Order Structure](json-structure/selling-partner-order-structure.json)
- [Advertising Campaign Structure](json-structure/advertising-campaign-structure.json)
- [Pay Checkout Session Structure](json-structure/pay-checkout-session-structure.json)

### JSON-LD Contexts

- [Amazon Context](json-ld/amazon-context.jsonld)

### Examples

- [Selling Partner Order Example](examples/selling-partner-order-example.json)
- [Advertising Campaign Example](examples/advertising-campaign-example.json)
- [Pay Checkout Session Example](examples/pay-checkout-session-example.json)

## Capabilities

### Shared Per-API Definitions

- [Selling Partner API Capabilities](capabilities/shared/selling-partner-api.yaml)
- [Advertising API Capabilities](capabilities/shared/advertising-api.yaml)
- [Pay API Capabilities](capabilities/shared/pay-api.yaml)

### Workflow Capabilities

- [Amazon Seller and Commerce](capabilities/amazon-seller-and-commerce.yaml)

## Vocabulary

- [Amazon Vocabulary](vocabulary/amazon-vocabulary.yaml)

## Rules

- [Amazon Spectral Rules](rules/amazon-spectral-rules.yml)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
