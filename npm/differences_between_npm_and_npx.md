# Differences between npm and npx

### npm(node package manager)
npm manages packages and doesn't run then.
When you execute bellow `npm install` command, that package will be installed on locally.

```bash
npm install package-name
```

If you want NodeJS to execute installed package from your terminal, below command that specifies only package name will fail.
```bash
$ package-name
```
Only globally installed packages can be executed by specifying package name only.

Local path must specified to run them.
Below command will successfully run that package.

```
$ ./node_modules/.bin/package-name
```

You can run a locally installed package by editing `packages.json` file to add that package in the scripts section like below.

```js
{
  "name": "project-name",
  "version": "1.0.0",
  "scripts": {
    "package-name": "package-name"
  }
}
```

Then run a package specified in `packages.json` by using `npm run` command.
```bash
npm run package-name
```

### npx
By default, `npx` will check whether packages exists in $PATH, or in the local project binaries, and execute that.
If package is not found on locally, npx will installed, execute, and remove locally that package.
So, by using npx, local environments will not be changed.(Also packages.json will not have package name which executed by npx command).

You can use npx when you just execute some package but don't need to keep it on locally.
