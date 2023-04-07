
## tutorial
https://www.youtube.com/watch?v=Nh9xW2-ZOEU&t=639s

init package.json:
```bash
$ npm init -y

//add this to config:
  "main": "dist/index.js",
  "types": "dist/index.d.js",
  "files": ['/dist'],
```

install typescript:
```bash
$ npm install typescript

$ npx tsc --init
//init the tsconfig.json with ALL the compiler options
```
//clear and create this configuration:
```json
{
  "compilerOptions": {
    "module": "Commonjs", 
    "target": "es2015",
    "sourceMap": true,
    "outDir": "./dist",
    "noImplicitAny": true,
    "declaration": true,
  },
  "include": ["src/**/*"],
  "exclude": ["node_modules"]
}
```
Compile TS:
`$ npx tsc`

NPM stuff
`npm login`
'npm publish'

## tester

Install ts-node:
https://www.npmjs.com/package/ts-node

```ts
import { sayHello } from 'ag-test-package-npm'

console.log(sayHello("from tester"));
```
