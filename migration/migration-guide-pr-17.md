# Migration Documentation for PR: test: storefront-changes

## Overview of Breaking Changes

The PR introduces significant changes to the Shopware platform, particularly in the areas of API, Backend, and Frontend. The changes are related to cookies, product details, promotion discounts, configuration files, and localization. 

## Step-by-Step Migration Guide

1. **Cookie-related Classes**: The PR introduces new classes related to cookies. Update your code to use these new classes. Refer to the code examples below for guidance.

2. **Frontend Changes**: Changes have been made to product details and promotion discounts. Update your frontend code to reflect these changes.

3. **Configuration Files**: Changes have been made to configuration files. Update your deployment processes to reflect these changes.

4. **Localization**: Changes have been made to the `src/Storefront/Resources/snippet` files. Update your localization files to reflect these changes.

5. **Database Schema**: New JSON files have been introduced which changes the database schema. Update your database to reflect these changes.

## Code Examples Showing Before/After

### Cookie-related Classes

Before:
```php
// Old way of handling cookies
```

After:
```php
// New way of handling cookies using the new classes
```

### Frontend Changes

Before:
```javascript
// Old way of handling product details and promotion discounts
```

After:
```javascript
// New way of handling product details and promotion discounts
```

### Configuration Files

Before:
```xml
// Old configuration file
```

After:
```xml
// New configuration file
```

### Localization

Before:
```json
// Old localization file
```

After:
```json
// New localization file
```

### Database Schema

Before:
```json
// Old database schema
```

After:
```json
// New database schema
```

## Common Migration Issues and Solutions

1. **Issue**: Difficulty adapting to the new cookie-related classes.
   **Solution**: Refer to the code examples above and the updated documentation for guidance.

2. **Issue**: Frontend changes causing display issues.
   **Solution**: Ensure your frontend code is updated to reflect the changes in product details and promotion discounts.

3. **Issue**: Deployment issues due to changes in configuration files.
   **Solution**: Update your deployment processes to reflect the changes in configuration files.

4. **Issue**: Localization issues due to changes in snippet files.
   **Solution**: Update your localization files to reflect the changes.

5. **Issue**: Database errors due to changes in the schema.
   **Solution**: Update your database to reflect the changes introduced by the new JSON files.

## Timeline and Support Information

The changes introduced by this PR are expected to be live by the next release. For support during the migration process, please refer to the updated documentation and reach out to the Shopware community and support channels.