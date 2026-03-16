---
'@salesforce/b2c-tooling-sdk': minor
---

`resolveConfig()` and the `ConfigSource` interface are now async. This enables config sources that perform async I/O such as keychain lookups, credential vaults, or network-based config stores.

**Breaking:** `resolveConfig()` now returns `Promise<ResolvedB2CConfig>` — callers must `await` the result. The `ConfigSource.load()` method return type is now `MaybePromise<ConfigLoadResult | undefined>`, so existing sync source implementations continue to work without changes.
