SystemJS Babel Extension
===

Supports loading TypeScript for `.ts` and ES modules for `.js` files natively in the browser for _easy development workflows_.

Builds on top of the [fetch hook](https://github.com/systemjs/systemjs/blob/master/docs/hooks.md#fetchurl---promise) in SystemJS supported by both the `system.js` and `s.js` builds.

The source transform is skipped for all `System.register` sources, thereby allowing interop of System modules, ES modules and TypeScript.

Specifically does not provide configuration hooks, because no type checking is performed and this is designed to handle current syntax only.

**Not Suitable for Production Workflows**

## Usage

```html
<script src="systemjs/dist/s.js"></script>
<script src="dist/systemjs-babel.js"></script>
<script>
  System.import('./es-module.js');
</script>
```

## LICENSE

MIT
