---
description: >-
  Key Digital Functionalities describe the required functions that Bekcn-Onix should be able to perform.
---

# Key Digital Functionalities

In General, this Building Block shall be accessible on various delivery channels such as Mobile, Kiosk, Web, and applications and should be digitally inclusive for users with different capabilities. The Building Block minor features such as physical delivery of goods and services, client feedback, etc. should be able to work on feature phones (without internet) as well. To facilitate various activities and different actors as described in section 2, the Beckn-Onix stack must have specific Key Digital Functionalities. Beckn network should have:

* Consumer Platforms (i.e. Ride-Hailing Apps, Food Delivery Apps, Healthcare Service Apps, Skill Development Apps etc.) to provide a rich, demand-centric experience;
* Provider Platforms (i.e. a Ride-Hailing and Transportation,  Food Delivery, Healthcare Services, Travel and Tourism, Financial Servicesor etc.) that provide a rich, supply-centric experience;
* Consumers (i.e. patients, travellers, organizations, etc.);
* Providers (i.e. hospitals, , hotels, organizations);
* Agent (i.e. government service personnel, sellers, drivers, doctors, etc.);
* Intent (i.e. a search by product, search by category, search by provider, etc.);
* Catalogs (i.e. products, offers, add-ons, services);
* Payments and Settlements (i.e. Cash on Delivery, Prepayment, T+n settlement, etc.);
* Order management (i.e. contracts, appointments, bids, service requests);
* Fulfillments (i.e. appointments, tender approval, delivery of goods and services);
* Management of order lifecycle activities (from ordering, delivery tracking to feedback, etc.).

The Beckn-Onix stack must utilize the above objects to primarily support various consumer-provider interactions like discovery, ordering, fulfillment, and post-fulfillment. For example, a patient (Consumer) on WhatsApp (Consumer Platform) can search (Discovery) for a doctor (Agent) by his name (Intent). This request can be sent to ORS (Healthcare Provider Platform) that returns a list of Hospitals (Providers), with the various services offered (Catalog). Once identified, the patient (Consumer) can book an appointment (Order) with the Doctor (Agent).

The various actors and their activities described in section 2 must be supported by a set of non-redundant, Key Digital Functionalities listed below:

## Catalog Management

This key digital functionality should allow providers to quickly and efficiently return a matching catalog upon receipt of a search intent. The Beckn-Onix must also allow authorized administrators of the host entity to create and manage aggregated catalogs of providers, products, and services that can operate across multiple locations and timings. This functionality does not only apply to catalogs of products and services, it can be used to publish any economic resource that has a fulfillment cycle. Admins must be able to create, read, update, or delete catalogs, and any sub-component of this catalog like Items/Categories/Providers/Locations/Agents/Fulfillments/Payments/etc.

In summary, the Building Block enables the cataloging of various elements such as providers/products/services/consumers/agents/etc., such that they can be searched, retrieved, and shared in appropriate workflows.&#x20;

## Inventory Management

Authorized users of provider platforms should be able to manage the inventory of various resources available in a catalog. Providers should be able to manage the availability of products/agents/vehicles/etc., dynamically/on a real-time basis<mark style="color:blue;">,</mark> in this Building Block.

## Quotation Management

This key digital functionality should allow consumers to select items, offers, and add-ons from a catalog. It should be able to transmit them to provider. Using this functionality, the provider must be able to send their quotation. The consumer should be able to evaluate the quotation in order to generate the respective orders. Providers should be able to calculate a quote basis the item/offers/add-ons selected and to add dynamic offers without being specifically requested by the consumer. For example, a consumer should be able to add items from a provider's catalog, add offers, select add-ons into a common cart, and view the total cart value. This functionality should also allow providers to request additional information from the consumer that is required to proceed to the next stage. This functionality should also allow consumers and providers to transmit requests to each other to allow consented information sharing required to decide on a quote.

## Terms Management

This key digital functionality should allow the consumer to share billing details, fulfillment details, legal jurisdiction of dispute and resolution mechanism, and any additional information required for the provider to generate the final contract/order with the terms of fulfillment, payment, cancellation, refund, returns, and replacements. Administrators of the provider platforms should be able to configure various rules for final quote calculation, payment terms, and other terms of service depending upon the information received from the consumer. Providers should be able to evaluate the additional information that was requested when executing the quote agreement function and re-calculate the quote. For example, a healthcare service might have a standard quote for general citizens, but provide a discounted rate when it discovers from the additional data that the consumer is a senior citizen. It should allow the consumer to view the final payment terms and all details that will be included in the final contract. This functionality should allow for the final draft order/contract to be exchanged between the consumer and the provider.

## Order Management

This key digital functionality should allow the consumer to confirm an order. It should allow the creation and confirmation of an order expressed as a dual-digitally signed contract, with the terms that were agreed upon. In case the terms require payment before the creation of the contract, it should: allow the transmission of the proof of payment made from the payer to the payee, allow the provider to transmit a contract to the consumer, allow the consumer to request the provider to update various elements of the contract, allow updates to the terms of the contract and inform the consumer of the update, and allow browsing of contracts based on its various attributes.

## Order Fulfillment&#x20;

This key digital functionality should allow the consumer of a service to receive various status updates regarding the fulfillment of an order. This should allow providers to send various fulfillment updates to the consumer, and allow providers to allocate service agents manually/algorithmically (e.g. ambulance allocation as a response to a nearby emergency). The order fulfilment could have a duration of workflow, depending upon the nature of the order. The Building Block should be able to facilitate all the processes and reflect the dynamic status of an order with updates/remarks/comments.

## Order Tracking&#x20;

Consumers should be able to track the fulfillment of an order in real-time. Providers should be able to stream real-time data to the consumer related to the fulfillment of an order. This tracking is not necessarily geospatial but can contain any information that provides the consumer with real-time information like course completion percentage in case of an online course. This functionality should render the real-time data to the consumer via a tracking page.&#x20;

## Order Cancellation

This key digital functionality should allow the consumer or the provider to cancel a contract. This functionality should allow a consumer to view the terms of cancellation sent by a provider in response to a cancellation request. It should also allow both parties to see the canceled order. Providers should be able to request a cancellation reason along with additional information related to the reason for the cancellation. Consumers should be able to provide a cancellation reason and additional information related to the cancellation request. Once a cancellation is agreed upon by both parties, the current and historical data related to this activity/chain of activities shall be rolled back or archived, as per the policy.

## Rating and Feedback Management

Users of this key digital functionality should be able to rate various entities involved in the fulfillment of a contract.  These users can be both consumers and providers. A consumer should be able to rate various aspects of the service like the agent, vehicle, quality of service, customer support, etc. A provider’s agent should be able to rate the consumer as well. Upon receipt of a rating, a provider can ask for additional feedback related to the rating. This means that the activity can occur throughout the cycle of various activities, not just at the end of a single process.

## Support Management

Users of this key digital functionality should be able to contact the support center to enquire about any issues that they may be facing and create a ticket. Customer support executives should be able to view details of a contract, fetch related information, view open tickets, and resolve them. If needed, customer support executives can fetch the contact details of a provider, or their agents to gain more information related to the fulfillment of an order.&#x20;

