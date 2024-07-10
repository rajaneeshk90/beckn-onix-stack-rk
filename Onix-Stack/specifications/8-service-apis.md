---
description: >-
  This section provides a reference for APIs that should be implemented by this
  Building Block.
---

# 8 Service APIs

This section provides a reference for APIs that should be implemented by this Building Block. The APIs defined here establish a blueprint for how the Building Block will interact with other Building Blocks. Additional APIs may be implemented by the Building Block, but the listed APIs define a minimal set of functionality that should be provided by any implementation of this Building Block.&#x20;

To develop the Beckn-Onix Building Block API, we have referred to various open-source specifications and data standards. The objective is to develop an API specification for this building block that is future-proof to accommodate a broad range of use cases that is agnostic of industry sector, region, and implementation technology.&#x20;

Privacy and Security is especially important. It is not recommended to create a “store-of-value” in between the consumer and the network. Instead a more federated approach is needed that transforms a “Store-of-value” into a “Flow-of-value”. Such an architecture will ensure privacy and security of data, minimize concentration risk, and allow for innovation to happen at the edges rather than at the center.&#x20;

The Beckn-Onix building block API specification uses Beckn protocol APIs and schema.

## 8.1 Catalog Management

Platform Administration APIs consist of all the endpoints that are used to provide user experience and manage the business workflows like catalog management, cart management, checkout, terms management, content management, etc. These follow REST Standards for the creation, read, update, and deletion of objects in the database.&#x20;

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml" path="/search" method="post" %}
[beckn-e-marketplace-bb-0.2-swagger.yaml](.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml" path="/catalog/{resource}/{id}" method="get" %}
[beckn-e-marketplace-bb-0.2-swagger.yaml](.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml" path="/catalog/{resource}/{id}" method="put" %}
[beckn-e-marketplace-bb-0.2-swagger.yaml](.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml" path="/catalog/{resource}/{id}" method="delete" %}
[beckn-e-marketplace-bb-0.2-swagger.yaml](.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml" path="/catalog/{resource}" method="post" %}
[beckn-e-marketplace-bb-0.2-swagger.yaml](.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml" path="/catalog/provider/{providerId}/{resource}/{id}" method="get" %}
[beckn-e-marketplace-bb-0.2-swagger.yaml](.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml" path="/catalog/provider/{providerId}/{resource}/{id}" method="put" %}
[beckn-e-marketplace-bb-0.2-swagger.yaml](.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml" path="/catalog/provider/{providerId}/{resource}/{id}" method="delete" %}
[beckn-e-marketplace-bb-0.2-swagger.yaml](.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml" path="/catalog/provider/{providerId}/{resource}" method="put" %}
[beckn-e-marketplace-bb-0.2-swagger.yaml](.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml)
{% endswagger %}

## 8.2 Inventory Management

Since inventory is a provider-centric feature, it does not interface with a customer. However, it is called by other services like quotation management, order management, and fulfillment management services.

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml" path="/search" method="post" %}
[beckn-e-marketplace-bb-0.2-swagger.yaml](.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml" path="/inventory/checkAvailability/{resource}/{id}" method="get" %}
[beckn-e-marketplace-bb-0.2-swagger.yaml](.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml" path="/inventory/item/add" method="post" %}
[beckn-e-marketplace-bb-0.2-swagger.yaml](.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml" path="/inventory/item/remove" method="post" %}
[beckn-e-marketplace-bb-0.2-swagger.yaml](.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml" path="/inventory/item/block" method="post" %}
[beckn-e-marketplace-bb-0.2-swagger.yaml](.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml" path="/inventory/addOn/unblock" method="post" %}
[beckn-e-marketplace-bb-0.2-swagger.yaml](.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml" path="/inventory/addOn/block" method="post" %}
[beckn-e-marketplace-bb-0.2-swagger.yaml](.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml" path="/inventory/item/unblock" method="post" %}
[beckn-e-marketplace-bb-0.2-swagger.yaml](.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml)
{% endswagger %}

## 8.3 Quotation Management

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml" path="/quotation" method="post" %}
[beckn-e-marketplace-bb-0.2-swagger.yaml](.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml)
{% endswagger %}

## 8.4 Order Terms Management

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml" path="/terms/payment" method="post" %}
[beckn-e-marketplace-bb-0.2-resolved (2).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml" path="/terms/fulfillment" method="post" %}
[beckn-e-marketplace-bb-0.2-resolved (2).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml" path="/terms/cancellation" method="post" %}
[beckn-e-marketplace-bb-0.2-resolved (2).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml>)
{% endswagger %}

## 8.5 Order Management

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml" path="/orders" method="post" %}
[beckn-e-marketplace-bb-0.2-swagger.yaml](.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml" path="/orders/{orderId}" method="get" %}
[beckn-e-marketplace-bb-0.2-swagger.yaml](.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml" path="/orders/{orderId}/updatePayment" method="put" %}
[beckn-e-marketplace-bb-0.2-swagger.yaml](.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml" path="/orders/{orderId}/updateFulfillment" method="put" %}
[beckn-e-marketplace-bb-0.2-swagger.yaml](.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml" path="/orders/{orderId}/updateBilling" method="put" %}
[beckn-e-marketplace-bb-0.2-swagger.yaml](.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml" path="/orders/{orderId}/updateItems" method="put" %}
[beckn-e-marketplace-bb-0.2-swagger.yaml](.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml" path="/orders/{orderId}/updateAddOns" method="put" %}
[beckn-e-marketplace-bb-0.2-swagger.yaml](.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml" path="/orders/{orderId}/cancel" method="put" %}
[beckn-e-marketplace-bb-0.2-swagger.yaml](.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger.yaml)
{% endswagger %}

## 8.6  Order Fulfillment

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml" path="/fulfillments" method="post" %}
[beckn-e-marketplace-bb-0.2-swagger (1).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml" path="/fulfillments/{fulfillmentId}" method="get" %}
[beckn-e-marketplace-bb-0.2-swagger (1).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml" path="/fulfillments/{fulfillmentId}" method="put" %}
[beckn-e-marketplace-bb-0.2-swagger (1).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml" path="/fulfillments/{fulfillmentId}" method="delete" %}
[beckn-e-marketplace-bb-0.2-swagger (1).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml" path="/fulfillment/checkServiceability" method="post" %}
[beckn-e-marketplace-bb-0.2-swagger (1).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml" path="/fulfillment/{fulfillmentId}/agent/allocate" method="put" %}
[beckn-e-marketplace-bb-0.2-swagger (1).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml" path="/fulfillment/{fulfillmentId}/agent/deallocate" method="delete" %}
[beckn-e-marketplace-bb-0.2-swagger (1).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml>)
{% endswagger %}

## 8.7 Order Tracking

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml" path="/tracking/start" method="post" %}
[beckn-e-marketplace-bb-0.2-swagger (1).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml" path="/tracking/stop" method="post" %}
[beckn-e-marketplace-bb-0.2-swagger (1).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml" path="/tracking/{order_id}/update_location" method="put" %}
[beckn-e-marketplace-bb-0.2-swagger (1).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml>)
{% endswagger %}

## 8.9 Rating and Feedback Management

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml" path="/forms" method="post" %}
[beckn-e-marketplace-bb-0.2-swagger (1).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml" path="/forms/{formId}" method="get" %}
[beckn-e-marketplace-bb-0.2-swagger (1).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml" path="/forms/{formId}" method="put" %}
[beckn-e-marketplace-bb-0.2-swagger (1).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml" path="/forms/{formId}" method="delete" %}
[beckn-e-marketplace-bb-0.2-swagger (1).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml" path="/generateFeedbackForRating" method="post" %}
[beckn-e-marketplace-bb-0.2-swagger (1).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml>)
{% endswagger %}

## 8.12 Support Management

These endpoints enables all customer support services to be managed.&#x20;

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml" path="/support/{orderId}" method="get" %}
[beckn-e-marketplace-bb-0.2-swagger (1).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml" path="/support/{orderId}" method="post" %}
[beckn-e-marketplace-bb-0.2-swagger (1).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml" path="/support/{orderId}" method="put" %}
[beckn-e-marketplace-bb-0.2-swagger (1).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml" path="/support/{orderId}" method="delete" %}
[beckn-e-marketplace-bb-0.2-swagger (1).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml" path="/support/{orderId}/agent" method="get" %}
[beckn-e-marketplace-bb-0.2-swagger (1).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml" path="/support/{orderId}/agent" method="put" %}
[beckn-e-marketplace-bb-0.2-swagger (1).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml" path="/support/{orderId}/agent" method="delete" %}
[beckn-e-marketplace-bb-0.2-swagger (1).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-swagger (1).yaml>)
{% endswagger %}

## 8.13 Order Lifecycle APIs

These APIs are implemented as a beckn protocol endpoint to enable the E-Marketplace BB to become accessible by any consumer application inside or outside the GovStack ecosystem.&#x20;

### 8.13.1 Requests

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml" path="/search" method="post" %}
[beckn-e-marketplace-bb-0.2-resolved (2).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml" path="/select" method="post" %}
[beckn-e-marketplace-bb-0.2-resolved (2).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml" path="/init" method="post" %}
[beckn-e-marketplace-bb-0.2-resolved (2).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml" path="/confirm" method="post" %}
[beckn-e-marketplace-bb-0.2-resolved (2).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml" path="/status" method="post" %}
[beckn-e-marketplace-bb-0.2-resolved (2).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml" path="/update" method="post" %}
[beckn-e-marketplace-bb-0.2-resolved (2).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml" path="/track" method="post" %}
[beckn-e-marketplace-bb-0.2-resolved (2).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml" path="/cancel" method="post" %}
[beckn-e-marketplace-bb-0.2-resolved (2).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml" path="/rating" method="post" %}
[beckn-e-marketplace-bb-0.2-resolved (2).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml" path="/support" method="post" %}
[beckn-e-marketplace-bb-0.2-resolved (2).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml" path="/get_rating_categories" method="post" %}
[beckn-e-marketplace-bb-0.2-resolved (2).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml" path="/get_return_reasons" method="post" %}
[beckn-e-marketplace-bb-0.2-resolved (2).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml" path="/get_cancellation_reasons" method="post" %}
[beckn-e-marketplace-bb-0.2-resolved (2).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml>)
{% endswagger %}

### 8.13.1 Callbacks

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml" path="/on_search" method="post" %}
[beckn-e-marketplace-bb-0.2-resolved (2).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml" path="/on_select" method="post" %}
[beckn-e-marketplace-bb-0.2-resolved (2).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml" path="/on_init" method="post" %}
[beckn-e-marketplace-bb-0.2-resolved (2).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml" path="/on_confirm" method="post" %}
[beckn-e-marketplace-bb-0.2-resolved (2).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml" path="/on_status" method="post" %}
[beckn-e-marketplace-bb-0.2-resolved (2).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml" path="/on_rating" method="post" %}
[beckn-e-marketplace-bb-0.2-resolved (2).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml" path="/on_support" method="post" %}
[beckn-e-marketplace-bb-0.2-resolved (2).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml" path="/rating_categories" method="post" %}
[beckn-e-marketplace-bb-0.2-resolved (2).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml" path="/cancellation_reasons" method="post" %}
[beckn-e-marketplace-bb-0.2-resolved (2).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml>)
{% endswagger %}

{% swagger src=".gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml" path="/return_reasons" method="post" %}
[beckn-e-marketplace-bb-0.2-resolved (2).yaml](<.gitbook/assets/beckn-e-marketplace-bb-0.2-resolved (2).yaml>)
{% endswagger %}



