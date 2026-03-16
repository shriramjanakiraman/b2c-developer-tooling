---
'@salesforce/b2c-cli': patch
'@salesforce/b2c-tooling-sdk': patch
---

Add `cartridges` config option to specify which cartridges to deploy/watch. Supports comma or colon-separated strings, or arrays in dw.json. Also accepts `cartridgesPath` as an alias. The `-c` flag still takes precedence when provided.
