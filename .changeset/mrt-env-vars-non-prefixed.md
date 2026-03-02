---
'@salesforce/b2c-tooling-sdk': patch
'@salesforce/b2c-cli': patch
'@salesforce/b2c-dx-mcp': patch
---

MRT environment variables now use non-prefixed names (`MRT_API_KEY`, `MRT_PROJECT`, `MRT_ENVIRONMENT`, `MRT_CLOUD_ORIGIN`) as primary. The `SFCC_`-prefixed versions continue to work as fallbacks.
