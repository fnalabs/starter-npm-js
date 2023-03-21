# starter(npm)<sup>js</sup>

[![JavaScript Style Guide][style-image]][style-url]

Starter kit for NPM packages.

## Overview

Overall, this starter kit provides the standard boilerplate constructs to develop and build a NPM package. It has some configurable project settings with included \*rc/\*ignore files for:

- [TypeScript](https://www.typescriptlang.org/) ([tsconfig.base.json](./tsconfig.base.json) for the latest JS features)
- [Git](https://git-scm.com/) ([.gitignore](./.gitignore), pretty much the standard Node.js one provided by Github)
- [NPM](https://www.npmjs.com/) ([.npmignore](./.npmignore), pretty much the .gitignore above with a few small changes)

## NPM

Also, it provides an extensible build process integrated with npm scripts. The following is a breakdown of npm scripts provided and how to use them:

- `npm run dev` - to run two nodemon processes automatically based on watched files, one to rebuild application code and the other to run tests.
- `npm run fix` - to automatically apply JS Standard Style to all JS code.
- `npm run lint` - to run JS Standard Style checks.
- `npm run release` - to test and build production code.
- `npm test` - to run unit tests.
- `npm version` - to run production test and build, git commit version update, and publish.
- `npm run tsc` - to build production output.

[LICENSE](./LICENSE)

[style-image]: https://img.shields.io/badge/code_style-standard-brightgreen.svg
[style-url]: https://standardjs.com
