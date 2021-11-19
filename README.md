# svelte-grommet-icons

[![NPM][npm]][npm-url]

> [Grommet SVG icons](https://github.com/grommet/grommet-icons) as Svelte components.

<!-- REPO_URL -->

Try it in the [Svelte REPL](https://svelte.dev/repl/dd12a60aba434d81b0cdea6e9e0aea45).

---

<!-- TOC -->

## Installation

**Yarn**

```bash
yarn add -D svelte-grommet-icons
```

**NPM**

```bash
npm i -D svelte-grommet-icons
```

**pnpm**

```bash
pnpm i -D svelte-grommet-icons
```

## Usage

### Basic

```svelte
<script>
  import { Analytics, Camera, DocumentImage } from "svelte-grommet-icons";
</script>

<Analytics />
<Camera />
<DocumentImage />
```

Refer to [ICON_INDEX.md](ICON_INDEX.md) for a list of supported icons.

### Direct import

Use the direct import for faster compiling during development.

**Note:** even if using base imports, unused imports are still tree shakeable by application bundlers like Rollup or webpack.

```html
<script>
  import Add from "svelte-grommet-icons/lib/Add.svelte";
</script>
```

## Using `svelte:component`

```svelte
<script>
  import * as icons from "svelte-grommet-icons";
</script>

{#each Object.entries(icons) as [icon, component]}
  <div>
    <svelte:component this={component} />
    {icon}
  </div>
{/each}
```

## TypeScript

Svelte version 3.31 or greater is required to use this library with TypeScript.

## [Changelog](CHANGELOG.md)

## License

[MIT](LICENSE)

[npm]: https://img.shields.io/npm/v/svelte-grommet-icons.svg?color=%237d4cdb&style=for-the-badge
[npm-url]: https://npmjs.com/package/svelte-grommet-icons
