<p align="center">
  <img src="./meta/check.png" width="700" alt="codechecks.io">
  <h3 align="center">Type Coverage Watcher</h3>
  <p align="center">Track missing type coverage in TypeScript projects to ensure type safety</p>

  <p align="center">
    <a href="https://circleci.com/gh/codechecks/type-coverage-watcher"><img alt="Build Status" src="https://circleci.com/gh/codechecks/type-coverage-watcher/tree/master.svg?style=svg"></a>
    <a href="/package.json"><img alt="Software License" src="https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square"></a>
  </p>
</p>

## Install

```sh
npm add --save-dev @codechecks/type-coverage-watcher
```

or

```sh
yarn add --dev @codechecks/type-coverage-watcher
```

## Usage

Add to your `codechecks.json` file:

<!-- prettier-ignore -->
```json5
{
  "checks": [
    {
      "name": "type-coverage-watcher"
    }

    // ...
  ]
}
```

Under the hood it uses [type-coverage](https://github.com/plantain-00/type-coverage) package.

## API

### typeCoverageWatcher(options: Options): Promise\<void>

#### options

```typescript
interface Options {
  tsconfigPath?: string;
}
```

##### tsconfigPath

optional `string`<br>\
Default: `tsconfig.json`<br>\
Path to typescript project configuration

## Contributing

All contributions are welcomed. Read more in [CONTRIBUTING.md](./CONTRIBUTING.md)

## Licence

MIT @ [codechecks.io](https://codechecks.io)
