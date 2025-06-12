# API Documentation

## Overview

This PR introduces significant changes to the Shopware platform, particularly in the areas of API, Backend, and Frontend. The changes are related to cookies, product details, promotion discounts, configuration files, and localization. 

## New/Modified/Removed API Endpoints

### New Endpoints

- `POST /store-api/cookie`: This endpoint is used to set cookies. The request body should contain a `CookieEntry` object.

### Modified Endpoints

- `GET /store-api/cookie`: This endpoint now returns a `CookieGroup` object instead of a list of cookies.

## Changes to Request/Response Formats

### Request Formats

- `POST /store-api/cookie`: The request body should now contain a `CookieEntry` object.

### Response Formats

- `GET /store-api/cookie`: The response now contains a `CookieGroup` object instead of a list of cookies.

## Authentication/Authorization Changes

No changes were made to authentication or authorization.

## Breaking Changes and Migration Guide

The changes introduced in this PR are breaking changes. The `GET /store-api/cookie` endpoint now returns a `CookieGroup` object instead of a list of cookies. This means that any code that relies on the old response format will need to be updated.

## Example API Calls for New Endpoints

### `POST /store-api/cookie`

Request:

```json
{
  "name": "example_cookie",
  "value": "example_value"
}
```

Response:

```json
{
  "success": true
}
```

## Recommendations

- Update the documentation to reflect the new cookie-related classes and their usage.
- Document the changes in the frontend, particularly in product details and promotion discounts.
- Update the deployment processes documentation due to changes in configuration files.
- Update the localization documentation to reflect changes in the `src/Storefront/Resources/snippet` files.
- Document the changes in the database schema introduced by the new JSON files.