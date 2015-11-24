# npm-module-checklist

> Steps to check when starting, working and publishing a module to NPM

- [ ] run linting and unit tests on each commit locally. [pre-git][pre-git], [ghooks][ghooks]

- [ ] validate commit message using [pre-git][pre-git] or [commitizen][commitizen]. This
enables other tools, like intelligent release notes.

- [ ] setup continuous integration server, like [TravisCI][travis] or [CircleCI][circle].

- [ ] check module published size and white list only necessary files, [tutorial][module size]

- [ ] setup [semantic-release][semantic-release] to automate publishing
and avoid breaking [semver][semver]. This is [important][semver important],
but is currently [broken][broken semver] in too many projects. Even this checklist is using semver!

- [ ] avoid surprizes by using exact versions of the top level dependencies. 
Use [save-exact][save-exact] NPM setting and [exact-semver][exact-semver] to enforce it.

- [ ] catch missing or invalid `package.json` values using [grunt-nice-package][grunt-nice-package] 
or [fixpack][fixpack]

[pre-git]: https://github.com/bahmutov/pre-git
[ghooks]: https://www.npmjs.com/package/ghooks

[commitizen]: https://www.npmjs.com/package/commitizen

[travis]: https://travis-ci.org/
[circle]: https://circleci.com/

[module size]: http://glebbahmutov.com/blog/smaller-published-NPM-modules/

[semantic-release]: https://github.com/semantic-release/semantic-release
[semver]: http://semver.org/
[semver important]: https://medium.com/javascript-scene/software-versions-are-broken-3d2dc0da0783#.h96ppopx3
[broken semver]: https://www.youtube.com/watch?v=tc2UgG5L7WM

[save-exact]: https://docs.npmjs.com/misc/config#save-exact
[exact-semver]: https://github.com/bahmutov/exact-semver

[grunt-nice-package]: https://github.com/bahmutov/grunt-nice-package
[fixpack]: https://github.com/henrikjoreteg/fixpack

### Small print

Author: Gleb Bahmutov &copy; 2015

* [@bahmutov](https://twitter.com/bahmutov)
* [glebbahmutov.com](http://glebbahmutov.com)
* [blog](http://glebbahmutov.com/blog/)

License: MIT - do anything with the code, but don't blame me if it does not work.

Spread the word: tweet, star on github, etc.

Support: if you find any problems with this module, email / tweet /
[open issue](https://github.com/bahmutov/npm-module-checklist/issues) on Github
