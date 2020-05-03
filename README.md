# node-typescript-es6module
Test Node.js and TypeScript with ES6 Modules

```
npm install
npm test
```

## .mjs extensions

.mjs extension don't seem to work like .js extenstion on relative imports.

```
git checkout mjs
npm test
```
output :-
```
C:\Users\aaron\Tests\TypeScript\node-typescript-es6module>npm test

> node-typescript-es6module@0.0.1 test C:\Users\aaron\Tests\TypeScript\node-typescript-es6module
> npm run build && node caller.js


> node-typescript-es6module@0.0.1 build C:\Users\aaron\Tests\TypeScript\node-typescript-es6module
> tsc && rename *.js *.mjs

caller.ts:1:22 - error TS2307: Cannot find module './callee.mjs'.

1 import { test } from './callee.mjs';
```
