# prettier-config
Threespot’s Prettier config settings

## Usage:
To enable the prettier's configuration, make sure you [install prettier](https://prettier.io/docs/en/install.html) as a `devDependency` in your `package.json` file. 

Once prettier is installed, drop `.prettierrc.js` in your project's root directory, and integrate it to your editor of choice. 

## Editor Integration 

Instead of using prettier's CLI api to format your JavaScript, you can integrate prettier into your text editor. 

### VS Code
1. Install Prettier extension via vscode
2. Reload the editor
3. In your user settings, add `editor.formatOnSave: true`

For more information on [VS Code prettier's extension](https://github.com/prettier/prettier-vscode). 

If you are not using VS code, visit [Prettier's editor integration](https://prettier.io/docs/en/editors.html) for instructions on your editor. 