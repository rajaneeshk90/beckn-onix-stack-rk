---
description: This section provides the context of the building block.
---

# Description

Beckn as a protocol defines an underlying structure for creation of Open Commerce Networks and conduct transaction over them. It defines a set of message structures in the form of core protocol specifications. GitHub - beckn/protocol-specifications: Core protocol specification for peer-to-peer consumer-provider interaction . While these describe a very generic framework, actual network implementations usually need to define other policies for their participants. These policies published by the network facilitator extends the core specifications by defining tag-groups, defining semantic meaning for these tag groups, imposing limitations on the fields through defining enumerations etc.

Beckn-Onix is a protocol stack initiated by FIDE, designed to deploy reliable, configurable, and fast Beckn protocol-enabled networks through a virtual appliance.

This initiative also seeks to engage the community in contributing to the development of secure, reliable, and high-performance ONIX builds suitable for production environments.

Think of it as analogous to Apache or Nginx for HTTP.

## **Current scope**

While there may be many such use cases within the current scope, the functional requirements to cover the services required from the Beckn-Onix stack has considered specific use cases like:

**Beckn Application Platform (BAP)**

1. [BAP-Use Case 1: Retail](./../use-case-definitions/BAP/Beckn-Onix-retail-BAP.md)
2. [BAP-Use Case 2: Mobility](./../use-case-definitions/BAP/Beckn-Onix-Mobility-BAP.md)

**Beckn Provider Platform (BPP)**

1. [BPP-Use Case 1: Retail](./../use-case-definitions/BPP/Beckn-Onix-Retail-BPP.md)
2. [BPP-Use Case 2: Mobility](./../use-case-definitions/BPP/Beckn-Onix-Mobility-BPP.md)

These use cases have business processes with several steps, wherein specific steps that involve the Beckn-Onix stack, was studied as example implementations (such as Discovery, Ordering, Fulfillment, and Post-Fulfillment of services rendered by individual entities and users in various roles.&#x20;

Currently, the following actors have been identified as "users" of the Beckn-Onix stack:

* "Network Facilitators (NFs)": Entities or individuals who help manage and coordinate activities within the Beckn network, ensuring that participants adhere to standards and protocols. These are the network custodians who will be responsible for creating necessary infra for the Beckn network and responsible for managing the same. Components in the network include Beckn Gateway and Registry.
* "Network Participants (NPs)": In the context of Beckn, network participants refer to the various entities that are part of the decentralized digital network. These participants can include:
    - BAP: an application or digital platform that interacts with the Beckn network to enable consumers to discover, request, and avail various services offered by service providers within the network. The BAP acts as an interface for consumers, providing them with the means to access a wide range of services through a unified platform.
    - BPP: a service provider that offers goods or services on the Beckn network. The BPP integrates with the Beckn protocol to make its offerings discoverable and accessible to consumers through Beckn Application Platforms (BAPs). By adhering to the Beckn standards, a BPP ensures seamless interactions and transactions within the decentralized digital commerce ecosystem.
