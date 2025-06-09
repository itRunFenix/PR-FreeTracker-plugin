# Troubleshooting PR-FreeTracker Plugin

This document will help you troubleshoot common issues when using PR-FreeTracker. Below are typical scenarios and suggested solutions.

---

## Table of Contents

1. [Plugin doesn't install correctly](#plugin-doesnt-install-correctly)
2. [Errors when fetching PR details](#errors-when-fetching-pr-details)
3. [PR data doesn't open directly on GitHub](#pr-data-doesnt-open-directly-on-github)
4. [Repository configuration issues](#repository-configuration-issues)
5. [Pull Requests not displaying](#pull-requests-not-displaying)
6. [Reporting issues](#reporting-issues)

---

## Plugin doesn't install correctly

If you encounter issues during plugin installation:

- Ensure you are using a compatible version of your IDE that supports PR-FreeTracker.
- Check system requirements in the [Prerequisites.md](https://github.com/itRunFenix/PR-FreeTracker-plugin/blob/master/Prerequisites.md) file.
- If necessary, reinstall the plugin by removing it and installing it again from the JetBrains Marketplace.

**Errors in IDE console**:  
Check the IDE logs by going to `Help` > `Show Log in Explorer/Finder` to see more details about the installation errors.

---

## Errors when fetching PR details

If PR data is not fetched properly:

- Verify that the correct repository path is set.
- Ensure that you are currently in a project with an available Git repository or that you have activated the repository in the 'My Repos' tab.
- Ensure all required tools, such as GitHub CLI, are installed (see [Prerequisites.md](https://github.com/itRunFenix/PR-FreeTracker/blob/master/Prerequisites.md)).
- If errors occur, try refreshing the data and check the IDE logs for more details.

---

## PR data doesn't open directly on GitHub

If PR data doesn't open directly on GitHub:

- Make sure the checkbox is checked. 
- Ensure that data is available. If the checkbox is unchecked, you can generate the data directly within the IDE to verify that is available.

---

## Repository configuration issues

If the plugin cannot recognize your repository or displays errors:

- Double-check that you are currently in a project with an available Git repository or that you have activated the repository in the 'My Repos' tab.
- Ensure the repository is properly initialized (e.g., contains a `.git` folder).
- Update the configuration if you have changed the repository location or settings.

---

## Pull Requests not displaying

If no pull requests are displayed:

- Ensure there are active open pull requests in the selected repository.
- Verify that the repository are correctly set and activated.
- Try manually generating a report using the GitHub CLI to check whether the issue lies with the plugin or the repository data.
- Ensure you are correctly logged in to the GitHub CLI.
- Please check that you have access to the repository specified in the plugin settings as the repo path.
- Verify the authentication status by running the following command: `gh auth status`. You should see output similar to this:
    ```
      ✓ Logged in to github.com account itRunFenix (keyring)
      - Active account: true
      - Git operations protocol: https
      - Token: gho_************************************
      - Token scopes: 'gist', 'read:org', 'repo', 'workflow'
    ```
- Check the output and ensure that you are logged in, and the account is set as active.
- If you see `Active account: false`, it means the user account is logged in, but it is not the currently active account for GitHub CLI (gh) operations.
- To activate the account, log in again by running `gh auth login` and follow the steps provided.

---

## Reporting issues

If you encounter problems you cannot resolve, report them:

- Before reporting an issue, please check for useful information here: [BUG](https://github.com/itRunFenix/PR-FreeTracker-plugin/blob/master/BUG.md).
- Create an issue on the [Issues](https://github.com/itRunFenix/PR-FreeTracker-plugin/issues) section of the GitHub repository.
- Include details such as the IDE version, plugin version, OS name and version, and steps to reproduce the problem.
- You may also attach IDE logs to help diagnose the issue (logs can be found in `Help` > `Show Log in Explorer/Finder`).

---

## Additional Resources

- [JetBrains Marketplace](https://plugins.jetbrains.com/)
- [GitHub CLI Documentation](https://cli.github.com/)
- [jq Documentation](https://stedolan.github.io/jq/)
