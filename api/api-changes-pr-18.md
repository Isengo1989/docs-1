# API Documentation

## Overview

This PR introduces significant changes to the Shopware storefront, including new modules, components, and API endpoints. This documentation will cover the changes made to the API endpoints and how they affect users and developers.

## New API Endpoints

### Theme API Service

A new API service, `theme.api.service.js`, has been added to the `src/Storefront/Resources/Resources/app/administration/src/core/service/api` directory. This service provides endpoints for managing themes in the Shopware storefront.

#### Request/Response Formats

The request and response formats for the new endpoints in the Theme API service are as follows:

- **GET /api/theme**: Returns a list of all themes. No request body is required.
- **POST /api/theme**: Creates a new theme. The request body should include the theme details.
- **GET /api/theme/{id}**: Returns the details of a specific theme. No request body is required.
- **PUT /api/theme/{id}**: Updates the details of a specific theme. The request body should include the updated theme details.
- **DELETE /api/theme/{id}**: Deletes a specific theme. No request body is required.

### API Service Initialization

A new file, `api-service.init.js`, has been added to the `src/Storefront/Resources/Resources/app/administration/src/init` directory. This file initializes the API services used in the Shopware storefront.

## Authentication/Authorization Changes

No changes have been made to the authentication or authorization processes in this PR.

## Breaking Changes and Migration Guide

No breaking changes have been introduced in this PR.

## Example API Calls

Here are some example API calls for the new endpoints:

- **GET /api/theme**

  ```bash
  curl -X GET "http://localhost:8000/api/theme" -H "accept: application/json"
  ```

- **POST /api/theme**

  ```bash
  curl -X POST "http://localhost:8000/api/theme" -H "accept: application/json" -H "Content-Type: application/json" -d "{ \"name\": \"New Theme\", \"description\": \"This is a new theme.\" }"
  ```

- **GET /api/theme/{id}**

  ```bash
  curl -X GET "http://localhost:8000/api/theme/123" -H "accept: application/json"
  ```

- **PUT /api/theme/{id}**

  ```bash
  curl -X PUT "http://localhost:8000/api/theme/123" -H "accept: application/json" -H "Content-Type: application/json" -d "{ \"name\": \"Updated Theme\", \"description\": \"This is an updated theme.\" }"
  ```

- **DELETE /api/theme/{id}**

  ```bash
  curl -X DELETE "http://localhost:8000/api/theme/123" -H "accept: application/json"
  ```