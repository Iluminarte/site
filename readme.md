<p align="center">
	<img src="https://raw.githubusercontent.com/stillas/logo/master/stillas.png" width="200" height="200">
</p>

<h1 align="center">Stillas</h1>

<p align="center">Scaffold for new projects (macOS or Linux).</p>

---

## Install & run

Setup:

```bash
npm run setup && cd site
```

Run (with live reload):

```bash
.././hugo server --theme="basic-theme" -D
```

After, go to `themes/basic-theme` and then.

## Stylus/CSS

### Tasks (npm scripts)

Lint:

```bash
npm run css-lint
```

Compile to CSS:

```bash
npm run css-compile
```

All (lint and compile):

```bash
npm run css
```

Watch:

```bash
npm run css-watch
```

## JavaScript

Includes: [Babel](https://babeljs.io/), [Vue.js](https://vuejs.org/) and [Browserify](https://browserify.org/).

### Tasks

Lint:

```bash
npm run js-lint
```

Compile:

```bash
ENV=[development or production] npm run js-compile
```

All (lint and compile):

```bash
ENV=[development or production] npm run js
```

Watch (default: `ENV=development`):

```bash
npm run js-watch
```

## Watch Stylus and JavaScript

```bash
npm run watch
```

## Build to production

Compile all:

```bash
npm run css && ENV=production npm run js
```

Build to `site/public` folder:

_Don't forget to change the option `baseURL` into `site/config.toml` to `""` or to your own host URL._

```bash
.././hugo --theme="basic-theme"
```


Then host it.

---

## License

The MIT License ([MIT](https://github.com/stillas/stillas/blob/development/license.md))

Copyright (c) 2017 marcker
