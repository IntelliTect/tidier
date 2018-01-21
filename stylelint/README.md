# tidier-stylelint

A collection of typescript linting rules based on the [Intellitect](https://github.com/intellitect) coding standards.

- [Contributing](#contributing)
- [Installation](#installation)
- [Usage](#usage)

---

## Contributing

If there are rules that need changed / updated, submit an [issue](https://github.com/IntelliTect/tidier/issues/new) or [pull request](https://github.com/IntelliTect/tidier/pulls).

---

## Installation

> **Note:**
> tidier-stylelint will soon be hosted as a stand-alone NPM package with proper versioning.

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

[Stylelint](http://stylelint.io/) is a linting utility for CSS and its various flavors (SASS, LESS, etc). There are integrations for all major IDEs that will automatically lint your `.css` and `.scss` files. The utility can also be run via command line.

Our rules are customized and influenced by several prominent leaders in the industry:

- [Github's Primer](https://primer.github.io/)
- [Airbnb's style guide](https://github.com/airbnb/css)
- [Mark Otto's Code Guide](http://codeguide.co/)

For documentation and examples on the available rules, refer to the following:

- [Stylelint List of available rules](http://stylelint.io/user-guide/rules/)
- [Stylelint standard configuration](https://github.com/stylelint/stylelint-config-standard)
- [stylelint-scss available rules](https://github.com/kristerkari/stylelint-scss)

There are currently two versions of our configuration:

- `css.js`  : rules for vanilla css
- `scss.js` : rules tailored for sass (scss), including variables, mixins, etc.

**To configure linting:**

1. Add an `.stylelintrc` file to your repository
2. Extend the tidier-stylelint config
    ```
    {
      "extends": ["./node_modules/@intellitect/tidier/stylelint/scss.js"]
    }
    ```
3. Add any additional custom rules

**Usage with your editor**:

Use a compatible plugin. Options are found on the [stylelint website](http://stylelint.io/user-guide/complementary-tools/#editor-plugins)

**Usage with Webpack**:

Use the [stylelint-webpack-plugin](https://github.com/JaKXz/stylelint-webpack-plugin) webpack plugin.

**Usage with Gulp**:

Use the [gulp-stylelint](https://github.com/olegskl/gulp-stylelint) plugin.
