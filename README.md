# vscode-settings
VScode settings

# Extensions

How to get:

- Open (Git) bash shell in VSCode
- Execute this bash command to list all extensions and pre-pend VSCode installation `code --list-extensions | xargs -L 1 echo code --install-extension`

Here are the extensions:

```
code --install-extension bierner.docs-view
code --install-extension catppuccin.catppuccin-vsc
code --install-extension dracula-theme.theme-dracula
code --install-extension eamodio.gitlens
code --install-extension enkia.tokyo-night
code --install-extension gerane.theme-mustard
code --install-extension github.github-vscode-theme
code --install-extension github.vscode-pull-request-github
code --install-extension grapecity.gc-excelviewer
code --install-extension graphql.vscode-graphqlcode --install-extension graphql.vscode-graphql-syntax
code --install-extension hai-bo.stata-language-server
code --install-extension hediet.vscode-drawio
code --install-extension kylebarron.stata-enhanced
code --install-extension meezilla.json
code --install-extension mechatroner.rainbow-csv
code --install-extension mhutchie.git-graph
code --install-extension mohamed-el-fodil-ihaddaden.shinysnip
code --install-extension ms-azuretools.vscode-docker
code --install-extension ms-python.debugpy
code --install-extension ms-python.isort
code --install-extension ms-python.python
code --install-extension ms-python.vscode-pylance
code --install-extension ms-toolsai.jupyter
code --install-extension ms-toolsai.jupyter-keymap
code --install-extension ms-toolsai.jupyter-renderers
code --install-extension ms-toolsai.vscode-jupyter-cell-tags
code --install-extension ms-toolsai.vscode-jupyter-slideshow
code --install-extension ms-vscode-remote.remote-containers
code --install-extension ms-vscode-remote.remote-ssh
code --install-extension ms-vscode-remote.remote-ssh-edit
code --install-extension ms-vscode-remote.remote-wsl
code --install-extension ms-vscode-remote.vscode-remote-extensionpack
code --install-extension ms-vscode.remote-explorer
code --install-extension ms-vscode.remote-server
code --install-extension pkief.material-icon-theme
code --install-extension posit.shinyuieditor
code --install-extension quarto.quarto
code --install-extension rdebugger.r-debugger
code --install-extension reditorsupport.r
code --install-extension ritwickdey.liveserver
code --install-extension robbowen.synthwave-vscode
code --install-extension sainnhe.everforest
code --install-extension sdras.night-owl
code --install-extension sumneko.lua
code --install-extension tomoki1207.pdf
code --install-extension uloco.theme-bluloco-light
code --install-extension vscode-icons-team.vscode-icons
code --install-extension vscodevim.vim
code --install-extension zainchen.json
```

# Settings

How to get

- File > Preferences > Settings
- Click icon to open as JSON

Alternatively:

- Open the command palette
- Type/select `Preferences: Open User Settings (JSON`

```
{
    "workbench.iconTheme": "vscode-icons",
    "quarto.path": "C:/Program Files/Quarto/bin/quarto.exe",
    "workbench.colorTheme": "Catppuccin Mocha",
    /* R */
    "r.bracketedPaste": true,
    "r.rterm.windows": "C:/WBG/Anaconda3/Scripts/radian.exe",
    "r.plot.useHttpgd": true,
    "Lua.runtime.pathStrict": true,
    "[python]": {
        "editor.formatOnType": true
    },
    /* Python */
    "python.defaultInterpreterPath":"C:/WBG/Anaconda3/python.exe",  
    "editor.minimap.enabled": false,
    /* Git */
    "git.autofetch": true,
    "githubPullRequests.fileListLayout": "tree",
    "githubPullRequests.pullBranch": "never",
    "git.openRepositoryInParentFolders": "always",
    "editor.accessibilitySupport": "off",
    /* Vim */
    "editor.lineNumbers": "relative",
    "vim.useSystemClipboard": true,
    "vim.normalModeKeyBindingsNonRecursive": [
        {
            "before": [
                "<C-p>"
            ],
            "commands": [
                "workbench.action.quickOpen",
            ]
        },
    ],
    "editor.tabSize": 2,
    "terminal.integrated.defaultProfile.windows": "Git Bash",
    "code-runner.executorMapByFileExtension": {
        ".do": "C:/Users/WB393438/utils/rundo.exe"
    },
    "code-runner.customCommand": "C:/Users/WB393438/utils/rundolines.exe",
    "stataRun.stataPath": "C:/Program Files/Stata18/StataMP-64.exe",
    "stataRun.whichApp": "stataMP",
    "stataRun.pasteSpeed": 1,
    "stataRun.advancePosition": false,
    "diffEditor.ignoreTrimWhitespace": false,
}
```

# Keybindings

The contents of `keybindings.json`

```
// Place your key bindings in this file to override the defaults
[
  // magrittr pipe in R, Rmd, and qmd files
  // note: only active in insert mode of Vim
  {
    "key": "Ctrl+Shift+m",
    "command": "type",
    "args": { "text": " |>\n\t"},
    "when": "editorTextFocus && editorLangId =~ /r|rmd|qmd"
  },
  {
    "key": "Alt+-",
    "command": "type",
    "args": { "text": " <- "},
    "when": "editorTextFocus && editorLangId =~ /r|rmd|qmd"
  },
  // terminal
  // move position
  {
    "key": "ctrl+alt+win+left",
    "command": "workbench.action.positionPanelLeft"
  },
  {
    "key": "ctrl+alt+win+right",
    "command": "workbench.action.positionPanelRight"
  },
  {
    "key": "ctrl+alt+win+down",
    "command": "workbench.action.positionPanelBottom"
  },
  // resize
  {
    "key": "ctrl+shift+left",
    "command": "workbench.action.terminal.resizePaneLeft"
  },
  {
    "key": "ctrl+shift+down",
    "command": "workbench.action.terminal.resizePaneDown"
  },
  {
    "key": "ctrl+shift+right",
    "command": "workbench.action.terminal.resizePaneRight"
  },
  // edit pane size
  // decrease
  {
    "key": "ctrl+alt+-",
    "command": "workbench.action.decreaseViewSize"
  },
  // increase
  {
    "key": "ctrl+alt+=",
    "command": "workbench.action.increaseViewSize"
  }
]
```

# Quarto snippets

See more details [here](https://gist.github.com/jthomasmock/11acebd4448f171f786e01397df34116?permalink_comment_id=4269591#gistcomment-4269591)

```
{
  "column-70-30": {
    "prefix": "column-70-30",
    "body": [
        ":::: {.columns}", 
        "", 
        "::: {.column width=\"70%\"}", 
        "Left column", 
        ":::", 
        "", 
        "::: {.column width=\"30%\"}", 
        "Right column", 
        ":::", 
        "", 
        "::::"
    ],
    "description": "quarto columns 70-30"
  },
  "column-50-50": {
    "prefix": "column-50-50",
    "body": [
        ":::: {.columns}", 
        "", 
        "::: {.column width=\"50%\"}", 
        "Left column", 
        ":::", 
        "", 
        "::: {.column width=\"50%\"}", 
        "Right column", 
        ":::", 
        "", 
        "::::"
    ],
    "description": "quarto columns 50-50"
  },
  "column-33-33-33": {
    "prefix": "column-33-33-33",
    "body": [
        ":::: {.columns}", 
        "", 
        "::: {.column width=\"33%\"}", 
        "Left column", 
        ":::", 
        "", 
        "::: {.column width=\"33%\"}", 
        "Middle column", 
        ":::", 
        "", 
        "::: {.column width=\"33%\"}", 
        "Right column", 
        ":::", 
        "", 
        "::::"
    ],
    "description": "quarto columns 50-50"
  },
  "panel": {
    "prefix": "panel",
    "body": ["::: {.panel-tabset}", "${1:body}", ":::"],
    "description": "quarto panel"
  },
  "fence": {
    "prefix": "fence",
    "body": [":::{.${1:type}}", "${2:body}", ":::"],
    "description": "quarto fence"
  },
  "aside": {
    "prefix": "",
    "body": ["::: aside", "${1:body}", ":::"],
    "description": "quarto aside"
  },
  "fragment": {
    "prefix": "",
    "body": ["::: {.fragment .${1:type}}", "${2:body}", ":::"],
    "description": "quarto fragment"
  },
  "details": {
    "prefix": "",
    "body": [
      "<details>",
        "\t<summary>${1:summary}</summary>",
        "\t${2:content}",
      "</details>",
     ],
     "description": "HTML details tag"
  },
  "include": {
    "prefix": "include",
    "body": [
      "{{< include ${1:file} >}}"
    ],
    "description": "quarto include"
  },
  "notes": {
    "prefix": "notes",
    "description": "Speaker's notes",
    "body": [
      "::: {.notes}",
      "${1:contents}",
      ":::"
    ]
  },
}
```
