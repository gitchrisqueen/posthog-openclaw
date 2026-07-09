---
'@posthog/openclaw': patch
---

Fall back to the `POSTHOG_API_KEY` environment variable when `apiKey` is not set (or blank) in the plugin config, make `apiKey` optional in the config schema so the plugin loads cleanly without an inline key, and add a `schemaCacheKey` to avoid duplicate AJV schema registration on plugin reload.
