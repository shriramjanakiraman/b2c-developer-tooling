---
'@salesforce/b2c-tooling-sdk': patch
---

Fix `--server` override dropping config from non-instance-bound sources. Previously, overriding the server hostname discarded all config values including credentials from global sources like config plugins. Now only values from the source that provided the conflicting hostname are dropped.
