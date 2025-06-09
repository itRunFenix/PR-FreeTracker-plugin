
# PR-FreeTracker Quick Start

### PR-FreeTracker is a plugin that allows you to efficiently manage and track Pull Requests (PRs) directly within your JetBrains IDE.

> **_Please note that any actions or decisions related to pull requests should be taken after reviewing the pull requests directly on GitHub._**
> **_PR-FreeTracker provides a comprehensive overview and status of your PRs._**

---

## Before We Start

Before using PR-FreeTracker, ensure that you have checked the [Prerequisites.md](https://github.com/itRunFenix/PR-FreeTracker-plugin/blob/master/Prerequisites.md) file and prepared your environment.

---

## Quick Start Guide

### 1. **Install the Plugin**

To get started with PR-FreeTracker, install the plugin from the JetBrains Marketplace.

### 2. **Accessing the Plugin**

Once installed, access PR-FreeTracker from both the **Tool-Windows (Right)** in your JetBrains IDE:

- **Tool-Windows (Right)**
- **Alt+Shift+Q** Keyboard Shortcuts

---

### 3. **Overview of Key Features**

PR-FreeTracker offers several tabs to manage your PRs:

#### **Tab: Report**
The **Report** tab provides a summary report of all your open Pull Requests, helping you quickly assess the state of your ongoing PRs.

Upon opening this tab, you will be presented with a personalized report, such as:

```bash
Welcome itRunFenix!
Here’s your personalized open Pull Request report:

Repository: itRunFenix/PR-FreeTracker-plugin

Total PRs: 6
Conflicted: 3
Changes Requested: 2
Pending Review: 2
Merge-Ready with Issues: 0
Fully Merge-Ready!: 1
```
This report gives you a quick glance at the state of all your open PRs, categorized by their status.

#### **Tab: Quick Filter** – predefined GitHub PR filters

This tab provides instant access to commonly used GitHub pull request filters. No need to type or configure anything – just click **APPLY** to launch the selected filter.

Available filters:
- **Authored by @me** – PRs you’ve created
- **Assigned to @me** – PRs assigned to you
- **My team’s review** – PRs where your team is requested to review
- **My review** – PRs where you’re requested to review
- **Open** – All open PRs
- **Closed** – PRs that were closed without merging
- **Merged** – Successfully merged PRs

#### **Tab: My Repos**
The **My Repos** tab allows for advanced configuration, though it is optional. By default, PR-FreeTracker operates within the context of the current project path, but these powerful settings enable you to browse and manage all your repositories without the need to switch contexts, even if you are working on a non-Git project.

- **Fetch Repositories**: Click this button to fetch/refresh the list of repositories and ensure you have the latest list of your repos.
- **Activate Repository**: Use the checkbox to select the repository you want to activate, allowing focused actions and operations on the selected repository.
- **Apply Changes**: After making adjustments, such as activating a repository, click 'Apply' to save your changes and ensure they take effect.

### 4. **Configure the Plugin**
PR-FreeTracker settings are project-specific, allowing you to switch between projects easily:

- **Repository Path**: Set the path to your desired repository, even if it differs from the current project. This allows seamless PR tracking across multiple repositories.

### 5. **Troubleshooting**
If you encounter any issues:

- Ensure that all required tools are installed and properly configured. [Prerequisites.md](https://github.com/itRunFenix/PR-FreeTracker-plugin/blob/master/Prerequisites.md)
- Check the plugin settings for any misconfigurations.
- Refer to the [Troubleshooting.md](https://github.com/itRunFenix/PR-FreeTracker-plugin/blob/master/Troubleshooting.md) for common issues and solutions.

## Additional Resources

- [JetBrains Marketplace](https://plugins.jetbrains.com/)
- [GitHub CLI Documentation](https://cli.github.com/)
- [jq Documentation](https://stedolan.github.io/jq/)
