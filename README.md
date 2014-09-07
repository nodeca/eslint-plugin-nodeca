ESLint custom rules for Nodeca projects
---------------------------------------

[![Build Status](https://travis-ci.org/nodeca/eslint-plugin-nodeca.svg?branch=master)](https://travis-ci.org/nodeca/eslint-plugin-nodeca)
[![NPM version](https://img.shields.io/npm/v/eslint-plugin-nodeca.svg)](https://www.npmjs.org/package/eslint-plugin-nodeca)

Playground with eslint rules, used in nodeca projects.

- __indent__ - check code identation. The same as existed in jshint, until was ripped off.
- __no-async-aliases__ - warn on deprecated methods in `async` module.
- __no-lodash-aliases__ - warn on deprecated methods in `lodash` module.
- __no-wire-anonymous__ - prohibit anon functions in event handlers of nodeca wire mediator.

Indent rule params:

- indent type - 'tabs' / 'spaces'
- indent size - 2

Config example (yaml):

```yaml
# acivate plugin

plugins:
  - nodeca

# enable rules

rules:
  nodeca/indent:                 [2, spaces, 2]
  nodeca/no-lodash-aliases:      2
  nodeca/no-async-aliases:       2
  nodeca/no-wire-anonymous:      1
```


Authors
-------

- Kirill Efimov [github/Kirill89](https://github.com/Kirill89)
- Vitaly Puzrin [github/puzrin](https://github.com/puzrin)


License
-------

[MIT](https://github.com/nodeca/eslint-plugin-nodeca/blob/master/LICENSE)