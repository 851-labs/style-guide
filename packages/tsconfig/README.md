# @851-labs/tsconfig

## Installation

```bash
pnpm i -D @851-labs/tsconfig
```

## Usage

| Name   | TypeScript Config                |
| ------ | -------------------------------- |
| base   | `@851-labs/tsconfig/base.json`   |
| nextjs | `@851-labs/tsconfig/nextjs.json` |
| node   | `@851-labs/tsconfig/node.json`   |

To use the shared TypeScript config, pick your desired config and set the following in `tsconfig.json`.

```json
{
  "extends": "@851-labs/tsconfig/<name>.json"
}
```

## License

MPL-2.0
