# ts-pkg-template

Template for writing node packages in TypeScript.

To install dependencies, run `npm i`.

Before publishing, don't forget to add `"name"` to `package.json`.

## Example

Working example can be installed with

```
npm i @turtlepu/say-hi
```

## .eslintrc

Also available as a gist [here](https://gist.github.com/TurtlePU/abf7f08a7ec32a17e62329e7fa351b06)

## Tips

* optimize dependencies: you might not need all of them
* add homepage / repo link to `package.json` as well
* set Git hook to run `npm run lint` before commit
* `npm run lint-fix` to auto fix some lint errors
* tweak `.eslintrc` to enforce desired codestyle

## Dev Dependencies overview

* `mocha`, `chai`, `nyc` &mdash; test framework, assertion lib, test coverage
* `eslint` &mdash; to enforce codestyle & find some semantic errors
* `@zerollup/ts-transform-paths`, `ttypescript` &mdash; to replace absolute paths with relative in build
* `tsconfig-paths` &mdash; same as before, but in tests
* `ts-node` &mdash; to run tests
* `rimraf` &mdash; to remove `dist/` on any OS