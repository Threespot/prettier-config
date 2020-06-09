# prettier-config
Threespot’s shareable config for [Prettier](https://prettier.io/)

## Install: 

[Install Prettier if you haven't already](https://prettier.io/docs/en/install.html).

Using `yarn`:

```bash
$ yarn add --dev @threespot/prettier-config
```

Using `npm`:
```bash
$ npm install --save-dev @threespot/prettier-config
```

To enable the rules you will have to add the configuration file in your `package.json` as a key/value pair. 

```jsonc
 {	
   "name": "my-project",
	 "version": "1.0.0",
   "prettier": "@threespot/prettier-config",
   ...
 }
```
If you don't want to add it to your `package.json` file, visit [prettier's documentation on shareable configuration](https://prettier.io/docs/en/configuration.html#sharing-configurations) for other options

## Integrating Prettier to your editor for onSave capabilities
Instead of using prettier's CLI to format your code, you can integrate prettier into your text editor to format your code on save. (recommended)

To integrate you can find your [specific editor on prettier's website](https://prettier.io/docs/en/editors.html). 

## Batch format project

1. Check your git history to ensure that it is clean
2. Install `@threespot/prettier-config`
3. Make sure you have the files you want to whitelist in your `.prettierignore` file 
4. Run Prettier via CLI either:
  - Add this script to your `package.json` file: `prettier-format-all: npx prettier --config-precedence prefer-file --write "**/*.js"`
    - You can now run a batch update using `yarn run prettier-format-all` or `npm run prettier-format-all` 
  - Alternativel, you can run `npx prettier --config-precedence prefer-file --write "**/*.js"`
5. Commit all the formatted files into a single commit