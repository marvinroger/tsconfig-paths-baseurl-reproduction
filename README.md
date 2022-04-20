# [tsconfig-paths #143](https://github.com/dividab/tsconfig-paths/issues/143) minimal reproduction

## Setup

```shell
npm i
```

## Reproduction

```shell
npm start
```

Fails with:

> Missing baseUrl in compilerOptions. tsconfig-paths will be skipped
> Error: Cannot find module '~/library'

## Control

Uncomment `// "baseUrl": ".",` in [tsconfig.json](tsconfig.json), and run `npm start`: it works fine.
