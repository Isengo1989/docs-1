# Configuration Documentation

## Change: Watcher Name

This documentation covers the changes made to the watcher name in the `composer.json` file.

### 1. Configuration Options

The watcher name for the Storefront has been changed. The old command `watch:storefront` has been replaced with the new command `watch:frontend`.

### 2. Environment Variable Changes

No environment variable changes were made in this update.

### 3. Default Value Changes

The default command to watch the Storefront has been changed from `watch:storefront` to `watch:frontend`.

### 4. Migration Steps for Existing Configurations

If you have any scripts, automation, or documentation that uses the `watch:storefront` command, you will need to update them to use the new `watch:frontend` command.

### 5. Examples of New Configuration Formats

In your scripts or automation, replace any instance of `watch:storefront` with `watch:frontend`.

Old command:
```
composer run watch:storefront
```

New command:
```
composer run watch:frontend
```

### Important Notes

Please ensure to inform all developers and users about this change in command. This can be done through release notes or documentation updates. All documentation that references the `watch:storefront` command should be updated to reflect the new `watch:frontend` command.