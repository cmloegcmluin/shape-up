# shape-up

[![npm version](https://badge.fury.io/js/%40cmloegcmluin%2Fshape-up.svg)](https://badge.fury.io/js/%40cmloegcmluin%2Fshape-up)

Purify geometry files.

Requires `https://github.com/jonnenauha/obj-simplify`.

## usage

`npm i @cmloegcmluin/shape-up`

Put your `.obj` files in `./geometry`.

`./node_modules/.bin/shape-up`

Your files will be:

1) snapped to nearby simple irrationals such as √2.
2) stripped of comments and other lines Blender's export included
3) deleted if they are the extra `.mtl` file Blender exports
4) minify decimal parts (`.000000` becomes ` `)
5) actually use `obj-simplify` to do the smart stuff e.g. consolidate duplicate geometry
