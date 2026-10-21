# @nxsa/sdc-tokens

SDC design tokens distributed as CSS custom properties, font faces, and a Tailwind CSS v4 theme.

## Install

```sh
npm install @nxsa/sdc-tokens
```

## CSS Variables

Import the package stylesheet from your application CSS:

```css
@import "@nxsa/sdc-tokens/tokens.css";

.card {
  color: var(--color-content-regular-primary);
  background: var(--color-bg-surface-primary);
}
```

The bundled font files are referenced by `tokens.css` and are included in the published package.

## Tailwind CSS v4

Import the package alongside Tailwind in your main stylesheet:

```css
@import "tailwindcss";
@import "@nxsa/sdc-tokens";
```

The package exposes its `@theme inline` declarations to Tailwind, so the registered tokens can be used as utility classes:

```html
<button class="bg-primary-700 text-neutral-0 font-bold">Continue</button>
```

## License

MIT
