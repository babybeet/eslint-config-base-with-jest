# eslint-config-base-with-jest [![](https://circleci.com/gh/babybeet/eslint-config-base-with-jest.svg?style=svg&logo=appveyor)](https://app.circleci.com/pipelines/github/babybeet/eslint-config-base-with-jest?branch=main)

[Base ESLint rules](https://github.com/babybeet/eslint-config-base) with support for linting Jest test files.

## Installation

- `npm`
  ```
  npm i -S @babybeet/eslint-config-base-with-jest
  ```
- `pnpm`
  ```
  pnpm i -S @babybeet/eslint-config-base-with-jest
  ```
- `yarn`

  ```
  yarn add @babybeet/eslint-config-base-with-jest
  ```

## Setting up

In your `.eslintrc.json` file, add the followings:

```json
{
  "$schema": "https://json.schemastore.org/eslintrc.json",
  "root": true,
  "ignorePatterns": ["!**/*"],
  "parserOptions": {
    "ecmaVersion": "latest",
    "sourceType": "module"
  },
  // It's recommended to use an override to not globally change your ESLint configuration.
  "overrides": [
    {
      "files": ["*.ts"],
      "extends": ["@babybeet/eslint-config-base-with-jest"],
      "rules": {
        // Add your own rule overrides if desired.
      }
    }
  ]
}
```
