# npm-reproducible-bug

steps:
1. `cd components/comp-a`
2. `npm install`

You'll be getting an error:
```
➜  comp-a npm i
npm WARN rollback Rolling back classnames@2.2.6 failed (this is probably harmless): /private/tmp/npm-issue/components/comp-c/node_modules/classnames is not a child of /private/tmp/npm-issue/components/comp-a
npm WARN comp-a@1.0.0 No description
npm WARN comp-a@1.0.0 No repository field.

npm ERR! code ENOENT
npm ERR! syscall rename
npm ERR! path /private/tmp/npm-issue/components/comp-a/node_modules/.staging/classnames-00a850cf
npm ERR! dest /private/tmp/npm-issue/components/comp-c/node_modules/classnames
npm ERR! errno -2
npm ERR! enoent ENOENT: no such file or directory, rename '/private/tmp/npm-issue/components/comp-a/node_modules/.staging/classnames-00a850cf' -> '/private/tmp/npm-issue/components/comp-c/node_modules/classnames'
npm ERR! enoent This is related to npm not being able to find a file.
npm ERR! enoent
```
