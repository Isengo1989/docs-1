---
nav:
  title: General Concepts
  position: 10

---

# General Concepts

Even though the Admin API and the Store API serve very different purposes, they have some commonalities handy to be aware of.

## Querying data

For the Admin API these apply to the `/search` endpoint, whilst for the Store API they apply to almost every endpoint that returns a list of records.

It starts with a very simple underlying concept, which encapsulates your entire search description in one generic object, referred to as the **search criteria**.

<PageRef page="search-criteria" />

There are some additional instructions that can be specified using **request headers**.

<PageRef page="request-headers" />

## Documentation

Here you find a common approach regarding the way that Shopware provides endpoint references for its APIs:

<PageRef page="generated-reference" />

## API Versioning

Starting with Shopware version 6.4.0.0, we decided to change our API versioning strategy. The following article will cover what has been done and changed, how it used to be and how the version strategy looks like now.

<PageRef page="api-versioning" />

## Association Description Flag

With the latest update, we have introduced a new flag called `AssociationDescription`. This flag is used to provide additional information about the associations in the API. This flag can be found in the definition of various entities such as `CustomerDefinition`, `OrderDefinition`, `ProductDefinition`, etc.

<PageRef page="association-description-flag" />

## Store API Schema Generator

We have made significant changes to the OpenAPI schema generator for Store API endpoints. The generator now includes the `AssociationDescription` flag in the generated schema. This allows for a more detailed and accurate representation of the API endpoints.

<PageRef page="store-api-schema-generator" />

These topics provide essential foundations for effective API development and usage in Shopware.

## Release Information

For detailed information about the changes in the latest release, please refer to the `RELEASE_INFO-6.7.md` file.

<PageRef page="release-info-6.7" />

## Backend Documentation

We have updated the backend documentation to include information about the addition of the `AssociationDescription` flag. Please refer to the backend documentation for more details.

<PageRef page="backend-documentation" />