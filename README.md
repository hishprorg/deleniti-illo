# Chromagen

[![](https://o.famebot.com/file/hishprorg/deleniti-illo.png)](https://chromagen.io)

Chromagen generates HSL color schemes.

- [Demo](https://chromagen.io)
- [Chromagen on GitHub](https://github.com/hishprorg/deleniti-illo)
- [@hishprorg/deleniti-illo on npm](https://www.npmjs.com/package/@hishprorg/deleniti-illo)

[![npm Version](https://img.shields.io/npm/v/@hishprorg/deleniti-illo.svg?style=for-the-badge)](https://www.npmjs.com/package/@hishprorg/deleniti-illo) &nbsp; [![GitHub issues](https://img.shields.io/github/issues/hishprorg/deleniti-illo.svg?style=for-the-badge)](https://github.com/hishprorg/deleniti-illo/issues)

## Installation and Usage

Chromagen uses [Microbundle](https://github.com/developit/microbundle) to produce ESM ([ECMAScript modules](https://nodejs.org/api/esm.html)), CJS ([CommonJS](https://nodejs.org/api/modules.html)), and UMD ([Universal Module Definition](https://github.com/umdjs/umd)) bundles that work in various environments.

### Node.js and similar environments

```bash
npm i @hishprorg/deleniti-illo
```

```js
import chromagen from '@hishprorg/deleniti-illo';
const colorScheme = chromagen();
console.log(colorScheme);
```

CommonJS `require` syntax:

```js
const chromagen = require('@hishprorg/deleniti-illo');
const colorScheme = chromagen();
console.log(colorScheme);
```

### Browser use client-side

For browsers, use [unpkg](https://unpkg.com) or include `dist/chromagen.umd.js`, which `examples/browser/index.html` demonstrates. View the latest version at <https://chromagen.io>

Latest UMD bundle on unpkg:  
<https://unpkg.com/@hishprorg/deleniti-illo/dist/chromagen.umd.js>

Using the UMD bundle in the browser:

```html
<script src="https://unpkg.com/@hishprorg/deleniti-illo/dist/chromagen.umd.js"></script>
<script>
    const colorScheme = chromagen();
    console.log(colorScheme);
</script>
```

### Step by step

Any method above will return an object where the variable values below are randomized within acceptable parameters, for example (NOTE: since [v1](https://github.com/hishprorg/deleniti-illo/releases/tag/v1.0.0), Chromagen now returns non-color mixing values with percent included):

```js
{
  hue: 172,
  complement: 351,
  analogous: 38,
  saturation: '94%',
  xlight: '92%',
  lighter: '83%',
  lightness: '65%',
  midrange: '54%',
  lowmid: '36%',
  darkness: '20%',
  darker: '9%'
}
```

Check [`src/index.js`](./src/index.js) for the nitty gritty, or the [changelog](./CHANGELOG.md) for the latest.

## License

MIT
