# Some Awesome Project

Project setup guidelines for my personal projects.

[![license](https://img.shields.io/badge/License-MIT-blue.svg?style=flat)](LICENSE)

## Option A: Clone this repo

### GitHub

#### Step 1 - Create a new repository

Write the name and description

#### Step 2 - Clone with SSH

Clone this repo.

```sh
cd ~/web
git clone git@github.com:SandroMiguel/some-awesome-project.git <YOUR-AWESOME-PROJECT>
cd <YOUR-AWESOME-PROJECT>
code .
```

#### Step 3 - Configure local name and email

I decided to use my professional email globally, and set up another email locally for my personal projects.

```sh
rm -fr .git
git init
git config --local user.name "SandroMiguel" <--- put your username here
git config --local user.email "sandromiguel@sandromiguel.com" <--- put your email here
```

#### Step 4 - Install the dependencies

```
yarn
```

#### Step 5 - Update the dependencies

```
yarn upgrade-interactive --latest
```

#### Step 6 - Documentation

Write a `README.md` that introduces and explains your project.

---

## Option B: Create a new repo from scratch

### GitHub

#### Step 1 - Create a new repository

Write the name and description (add readme and license)

#### Step 2 - Clone with SSH

Clone the online repo.

```sh
cd ~/web
git clone git@github.com:SandroMiguel/<YOUR-AWESOME-PROJECT>.git
cd <YOUR-AWESOME-PROJECT>
code .
```

#### Step 3 - Configure local name and email

I decided to use my professional email globally, and set up another email locally for my personal projects.

```sh
git config --local user.name "SandroMiguel" <--- put your username here
git config --local user.email "sandromiguel@sandromiguel.com" <--- put your email here
```

#### Step 4 - Add `.gitignore`

Use [gitignore-boilerplate](https://github.com/SandroMiguel/gitignore-boilerplate)

### Package Management

#### Step 6 - Add `package.json`

Use [package.json-boilerplate](https://github.com/SandroMiguel/package.json-boilerplate)

**ProTip**: Sync Github topics with `package.json` file keywords

### Conventional Commit Messages & Semantic Versioning

#### Step 7 - Use [standard-commit](https://github.com/SandroMiguel/standard-commit)

### EditorConfig

#### Step 8 - Add `.editorconfig`

Use [editorconfig-boilerplate](https://github.com/SandroMiguel/editorconfig-boilerplate)

### Linting & Code Formatter

#### Step 9 - Install [eslint-config-cecilia](https://github.com/SandroMiguel/eslint-config-cecilia)

### Documentation

#### Step 10 - Write a `README.md` that introduces and explains your project.

#### Step 11 - Add [CONTRIBUTING.md](CONTRIBUTING.md)

---

## Visual Studio Code settings

#### Configure Workspace

**Workspace** settings

`.vscode/settings.json`

```
{
    "workbench.colorCustomizations": {
        "activityBar.background": "#d40000",
        "activityBar.activeBackground": "#FF5050",
        "activityBar.activeBorder": "#ffffff",
        "activityBar.foreground": "#000000",
        "activityBar.inactiveForeground": "#ffffff",
        "activityBarBadge.background": "#000000",
        "activityBarBadge.foreground": "#ffffff",
        "statusBar.background": "#d40000",
        "statusBarItem.hoverBackground": "#FF5050",
        "statusBar.foreground": "#ffffff"
    }
}
```

**User** settings

`~/.config/Code/User/settings.json`

```
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
  "cSpell.userWords": ["autoload", "phpcs", "noreferrer"],
  "diffEditor.ignoreTrimWhitespace": false,
  "editor.codeActionsOnSave": {
    "source.fixAll": true
  },
  "editor.fontFamily": "'JetBrains Mono', monospace",
  "editor.fontSize": 15,
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
  "eslint.alwaysShowStatus": true,
  "eslint.debug": true,
  "explorer.confirmDelete": false,
  "explorer.confirmDragAndDrop": false,
  "gitblame.statusBarMessageFormat": "Blame ${author.name} ( ${author.date} )",
  "gitlens.codeLens.enabled": false,
  "javascript.preferences.importModuleSpecifier": "non-relative",
  "javascript.updateImportsOnFileMove.enabled": "always",
  "php.suggest.basic": false,
  "phpCodeSniffer.standard": "Custom",
  "phpCodeSniffer.autoExecutable": true,
  "phpCodeSniffer.standardCustom": "~/phpcs-cecilia-standard",
  "terminal.integrated.copyOnSelection": true,
  "terminal.integrated.cursorBlinking": true,
  "terminal.integrated.cursorStyle": "line",
  "terminal.integrated.drawBoldTextInBrightColors": false,
  "terminal.integrated.fontFamily": "Source Code Pro",
  "terminal.integrated.fontSize": 15,
  "terminal.integrated.rendererType": "dom",
  "todo-tree.filtering.includeGlobs": ["**/*.php", "**/*.js"],
  "todo-tree.tree.showScanModeButton": false,
  "typescript.tsserver.log": "off",
  "versionlens.showVersionLensesAtStartup": false,
  "vsicons.dontShowNewVersionMessage": true,
  "vsintellicode.modify.editor.suggestSelection": "automaticallyOverrodeDefaultValue",
  "workbench.colorCustomizations": {
    "editor.findMatchBackground": "#00cc44a8",
    "editor.findMatchHighlightBackground": "#ff7b00a1"
  },
  "workbench.colorTheme": "Visual Studio Dark",
  "workbench.editor.wrapTabs": true
}
```

## Contributing

Want to contribute? All contributions are welcome. Read the [contributing guide](CONTRIBUTING.md).

## Questions

If you have questions tweet me at [@sandro_m_m](https://twitter.com/sandro_m_m) or [open an issue](../../issues/new).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

**~ sharing is caring ~**
