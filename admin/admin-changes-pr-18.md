# Administration Documentation

## Overview of Administrative Changes

This PR introduces significant changes to the Shopware storefront. The changes include the addition of new modules, components, and API endpoints. The new modules include 'sw-settings-storefront' and 'sw-theme-manager'. These modules provide new functionalities for storefront settings and theme management respectively. 

## New Admin Features

### sw-settings-storefront Module

This module provides a new interface for managing storefront settings. It includes a new page `sw-settings-storefront-index` and a new component `sw-settings-storefront-configuration`. The page provides an overview of the storefront settings, while the component provides the functionality to modify these settings.

### sw-theme-manager Module

This module provides a new interface for managing themes. It includes a new component `sw-theme-modal` for creating and editing themes, and `sw-theme-list-item` for listing and selecting themes. The module also includes a new mixin `sw-theme.mixin.js` that provides common functionalities for theme management.

### New API Endpoints

New API endpoints have been added for theme management. These endpoints are provided by the new service `theme.api.service.js`. The service provides functionalities for creating, updating, deleting, and retrieving themes.

## New Admin Workflows

The new modules introduce new workflows for managing storefront settings and themes. 

For storefront settings, administrators can navigate to the `sw-settings-storefront-index` page where they can view and modify the settings using the `sw-settings-storefront-configuration` component.

For theme management, administrators can navigate to the theme manager where they can create, edit, delete, and select themes using the `sw-theme-modal` and `sw-theme-list-item` components.

## Migration Steps for Admin Users

Admin users will need to update their Shopware installation to include the new modules and components. This can be done by pulling the latest changes from the Shopware repository and running the necessary update scripts.

## Updated Admin Permissions or Access

The new modules and components require new permissions for access. These permissions are defined in the `acl/index.js` file in the `sw-theme-manager` module. Administrators will need to update their user roles to include these new permissions.

## Conclusion

The changes introduced in this PR significantly enhance the administrative capabilities of the Shopware storefront. Administrators now have more control over storefront settings and theme management. The new API endpoints also provide developers with more flexibility in interacting with themes.