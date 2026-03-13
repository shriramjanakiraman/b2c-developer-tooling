---
'@salesforce/b2c-tooling-sdk': patch
---

Strip `development` export conditions from package.json during publish. Fixes `MODULE_NOT_FOUND` errors when plugins or consumers install the SDK from npm, where the `src/` directory is not included.
