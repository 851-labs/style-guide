# @851-labs/eslint

## Installation

> [!NOTE]  
> Eslint is a peer-dependency of this package and should also be installed.

```bash
pnpm i -D eslint @types/eslint @851-labs/eslint
```

## Usage

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
  "lint": "",
  "lint:fix": "pnpm format --fix"
}
```

## License

MPL-2.0
