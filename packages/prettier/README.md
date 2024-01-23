# @851-labs/prettier

## Installation

> [!NOTE]  
> Prettier is a peer-dependency of this package and should also be installed.

```bash
pnpm i -D prettier @851-labs/prettier
```

## Usage

To use the shared Prettier config, set the following in `package.json`.

```json
{
  "prettier": "@851-labs/prettier"
}
```

If you need to extend/override the shared config, create a `prettier.config.mjs` file and destructure the shared config.

> [!NOTE]  
> Prettier does not offer a native way to extend the configuration. See [sharing configuration](https://prettier.io/docs/en/configuration.html#sharing-configurations) docs and [#7763](https://github.com/prettier/prettier/issues/7763) issue for more info.

```mjs
import defaultConfig from "@851-labs/prettier";

/** @type {import("prettier").Config} */
const config = {
  ...defaultConfig,
  tailwindConfig: "./tailwind.config.ts",
};

export default config;
```

## Scripts

```json
"scripts": {
  "format": "prettier --check . --ignore-path .gitignore",
  "format:fix": "pnpm format --write"
}
```

## License

MPL-2.0
