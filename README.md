# GD Macro Previews

Community macro previews for Geometry Dash levels, used by the **Macro Preview** Geode mod.

## Structure

```
index.json          ← Level ID → macro metadata lookup
macros/
  12345.mhr         ← Mega Hack v7 replay
  67890.json        ← Echo replay
```

## Adding a macro (maintainer)

1. Download the macro from the submission issue
2. Name it `{levelID}.mhr` or `{levelID}.json`
3. Place it in `macros/`
4. Add an entry to `index.json`:

```json
"LEVEL_ID": {
    "mhr":         true,
    "json":        false,
    "uploader":    "PlayerName",
    "description": "Brief description"
}
```

5. Commit and push — the mod picks it up instantly via raw.githubusercontent.com

## Submitting a macro (players)

Use the **Submit** button inside the game on any level info page.
It opens a pre-filled GitHub issue — just attach your macro file and submit.
