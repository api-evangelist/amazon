# Amazon Selling Partner API - GraphQL Schema

## Overview

This conceptual GraphQL schema models the Amazon Selling Partner API (SP-API) surface.
The SP-API is Amazon's modern RESTful API platform that replaced the deprecated Amazon
Marketplace Web Service (MWS). It enables sellers and vendors to programmatically manage
marketplace operations across North America, Europe, and Far East regions.

**Schema file:** `amazon-schema.graphql`
**Source:** https://developer-docs.amazon.com/sp-api/
**GitHub:** https://github.com/amzn

## Type Coverage

The schema covers 80+ named types organized into functional domains:

### Account and Marketplace
- `SellerAccount` — top-level seller identity with marketplace participations
- `Marketplace` — individual Amazon marketplace (e.g., amazon.com, amazon.co.uk)
- `MarketplaceParticipation` — seller's participation status in a marketplace
- `Participation` — active/suspended listing state
- `Seller` — seller profile with feedback rating
- `SellerFeedback` — individual feedback records from buyers

### Orders
- `Order` — core order record with status, totals, dates, and addresses
- `OrderItem` — individual line item within an order (ASIN, SKU, quantities, prices)
- `OrderShipment` — shipment record associated with an order
- `ShipmentItem` — individual item within a shipment
- `OrderFee` — fees applied to an order
- `BuyerInfo` — buyer email, name, and tax information
- `BuyerTaxInfo` — company and tax classification for B2B orders
- `TaxClassification` — buyer tax classification key-value pair
- `TaxCollection` — tax collection model and responsible party
- `ProductInfo` — package quantity metadata on order items
- `PointsGranted` — Amazon Points granted with an order item

### Fulfillment (FBA and MFN)
- `Fulfillment` — fulfillment order record with status and shipping details
- `FulfillmentItem` — item within a fulfillment order
- `FulfillmentShipment` — outbound shipment from a fulfillment center
- `FulfillmentShipmentItem` — item within a fulfillment shipment
- `FulfillmentShipmentPackage` — package within a fulfillment shipment
- `FeatureSettings` — FBA feature constraints (e.g., SNSWUS)
- `FBAShipment` — inbound shipment to an FBA fulfillment center
- `FBAShipmentItem` — individual item in an FBA inbound shipment
- `PrepDetails` — prep instruction and ownership for an FBA item
- `EstimatedBoxContentsFee` — estimated fee for box contents labeling
- `MultiChannelFulfillment` — MCF order for non-Amazon sales channels

### Inventory
- `Inventory` — MFN inventory by SKU with supply breakdown
- `InventorySupplyDetail` — supply type and availability window
- `FBAInventory` — FBA inventory record with condition and FNSKU
- `InventoryDetails` — fulfillable, reserved, researching, unfulfillable breakdown
- `ReservedQuantity` — detail on reserved inventory (customer orders, processing)
- `ResearchingQuantity` — inventory under investigation
- `ResearchingQuantityEntry` — named research quantity bucket
- `UnfulfillableQuantity` — reason-code breakdown of unsellable units
- `Replenishment` — restocking recommendation with suggested quantity and date

### Catalog
- `Catalog` — marketplace-scoped collection of catalog items
- `CatalogItem` — full catalog record with attributes, images, identifiers, and sales ranks
- `ItemSummary` — marketplace-specific summary (brand, name, classification)
- `BrowseClassification` — browse tree classification with display name
- `ItemAttributes` — product attributes (title, brand, description, dimensions, weight)
- `ItemIdentifier` — product identifier (ASIN, EAN, UPC, ISBN, etc.)
- `ItemImage` — product image with variant tag and dimensions
- `CatalogProductType` — product type definition associated with a catalog item
- `SalesRank` — sales rank within a category
- `VariationData` — ASIN variation relationships
- `VendorDetails` — vendor-specific catalog metadata

### Listings
- `ListingItem` — seller's listed item with attributes, status, and offers
- `ListingStatus` — listing lifecycle status
- `ListingIssue` — validation issue (code, message, severity)
- `FulfillmentAvailability` — per-channel fulfillment quantity
- `ProcurementData` — cost price for vendor-managed listings
- `ListingSubmissionResponse` — result of a listing create/update/delete operation

### Pricing and Offers
- `ItemPricing` — pricing data for an ASIN including competitive offers
- `ItemIdentifiers` — marketplace ASIN and SKU identifier pair
- `MarketplaceASIN` — ASIN scoped to a marketplace
- `SKUIdentifier` — seller SKU scoped to a marketplace
- `PricingProduct` — offers, lowest listings, and buy box prices for a product
- `Offer` — a seller's active offer (price, condition, fulfillment channel)
- `OfferDetail` — competitive offer detail with shipping and prime information
- `PriceType` — landed price, listing price, shipping, and points
- `LowestOfferListing` — lowest offer by condition and quantity tier
- `BuyBoxPrice` — current Buy Box price by condition
- `QuantityDiscount` — quantity tier price break
- `SellerFeedbackRating` — feedback rating summary for an offer's seller
- `ShippingTime` — estimated shipping time range and availability
- `PrimeInformation` — Prime and National Prime eligibility flags

### Product Advertising
- `ProductAdvertising` — product data for affiliate/advertising use cases
- `ProductAdvertisingOffer` — offer detail for advertising context
- `DeliveryInfo` — Prime and free shipping eligibility
- `ShippingCharge` — shipping cost with rate details
- `LoyaltyPoints` — loyalty points on offer
- `MerchantInfo` — merchant profile (name, rating, feedback count)
- `OfferPrice` — display price with savings breakdown
- `Savings` — price savings amount and percentage
- `ProgramEligibility` — Buy Box winner, Prime exclusive, Prime Pantry flags
- `VariationAttribute` — variation dimension (e.g., Color: Red)
- `CustomerReviews` — review count and star rating
- `StarRating` — numeric and display star rating value

### Identifiers
- `ASIN` — Amazon Standard Identification Number
- `EAN` — European Article Number
- `UPC` — Universal Product Code
- `GTIN` — Global Trade Item Number (typed wrapper)

### Brand, Category, Browse
- `Brand` — brand identity with marketplace scoping
- `Category` — product category tree node with parent/children
- `CatalogCategory` — catalog-level category with sales ranks
- `Browse` — browse tree root for a marketplace
- `BrowseNode` — individual browse tree node with ancestor/children

### Product (generic)
- `Product` — unified product view combining catalog, pricing, inventory, and offers

### Reports
- `Report` — asynchronous report record with type, status, and document reference
- `ReportSchedule` — recurring report schedule with period and next run time
- `ReportDocument` — signed download URL for a completed report
- `ReportList` — paginated list of reports

### Feeds
- `Feed` — asynchronous feed submission record
- `FeedDocument` — signed upload/download URL for feed data
- `FeedList` — paginated list of feeds

### Notifications
- `Notification` — event notification payload by type
- `Subscription` — notification subscription linking type to destination
- `ProcessingDirective` — event filter configuration on a subscription
- `EventFilter` — event type and marketplace scope filter
- `Destination` — notification delivery endpoint (SQS or EventBridge)
- `DestinationResource` — union of SQS and EventBridge resources
- `SQSResource` — SQS queue ARN
- `EventBridgeResource` — EventBridge bus name, region, and account

### Finance
- `Finance` — financial event group (settlement period)
- `FinancialEvent` — transaction-level financial event (order, refund, adjustment)
- `ChargeComponent` — charge type and amount
- `FeeComponent` — fee type and amount
- `DirectPayment` — direct payment type and amount
- `ServiceFee` — service fee record (referral, FBA, etc.)
- `FinancialEvents` — container for all financial event lists in a group
- `FinancialEventList` — paginated financial events with next token
- `FinanceList` — paginated list of financial event groups

### Deals, Coupons, Promotions
- `Coupon` — digital coupon with discount value and eligible ASINs
- `Deal` — limited-time deal with price and eligibility
- `Promotion` — promotion record with discount type and amount

### Vendor (1P)
- `VendorOrder` — purchase order from Amazon to a vendor
- `VendorOrderDetails` — full purchase order detail with parties and items
- `VendorOrderItem` — line item on a vendor purchase order
- `VendorQuantity` — quantity with unit of measure
- `PartyIdentification` — party (buyer/seller/ship-to) with address and tax info
- `TaxRegistrationDetails` — tax registration type and number
- `VendorShipment` — vendor's shipment confirmation
- `VendorShipmentDetails` — carrier and logistics details for vendor shipment
- `VendorCarrierDetails` — carrier name, SCAC code, and PRO number
- `Bill` — bill of lading reference
- `VendorShipmentItem` — item on a vendor shipment confirmation

### Solicitations and Messaging
- `SolicitationAction` — available solicitation action with constraints
- `SolicitationConstraints` — required flag and valid values for solicitation
- `MessagingAction` — buyer-seller messaging action

### Shipping and Packages
- `Shipment` — shipping label purchase record
- `Package` — individual package with dimensions, weight, and tracking
- `LabelSpecification` — label format and stock size
- `ParcelInput` — parcel dimensions and weight for rate shopping
- `TrackingInfo` — full tracking record with event history
- `TrackingEventSummary` — latest status code and date
- `TrackingEvent` — individual tracking scan event

### Customer Metrics
- `CustomerMetrics` — seller performance metrics (sales, units, feedback, refunds)

### Common Value Objects
- `Money` — amount and currency code
- `Weight` — value and unit (oz, g, kg, lb)
- `Dimensions` — length, width, height, and unit
- `Address` — postal address with international country code support
- `DateRange` — start and end DateTime pair
- `PageToken` — next-page cursor

## Query Operations

The `Query` type exposes read operations across all domains:

- **Account:** `sellerAccount`, `marketplaces`, `marketplace`
- **Orders:** `orders` (filtered list), `order`, `orderItems`
- **Catalog:** `catalogItem`, `searchCatalogItems`
- **Listings:** `listingItem`, `listingItems`
- **Pricing:** `itemPricing`, `competitivePricing`
- **Inventory:** `inventory`, `fbaInventory`
- **Reports:** `report`, `reports`, `reportDocument`, `reportSchedules`
- **Feeds:** `feed`, `feeds`, `feedDocument`
- **Finance:** `financeGroups`, `financialEvents`
- **Fulfillment:** `fulfillmentOrder`, `fbaShipment`, `fbaShipments`
- **Notifications:** `subscriptions`, `destinations`
- **Browse:** `browseNode`, `category`
- **Vendor:** `vendorOrders`
- **Deals:** `deals`, `coupons`
- **Shipping:** `shipment`, `tracking`
- **Metrics:** `customerMetrics`

## Mutation Operations

The `Mutation` type exposes write operations:

- **Orders:** `confirmShipment`
- **Listings:** `putListingItem`, `deleteListingItem`, `patchListingItem`
- **Feeds:** `createFeed`, `createFeedDocument`
- **Reports:** `createReport`, `cancelReport`, `createReportSchedule`, `cancelReportSchedule`
- **Fulfillment:** `createFulfillmentOrder`, `updateFulfillmentOrder`, `cancelFulfillmentOrder`, `createFBAInboundShipment`, `updateFBAInboundShipment`
- **Notifications:** `createSubscription`, `deleteSubscription`, `createDestination`, `deleteDestination`
- **Vendor:** `submitAcknowledgement`, `submitShipmentConfirmation`
- **Pricing:** `submitPriceUpdate`
- **Messaging:** `sendInvoice`, `sendDigitalAccessKey`, `requestReview`
- **Shipping:** `createShipment`, `cancelShipment`

## References

- SP-API Developer Docs: https://developer-docs.amazon.com/sp-api/
- SP-API GitHub Models: https://github.com/amzn/selling-partner-api-models
- Selling Partner API Reference: https://developer-docs.amazon.com/sp-api/reference
- Amazon Marketplace Web Service (deprecated): https://docs.developer.amazonservices.com/
