# Deployment Documentation for PR 'Test all 666'

## Overview

This document provides comprehensive deployment documentation for the changes introduced in the PR titled 'Test all 666'. The PR has a significant impact on the documentation due to changes in the PR template, addition of new workflow files, modifications in the configuration files, and changes in the upgrade process. 

## Changes to Build/Deployment Process

The changes in the PR have led to modifications in the build and deployment process. The '.github/workflows/05-deploy.yml' file has been modified, which may affect the deployment process. 

## New/Modified CI/CD Workflows

Several new workflow files have been added and existing ones have been modified. 

- A new workflow file '.github/workflows/01-needs-triage-labeler.yml' has been added. This workflow automatically labels new issues that need triage. 

- The '.github/workflows/05-prepare-release.yml' file has been modified. This workflow prepares the release by creating a release branch, updating the version, and creating a PR. 

- The '.github/workflows/integration.yml' file has been modified. This workflow runs integration tests. 

- The '.github/workflows/nightly.yml' file has been modified. This workflow runs nightly builds. 

## Infrastructure Requirements

There are no new infrastructure requirements introduced by this PR. 

## Deployment Steps Changes

The changes in the '.github/workflows/05-deploy.yml' file may lead to changes in the deployment steps. Please review this file to understand the changes and adjust your deployment process accordingly. 

## Environment Setup Modifications

The changes in the '.github/bin/check_workflow.bash' and '.github/bin/split.bash' files may lead to modifications in the environment setup. Please review these files to understand the changes and adjust your environment setup process accordingly. 

## Recommendations

- Update the 'resources/guidelines/code/contribution.md' to reflect the changes in the PR template.
- Update the 'README.md' to include the new workflow file '.github/workflows/01-needs-triage-labeler.yml'.
- Update the 'LP-01-familiarise-yourself-with-shopware/CO-03-shopware-setup/LU-03-setup-project.md' to reflect any changes in the setup/deployment process due to the modifications in the configuration files.
- Update the upgrade documentation files to reflect the changes in the upgrade process. 

## Conclusion

The changes introduced in the PR 'Test all 666' have a significant impact on the deployment process. It is recommended to review the changes and update your processes accordingly.