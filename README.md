# Amazon (amazon)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Amazon is a global technology and e-commerce company offering a wide range of consumer and developer APIs including the Selling Partner API for marketplace sellers, Advertising API for campaign management, Amazon Pay for payments, Alexa Skills Kit for voice experiences, Amazon Appstore for mobile applications, and the Creators API for affiliate publishers. These APIs power Amazon's ecosystem of sellers, developers, advertisers, and content creators.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

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
- **Modified:** 2026-05-19

## APIs

### Amazon Selling Partner API

The Amazon Selling Partner API (SP-API) is a RESTful API that enables Amazon sellers and vendors to programmatically manage their marketplace operations including listings, orders, payments, reports, and fulfillment. It replaces the deprecated Amazon Marketplace Web Service (MWS) and provides access to region-specific endpoints for North America, Europe, and Far East marketplaces.

- **Human URL:** [https://developer-docs.amazon.com/sp-api](https://developer-docs.amazon.com/sp-api)
- **Base URL:** `https://sellingpartnerapi-na.amazon.com`

#### Tags

- E-Commerce
- Fulfillment
- Marketplace
- Orders
- Sellers

#### Properties

- [Documentation](https://developer-docs.amazon.com/sp-api)
- [OpenAPI](openapi/amazon-selling-partner-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/amazon-selling-partner-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/amazon-selling-partner-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/selling-partner-order-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Amazon Advertising API

The Amazon Advertising API enables programmatic management of advertising campaigns on Amazon including Sponsored Products, Sponsored Brands, and Sponsored Display campaigns across various marketplaces. Developers can create, manage, and optimize campaigns, access reporting data, and manage budgets and targeting.

- **Human URL:** [https://advertising.amazon.com/API/docs/en-us/reference/api-overview](https://advertising.amazon.com/API/docs/en-us/reference/api-overview)
- **Base URL:** `https://advertising-api.amazon.com`

#### Tags

- Advertising
- Campaigns
- Marketing
- Sponsored Products

#### Properties

- [Documentation](https://advertising.amazon.com/API/docs/en-us/reference/api-overview)
- [OpenAPI](openapi/amazon-advertising-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/amazon-advertising-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/amazon-advertising-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Amazon Creators API

The Amazon Creators API provides programmatic access to Amazon product data for publishers, influencers, and affiliate partners. It is the recommended replacement for the Product Advertising API and requires Amazon Associates membership with qualifying sales history.

- **Human URL:** [https://affiliate-program.amazon.com/creatorsapi/docs/en-us/introduction](https://affiliate-program.amazon.com/creatorsapi/docs/en-us/introduction)
- **Base URL:** `https://affiliate-program.amazon.com/creatorsapi`

#### Tags

- Affiliates
- Content Creators
- E-Commerce
- Products

#### Properties

- [Documentation](https://affiliate-program.amazon.com/creatorsapi/docs/en-us/introduction)
- [Postman Collection](collections/amazon-advertising-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/amazon-advertising-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/amazon-pay-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/amazon-pay-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/amazon-selling-partner-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/amazon-selling-partner-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Amazon Pay API

The Amazon Pay API enables merchants to integrate Amazon Pay for payment processing on their websites and mobile applications. It supports one-time purchases, subscriptions, and recurring payments with checkout session management, charge operations, and refund capabilities.

- **Human URL:** [https://developer.amazon.com/docs/amazon-pay-api-v2/introduction.html](https://developer.amazon.com/docs/amazon-pay-api-v2/introduction.html)
- **Base URL:** `https://pay-api.amazon.com`

#### Tags

- Checkout
- E-Commerce
- Payments
- Subscriptions

#### Properties

- [Documentation](https://developer.amazon.com/docs/amazon-pay-api-v2/introduction.html)
- [OpenAPI](openapi/amazon-pay-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/amazon-pay-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/amazon-pay-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Amazon Alexa Skills Kit API

The Alexa Skills Kit (ASK) REST APIs enable developers to create, manage, test, and deploy custom voice skills for Alexa-enabled devices including skill manifest management, interaction model building, and hosted skill management for voice experiences and smart home integrations.

- **Human URL:** [https://developer.amazon.com/en-US/docs/alexa/rest-apis/rest-apis.html](https://developer.amazon.com/en-US/docs/alexa/rest-apis/rest-apis.html)
- **Base URL:** `https://api.amazonalexa.com`

#### Tags

- Alexa
- Skills
- Smart Home
- Voice

#### Properties

- [Documentation](https://developer.amazon.com/en-US/docs/alexa/rest-apis/rest-apis.html)
- [Postman Collection](collections/amazon-advertising-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/amazon-advertising-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/amazon-pay-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/amazon-pay-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/amazon-selling-partner-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/amazon-selling-partner-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Amazon Appstore API

The Amazon Appstore Developer APIs provide tools for managing app submissions, testing, and monetization through in-app purchases on the Amazon Appstore for Android and Fire OS applications.

- **Human URL:** [https://www.developer.amazon.com/docs/apps-and-games/documentation.html](https://www.developer.amazon.com/docs/apps-and-games/documentation.html)
- **Base URL:** `https://developer.amazon.com/api/appstore`

#### Tags

- App Store
- Apps
- In-App Purchases
- Mobile

#### Properties

- [Documentation](https://www.developer.amazon.com/docs/apps-and-games/documentation.html)
- [Postman Collection](collections/amazon-advertising-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/amazon-advertising-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/amazon-pay-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/amazon-pay-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/amazon-selling-partner-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/amazon-selling-partner-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/amazon)
- [Portal](https://developer.amazon.com/)
- [Website](https://www.amazon.com/)
- [Documentation](https://developer.amazon.com/docs/)
- [Terms of Service](https://developer.amazon.com/support/legal/da)
- [Privacy Policy](https://www.amazon.com/gp/help/customer/display.html?nodeId=468496)
- [Support](https://developer.amazon.com/support)
- [GitHub Organization](https://github.com/amzn)
- [Console](https://developer.amazon.com/dashboard)
- [Sign Up](https://www.amazon.com/ap/register?openid.assoc_handle=aws)
- [Login](https://developer.amazon.com/login)
- [Blog](https://developer.amazon.com/blogs/)
- [YouTube](https://www.youtube.com/c/AmazonDeveloper)
- [Contact](https://www.amazon.com/gp/help/customer/contact-us)
- [JSON-LD](json-ld/amazon-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Spectral Rules](rules/amazon-spectral-rules.yml)
- [Vocabulary](vocabulary/amazon-vocabulary.yaml)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [L L Ms Txt](https://developer.amazon.com/llms.txt)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
