# Configuration Documentation

## PR Title: change: watcher-name

This PR introduces a change in the watcher name used in the development process, specifically when working with the Storefront. The watcher name has been changed from `watch:storefront` to `watch:frontend`.

## File Changes

The change has been made in the `composer.json` file:

```diff
- "watch:storefront": "..."
+ "watch:frontend": "..."
```

## Configuration Changes

### New/Modified Configuration Options

The `watch:storefront` script has been renamed to `watch:frontend`. This change affects the development process, specifically when working with the Storefront.

### Environment Variable Changes

No environment variable changes were introduced in this PR.

### Default Value Changes

No default value changes were introduced in this PR.

### Migration Steps for Existing Configurations

Developers who have been using the `watch:storefront` script should now use the `watch:frontend` script. No other changes are required.

### Examples of New Configuration Formats

To start the watcher for the Storefront, use the following command:

```bash
composer run watch:frontend
```

## Impact

This change is relatively minor but important for developers to note. There is no apparent impact on the end-users or the functionality of the application.

## Recommendations

Update any developer documentation or guides that reference the `watch:storefront` script to reflect the new `watch:frontend` script.