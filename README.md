ESLint custom rules for Nodeca projects
=======================================

[![Build Status](https://travis-ci.org/nodeca/eslint-plugin-nodeca.svg?branch=master)](https://travis-ci.org/nodeca/eslint-plugin-nodeca)
[![NPM version](https://img.shields.io/npm/v/eslint-plugin-nodeca.svg)](https://www.npmjs.org/package/eslint-plugin-nodeca)

Playground with [ESLint](http://eslint.org/) rules, used in nodeca projects.

- __indent__ - check code identation. The same as existed in jshint, until was ripped off.
- __no-async-aliases__ - warn on deprecated methods in `async` module.
- __no-lodash-aliases__ - warn on deprecated methods in `lodash` module.
- __no-wire-anonymous__ - prohibit anon functions in event handlers of nodeca wire mediator.

Indent rule
-----------

Params:

- __indent type__ - 'tabs' / 'spaces' (default - spaces)
- __indent size__ - 2 (default)

Config example (yaml):

```yaml
# acivate plugin

plugins:
  - nodeca

# enable rules

rules:
  nodeca/indent: [ 2, spaces, 2 ]

  # If you are ok with defaults:
  #
  # nodeca/indent: 2
```


Authors
-------

- Kirill Efimov [github/Kirill89](https://github.com/Kirill89)
- Vitaly Puzrin [github/puzrin](https://github.com/puzrin)


License
-------

[MIT](https://github.com/nodeca/eslint-plugin-nodeca/blob/master/LICENSE)