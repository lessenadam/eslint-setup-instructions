# eslint-setup-instructions

## One line install

```
$ npm init -y && yarn add -D eslint prettier eslint-config-prettier eslint-config-airbnb-base && touch .eslintrc.js .prettierrc
```

Get the eslint config and prettier config contents from the directories in this repo


## Reminders / notes

**base eslint packages**
- eslint
- eslint-config-airbnb-base
    - adds the base rules

**prettier extension**
- prettier
- eslint-config-prettier 
    - tuns off conflicts 
- eslint-plugin-prettier
    - adds the rules

**files**
- .eslintrc.js
    - `extends` (applies to "configs" and automatically pulls in the rules)
    - `plugins` (makes certain rules available)
    - `env` and `parserOptions` are for certain default configs, etc
    - `root: true` may be needed to avoid conflicts with eslintrc files higher up the folder chain
    - [full config file docs](https://eslint.org/docs/user-guide/configuring/configuration-files#using-configuration-files)
- .prettierrc

**usage notes**
- changes to the eslint config file will restart the and show up automatically in the editor
- changes to prettier config will not, but you can restart the eslint server as a vs code option
- prettier can be configured to run separately from eslint and to run on save but you may need to reference the [configuration docs](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode#extension-settings)


