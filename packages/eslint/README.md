# @851-labs/eslint-config

## Installation

> [!NOTE]  
> ESlint is a peer-dependency of this package and should also be installed.

```bash
pnpm i -D eslint @851-labs/eslint-config
```

## Usage

The ESLint package is designed to be composable. To use the shared ESLint config, pick the configs that suit your needs and set the following in `package.json`.

```json
"eslintConfig": {
  "root": true,
  "extends": [
    "@851-labs/eslint/base",
    "@851-labs/eslint/nextjs",
    "@851-labs/eslint/react"
  ]
}
```

## Scripts

```json
"scripts": {
  "lint": "eslint .",
  "lint:fix": "pnpm format --fix"
}
```

## License

MPL-2.0
