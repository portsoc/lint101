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

## Additional rules

This is far from an exhaustive list.  Consider it examples of the kind of useful thing you can find.

* [require let or const instead of var (no-var)](http://eslint.org/docs/rules/no-var)
* [enforce consistent indentation (indent)](http://eslint.org/docs/rules/indent)
* [enforce consistent linebreak style (linebreak-style)](http://eslint.org/docs/rules/linebreak-style)
* [enforce the consistent use of either backticks, double, or single quotes (quotes)](http://eslint.org/docs/rules/quotes)
* [require or disallow semicolons instead of ASI (semi)](http://eslint.org/docs/rules/semi)
* [Disallow Early Use (no-use-before-define)](http://eslint.org/docs/rules/no-use-before-define)

* [Disallow or enforce spaces inside of parentheses (space-in-parens)](http://eslint.org/docs/rules/space-in-parens)
