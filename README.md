# PR-FreeTracker

![PR-FreeTracker-icon](images/PR-FreeTracker-iconbig.png)

## PR-FreeTracker is a plugin designed for JetBrains IDEs, which helps you track and manage open Pull Requests from GitHub, providing detailed insights into their statuses, labels, reviews, and merge conflicts.

> **_Please note that any actions or decisions related to pull requests should be taken after reviewing the pull requests directly on GitHub._**
> **_PR-FreeTracker is intended for informational purposes only and provides an overview of pull requests._**

## Install the Plugin
To get started with PR-FreeTracker, you need to install the plugin. Follow the steps below to install it:

1. **Open your IDE**: Launch the IDE where you want to install the PR-FreeTracker plugin.
2. **Navigate to Plugin Installation**: Go to the JetBrains Marketplace or the Plugins section within your IDE.
3. **Search for PR-FreeTracker**: Use the search functionality to find the PR-FreeTracker plugin.
4. **Install the Plugin**: Follow the prompts to install PR-FreeTracker.

For more details and to install the plugin, visit the [JetBrains Marketplace](https://plugins.jetbrains.com/).

## Getting Started

- Once the plugin is installed, please follow our [Prerequisites.md](https://github.com/itRunFenix/PR-FreeTracker-plugin/blob/master/Prerequisites.md) for a step-by-step list of requirements to prepare your environment. 
- After completing the setup, follow our [Quick Start guide](https://github.com/itRunFenix/PR-FreeTracker-plugin/blob/master/QuickStart.md) for a step-by-step guide with screenshots to get up and running quickly. 
- You can then start efficiently manage your Pull Requests to keep track of their status, ensuring you stay updated on all changes and actions needed.

If you encounter any issues or need assistance, please refer to the [Troubleshooting.md](https://github.com/itRunFenix/PR-FreeTracker-plugin/blob/master/Troubleshooting.md) or open an issue on the [GitHub repository](https://github.com/itRunFenix/PR-FreeTracker-plugin/issues).

---

## ⚙️ Configuration Notes

PR-FreeTracker stores your project-specific settings (such as the last used repository) in the following file:

- `.idea/pr-free-settings.xml`

This file:
- is **local to your IDE project**,
- **does not need to be shared** with collaborators,
- can safely be excluded from version control.

### 💡 Suggested `.gitignore` entry:
```gitignore
.idea/pr-free-settings.xml
```

📖 [How plugin settings are stored and ignored](https://github.com/itRunFenix/PR-FreeTracker-plugin/blob/master/Configuration.md))

---

Feel free to reach out if you have any questions or feedback. We appreciate your contributions to improving PR-FreeTracker!
