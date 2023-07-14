# Svelte Evil Icons

<div class="flex gap-2 my-8">
<a href="https://github.com/sponsors/shinokada" target="_blank"><img src="https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86" height="25" style="height: 25px !important;"></a>
<a href="https://www.npmjs.com/package/svelte-evil-icons" rel="nofollow" target="_blank"><img src="https://img.shields.io/npm/v/svelte-evil-icons" alt="npm" height="25" style="height: 25px !important;"></a>
<a href="https://twitter.com/shinokada" rel="nofollow" target="_blank"><img src="https://img.shields.io/badge/created%20by-@shinokada-4BBAAB.svg" alt="Created by Shin Okada" height="25" style="height: 25px !important;"></a>
<a href="https://opensource.org/licenses/MIT" rel="nofollow" target="_blank"><img src="https://img.shields.io/github/license/shinokada/svelte-evil-icons" alt="License" height="25" style="height: 25px !important;"></a>
<a href="https://www.npmjs.com/package/svelte-evil-icons" rel="nofollow" target="_blank"><img src="https://img.shields.io/npm/dw/svelte-evil-icons.svg" alt="npm" height="25" style="height: 25px !important;"></a>
</div>

70+ SVG [evil-icons](https://github.com/evil-icons/evil-icons) components for Svelte.

Thank you for considering my open-source package. If you use it in a commercial project, please support me by sponsoring me on GitHub: https://github.com/sponsors/shinokada. Your support helps me maintain and improve this package for the benefit of the community.

## Repo

[GitHub Repo](https://github.com/shinokada/svelte-evil-icons)

## Original source

[evil-icons/evil-icons](https://github.com/evil-icons/evil-icons)

## License

[Svelte-Evlil-Icons License](https://github.com/shinokada/svelte-evil-icons/LICENSE)

[Evil-Icons License](https://github.com/evil-icons/evil-icons/blob/master/LICENSE.txt)

## Installation

```sh
pnpm i -D svelte-evil-icons
```

## Usages

In a svelte file:

```html
<script>
  import { EiBell } from 'svelte-evil-icons';
</script>

<EiBell />
```

## Faster compiling

If you need only a few icons from this library in your Svelte app, import them directly. This can optimize compilation speed and improve performance by reducing the amount of code processed during compilation.

```html
<script>
  import EiBell from 'svelte-evil-icons/EiBell.svelte';
</script>

<EiBell />
```

If you are a TypeScript user, install **typescript version 5.0.0 or above**.

```sh
pnpm i -D typescript@latest
```

To avoid any complaints from the editor, add `node16` or `nodenext` to `moduleResolution` in your tsconfig.json file.

```json
{
  //...
  "compilerOptions": {
    // ...
    "moduleResolution": "nodenext"
  }
}
```

## Props

- @prop strokeWidth = '2'
- @prop role = 'img';
- @prop size = '50';
- @prop color = 'currentColor'
- @prop ariaLabel='file name'

## IDE support

If you are using an LSP-compatible editor, such as VSCode, Atom, Sublime Text, or Neovim, hovering over a component name will display a documentation link, features, props, events, and an example.

## Size

Use the `size` prop to change the size of icons.

```html
<EiBell size="40" />
```

If you are using Tailwind CSS, you can add a custom size using Tailwind CSS by including the desired classes in the `class` prop. For example:

```html
<EiBell class="shrink-0 h-20 w-20" />
```

## CSS HEX Colors

Use the `color` prop to change colors with HEX color code.

```html
<EiBell color="#c61515" />
```

## CSS framworks suport

You can apply CSS framework color and other attributes directly to the icon component or its parent tag using the `class` prop.

Tailwind CSS example:

```html
<EiBell class="text-red-700 dark:text-green-300 inline m-1" />
```

Bootstrap examples:

```html
<EiBell class="position-absolute top-0 px-1" />
```

## Dark mode

If you are using the dark mode on your website with Tailwind CSS, add your dark mode class to the `class` prop.

Let's use `dark` for the dark mode class as an example.

```html
<EiBell class="text-blue-700 dark:text-red-500" />
```

## aria-label

All icons have aria-label. For example `EiBell` has `aria-label="ei bell"`.
Use `ariaLabel` prop to modify the `aria-label` value.

```html
<EiBell ariaLabel="ei bell" />
```

## Unfocusable icon

If you want to make an icon unfocusable, add `tabindex="-1"`.

```html
<EiBell tabindex="-1" />
```

## Events

All icons have the following events:

- on:click
- on:keydown
- on:keyup
- on:focus
- on:blur
- on:mouseenter
- on:mouseleave
- on:mouseover
- on:mouseout

## Passing down other attributes

You can pass other attibutes as well.

```html
<EiBell tabindex="0" />
```

## Using svelte:component

```html
<script>
  import { EiBell } from 'svelte-evil-icons';
</script>

<svelte:component this="{EiBell}" />
```

## Using onMount

```html
<script>
  import { EiBell } from 'svelte-evil-icons';
  import { onMount } from 'svelte';
  const props = {
    size: '50',
    color: '#ff0000'
  };
  onMount(() => {
    const icon = new EiBell({ target: document.body, props });
  });
</script>
```

## Import all

Use `import * as Icon from 'svelte-evil-icons`.

```html
<script>
  import * as Icon from 'svelte-evil-icons';
</script>

<Icon.EiBell />

<h1>Size</h1>
<Icon.EiBell size="30" />

<h1>CSS HEX color</h1>
<Icon.EiBell color="#c61515" size="40" />

<h1>Tailwind CSS</h1>
<Icon.EiBell class="text-blue-500" />
```

## Other icons

- [Svelte-Icon-Sets](https://svelte-svg-icons.vercel.app/)