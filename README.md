# Some Awesome Project

Project setup guidelines for my personal projects.

[![license](https://img.shields.io/badge/License-MIT-blue.svg?style=flat)](LICENSE)

## GitHub

### Step 1 - Create a new repository

Write the name and description (add readme and license)

### Step 2 - Clone with SSH

Clone the online repo.

```
cd ~/web
git clone git@github.com:SandroMiguel/<SOME-AWESOME-PROJECT>.git
cd <SOME-AWESOME-PROJECT>
code .
```

## .gitignore

### Step 3 - Use [gitignore-boilerplate](https://github.com/SandroMiguel/gitignore-boilerplate)

## Visual Studio Code settings

### Step 4 - Configure `.vscode/settings.json`

```
{
  "window.zoomLevel": 0,
  "editor.tokenColorCustomizations": {
    "comments": "#FFF",
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
          "foreground": "#FFF"
        }
      }
    ]
  },
  "editor.fontSize": 15,
  "gitlens.codeLens.enabled": false,
  "terminal.integrated.cursorStyle": "line",
  "terminal.integrated.copyOnSelection": true,
  "terminal.integrated.cursorBlinking": true,
  "terminal.integrated.fontWeightBold": "normal",
  "terminal.integrated.fontSize": 13,
  "terminal.integrated.drawBoldTextInBrightColors": false,
  "terminal.integrated.fontFamily": "Monospace",
  "javascript.preferences.importModuleSpecifier": "non-relative",
  "terminal.integrated.rendererType": "dom",
  "[javascriptreact]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "explorer.confirmDragAndDrop": false,
  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "editor.formatOnSave": true,
  "peacock.favoriteColors": [
    {
      "name": "Angular Red",
      "value": "#b52e31"
    },
    {
      "name": "Auth0 Orange",
      "value": "#eb5424"
    },
    {
      "name": "Azure Blue",
      "value": "#007fff"
    },
    {
      "name": "C# Purple",
      "value": "#68217A"
    },
    {
      "name": "Gatsby Purple",
      "value": "#639"
    },
    {
      "name": "Go Cyan",
      "value": "#5dc9e2"
    },
    {
      "name": "Java Blue-Gray",
      "value": "#557c9b"
    },
    {
      "name": "JavaScript Yellow",
      "value": "#f9e64f"
    },
    {
      "name": "Mandalorian Blue",
      "value": "#1857a4"
    },
    {
      "name": "Node Green",
      "value": "#215732"
    },
    {
      "name": "React Blue",
      "value": "#00b3e6"
    },
    {
      "name": "Something Different",
      "value": "#832561"
    },
    {
      "name": "Vue Green",
      "value": "#42b883"
    }
  ],
  "php-cs-fixer.executablePath": "${extensionPath}/php-cs-fixer.phar",
  "php-cs-fixer.lastDownload": 1559774512768,
  "php.validate.run": "onType",
  "phpcs.showSources": true,
  "phpcs.executablePath": "./vendor/squizlabs/php_codesniffer/bin/phpcs",
  "workbench.colorCustomizations": {
    "activityBar.background": "#7263b5",
    "activityBar.activeBorder": "#cc9d93",
    "activityBar.foreground": "#e7e7e7",
    "activityBar.inactiveForeground": "#e7e7e799",
    "activityBarBadge.background": "#cc9d93",
    "activityBarBadge.foreground": "#15202b",
    "titleBar.activeBackground": "#594a9b",
    "titleBar.inactiveBackground": "#594a9b99",
    "titleBar.activeForeground": "#e7e7e7",
    "titleBar.inactiveForeground": "#e7e7e799",
    "statusBar.background": "#594a9b",
    "statusBarItem.hoverBackground": "#7263b5",
    "statusBar.foreground": "#e7e7e7"
  },
  "peacock.color": "#594a9b",
  "editor.codeActionsOnSave": {
    "source.fixAll": true
  }
}
```

## Package Management

### Step 5 - Use [package.json-boilerplate](https://github.com/SandroMiguel/package.json-boilerplate)

**ProTip**: Sync Github topics with `package.json` file keywords

## Conventional Commit Messages & Semantic Versioning

### Step 6 - Use [standard-commit](https://github.com/SandroMiguel/standard-commit)

## EditorConfig

### Step 7 - Use [editorconfig-boilerplate](https://github.com/SandroMiguel/editorconfig-boilerplate)

## Linting & Code Formatter

### Step 8 - Use [eslint-config-cecilia](https://github.com/SandroMiguel/eslint-config-cecilia)

## Add other files

### Step 9 - Add [CONTRIBUTING.md](CONTRIBUTING.md)

## Contributing

Want to contribute? All contributions are welcome. Read the [contributing guide](CONTRIBUTING.md).

## Questions

If you have questions tweet me at [@sandro_m_m](https://twitter.com/sandro_m_m) or [open an issue](../../issues/new).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

**~ sharing is caring ~**
