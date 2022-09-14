When you want to debug typescript code, you need to specify `ts-node/register` in launch.json.

launch.json example are below.

```json
{
  "version": "0.2.0",
  "configurations": [
    {
      "type": "pwa-node",
      "request": "launch",
      "name": "Dubug TypeScript",
      "skipFiles": [
        "<node_internals>/**"
      ],
      "program": "${file}",
      "runtimeArgs": ["-r", "ts-node/register", "-r", "tsconfig-paths/register"],
      "outFiles": [
        "${workspaceFolder}/**/*.js"
      ]
    }
  ]
}

```
