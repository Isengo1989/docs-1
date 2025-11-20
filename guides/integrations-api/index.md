---
nav:
  title: Integrations / API
  position: 40

---

# Integrations/API

Generally, Shopware provides two APIs that serve two aspects of integrations with our platform. Both APIs are based on HTTP and though they serve different use cases, they share some underlying concepts. We recommend understanding these concepts before diving deeper into either of the APIs.

<PageRef page="general-concepts/" />

## Customer-facing interactions - Store API

Frontend applications usually provide interfaces for users \(customers\). These applications usually don't expose sensitive data and have two layers of users - anonymous and authenticated i.e., unregistered and registered. Payloads are usually small, performance and availability are critical.

<PageRef page="https://shopware.stoplight.io/docs/store-api/7b972a75a8d8d-shopware-store-api" title="Store API Endpoint Reference" target="_blank" />

## Backend-facing integrations - Admin API

These integrations are characterized by the exchange of structured data, synchronizations, imports, exports and notifications. Performance is also important in terms of high data loads rather than fast response times. Consistency, error handling, and transaction-safety are critical.

<PageRef page="https://shopware.stoplight.io/docs/admin-api/8d53c59b2e6bc-shopware-admin-api" title="Admin API Endpoint Reference" target="_blank" />

Shopware's Store and Admin APIs offer essential technical resources for you to interact with and customize the platform's core functions, enabling tailored solutions and seamless integration.

## Updates in Version 6.7

In the latest version, we have introduced the `AssociationDescription` flag. This flag is used to provide additional information about the associations in our data model. This is particularly useful for developers who are building integrations with our platform and need to understand the relationships between different entities.

We have also made significant updates to our OpenAPI schema generator for Store API endpoints. This includes the addition of over 300 lines of code to improve the accuracy and completeness of the generated schemas.

For more details about these changes, please refer to the `RELEASE_INFO-6.7.md` file.

<PageRef page="https://github.com/shopware/platform/blob/trunk/RELEASE_INFO-6.7.md" title="Release Info 6.7" target="_blank" />

## AssociationDescription Flag

The `AssociationDescription` flag is a new feature in our data model. It provides additional information about the associations between different entities in our data model. This is particularly useful for developers who are building integrations with our platform and need to understand the relationships between different entities.

For more information about how to use the `AssociationDescription` flag, please refer to our backend documentation.

<PageRef page="https://shopware.stoplight.io/docs/backend-api/8d53c59b2e6bc-shopware-backend-api" title="Backend API Documentation" target="_blank" />