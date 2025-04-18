<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@lynx-js/rspeedy](./rspeedy.md) &gt; [Output](./rspeedy.output.md) &gt; [cssModules](./rspeedy.output.cssmodules.md)

## Output.cssModules property

The [CssModules](./rspeedy.cssmodules.md) option is used for the customization of CSS Modules configurations.

**Signature:**

```typescript
cssModules?: CssModules | undefined;
```

## Remarks

The CSS module is enabled for `*.module.css`<!-- -->, `*.module.scss` and `*.module.less`<!-- -->. Use [CssModules.auto](./rspeedy.cssmodules.auto.md) to customize the filtering behavior.

## Example 1

Disable CSS modules:

```js
import { defineConfig } from '@lynx-js/rspeedy'
export default defineConfig({
  output: {
    cssModules: {
      auto: false,
    },
  },
})
```

## Example 2

Enable CSS modules for all CSS files:

```js
import { defineConfig } from '@lynx-js/rspeedy'
export default defineConfig({
  output: {
    cssModules: {
      auto: () => true,
    },
  },
})
```

