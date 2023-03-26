# 我VsCode中的Vim配置

```vim
 "vim.visualModeKeyBindingsNonRecursive": [
    {
      "before": ["p"],
      "after": ["p", "g", "v", "y"]
    }
  ],
  "vim.commandLineModeKeyBindingsNonRecursive": [],
  "vim.insertModeKeyBindings": [
    {
      "before": ["j", "j"],
      "after": ["<Esc>"]
    }
  ],
  "vim.normalModeKeyBindingsNonRecursive": [
    {
      "before": ["<C-j>"],
      "after": ["4", "j"]
    },
    {
      "before": ["<C-k>"],
      "after": ["4", "k"]
    },
    {
      "before": ["H"],
      "after": ["^"]
    },
    {
      "before": ["L"],
      "after": ["$"]
    },
    {
      "before": ["<C-b>"],
      "commands": ["workbench.view.explorer"]
    },
    {
      "before": ["<C-l>"],
      "commands": ["workbench.action.nextEditor"]
    },
    {
      "before": ["<C-h>"],
      "commands": ["workbench.action.previousEditor"]
    },
    {
      "before": ["<leader>", "d"],
      "after": ["d", "d"]
    },
    {
      "before": ["<C-n>"],
      "commands": [":nohl"]
    },
    {
      "before": ["K"],
      "commands": ["lineBreakInsert"],
      "silent": true
    }
  ],
  "vim.leader": "<space>",
  "vim.handleKeys": {
    "<C-a>": false,
    "<C-f>": false,
    "<C-n>": false,
    "<C-c>": false,
    "<C-v>": false
  },
  "vim.statusBarColorControl": true,
  "vim.statusBarColors.normal": ["#8FBCBB", "#434C5E"],
  "vim.statusBarColors.insert": "#BF616A",
  "vim.statusBarColors.visual": "#B48EAD",
  "vim.statusBarColors.visualline": "#B48EAD",
  "vim.statusBarColors.visualblock": "#A3BE8C",
  "vim.statusBarColors.replace": "#D08770",
  "vim.statusBarColors.commandlineinprogress": "#007ACC",
  "vim.statusBarColors.searchinprogressmode": "#007ACC",
  "vim.statusBarColors.easymotionmode": "#007ACC",
  "vim.statusBarColors.easymotioninputmode": "#007ACC",
  "vim.statusBarColors.surroundinputmode": "#007ACC",
  "workbench.iconTheme": "material-icon-theme",
  "workbench.colorTheme": "Visual Studio Light",
  "material-icon-theme.folders.theme": "specific",
  "material-icon-theme.folders.color": "#26a69a",
  "material-icon-theme.hidesExplorerArrows": true,
  "material-icon-theme.activeIconPack": "react_redux",
  "editor.fontFamily": "'Hack-Italic', Menlo, 'Input Sans Narrow', Monaco, 'Courier New', monospace",
  //输入法(需要自己去安装 im-select 插件)
  "vim.autoSwitchInputMethod.enable": true,
  "vim.autoSwitchInputMethod.defaultIM": "com.apple.keylayout.ABC",
  "vim.autoSwitchInputMethod.obtainIMCmd": "/opt/homebrew/bin/im-select",
  "vim.autoSwitchInputMethod.switchIMCmd": "/opt/homebrew/bin/im-select {im}",
  "workbench.colorCustomizations": {
    "statusBar.background": "#B48EAD",
    "statusBar.noFolderBackground": "#B48EAD",
    "statusBar.debuggingBackground": "#B48EAD",
    "statusBar.foreground": "#434C5E",
    "statusBar.debuggingForeground": "#434C5E"
  },
  "[jsonc]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[vue]": {
    "editor.defaultFormatter": "Vue.volar"
  },
  "[javascript]": {
    "editor.defaultFormatter": "vscode.typescript-language-features"
  },
  "vetur.format.defaultFormatterOptions": {
    "prettier": {
      "singleQuote": true,
      "semi": false
    }
  },

```