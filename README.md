# @mnao305/renovate-config

[Shareable config](https://docs.renovatebot.com/config-presets) for [Renovate](https://docs.renovatebot.com/)

## Usage

Enable Renovate in your repo and just `extends` in `renovate.json`.

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": [
    "github>mnao305/renovate-config"
  ]
}
```

This preset uses Renovate's best-practices preset as the base, waits 14 days before normal version updates, keeps GitHub Actions digest pins on exact SemVer tags, runs routine updates outside typical working hours in Asia/Tokyo, labels vulnerability alerts, and automerges patch updates after checks pass.

`default.json` is the shareable preset entrypoint. `renovate.json` is only for this repository and extends the local preset so the configuration stays in one place.
