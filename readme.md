# ANTIGRAVITY IDE: OPTIMIZED CUSTOM JSON

## 1. What is this project?
The **Antigravity IDE Configuration** is a high-performance optimization blueprint for the Antigravity fork of VS Code. It transforms the standard development environment into a suoer neat agentic IDE. It is designed to minimize system resource consumption (RAM/CPU) while maximizing the capabilities of AI-driven coding agents.

## 2. What it solves
*   **Bloatware Fatigue:** Eliminates unnecessary UI rendering, background telemetry, and redundant decorations.
*   **Latency Spikes:** Offloads rendering to the GPU and simplifies the UI stack for an instant-response feel.
*   **Context Fragmentation:** Configures deep-indexing for agents, allowing them to understand your entire project instead of single files.
*   **Maintenance Overhead:** Automates code hygiene (linting, formatting, imports) at the moment of saving.

## 3. Setup Instructions

### Linux
1. Open terminal and navigate to your VS Code config directory: `~/.config/Antigravity/User/`.
2. Open `settings.json`.
3. Paste the configuration provided below and save.

### macOS
1. Open VS Code.
2. Press `Cmd + Shift + P` and search for "Open User Settings (JSON)".
3. Paste the configuration and save.

### Windows
1. Open VS Code.
2. Press `Ctrl + Shift + P` and search for "Open User Settings (JSON)".
3. Paste the configuration and save.

---

## 4. What makes it special?
*   **Hardware Overdrive:** Strips the IDE down to the bare essentials for extreme speed.
*   **HUD-Style Efficiency:** Provides visible, clean UI elements (Activity Bar, Breadcrumbs) while disabling heavy animations and shadows.
*   **Autonomous Logic:** The "Self-Healing" system ensures that code is always production-ready, minimizing the need for manual fixes.

---

## 5. The Configuration (settings.json)

```json
{
  "/* --- [1] HARDWARE OVERDRIVE (Maximum Speed / Minimum RAM) --- */": "",
  "editor.minimap.enabled": false,
  "editor.scrollbar.vertical": "hidden",
  "editor.scrollbar.horizontal": "hidden",
  "editor.overviewRulerBorder": false,
  "editor.hideCursorInOverviewRuler": true,
  "editor.renderLineHighlight": "none",
  "editor.occurrenceHighlight": "off",
  "editor.selectionHighlight": false,
  "editor.links": false,
  "editor.colorDecorators": false,
  "editor.bracketPairColorization.enabled": true,
  "editor.guides.indentation": false,
  "editor.renderWhitespace": "none",
  "editor.cursorSmoothCaretAnimation": "on",
  "editor.cursorBlinking": "expand",
  "editor.smoothScrolling": true,
  "workbench.list.smoothScrolling": true,
  "workbench.editor.limit.enabled": true,
  "workbench.editor.limit.value": 3,
  "terminal.integrated.gpuAcceleration": "on",
  "terminal.integrated.scrollback": 5000,
  "files.autoSave": "onFocusChange",
  "git.autorefresh": false,
  "git.enableSmartCommit": true,

  "/* --- [2] PRODUCT-BUILDER HUD (Visual Sharpness & Usability) --- */": "",
  "editor.fontFamily": "'JetBrains Mono', 'Fira Code', 'Menlo', 'Monaco', monospace",
  "editor.fontWeight": "500",
  "editor.fontSize": 13,
  "editor.lineHeight": 1.6,
  "editor.letterSpacing": 0.4,
  "editor.fontLigatures": true,
  "workbench.fontAliasing": "antialiased",
  "workbench.activityBar.location": "default",
  "workbench.activityBar.visible": true,
  "workbench.statusBar.visible": true,
  "workbench.layoutControl.enabled": true,
  "breadcrumbs.enabled": true,
  "window.menuBarVisibility": "compact",
  "window.titleBarStyle": "custom",

  "/* --- [3] ANTIGRAVITY AGENT: FULL PRODUCT AUTONOMY --- */": "",
  "chat.viewSessions.orientation": "stacked",
  "chat.agent.maxContextTokens": 128000,
  "chat.thinking.style": "compact",
  "chat.agent.thinking.terminalTools": true,
  "chat.tools.autoExpandFailures": true,
  "chat.notifyWindowOnResponseReceived": true,
  "chat.editMode.hidden": true,
  "inlineChat.renderMode": "lightweight",
  "antigravity.ai.streamResponsiveness": 1.0,
  "antigravity.agent.indexing.depth": 15,
  "antigravity.agent.autoBrowserExecution": "manual",
  "antigravity.agent.telemetry.enabled": false,
  "antigravity.agent.workspaceTrust.enabled": true,
  "chat.mcp.assisted.nuget.enabled": true,
  "chat.mcp.gallery.enabled": true,

  "/* --- [4] THE \"HIDDEN\" PRODUCTIVITY GEMS --- */": "",
  "editor.linkedEditing": true,
  "editor.suggest.insertMode": "replace",
  "editor.acceptSuggestionOnEnter": "on",
  "editor.snippetSuggestions": "top",
  "editor.suggest.preview": true,
  "editor.suggest.showMethods": true,
  "editor.rename.enablePreview": false,
  "editor.codeLens": false,
  "editor.lightbulb.enabled": "off",
  "editor.hover.delay": 1000,
  "editor.parameterHints.enabled": false,
  "workbench.editor.restoreViewState": true,
  "workbench.view.alwaysShowHeaderActions": false,
  "explorer.confirmDragAndDrop": false,
  "explorer.confirmDelete": false,
  "files.insertFinalNewline": true,
  "files.trimTrailingWhitespace": true,
  "search.useIgnoreFiles": true,
  "search.useGlobalIgnoreFiles": true,

  "/* --- [5] SELF-HEALING & AUTOMATIC CLEANUP --- */": "",
  "editor.formatOnSave": true,
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": "explicit",
    "source.organizeImports": "explicit",
    "source.addMissingImports": "explicit"
  },

  "/* --- [6] SYSTEM-LEVEL SHIELDING (Zero Bloat) --- */": "",
  "files.watcherExclude": {
    "**/.git/objects/**": true,
    "**/node_modules/**": true,
    "**/dist/**": true,
    "**/build/**": true,
    "**/.cache/**": true,
    "**/tmp/**": true,
    "**/Library/Caches/**": true,
    "**/$Recycle.Bin/**": true
  },

  "/* --- [7] BROWSER & PLATFORM BRIDGE --- */": "",
  "workbench.externalBrowser": "floorp",
  "debug.javascript.autoAttachFilter": "smart",
  "liveServer.settings.NoBrowser": true,
  "window.nativeTabs": false
}
```

---

## 6. Warnings & Browser Setup
*   **Browser Requirement:** This config sets `workbench.externalBrowser` to `floorp`. If you do not have Floorp installed, your debug launch configurations may fail. Update the `"workbench.externalBrowser"` value to `"chrome"`, `"brave"`, or `"firefox"` if needed.
*   **Extensions Warning:** The self-healing system relies on **ESLint** and **Prettier**. If these are not installed, the `editor.codeActionsOnSave` will do nothing.
*   **Performance Note:** While this config is light, installing 50+ extensions will still consume memory. Keep the extension count lean.

---

## 7. Productivity Tips
*   **Command Palette:** Use `Ctrl/Cmd + Shift + P` for *everything*. It is faster than navigating menus.
*   **Quick Jump:** Use `Ctrl/Cmd + P` to jump between files instantly.
*   **Hide/Show:** Press `Ctrl/Cmd + B` to toggle the Activity Bar if you need to gain extra screen real estate for deep work.
*   **Workspace Limit:** We limit open editors to 3. If you find this too restrictive, increase `"workbench.editor.limit.value"` in the config.

---

## 8. Required Extensions for Maximum Power
To make this IDE fully functional, install these via the Extensions view:
1. **ESLint:** Essential for the Self-Healing system.
2. **Prettier - Code formatter:** Ensures consistent code style.
3. **GitHub Copilot:** Recommended for agentic code completion.
4. **Error Lens:** Makes errors immediately visible on the line.
5. **Path Intellisense:** Drastically speeds up file path imports.
6. **Turbo Console Log:** Instant debug logging for rapid development.
