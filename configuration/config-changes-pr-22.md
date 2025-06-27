# Configuration Documentation

## Overview

This documentation covers the changes made to the `composer.json` file in the Shopware project. The changes involve renaming a script command. This change affects the documentation where the old command is mentioned. The affected documentation needs to be updated to reflect this change.

## Configuration Changes

### Modified Configuration Options

The `watch:storefront` command in the `composer.json` file has been renamed to `watch:frontend`.

### Environment Variable Changes

No environment variable changes were made in this update.

### Default Value Changes

No default value changes were made in this update.

## Migration Steps for Existing Configurations

If you have any scripts or processes that rely on the `watch:storefront` command, you will need to update them to use the new `watch:frontend` command.

## Examples of New Configuration Formats

In the `composer.json` file, the command has been updated as follows:

```json
"scripts": {
    "watch:frontend": "..."
}
```

## Recommendations

- Update the command 'watch:storefront' to 'watch:frontend' in the documentation.
- Inform developers about the change in the command name.
- Check if there are other references to the old command in the documentation and update them as well.

## Conclusion

This change is part of our ongoing efforts to improve the clarity and consistency of our codebase. We appreciate your understanding and cooperation in adapting to these changes. If you have any questions or concerns, please feel free to reach out to us.