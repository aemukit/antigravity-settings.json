# TECHNICAL CONFIGURATION: AGENTIC IDE & HARDWARE OVERDRIVE

This document provides a high-performance `settings.json` configuration and deployment blueprint for a 2026-standard agentic development environment optimized for speed, focus, low memory overhead, and autonomous workflow acceleration.

---

# 1. DEPLOYMENT INSTRUCTIONS

To apply this configuration correctly, follow the sequence below carefully.

## 1.1 Open Command Palette
Press:

- **Windows/Linux:** `Ctrl + Shift + P`
- **Mac:** `Cmd + Shift + P`

## 1.2 Open JSON Settings
Search for:

```txt
Preferences: Open User Settings (JSON)
```

Then select the command.

## 1.3 Replace Existing Configuration
Delete the entire current configuration inside your `settings.json` file and paste the configuration block below.

## 1.4 Save & Initialize
Press:

- `Ctrl + S`
- or `Cmd + S`

The environment will apply changes instantly without requiring a restart.

---

# 2. SETTINGS.JSON

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

  "/* --- [2] PRODUCT-BUILDER HUD (Visual Sharpness) --- */": "",
  "editor.fontFamily": "'JetBrains Mono', 'Fira Code', 'Menlo', 'Monaco', monospace",
  "editor.fontWeight": "500",
  "editor.fontSize": 13,
  "editor.lineHeight": 1.6,
  "editor.letterSpacing": 0.4,
  "editor.fontLigatures": true,
  "workbench.fontAliasing": "antialiased",
  "workbench.activityBar.location": "hidden",
  "workbench.statusBar.visible": true,
  "workbench.layoutControl.enabled": false,
  "breadcrumbs.enabled": false,
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

  "/* --- [4] THE PRODUCTIVITY CORE --- */": "",
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

# 3. PERFORMANCE AUDIT — BEFORE VS AFTER

| Metric | Standard IDE | Agentic Optimized |
|---|---|---|
| UI Latency | Visible scroll lag & heavy rendering | GPU-accelerated minimal rendering |
| Memory Ceiling | Unlimited tab accumulation | Strict 3-tab workflow |
| Agent Context | Single-file awareness | Full project indexing depth |
| Code Hygiene | Manual formatting & linting | Automated save-to-fix pipeline |
| Workspace Focus | Visual clutter | HUD-style precision layout |
| Navigation Speed | Multi-click workflows | Keyboard-first operations |

---

# 4. CRITICAL BROWSER OPTIMIZATION

The default configuration uses the **Floorp Browser** for efficient debugging and lightweight execution.

If you use another browser, replace this line:

```json
"workbench.externalBrowser": "floorp"
```

With one of the supported values below:

| Browser | Value |
|---|---|
| Google Chrome | `"chrome"` |
| Microsoft Edge | `"msedge"` |
| Brave Browser | `"brave"` |
| Firefox | `"firefox"` |

> Ensure the browser executable is available in your operating system PATH for instant execution and reduced launch overhead.

---

# 5. ADVANCED PRODUCTIVITY FEATURES

## 5.1 Autonomous Intelligence Layer
The configuration enables large-context agent execution with deep indexing support, allowing the environment to understand relationships across the entire project instead of isolated files.

## 5.2 Visual Ergonomics Engine
The typography stack combines:

- JetBrains Mono
- Fira Code
- Optimized spacing
- Medium font weight
- Compact rendering

This creates a high-clarity development HUD designed for extended sessions exceeding 10 hours.

## 5.3 Self-Healing Save System
Every save action automatically triggers:

- ESLint fixes
- Import organization
- Missing import injection
- Prettier formatting

This reduces maintenance overhead and keeps the codebase continuously production-ready.

## 5.4 Zero-Bloat Runtime Strategy
The configuration aggressively disables:

- unnecessary rendering
- background watchers
- redundant UI overlays
- excessive Git refresh cycles

This dramatically improves responsiveness on lower-end hardware while preserving high-end scalability.

---

# 6. POST-INSTALLATION CHECKLIST

- [ ] Memorize `Ctrl + B` for Sidebar Toggle
- [ ] Memorize `Ctrl + P` for Instant File Search
- [ ] Install Prettier Extension
- [ ] Install ESLint Extension
- [ ] Enable Hardware Accelerated GPU Scheduling
- [ ] Restart VS Code after initial configuration
- [ ] Verify terminal GPU acceleration is functioning

---

# 7. RECOMMENDED EXTENSIONS

For maximum compatibility and workflow efficiency, install the following extensions:

```txt
ESLint
Prettier - Code formatter
GitHub Copilot
Error Lens
Pretty TypeScript Errors
Path Intellisense
Turbo Console Log
```

---

# 8. FINAL NOTES

This configuration is designed around four principles:

1. Maximum execution speed
2. Minimal cognitive noise
3. Autonomous maintenance
4. Full-project AI awareness

The objective is not aesthetics alone — it is sustained high-performance software production with reduced friction, reduced latency, and increased strategic focus.
