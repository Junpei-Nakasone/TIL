# What is SourceMap

Source map enable us to debug TypeScript code. A source map file maps from transpiled JavaScript code to original TypeScript code so that debugger can reconstructed the original TypeScript code while debugging.

If you want to use source map, you need to Add sourceMap in `tsconfig.json`

```json
Copy
{
  "compilerOptions": {
    ...
    "sourceMap": true
  },
  ...
}
```
