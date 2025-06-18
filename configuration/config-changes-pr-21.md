# Configuration Documentation for PR: Test all 666

## Overview

This PR introduces significant changes to the project's configuration and workflow files. It adds a new workflow file, modifies several existing ones, and changes the upgrade process. This documentation provides a comprehensive overview of these changes and their impact on the project's configuration.

## New Configuration Options

### .github/workflows/01-needs-triage-labeler.yml

A new workflow file has been added to the project. This workflow automatically labels new issues that need triage. The configuration options for this workflow are located within the file itself.

## Modified Configuration Options

Several existing workflow files have been modified, including:

- .github/workflows/05-deploy.yml
- .github/workflows/05-prepare-release.yml
- .github/workflows/admin.yml
- .github/workflows/backport.yml
- .github/workflows/downstream.yml
- .github/workflows/integration.yml
- .github/workflows/nightly.yml
- .github/workflows/php.yml
- .github/workflows/storefront.yml
- .github/workflows/sync.yml

The changes to these files primarily involve the removal of redundant code and the addition of new steps to improve the workflows' efficiency and reliability.

## Removed Configuration Options

The changes in this PR have resulted in the removal of several configuration options from the following files:

- .github/workflows/05-deploy.yml
- .github/workflows/admin.yml
- .github/workflows/storefront.yml
- .github/workflows/php.yml

## Environment Variable Changes

There are no changes to environment variables in this PR.

## Default Value Changes

There are no changes to default values in this PR.

## Migration Steps for Existing Configurations

Due to the changes in this PR, users may need to update their existing configurations. The specific steps will depend on the individual configuration, but in general, users should:

1. Review the changes in this PR to understand their impact.
2. Update any configuration files that reference the modified or removed options.
3. Test the updated configuration to ensure it works as expected.

## Examples of New Configuration Formats

The new workflow file, .github/workflows/01-needs-triage-labeler.yml, uses the following format:

```yaml
name: "Label issues that need triage"
on:
  issues:
    types: [opened]
jobs:
  label:
    runs-on: ubuntu-latest
    steps:
    - name: "Label issues"
      uses: actions/labeler@v3
      with:
        repo-token: "${{ secrets.GITHUB_TOKEN }}"
        configuration-path: .github/labeler.yml
```

This configuration specifies that the workflow should run whenever a new issue is opened. It uses the `actions/labeler` action to automatically apply labels based on the rules defined in `.github/labeler.yml`.

## Conclusion

This PR introduces significant changes to the project's configuration and workflows. Users should review these changes carefully and update their configurations as necessary.