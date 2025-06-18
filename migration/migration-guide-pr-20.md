# Migration Documentation for PR: Update Shopware

## Overview of Breaking Changes

The PR titled 'Update Shopware' introduces significant changes to the Shopware application. The changes span across configuration, frontend, backend, infrastructure, and workflow files. Several new files were added, and one file was removed. These changes affect the setup, deployment, functionality, user interface, and user experience of the application, as well as the process of creating and submitting PRs and formatting issue descriptions for Jira.

## Step-by-Step Migration Guide

1. **Update Configuration Files**: The configuration files `.bc-exclude.php`, `.danger.php`, `.devcontainer/devcontainer.json`, `.editorconfig`, `.git-blame-ignore-revs`, `.gitattributes`, and `.github/CODEOWNERS` have been modified. Update your local copies of these files to match the new versions.

2. **Update Frontend and Backend Files**: The frontend and backend files `.github/DISCUSSION_TEMPLATE/proposals.yml`, `.github/ISSUE_TEMPLATE/bug_report.yml`, and `.github/ISSUE_TEMPLATE/config.yml` have been modified. New files `.github/ISSUE_TEMPLATE/epic.yaml`, `.github/ISSUE_TEMPLATE/story.yaml`, and `.github/ISSUE_TEMPLATE/technical_todo.yaml` have been added. Update your local copies of these files and add the new files to your local repository.

3. **Update Infrastructure Files**: The infrastructure files `.github/bin/check_workflow.bash`, `.github/bin/generate-phpunit-matrix.php`, and `.github/bin/split.bash` have been modified. New files `.github/bin/blue-green-check.php`, `.github/bin/js/.gitignore`, `.github/bin/js/package-lock.json`, and `.github/bin/js/package.json` have been added. Update your local copies of these files and add the new files to your local repository.

4. **Update Workflow Files**: The workflow files `.github/codecov.yml`, `.github/labeler.yml`, `.github/workflows/01-danger.yml`, and `.github/workflows/05-deploy.yml` have been modified. New files `.github/actions/ats/action.yaml`, `.github/dependabot.yml`, and `.github/workflows/01-needs-triage-labeler.yml` have been added. The file `.github/workflows/01-format-issue-description-for-jira.yml` has been removed. Update your local copies of these files, add the new files to your local repository, and remove the deleted file from your local repository.

5. **Update PR Template**: The PR template `.github/PULL_REQUEST_TEMPLATE.md` has been modified. Update your local copy of this file to match the new version.

## Code Examples Showing Before/After

Due to the extensive nature of the changes, it is not feasible to provide before and after code examples for all changes. Please refer to the PR for specific changes.

## Common Migration Issues and Solutions

1. **Issue**: Conflicts when merging the updated files into your local repository.
   **Solution**: Resolve the conflicts manually by comparing the changes and deciding which version to keep.

2. **Issue**: Errors when running the application after updating the files.
   **Solution**: Ensure that all dependencies are correctly installed and that the application is correctly configured according to the updated files.

## Timeline and Support Information

The changes are effective immediately upon merging the PR. If you encounter any issues during the migration process, please create an issue in the Shopware repository or contact the Shopware support team.

## Important Notes

Please ensure to update the related documentation files to reflect these changes. The 'contribution.md' file should be updated to reflect the changes in the PR template. The 'LU-03-setup-project.md' file should include the changes in the configuration files. The '07-embedding-external-repositories.md' file should reflect the changes in the frontend and backend files. The '01-general.md' file should include the changes in the infrastructure files. The 'README.md' file should reflect the changes in the workflow files and the removal of the '.github/workflows/01-format-issue-description-for-jira.yml' file.