# tidier-tslint

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
> tidier-tslint will soon be hosted as a stand-alone NPM package with proper versioning.

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

[TSLint](https://palantir.github.io/tslint/) is a linting utility for Typescript. There are some IDE integrations that will automatically lint your `.ts` and `.tsx` files, but support varies. The utility can also be run via command line.

Our rules are heavily influenced by the [Airbnb Javascript style guide](https://github.com/airbnb/javascript).

There are currently two versions of our configuration:

- `back-end`  : rules for server-side development
- `front-end` : rules for client-side development

For documentation and examples on the available rules, please refer to the following:

- [TSLint List of available rules](https://palantir.github.io/tslint/rules/)
- [TSLint TS rule standard configuration](https://github.com/palantir/tslint/blob/master/src/configs/latest.ts)
- [TSLint-react Rules](https://github.com/palantir/tslint-react)
- [Tslint-eslint JS Rules](https://github.com/buzinas/tslint-eslint-rules)

**To configure linting:**

1. Add a `tslint.json` file to your repository
2. Extend the tidier-tslint config
    ```
    {
      "extends": ["./node_modules/@intellitect/tidier/tslint/front-end"]
    }
    ```
3. Add any additional custom rules

**Usage with Webpack**:

Use the [tslint-loader](https://www.npmjs.com/package/tslint-loader) webpack loader.

**Usage with Gulp**:

Use the [tslint-gulp](https://www.npmjs.com/package/gulp-tslint) plugin.
