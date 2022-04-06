# browserslist-issue-edge-97

Running `npx browserslist@latest --update-db` results in the following error:

```
❯ npx browserslist@latest --update-db
browserslist: Unknown version 97 of Edge
Latest version:     1.0.30001325
Installed version:  none
Removing old caniuse-lite from lock file
Installing new caniuse-lite version
$ yarn add -W caniuse-lite
Cleaning package.json dependencies from caniuse-lite
$ yarn remove -W caniuse-lite
caniuse-lite has been successfully updated

Error: Command failed: npx browserslist
browserslist: Unknown version 97 of Edge

    at checkExecSyncError (node:child_process:826:11)
    at Object.execSync (node:child_process:900:15)
    at getBrowsersList (/Users/jb/node_modules/browserslist/update-db.js:62:6)
    at updateDB (/Users/jb/node_modules/browserslist/update-db.js:322:23)
    at Object.<anonymous> (/Users/jb/node_modules/browserslist/cli.js:43:3)
    at Module._compile (node:internal/modules/cjs/loader:1101:14)
    at Object.Module._extensions..js (node:internal/modules/cjs/loader:1153:10)
    at Module.load (node:internal/modules/cjs/loader:981:32)
    at Function.Module._load (node:internal/modules/cjs/loader:822:12)
    at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:81:12)

Problem with browser list retrieval.
Target browser changes won’t be shown.
```