# Some Awesome Project

A set of project setup guidelines for my personal projects.

[![license](https://img.shields.io/badge/License-MIT-blue.svg?style=flat)](LICENSE)

## Overview

**Some Awesome Project** provides a set of guidelines for setting up my personal projects. Whether you choose to clone an existing repository or create a new one from scratch, these steps will help you get started quickly.

## Getting Started

### Option A: Clone this repo

1. **Create a new repository**: Start by creating a new repository on GitHub with a name and description.

2. **Clone with SSH**: Clone this repository to your local machine using SSH.

```sh
cd ~/web
git clone git@github.com:SandroMiguel/some-awesome-project.git <YOUR-AWESOME-PROJECT>
cd <YOUR-AWESOME-PROJECT>
code .
```

3. **Configure local name and email**: Customize your Git configuration with your username and email.

I decided to use my professional email globally, and set up another email locally for my personal projects.

```sh
rm -fr .git
git init
git config --local user.name "SandroMiguel" <--- put your username here
git config --local user.email "sandromiguel@sandromiguel.com" <--- put your email here
```

4. **Install the dependencies**

```sh
yarn
```

5. **Update the dependencies**

```sh
yarn upgrade-interactive
```

6. **Documentation**: Don't forget to write a `README.md` that introduces and explains your project.

---

### Option B: Create a new repo from scratch

1. **Create a new repository**: Start by creating a new repository on GitHub with a name, description, and choose to add a README and license.

2. **Clone with SSH**: Clone the online repository to your local machine using SSH.

```sh
cd ~/web
git clone git@github.com:SandroMiguel/<YOUR-AWESOME-PROJECT>.git
cd <YOUR-AWESOME-PROJECT>
code .
```

3. **Configure local name and email**: Customize your Git configuration with your username and email.

I decided to use my professional email globally, and set up another email locally for my personal projects.

```sh
git config --local user.name "SandroMiguel" <--- put your username here
git config --local user.email "sandromiguel@sandromiguel.com" <--- put your email here
```

4. **Add `.gitignore`**: Use [gitignore-boilerplate](https://github.com/SandroMiguel/gitignore-boilerplate)

5. **Add `package.json`**: Use [package.json-boilerplate](https://github.com/SandroMiguel/package.json-boilerplate)

**ProTip**: Sync Github topics with `package.json` file keywords

6. **Conventional Commit Messages & Semantic Versioning**: See [standard-commit](https://github.com/SandroMiguel/standard-commit)

7. **Add `.editorconfig`**: Use [editorconfig-boilerplate](https://github.com/SandroMiguel/editorconfig-boilerplate)

8. **Linting & Code Formatter**: Install [eslint-config-cecilia](https://github.com/SandroMiguel/eslint-config-cecilia)

9. **Documentation**: Write a `README.md` that introduces and explains your project.

10. **Constributing**: Add [CONTRIBUTING.md](CONTRIBUTING.md)

---

## Visual Studio Code settings

### Configure Workspace

**Workspace** settings

`.vscode/settings.json`

```json
{
    "workbench.colorCustomizations": {
        "activityBar.background": "#3eaeca99",
        "activityBarBadge.background": "#3eaeca",
        "activityBarBadge.foreground": "#000000",
        "titleBar.activeBackground": "#157A6E",
        "titleBar.activeForeground": "#FEFBFC",
        "statusBar.background": "#3eaeca99",
        "statusBarItem.hoverBackground": "#4580da",
        "statusBar.foreground": "#e7e7e7"
    }
}
```

**User** settings

`~/.config/Code/User/settings.json`

```json
{
    "[html]": {
        "editor.formatOnSave": false
    },
    "[javascript]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "[javascriptreact]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "[json]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "[jsonc]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "[php]": {
        "editor.defaultFormatter": "bmewburn.vscode-intelephense-client"
    },
    "[typescript]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "cSpell.userWords": ["autoload", "noreferrer", "phpcs", "stylelint"],
    "diffEditor.ignoreTrimWhitespace": false,
    "editor.codeActionsOnSave": {
        "source.fixAll": "explicit"
    },
    "editor.fontFamily": "Fira Code",
    "editor.fontLigatures": true,
    "editor.fontSize": 16,
    "editor.formatOnSave": true,
    "editor.matchBrackets": "never",
    "editor.suggest.insertMode": "replace",
    "editor.suggest.showWords": false,
    "editor.suggestSelection": "first",
    "editor.tokenColorCustomizations": {
        "comments": "#b1b1b1",
        "variables": "#FF6D4A",
        "functions": "#00B2BF",
        "strings": "#FFF",
        "numbers": "#518EAF",
        "keywords": "#337DED",
        "types": "#ffaa00",
        "textMateRules": [
            {
                "scope": "comment",
                "settings": {
                    "foreground": "#b1b1b1"
                }
            }
        ]
    },
    "eslint.debug": true,
    "explorer.confirmDelete": false,
    "explorer.confirmDragAndDrop": false,
    "gitblame.statusBarMessageFormat": "Blame ${author.name} ( ${author.date} )",
    "javascript.preferences.importModuleSpecifier": "non-relative",
    "javascript.updateImportsOnFileMove.enabled": "always",
    "php.suggest.basic": false,
    "phpcs.standard": "~/phpcs-cecilia-standard",
    "phpcs.executablePath": "/home/sandro/.config/composer/vendor/bin/phpcs",
    "security.workspace.trust.untrustedFiles": "open",
    "terminal.integrated.copyOnSelection": true,
    "terminal.integrated.cursorBlinking": true,
    "terminal.integrated.cursorStyle": "line",
    "terminal.integrated.drawBoldTextInBrightColors": false,
    "terminal.integrated.fontFamily": "noto mono",
    "terminal.integrated.fontSize": 16,
    "todo-tree.filtering.includeGlobs": ["**/*.php", "**/*.js"],
    "typescript.tsserver.log": "off",
    "workbench.colorCustomizations": {
        "editorBracketHighlight.unexpectedBracket.foreground": "#db6165",
        "editor.findMatchBackground": "#cc00aaa8",
        "editor.findMatchHighlightBackground": "#1d3d0379",
        "editor.findMatchHighlightBorder": "#c1fccd"
    },
    "workbench.editor.wrapTabs": true,
    "workbench.colorTheme": "Visual Studio Dark",
    "files.watcherExclude": {
        "**/.yarn/**": true
    },
    "editor.wordWrap": "on",
    "path-intellisense.autoTriggerNextSuggestion": true,
    "editor.bracketPairColorization.enabled": false,
    "php-docblocker.useShortNames": true,
    "better-comments.tags": [
        {
            "tag": "@deprecated",
            "color": "#FFFFFF",
            "strikethrough": false,
            "underline": false,
            "backgroundColor": "#FF2D00",
            "bold": false,
            "italic": false
        },
        {
            "tag": "!",
            "color": "#FF2D00",
            "strikethrough": false,
            "underline": false,
            "backgroundColor": "transparent",
            "bold": false,
            "italic": false
        },
        {
            "tag": "?",
            "color": "#3498DB",
            "strikethrough": false,
            "underline": false,
            "backgroundColor": "transparent",
            "bold": false,
            "italic": false
        },
        {
            "tag": "//",
            "color": "#474747",
            "strikethrough": true,
            "underline": false,
            "backgroundColor": "transparent",
            "bold": false,
            "italic": false
        },
        {
            "tag": "TODO",
            "color": "#FF8C00",
            "strikethrough": false,
            "underline": false,
            "backgroundColor": "transparent",
            "bold": false,
            "italic": false
        },
        {
            "tag": "*",
            "color": "#98C379",
            "strikethrough": false,
            "underline": false,
            "backgroundColor": "transparent",
            "bold": false,
            "italic": false
        }
    ]
}
```

## Contributing

Want to contribute? All contributions are welcome. Read the [contributing guide](CONTRIBUTING.md).

## Questions

If you have questions tweet me at [@sandro_m_m](https://twitter.com/sandro_m_m) or [open an issue](../../issues/new).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

**~ sharing is caring ~**
