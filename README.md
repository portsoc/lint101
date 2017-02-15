# lint me

An example of linter use.

## Install and Run

```shell
git clone https://github.com/portsoc/ws_lint.git
cd ws_lint
npm install
npm test
```

Installing and running should highlight 14 errors.  These are identified using the [ESLinter recommended rules](http://eslint.org/docs/rules/), as well as extras that are added in the `eslintConfig` element in `package.json`

## Installing linters in Atom
There are several linter options in atom; for example, the [linter](https://atom.io/packages/linter) package is an extensible base-linter that supports [eslint](https://atom.io/packages/linter-eslint) and [many other linting tools](http://atomlinter.github.io/)

```shell
apm install linter
apm install linter-eslint
```

Once installed, the errors that are reported by `npm test` should appear alongside the code in your editor, giving you edit-time feedback.

## Additional rules

This is far from an exhaustive list.  Consider it examples of the kind of useful thing you can find.

* [require let or const instead of var (no-var)](http://eslint.org/docs/rules/no-var)
* [enforce consistent indentation (indent)](http://eslint.org/docs/rules/indent)
* [enforce consistent linebreak style (linebreak-style)](http://eslint.org/docs/rules/linebreak-style)
* [enforce the consistent use of either backticks, double, or single quotes (quotes)](http://eslint.org/docs/rules/quotes)
* [require or disallow semicolons instead of ASI (semi)](http://eslint.org/docs/rules/semi)
* [Disallow Early Use (no-use-before-define)](http://eslint.org/docs/rules/no-use-before-define)

* [Disallow or enforce spaces inside of parentheses (space-in-parens)](http://eslint.org/docs/rules/space-in-parens)

## Additional Styles

There are many different rule sets that can be used as a base for your linting.  We have included the Google style-guide in the 'package.json' dev-dependenceies, and also Doug Crockford's stricter more disciplinarian rules, for reference if you also enjoy his book [JavaScript; The Good Parts](http://amzn.to/2kJg9cj).

Only one set of base rules is allowed at a time so remove the underscore from one of these at a time (in `package.json`).

```json
  "extends": "eslint:recommended",
  "_extends": "crockford",
  "_extends": "google",
```
