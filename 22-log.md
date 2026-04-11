# Log

```
yunohost log {list,show,display,share} ... [-h]
```

## Actions

| Command | Description | Options |
|---------|-------------|---------|
| `list` | List operation logs | `-l LIMIT` (default 50), `-d` (with details), `-s` (with sub-operations) |
| `show <path>` | Display log content | `-n NUMBER`, `--share` (yunopaste), `-i` (filter irrelevant), `-s` (with sub-operations) |
| `display <path>` | Alias for `show` | Same options |
| `share <path>` | Share log on yunopaste | — |

**Prev:** [Hook](21-hook.md) · **Next:** [Diagnosis](23-diagnosis.md)
