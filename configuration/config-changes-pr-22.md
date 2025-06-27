# Configuration Documentation

## Overview

This documentation covers the changes made to the `watcher-name` in the `composer.json` file. The changes were necessary to enhance the functionality of the watcher and improve the overall performance of the application.

## Changes

### Modified Configuration Options

The `watcher-name` configuration option in the `composer.json` file has been modified. This change affects how the watcher behaves and interacts with the rest of the application.

### Default Value Changes

The default value for the `watcher-name` configuration option has been changed. This change will affect all instances of the application where the default configuration is used.

## Migration Steps

For existing configurations, you will need to update the `watcher-name` configuration option in your `composer.json` file to match the new default value. This can be done manually by editing the `composer.json` file, or automatically by running a migration script.

## Examples

Here is an example of the new configuration format:

```json
{
  "watcher-name": "new-watcher-name"
}
```

Replace `"new-watcher-name"` with the name of your watcher.

## Conclusion

These changes to the `watcher-name` configuration option will help improve the performance and functionality of the application. Please ensure to update your existing configurations to avoid any potential issues.