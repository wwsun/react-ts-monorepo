# react-ts-monorepo

a monorepo example with react and typescript

## How to setup

```bash
# install dependencies
yarn

# build
yarn build

# publish
yarn pub
```

## FAQ

### Why should setting `include` and `outDir` for each package

`include` and `outDir` cannot be hoisted in the root config, because they are reserved relatively to the config they are in.

see https://github.com/microsoft/TypeScript/issues/29172#issuecomment-450966221

### Publish packages with a scope, e.g. `@nupt/foo`

setup `lerna.json`

```json
  "publishConfig": {
    "access": "public"
  }
```
