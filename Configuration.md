# ⚙️ Plugin Configuration Storage

PR-FreeTracker and PR-FlowTracker store your **project-specific plugin state** (e.g. the last used GitHub repository) inside your IDE’s `.idea/` directory. 

These files allow the plugin to remember your selections between sessions without affecting other users or your Git repository.

---

## 🗂 File Locations

| Plugin           | Configuration File             |
|------------------|--------------------------------|
| PR-FreeTracker   | `.idea/pr-free-settings.xml`   |
| PR-FlowTracker   | `.idea/pr-flow-settings.xml`   |

These files:
- are **local** to your IDE project,
- **should not be versioned or shared**,
- contain only repositories fetched via the “Fetch Repositories” button in the My Repos tab (including private ones),
- may **interfere with Git operations** (e.g. branch switching) if not ignored.

---

## ✍️ Manual Editing
These configuration files are plain XML and may be manually edited if needed.

For example:

- To remove a repository from the plugin’s dropdown or reports, you can directly delete its entry from the XML file.

- This is helpful if you accidentally added an invalid path or want to clean up old test entries.

---

## 🧾 Recommended `.gitignore` entries

Add these lines to your root `.gitignore` file:

```gitignore
# Plugin configuration (local settings)
.idea/pr-free-settings.xml
.idea/pr-flow-settings.xml
```

---

## 🛠 If these files are already tracked in Git
If the configuration files were accidentally committed before adding them to .gitignore, Git will continue tracking them. To stop this, run:

``` 
git rm --cached .idea/pr-free-settings.xml
git rm --cached .idea/pr-flow-settings.xml
git commit -m "Remove plugin settings files from version control"
```

After that, .gitignore will fully take effect and the files will remain local only.

---


## ✅ Summary
These files are essential for local plugin behavior, but not intended for Git.

Ignoring them keeps your Git history clean and prevents accidental PR tracking data from being committed.

