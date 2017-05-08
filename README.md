# js-npm-starter
Starter kit for NPM packages.

## Overview
Overall, this starter kit provides the standard boilerplate constructs to build an NPM package. It provides ES2015+ through Babel with both published code and test code. It has configurable project settings rather than a heavy handed approach with included \*rc/\*ignore files for:
- [Babel](https://babeljs.io/) ([.babelrc](./.babelrc) for development, see build config for production code)
- [ESLint](http://eslint.org/) ([.eslintrc](./.eslintrc))
- [JSBeautify](http://jsbeautifier.org/) ([.jsbeautifyrc](./.jsbeautifyrc) also includes beautify settings for HTML and CSS)
- [Git](https://git-scm.com/) ([.gitignore](./.gitignore), pretty much the standard Node.js one provided by Github)
- [NPM](https://www.npmjs.com/) ([.npmignore](./.npmignore), pretty much the .gitignore above with a few small changes)

Also, it provides an extensible build process integrated with npm scripts and Gulp under the hood when necessary to simplify build needs rather than rolling your own custom scripts. The [gulpfile](./gulpfile.babel.js), written in ES2015+, is paired with a [build config](./conf/buildConfig.json) to help manage the complexity that build processes can sometimes require. The following is a breakdown of npm scripts provided and how to use them:
- `npm run build` A basic wrapper to build production output. Can be run independently but is included in some of the following scripts.
- `npm run build:dev` A basic wrapper to run a Gulp development process. This is typically used independently.
- `npm test` A basic wrapper to run the only linting and tests and nothing else.
- `npm version <version_bump>` This invokes a multi-step process to run a production build, commit, and publish the [version](https://docs.npmjs.com/cli/version) of your npm package.
- `npm run version:pre --increment=<version_bump> [--preid=<prerelease_tag>]` A wrapper around `npm version ...`, this allows the injection of [prerelease tags](https://www.npmjs.com/package/semver#prerelease-tags) to your npm package. This provides an even greater degree on semantic versions beyond the default provided by `npm version ...` above.

- **NOTE:** This requires the `gulp-cli` and `semver` packages to be installed globally in order to work.

## Guarantees
[There are none](./LICENSE).
