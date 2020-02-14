# prettier-config
Threespot’s shareable config for [Prettier](https://prettier.io/)

## Install: 

To install Prettier and prettier-config:

```bash
$ yarn add prettier-config prettier --dev
```

If you already installed prettier:

```bash
$ yarn add prettier-config --dev
```

## Usage:
To enable these rules reference it in your `package.json`:

```jsonc
 {
    // ...
    "prettier": "prettier-config" 
 }
```

If you don't want to reference it via `package.json`, visit [prettier's documentation on shareable configuration](https://prettier.io/docs/en/configuration.html#sharing-configurations) to use one of their other options.

## Editor Integration 

Instead of using prettier's CLI api to format your JavaScript, you can integrate prettier into your text editor. 

### VS Code
1. Install Prettier extension via vscode
2. Reload the editor
3. In your user settings, add `editor.formatOnSave: true`

For more information on [VS Code prettier's extension](https://github.com/prettier/prettier-vscode). 

If you are not using VS code, visit [Prettier's editor integration](https://prettier.io/docs/en/editors.html) for instructions on your editor. 