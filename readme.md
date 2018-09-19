# ekst

[![npm](https://img.shields.io/npm/v/ekst.svg?style=flat-square)](https://www.npmjs.com/package/ekst) [![tests](https://img.shields.io/travis/deepsweet/ekst/master.svg?label=tests&style=flat-square)](https://travis-ci.org/deepsweet/ekst) [![coverage](https://img.shields.io/codecov/c/github/deepsweet/ekst.svg?style=flat-square)](https://codecov.io/github/deepsweet/ekst)

Append, prepend, replace or remove [basename](https://nodejs.org/api/path.html#path_path_basename_path_ext) extensions.

## Requirements

* Node.js >= 8.6.0

## Install

```sh
$ yarn add ekst
# or
$ npm install ekst
```

## Usage

```js
import { appendExt, prependExt, replaceExt, removeExt } from 'ekst'

appendExt('file.a.b', '.c') // file.a.b.c
prependExt('file.b.c', '.a') // file.a.b.c
replaceExt('file.a.d.d.c', '.d', '.b') // file.a.b.b.c
removeExt('file.a.d.b.d.c.d.d', '.d') // file.a.b.c
```
