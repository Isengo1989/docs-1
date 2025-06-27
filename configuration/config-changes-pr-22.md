# Configuration Documentation

## Change: Watcher Name

This documentation covers the changes made to the watcher name in the `composer.json` file. The watcher name has been changed from `watch:storefront` to `watch:frontend`.

### New/Modified/Removed Configuration Options

- **Modified**: The watcher name in the `composer.json` file has been changed. The previous name was `watch:storefront`, and the new name is `watch:frontend`.

### Environment Variable Changes

- No environment variable changes were made in this update.

### Default Value Changes

- The default value for the watcher name has been changed from `watch:storefront` to `watch:frontend`.

### Migration Steps for Existing Configurations

1. Open the `composer.json` file in your project.
2. Locate the `scripts` section.
3. Find the `watch:storefront` script.
4. Change the name of the script from `watch:storefront` to `watch:frontend`.
5. Save and close the `composer.json` file.

### Examples of New Configuration Formats

In the `composer.json` file, the `scripts` section should now look like this:

```json
"scripts": {
    "watch:frontend": "..."
}
```

## Important Notes

Please note that this change will affect the setup or deployment process. Developers who use this script for enabling hot module reloading for the Storefront will need to use the new script name, `watch:frontend`.

All references to the `watch:storefront` script in the documentation should be updated to `watch:frontend`.