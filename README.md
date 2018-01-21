# tidier

A collection of configuration files for linters and formatters based on the [Intellitect](https://github.com/intellitect) coding standards.

> **Note:**
> This repo currently homes multiple packages that will be distributed separately.

- [Contributing](#contributing)
- [Installation](#installation)
- [Packages](#packages)
  - [tidier-tslint](#tidier-tslint) - Typescript
  - [tidier-eslint](#tidier-eslint) - Javascript
  - [tidier-styleLint](#tidier-stylelint) - (S)CSS

---

## Contributing

If there are rules that need changed / updated, submit an [issue](https://github.com/IntelliTect/tidier/issues/new) or [pull request](https://github.com/IntelliTect/tidier/pulls).

---

## Installation

> **Note:**
> All tidier resources will soon be hosted as stand-alone NPM packages with proper versioning.

**via NPM**:

```bash
npm install --save-dev ssh://github.com/IntelliTect/tidier.git
```

**via Yarn**:

```bash
yarn add --dev ssh://github.com/IntelliTect/tidier.git
```

---

## Packages

> **Note:**
> Any time you add linting or formatting to an existing repo, please do so in separate commits from other features/bug fixes. This helps keep your commits focused on a logical set of changes and makes code review a much easier process.

### tidier-tslint

[tidier-tslint documentation](tslint/README.md)

[TSLint](https://palantir.github.io/tslint/) is a linting utility for Typescript. There are some IDE integrations that will automatically lint your `.ts` and `.tsx` files, but support varies. The utility can also be run via command line.

### tidier-eslint

[tidier-eslint documentation](eslint/README.md)

[ESLint](http://eslint.org/) is a linting utility for Javascript. There are integrations for all major IDEs that will automatically lint your `.js` and `.jsx` files. The utility can also be run via command line.

### tidier-stylelint

[tidier-stylelint documentation](stylelint/README.md)

[Stylelint](http://stylelint.io/) is a linting utility for CSS and its various flavors (SASS, LESS, etc). There are integrations for all major IDEs that will automatically lint your `.css` and `.scss` files. The utility can also be run via command line.
