# renovate-config
Shared configurations for Renovate bot

Use as [described in the Renovate docs](https://docs.renovatebot.com/config-presets/):

```json
{
  "extends": ["github>AmpelProject/renovate-config"]
}
```

## default

This is intended to keep noise down while upgrading Ampel-internal dependencies as rapidly as possible.

Monthly:
- minor and patch updates to install dependencies are grouped together, and automatically merged when tests pass
- ditto for dev dependencies
- major updates create individual PRs

Every run:
- Ampel packages are bumped

