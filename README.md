# prettier-config
Threespot’s shareable config for [Prettier](https://prettier.io/)

## Install

Using `yarn`:

```bash
$ yarn add --dev @threespot/prettier-config
```

Using `npm`:
```bash
$ npm install --save-dev @threespot/prettier-config
```

To enable rules you will have to add the key/value pair `"prettier": "@threespot/prettier-config"` to your root level `package.json` file.

If you don't want to add it to your `package.json` file, visit [prettier's documentation on shareable configuration](https://prettier.io/docs/en/configuration.html#sharing-configurations) for other options

## Integrating Prettier to your editor for onSave capabilities
Instead of using prettier's CLI to format your code, you can integrate prettier into your text editor to format your code on save. (recommended)

[Instructions for integrating prettier to your specific text editor.](https://prettier.io/docs/en/editors.html)

## Batch format via CLI

To use the CLI batch script you will have to [install prettier](https://prettier.io/docs/en/install.html) as a devDependency.

Note: The batching process formats EVERYTHING except for JavaScript files located in node_modules. We recommend whitelisting the files you want prettier to format via `.prettierignore`. You can view an example of the whitelisting pattern in this repo: `.example.prettierignore`. 

1. Check your git history to ensure that it is clean
2. Install `@threespot/prettier-config`
3. Whitelist the files you want the format to alter in your `.prettierignore` file.
4. Add this script to your `package.json`:

    `prettier-format-all: npx prettier --config-precedence prefer-file --write \"**/*.js\`
    
    Alternatively you can run: `yarn run prettier-format-all` or `npm run prettier-format-all` in the CLI.

5. Commit all the formatted files into a single commit