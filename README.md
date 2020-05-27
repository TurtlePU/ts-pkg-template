# ts-pkg-template

Template for writing node packages in TypeScript.

To check out the sample package:

```
npm i ts-pkg-template
```

To install dependencies, run `npm i`.

Before publishing, don't forget to add `"name"` to `package.json`.

## Tips

* add homepage / repo link to `package.json` as well
* set Git hook to run `npm run tests && npm run lint` before commit
* optimize dependencies: you may not need all of them
* tweak `.eslintrc` to enforce desired codestyle

## Dev Dependencies overview

* `mocha`, `chai`, `nyc` &mdash; test framework, assertion lib, test coverage
* `eslint` &mdash; to enforce codestyle & find some semantic errors
* `@zerollup/ts-transform-paths`, `ttypescript` &mdash; to replace absolute paths with relative in build
* `tsconfig-paths` &mdash; same as before, but in tests
* `ts-node` &mdash; to run tests
* `rimraf` &mdash; to remove `dist/` on any OS