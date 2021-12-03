# Astro Starter Kit: Blog

**NOTE: ** The issue has been fixed in [Astro v0.21.9](https://github.com/withastro/astro/blob/main/packages/astro/CHANGELOG.md#0219) , [PR](https://github.com/withastro/astro/pull/2107). Archiving the repo. 

```
npm init astro -- --template blog
```

[![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/amithgeorge/astro-blog-build-error)


## Issue 

Running `npm run build` fails with error message 

```shell
❯ npm run build

> @example/blog@0.0.1 build
> astro build

11:11 AM [config] Set "buildOptions.site" to generate correct canonical URLs and sitemap
'pathToFileURL' is not exported by __vite-browser-external, imported by node_modules/astro/dist/runtime/server/index.js
file: <path>/astro-blog-build-error/node_modules/astro/dist/runtime/server/index.js:33:9
31: };
32: import shorthash from "shorthash";
33: import { pathToFileURL } from "url";
             ^
34: import { extractDirectives, generateHydrateScript } from "./hydration.js";
35: import { serializeListValue } from "./util.js";
Error: 'pathToFileURL' is not exported by __vite-browser-external, imported by node_modules/astro/dist/runtime/server/index.js
```
