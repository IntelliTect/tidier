# tidier-eslint

A collection of javascript linting rules based on the [Intellitect](https://github.com/intellitect) coding standards.

- [Contributing](#contributing)
- [Installation](#installation)
- [Usage](#usage)

---

## Contributing

If there are rules that need changed / updated, submit an [issue](https://github.com/IntelliTect/tidier/issues/new) or [pull request](https://github.com/IntelliTect/tidier/pulls).

---

## Installation

> **Note:**
> tidier-eslint will soon be hosted as a stand-alone NPM package with proper versioning.

**via NPM**:

```bash
npm install --save-dev ssh://github.com/IntelliTect/tidier.git
```

**via Yarn**:

```bash
yarn add --dev ssh://github.com/IntelliTect/tidier.git
```

---

## Usage

[ESLint](http://eslint.org/) is a linting utility for Javascript. There are integrations for all major IDEs that will automatically lint your `.js` and `.jsx` files. The utility can also be run via command line.

Our rules are currently based on the default Airbnb Javascript style guide [[link](https://github.com/airbnb/javascript)], but will soon include more fine-grained customization.

For documentation and examples on the available rules, refer to the following:

- [ESLint List of available rules](http://eslint.org/docs/rules/)
- [Airbnb JS rule configuration](https://github.com/airbnb/javascript)
- [Airbnb React rule configuration](https://github.com/airbnb/javascript/tree/master/react)

**To configure linting:**

1. Add an `.eslintrc` file to your repository
2. Extend the tidier-eslint config
    ``` javascript
    {
      "extends": "./node_modules/@intellitect/tidier/eslint/index.js"
    }
    ```
3. Add any additional custom rules

**Usage with Webpack**:

Use the [eslint-loader](https://github.com/MoOx/eslint-loader) webpack loader.

**Usage with Gulp**:

Use the [eslint-gulp](https://github.com/adametry/gulp-eslint) plugin.
