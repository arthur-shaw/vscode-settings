# vscode-settings
VScode settings

# Extensions

How to get:

- Open (Git) bash shell in VSCode
- Execute this bash command to list all extensions and pre-pend VSCode installation `code --list-extensions | xargs -L 1 echo code --install-extension`

Here are the extensions:

```
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
code --install-extension wallabyjs.quokka-vscode
code --install-extension zhuangtongfa.material-theme
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
    "quarto.path": "C:\\\\Program Files\\\\RStudio\\\\resources\\\\app\\\\bin\\\\quarto\\\\bin\\\\quarto.exe",
    "workbench.colorTheme": "Catppuccin Mocha",
    "r.bracketedPaste": true,
    "r.rterm.windows": "C:\\\\WBG\\\\Anaconda3\\\\Scripts\\\\radian.exe",
    "Lua.runtime.pathStrict": true,
    "[python]": {
        "editor.formatOnType": true
    },
    "python.defaultInterpreterPath": "C:\\Users\\wb393438\\AppData\\Local\\Programs\\Python\\Python311\\python.exe",
    "editor.minimap.enabled": false,
    "git.autofetch": true,
    "githubPullRequests.fileListLayout": "tree",
    "githubPullRequests.pullBranch": "never",
    "git.openRepositoryInParentFolders": "always",
    "editor.accessibilitySupport": "off",
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
    "terminal.integrated.defaultProfile.windows": "Git Bash"
}
```
