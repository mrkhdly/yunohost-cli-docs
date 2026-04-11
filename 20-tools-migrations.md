# Tools - Migrations

```
yunohost tools migrations {list,run,migrate,state} ... [-h]
```

## Actions

| Command | Description | Options |
|---------|-------------|---------|
| `list` | List migrations | `--pending`, `--done` |
| `run [targets ...]` | Run migrations (all pending by default) | `--skip`, `--force-rerun`, `--auto`, `--accept-disclaimer` |
| `migrate` | Alias for `run` | Same options |
| `state` | Show current migration state | — |

**Prev:** [Tools](19-tools.md) · **Next:** [Hook](21-hook.md)
