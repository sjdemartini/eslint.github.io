---
title: List of available rules
layout: doc
---
<!-- Note: No pull requests accepted for this file. See README.md in the root directory for details. -->

# Rules

Rules in ESLint are divided into several categories to help you better understand their value. All rules are disabled by default. ESLint recommends some rules to catch common problems, and you can use these recommended rules by including `extends: "eslint:recommended"` in your configuration file. The rules that will be enabled when you inherit from `eslint:recommended` are indicated below as "(recommended)". For more information on how to configure rules and use `extends`, please see the [configuration documentation](../user-guide/configuring).

Some rules are fixable using the `--fix` command line flag. Those rules are marked as "(fixable)" below. Currently these fixes are mostly limited only to whitespace fixes.

## Possible Errors

The following rules point out areas where you might have made mistakes.

* [comma-dangle](comma-dangle): require or disallow trailing commas (recommended)
* [no-cond-assign](no-cond-assign): disallow assignment operators in conditional expressions (recommended)
* [no-console](no-console): disallow the use of `console` (recommended)
* [no-constant-condition](no-constant-condition): disallow constant expressions in conditions (recommended)
* [no-control-regex](no-control-regex): disallow control characters in regular expressions (recommended)
* [no-debugger](no-debugger): disallow the use of `debugger` (recommended)
* [no-dupe-args](no-dupe-args): disallow duplicate arguments in `function` definitions (recommended)
* [no-dupe-keys](no-dupe-keys): disallow duplicate keys in object literals (recommended)
* [no-duplicate-case](no-duplicate-case): disallow duplicate case labels (recommended)
* [no-empty](no-empty): disallow empty block statements (recommended)
* [no-empty-character-class](no-empty-character-class): disallow empty character classes in regular expressions (recommended)
* [no-ex-assign](no-ex-assign): disallow reassigning exceptions in `catch` clauses (recommended)
* [no-extra-boolean-cast](no-extra-boolean-cast): disallow unnecessary boolean casts (recommended)
* [no-extra-parens](no-extra-parens): disallow unnecessary parentheses
* [no-extra-semi](no-extra-semi): disallow unnecessary semicolons (recommended) (fixable)
* [no-func-assign](no-func-assign): disallow reassigning `function` declarations (recommended)
* [no-inner-declarations](no-inner-declarations): disallow `function` or `var` declarations in nested blocks (recommended)
* [no-invalid-regexp](no-invalid-regexp): disallow invalid regular expression strings in `RegExp` constructors (recommended)
* [no-irregular-whitespace](no-irregular-whitespace): disallow irregular whitespace outside of strings and comments (recommended)
* [no-negated-in-lhs](no-negated-in-lhs): disallow negating the left operand in `in` expressions (recommended)
* [no-obj-calls](no-obj-calls): disallow calling global object properties as functions (recommended)
* [no-regex-spaces](no-regex-spaces): disallow multiple spaces in regular expression literals (recommended)
* [no-sparse-arrays](no-sparse-arrays): disallow sparse arrays (recommended)
* [no-unexpected-multiline](no-unexpected-multiline): disallow confusing multiline expressions (recommended)
* [no-unreachable](no-unreachable): disallow unreachable code after `return`, `throw`, `continue`, and `break` statements (recommended)
* [use-isnan](use-isnan): require calls to `isNaN()` when checking for `NaN` (recommended)
* [valid-jsdoc](valid-jsdoc): enforce valid JSDoc comments
* [valid-typeof](valid-typeof): enforce comparing `typeof` expressions against valid strings (recommended)

## Best Practices

These are rules designed to prevent you from making mistakes. They either prescribe a better way of doing something or help you avoid footguns.

* [accessor-pairs](accessor-pairs): enforce getter and setter pairs in objects
* [array-callback-return](array-callback-return): enforce `return` statements in callbacks of array methods
* [block-scoped-var](block-scoped-var): enforce the use of variables within the scope they are defined
* [complexity](complexity): enforce a maximum cyclomatic complexity allowed in a program
* [consistent-return](consistent-return): require `return` statements to either always or never specify values
* [curly](curly): enforce consistent brace style for all control statements
* [default-case](default-case): require `default` cases in `switch` statements
* [dot-location](dot-location): enforce consistent newlines before and after dots
* [dot-notation](dot-notation): enforce dot notation whenever possible
* [eqeqeq](eqeqeq): require the use of `===` and `!==`
* [guard-for-in](guard-for-in): require `for-in` loops to include an `if` statement
* [no-alert](no-alert): disallow the use of `alert`, `confirm`, and `prompt`
* [no-caller](no-caller): disallow the use of `arguments.caller` or `arguments.callee`
* [no-case-declarations](no-case-declarations): disallow lexical declarations in case clauses (recommended)
* [no-div-regex](no-div-regex): disallow division operators explicitly at the beginning of regular expressions
* [no-else-return](no-else-return): disallow `else` blocks after `return` statements in `if` statements
* [no-empty-function](no-empty-function): disallow empty functions
* [no-empty-pattern](no-empty-pattern): disallow empty destructuring patterns (recommended)
* [no-eq-null](no-eq-null): disallow `null` comparisons without type-checking operators
* [no-eval](no-eval): disallow the use of `eval()`
* [no-extend-native](no-extend-native): disallow extending native types
* [no-extra-bind](no-extra-bind): disallow unnecessary calls to `.bind()`
* [no-extra-label](no-extra-label): disallow unnecessary labels
* [no-fallthrough](no-fallthrough): disallow fallthrough of `case` statements (recommended)
* [no-floating-decimal](no-floating-decimal): disallow leading or trailing decimal points in numeric literals
* [no-implicit-coercion](no-implicit-coercion): disallow shorthand type conversions
* [no-implicit-globals](no-implicit-globals): disallow `var` and named `function` declarations in the global scope
* [no-implied-eval](no-implied-eval): disallow the use of `eval()`-like methods
* [no-invalid-this](no-invalid-this): disallow `this` keywords outside of classes or class-like objects
* [no-iterator](no-iterator): disallow the use of the `__iterator__` property
* [no-labels](no-labels): disallow labeled statements
* [no-lone-blocks](no-lone-blocks): disallow unnecessary nested blocks
* [no-loop-func](no-loop-func): disallow `function` declarations and expressions inside loop statements
* [no-magic-numbers](no-magic-numbers): disallow magic numbers
* [no-multi-spaces](no-multi-spaces): disallow multiple spaces (fixable)
* [no-multi-str](no-multi-str): disallow multiline strings
* [no-native-reassign](no-native-reassign): disallow reassigning native objects
* [no-new](no-new): disallow `new` operators outside of assignments or comparisons
* [no-new-func](no-new-func): disallow `new` operators with the `Function` object
* [no-new-wrappers](no-new-wrappers): disallow `new` operators with the `String`, `Number`, and `Boolean` objects
* [no-octal](no-octal): disallow octal literals (recommended)
* [no-octal-escape](no-octal-escape): disallow octal escape sequences in string literals
* [no-param-reassign](no-param-reassign): disallow reassigning `function` parameters
* [no-proto](no-proto): disallow the use of the `__proto__` property
* [no-redeclare](no-redeclare): disallow `var` redeclaration (recommended)
* [no-return-assign](no-return-assign): disallow assignment operators in `return` statements
* [no-script-url](no-script-url): disallow `javascript:` urls
* [no-self-assign](no-self-assign): disallow assignments where both sides are exactly the same (recommended)
* [no-self-compare](no-self-compare): disallow comparisons where both sides are exactly the same
* [no-sequences](no-sequences): disallow comma operators
* [no-throw-literal](no-throw-literal): disallow throwing literals as exceptions
* [no-unmodified-loop-condition](no-unmodified-loop-condition): disallow unmodified loop conditions
* [no-unused-expressions](no-unused-expressions): disallow unused expressions
* [no-unused-labels](no-unused-labels): disallow unused labels (recommended)
* [no-useless-call](no-useless-call): disallow unnecessary calls to `.call()` and `.apply()`
* [no-useless-concat](no-useless-concat): disallow unnecessary concatenation of literals or template literals
* [no-useless-escape](no-useless-escape): disallow unnecessary escape characters
* [no-void](no-void): disallow `void` operators
* [no-warning-comments](no-warning-comments): disallow specified warning terms in comments
* [no-with](no-with): disallow `with` statements
* [radix](radix): enforce the consistent use of the radix argument when using `parseInt()`
* [vars-on-top](vars-on-top): require `var` declarations be placed at the top of their containing scope
* [wrap-iife](wrap-iife): require parentheses around immediate `function` invocations
* [yoda](yoda): require or disallow "Yoda" conditions

## Strict Mode

These rules relate to using strict mode and strict mode directives.

* [strict](strict): require or disallow strict mode directives

## Variables

These rules have to do with variable declarations.

* [init-declarations](init-declarations): require or disallow initialization in `var` declarations
* [no-catch-shadow](no-catch-shadow): disallow `catch` clause parameters from shadowing variables in the outer scope
* [no-delete-var](no-delete-var): disallow deleting variables (recommended)
* [no-label-var](no-label-var): disallow labels that share a name with a variable
* [no-restricted-globals](no-restricted-globals): disallow specified global variables
* [no-shadow](no-shadow): disallow `var` declarations from shadowing variables in the outer scope
* [no-shadow-restricted-names](no-shadow-restricted-names): disallow identifiers from shadowing restricted names
* [no-undef](no-undef): disallow the use of undeclared variables unless mentioned in `/*global */` comments (recommended)
* [no-undef-init](no-undef-init): disallow initializing variables to `undefined`
* [no-undefined](no-undefined): disallow the use of `undefined` as an identifier
* [no-unused-vars](no-unused-vars): disallow unused variables (recommended)
* [no-use-before-define](no-use-before-define): disallow the use of variables before they are defined

## Node.js and CommonJS

These rules are specific to JavaScript running on Node.js or using CommonJS in the browser.

* [callback-return](callback-return): require `return` statements after callbacks
* [global-require](global-require): require `require()` calls to be placed at top-level module scope
* [handle-callback-err](handle-callback-err): require error handling in callbacks
* [no-mixed-requires](no-mixed-requires): disallow `require` calls to be mixed with regular `var` declarations
* [no-new-require](no-new-require): disallow `new` operators with calls to `require`
* [no-path-concat](no-path-concat): disallow string concatenation with `__dirname` and `__filename`
* [no-process-env](no-process-env): disallow the use of `process.env`
* [no-process-exit](no-process-exit): disallow the use of `process.exit()`
* [no-restricted-modules](no-restricted-modules): disallow specified modules when loaded by `require`
* [no-sync](no-sync): disallow synchronous methods

## Stylistic Issues

These rules are purely matters of style and are quite subjective.

* [array-bracket-spacing](array-bracket-spacing): enforce consistent spacing inside array brackets (fixable)
* [block-spacing](block-spacing): enforce consistent spacing inside single-line blocks (fixable)
* [brace-style](brace-style): enforce consistent brace style for blocks
* [camelcase](camelcase): enforce camelcase naming convention
* [comma-spacing](comma-spacing): enforce consistent spacing before and after commas (fixable)
* [comma-style](comma-style): enforce consistent comma style
* [computed-property-spacing](computed-property-spacing): enforce consistent spacing inside computed property brackets (fixable)
* [consistent-this](consistent-this): enforce consistent naming when capturing the current execution context
* [eol-last](eol-last): enforce at least one newline at the end of files (fixable)
* [func-names](func-names): enforce named `function` expressions
* [func-style](func-style): enforce the consistent use of either `function` declarations or expressions
* [id-blacklist](id-blacklist): disallow specified identifiers
* [id-length](id-length): enforce minimum and maximum identifier lengths
* [id-match](id-match): require identifiers to match a specified regular expression
* [indent](indent): enforce consistent indentation (fixable)
* [jsx-quotes](jsx-quotes): enforce the consistent use of either double or single quotes in JSX attributes (fixable)
* [key-spacing](key-spacing): enforce consistent spacing between keys and values in object literal properties
* [keyword-spacing](keyword-spacing): enforce consistent spacing before and after keywords (fixable)
* [linebreak-style](linebreak-style): enforce consistent linebreak style (fixable)
* [lines-around-comment](lines-around-comment): require empty lines around comments
* [max-depth](max-depth): enforce a maximum depth that blocks can be nested
* [max-len](max-len): enforce a maximum line length
* [max-nested-callbacks](max-nested-callbacks): enforce a maximum depth that callbacks can be nested
* [max-params](max-params): enforce a maximum number of parameters in `function` definitions
* [max-statements](max-statements): enforce a maximum number of statements allowed in `function` blocks
* [max-statements-per-line](max-statements-per-line): enforce a maximum number of statements allowed per line
* [new-cap](new-cap): require constructor `function` names to begin with a capital letter
* [new-parens](new-parens): require parentheses when invoking a constructor with no arguments
* [newline-after-var](newline-after-var): require or disallow an empty line after `var` declarations
* [newline-before-return](newline-before-return): require an empty line before `return` statements
* [newline-per-chained-call](newline-per-chained-call): require a newline after each call in a method chain
* [no-array-constructor](no-array-constructor): disallow `Array` constructors
* [no-bitwise](no-bitwise): disallow bitwise operators
* [no-continue](no-continue): disallow `continue` statements
* [no-inline-comments](no-inline-comments): disallow inline comments after code
* [no-lonely-if](no-lonely-if): disallow `if` statements as the only statement in `else` blocks
* [no-mixed-spaces-and-tabs](no-mixed-spaces-and-tabs): disallow mixed spaces and tabs for indentation (recommended)
* [no-multiple-empty-lines](no-multiple-empty-lines): disallow multiple empty lines
* [no-negated-condition](no-negated-condition): disallow negated conditions
* [no-nested-ternary](no-nested-ternary): disallow nested ternary expressions
* [no-new-object](no-new-object): disallow `Object` constructors
* [no-plusplus](no-plusplus): disallow the unary operators `++` and `--`
* [no-restricted-syntax](no-restricted-syntax): disallow specified syntax
* [no-spaced-func](no-spaced-func): disallow spacing between `function` identifiers and their applications (fixable)
* [no-ternary](no-ternary): disallow ternary operators
* [no-trailing-spaces](no-trailing-spaces): disallow trailing whitespace at the end of lines (fixable)
* [no-underscore-dangle](no-underscore-dangle): disallow dangling underscores in identifiers
* [no-unneeded-ternary](no-unneeded-ternary): disallow ternary operators when simpler alternatives exist
* [no-whitespace-before-property](no-whitespace-before-property): disallow whitespace before properties
* [object-curly-spacing](object-curly-spacing): enforce consistent spacing inside braces (fixable)
* [one-var](one-var): enforce variables to be declared either together or separately in functions
* [one-var-declaration-per-line](one-var-declaration-per-line): require or disallow newlines around `var` declarations
* [operator-assignment](operator-assignment): require or disallow assignment operator shorthand where possible
* [operator-linebreak](operator-linebreak): enforce consistent linebreak style for operators
* [padded-blocks](padded-blocks): require or disallow padding within blocks
* [quote-props](quote-props): require quotes around object literal property names
* [quotes](quotes): enforce the consistent use of either backticks, double, or single quotes (fixable)
* [require-jsdoc](require-jsdoc): require JSDoc comments
* [semi](semi): require or disallow semicolons instead of ASI (fixable)
* [semi-spacing](semi-spacing): enforce consistent spacing before and after semicolons (fixable)
* [sort-imports](sort-imports): enforce sorted import declarations within module
* [sort-vars](sort-vars): require variables within the same declaration block to be sorted
* [space-before-blocks](space-before-blocks): enforce consistent spacing before blocks (fixable)
* [space-before-function-paren](space-before-function-paren): enforce consistent spacing before `function` definition opening parenthesis (fixable)
* [space-in-parens](space-in-parens): enforce consistent spacing inside parentheses (fixable)
* [space-infix-ops](space-infix-ops): require spacing around operators (fixable)
* [space-unary-ops](space-unary-ops): enforce consistent spacing before or after unary operators (fixable)
* [spaced-comment](spaced-comment): enforce consistent spacing after the `//` or `/*` in a comment (fixable)
* [wrap-regex](wrap-regex): require parenthesis around regex literals

## ECMAScript 6

These rules are only relevant to ES6 environments.

* [arrow-body-style](arrow-body-style): require braces around arrow function bodies
* [arrow-parens](arrow-parens): require parentheses around arrow function arguments
* [arrow-spacing](arrow-spacing): enforce consistent spacing before and after the arrow in arrow functions (fixable)
* [constructor-super](constructor-super): require `super()` calls in constructors (recommended)
* [generator-star-spacing](generator-star-spacing): enforce consistent spacing around `*` operators in generator functions (fixable)
* [no-class-assign](no-class-assign): disallow reassigning class members (recommended)
* [no-confusing-arrow](no-confusing-arrow): disallow arrow functions where they could be confused with comparisons
* [no-const-assign](no-const-assign): disallow reassigning `const` variables (recommended)
* [no-dupe-class-members](no-dupe-class-members): disallow duplicate class members (recommended)
* [no-duplicate-imports](no-duplicate-imports): disallow duplicate module imports
* [no-new-symbol](no-new-symbol): disallow `new` operators with the `Symbol` object (recommended)
* [no-restricted-imports](no-restricted-imports): disallow specified modules when loaded by `import`
* [no-this-before-super](no-this-before-super): disallow `this`/`super` before calling `super()` in constructors (recommended)
* [no-useless-constructor](no-useless-constructor): disallow unnecessary constructors
* [no-var](no-var): require `let` or `const` instead of `var`
* [object-shorthand](object-shorthand): require or disallow method and property shorthand syntax for object literals
* [prefer-arrow-callback](prefer-arrow-callback): require arrow functions as callbacks
* [prefer-const](prefer-const): require `const` declarations for variables that are never reassigned after declared
* [prefer-reflect](prefer-reflect): require `Reflect` methods where applicable
* [prefer-rest-params](prefer-rest-params): require rest parameters instead of `arguments`
* [prefer-spread](prefer-spread): require spread operators instead of `.apply()`
* [prefer-template](prefer-template): require template literals instead of string concatenation
* [require-yield](require-yield): require generator functions to contain `yield`
* [template-curly-spacing](template-curly-spacing): require or disallow spacing around embedded expressions of template strings (fixable)
* [yield-star-spacing](yield-star-spacing): require or disallow spacing around the `*` in `yield*` expressions (fixable)

## Removed

These rules existed in a previous version of ESLint but have since been replaced by newer rules.

* [generator-star](generator-star): enforce consistent positioning of the `*` in generator functions (replaced by [generator-star-spacing](generator-star-spacing))
* [global-strict](global-strict): require or disallow `"use strict"` in the global scope (replaced by [strict](strict))
* [no-arrow-condition](no-arrow-condition): disallow arrow functions where conditions are expected (replaced by [no-confusing-arrow](no-confusing-arrow) and [no-constant-condition](no-constant-condition))
* [no-comma-dangle](no-comma-dangle): disallow trailing commas in object literals (replaced by [comma-dangle](comma-dangle))
* [no-empty-class](no-empty-class): disallow empty character classes in regular expressions (replaced by [no-empty-character-class](no-empty-character-class))
* [no-empty-label](no-empty-label): disallow labels for anything other than loops and switches (replaced by [no-labels](no-labels))
* [no-extra-strict](no-extra-strict): disallow `"use strict";` when already in strict mode (replaced by [strict](strict))
* [no-reserved-keys](no-reserved-keys): disallow the use of reserved words as object literal keys (replaced by [quote-props](quote-props))
* [no-space-before-semi](no-space-before-semi): disallow spacing before semicolons (replaced by [semi-spacing](semi-spacing))
* [no-wrap-func](no-wrap-func): disallow parentheses around non-IIFE statements (replaced by [no-extra-parens](no-extra-parens))
* [space-after-function-name](space-after-function-name): enforce consistent spacing after `function` names (replaced by [space-before-function-paren](space-before-function-paren))
* [space-after-keywords](space-after-keywords): enforce consistent spacing after specified keywords (fixable) (replaced by [keyword-spacing](keyword-spacing))
* [space-before-function-parentheses](space-before-function-parentheses): enforce consistent spacing before `function` parentheses (replaced by [space-before-function-paren](space-before-function-paren))
* [space-before-keywords](space-before-keywords): enforce consistent spacing before specified keywords (fixable) (replaced by [keyword-spacing](keyword-spacing))
* [space-in-brackets](space-in-brackets): enforce consistent spacing inside brackets (replaced by [object-curly-spacing](object-curly-spacing) and [array-bracket-spacing](array-bracket-spacing))
* [space-return-throw-case](space-return-throw-case): require spacing after `return`, `throw`, and `case` (fixable) (replaced by [keyword-spacing](keyword-spacing))
* [space-unary-word-ops](space-unary-word-ops): enforce consistent spacing before and after unary operators (replaced by [space-unary-ops](space-unary-ops))
* [spaced-line-comment](spaced-line-comment): enforce consistent spacing after the `//` in line comments (replaced by [spaced-comment](spaced-comment))
