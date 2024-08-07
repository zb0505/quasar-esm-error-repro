# Quasar error repro

A repository containing code to reproduce error:
```txt
Error [ERR_REQUIRE_ESM]: require() of ES Module C:\...\node_modules\electron-store\index.js from C:\...\.quasar\electron\electron-main.js not supported.
Instead change the require of index.js in C:\...\.quasar\electron\electron-main.js to a dynamic import() which is available in all CommonJS modules.
    at c._load (node:electron/js2c/node_init:2:17025)
    at electron-store (C:\...\.quasar\electron\electron-main.js:179:18)
    at __webpack_require__ (C:\...\.quasar\electron\electron-main.js:413:42)
    at eval (webpack://player/./src/electron/app.ts?:27:72)
    at ./src/electron/app.ts (C:\...\.quasar\electron\electron-main.js:29:1)
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
