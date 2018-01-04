# starter(npm)<sup>js</sup>

[![Dependency Status][depstat-image]][depstat-url]
[![Dev Dependency Status][devdepstat-image]][devdepstat-url]
[![JavaScript Style Guide][style-image]][style-url]

Starter kit for NPM packages.

## Overview
Overall, this starter kit provides the standard boilerplate constructs to develop and build a NPM package. It has some configurable project settings with included \*rc/\*ignore files for:
- [Babel](https://babeljs.io/) ([.babelrc](./.babelrc) for import/export syntactic sugar)
- [Git](https://git-scm.com/) ([.gitignore](./.gitignore), pretty much the standard Node.js one provided by Github)
- [NPM](https://www.npmjs.com/) ([.npmignore](./.npmignore), pretty much the .gitignore above with a few small changes)

## NPM
Also, it provides an extensible build process integrated with npm scripts. The following is a breakdown of npm scripts provided and how to use them:
- `npm run build` - to build production output.
- `npm run coverage` - to report test coverage to Codecov.
- `npm run dev` - to run two nodemon processes automatically based on watched files, one to rebuild application code and the other to run tests.
- `npm run fix` - to automatically apply JS Standard Style to all JS code.
- `npm run release` - to test, build, and compress production code.
- `npm test` - to run JS Standard Style checks and unit tests.
- `npm version` - to run production test and build, git commit version update, and publish.

[LICENSE](./LICENSE)

[depstat-image]: https://img.shields.io/david/fnalabs/starter-npm-js.svg
[depstat-url]: https://david-dm.org/fnalabs/starter-npm-js

[devdepstat-image]: https://img.shields.io/david/dev/fnalabs/starter-npm-js.svg
[devdepstat-url]: https://david-dm.org/fnalabs/starter-npm-js?type=dev

[style-image]: https://img.shields.io/badge/code_style-standard-brightgreen.svg
[style-url]: https://standardjs.com
