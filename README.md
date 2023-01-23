# Bundle size comparison

## How did a get the bundle size?

1. Initialized the lib repo using the command on the _Initialized With_ column
2. Deleted all assets, images and css files. Added only a `h1` to the entry app file
3. Built the app using `npm run build`
4. Got the bundle size from the vite production build

## Result

![Chart](/chart.png)

## Libs

| Lib     | Version   | Bundle Size | Bundle Size (gzip) | Initialized With                                 |
| ------- | --------- | ----------- | ------------------ | ------------------------------------------------ |
| React   | `18.2.0`  | `142.90 kB` | `45.88 kB`         | `pnpm create vite react --template react-ts`     |
| SolidJS | `1.6.6`   | `6.57 kB`   | `2.76 kB`          | `npx degit solidjs/templates/ts solidjs`         |
| Preact  | `10.11.3` | `10.14 kB`  | `4.19 kB`          | `pnpm create vite preact --template preact-ts`   |
| Vue     | `3.2.45`  | `52.24 kB`  | `21.08 kB`         | `pnpm create vite vue --template vue-ts`         |
| Svelte  | `3.54.0`  | `38.46 kB`  | `19.49 kB`         | `pnpm create svelte svelte --template svelte-ts` |
