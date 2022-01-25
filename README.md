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
    "peacock.color": "#f5027b",
    "workbench.colorCustomizations": {
        "activityBar.background": "#fd2d95",
        "activityBar.activeBackground": "#fd2d95",
        "activityBar.activeBorder": "#70dd02",
        "activityBar.foreground": "#e7e7e7",
        "activityBar.inactiveForeground": "#e7e7e799",
        "activityBarBadge.background": "#70dd02",
        "activityBarBadge.foreground": "#15202b",
        "titleBar.activeBackground": "#f5027b",
        "titleBar.inactiveBackground": "#f5027b99",
        "titleBar.activeForeground": "#e7e7e7",
        "titleBar.inactiveForeground": "#e7e7e799",
        "statusBar.background": "#f5027b",
        "statusBarItem.hoverBackground": "#fd2d95",
        "statusBar.foreground": "#e7e7e7"
    }
}
```

**User** settings

`~/.config/Code/User/settings.json`

```
{
  "[html]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
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
  "editor.codeActionsOnSave": {
    "source.fixAll": true
  },
  "editor.fontFamily": "'Ubuntu Mono', monospace",
  "editor.fontSize": 17,
  "editor.formatOnSave": true,
  "editor.suggestSelection": "first",
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
  "eslint.alwaysShowStatus": true,
  "eslint.debug": true,
  "explorer.confirmDelete": false,
  "explorer.confirmDragAndDrop": false,
  "gitlens.codeLens.enabled": false,
  "javascript.preferences.importModuleSpecifier": "non-relative",
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
  "php.validate.run": "onType",
  "phpcs.showSources": true,
  "phpcs.executablePath": "/home/sandro/.composer/vendor/bin/phpcs",
  "terminal.integrated.copyOnSelection": true,
  "terminal.integrated.cursorBlinking": true,
  "terminal.integrated.cursorStyle": "line",
  "terminal.integrated.drawBoldTextInBrightColors": false,
  "terminal.integrated.fontFamily": "'Ubuntu Mono', monospace",
  "terminal.integrated.fontSize": 15,
  "terminal.integrated.rendererType": "dom",
  "typescript.tsserver.log": "verbose",
  "vsicons.dontShowNewVersionMessage": true,
  "vsintellicode.modify.editor.suggestSelection": "automaticallyOverrodeDefaultValue",
  "window.zoomLevel": 0
}
```

## Contributing

Want to contribute? All contributions are welcome. Read the [contributing guide](CONTRIBUTING.md).

## Questions

If you have questions tweet me at [@sandro_m_m](https://twitter.com/sandro_m_m) or [open an issue](../../issues/new).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

**~ sharing is caring ~**
