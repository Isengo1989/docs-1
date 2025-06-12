# Administration Documentation

## Overview of Administrative Changes

This PR introduces significant changes to the Shopware platform, particularly in the areas of API, Backend, and Frontend. The changes are related to cookies, product details, promotion discounts, configuration files, and localization.

## Removed/Modified Admin Features

No admin features were removed in this PR. However, several files were modified. These include:

- `sw-product-detail-variants.html.twig` and `sw-product-detail-variants.spec.js` in the `sw-product` module.
- `index.js`, `sw-promotion-discount-component.html.twig`, `sw-promotion-discount-component.scss`, and `sw-promotion-discount-component.spec.js` in the `sw-promotion-v2` module.

## New Admin Workflows

No new admin workflows were introduced in this PR.

## Migration Steps for Admin Users

Due to the changes in configuration files, admin users may need to update their deployment processes. Specific steps will depend on the individual deployment setup.

## Updated Admin Permissions or Access

No changes were made to admin permissions or access in this PR.

## Detailed Changes

### Cookies

New cookie-related classes were introduced. Documentation should be updated to reflect their usage.

### Frontend

Changes were made to product details and promotion discounts. These changes should be documented to help users understand how to use the updated features.

### Configuration Files

Changes were made to configuration files. The deployment processes documentation should be updated to reflect these changes.

### Localization

Changes were made to the `src/Storefront/Resources/snippet` files. The localization documentation should be updated to reflect these changes.

### Database Schema

New JSON files introduced changes to the database schema. These changes should be documented to help developers understand the new schema.

## Conclusion

This PR introduces significant changes to the Shopware platform. It is crucial that the documentation is updated to reflect these changes, to ensure that users and developers can understand and adapt to the new features and workflows.