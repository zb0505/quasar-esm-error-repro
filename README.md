# Quasar error repro

A repository containing code to reproduce error:
```txt
Error [ERR_REQUIRE_ESM]: require() of ES Module
/tmp/.mount_TGGPla6sVv0t/resources/app.asar/node_modules/conf/dist/source/index.js
from
/tmp/.mount_TGGPla6sVv0t/resources/app.asar/electron-main.js
not supported.
```

## Steps to reproduce

#### 1) Install dependencies
```bash
npm install
```

#### 2) Start the app in Electron mode
```bash
npx quasar dev -m electron
```
