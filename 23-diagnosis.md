# Diagnosis

```
yunohost diagnosis {list,show,get,run,ignore,unignore} ... [-h]
```

## Actions

| Command | Description | Key Options |
|---------|-------------|-------------|
| `list` | List diagnosis categories | — |
| `show [categories ...]` | Show recent results | `--full`, `--issues`, `--share`, `--human-readable` |
| `get <category> [CRITERIA ...]` | Fetch raw test data | Criteria from `meta` in `show` output |
| `run [categories ...]` | Run diagnosis | `--force`, `--except-if-never-ran-yet`, `--email` |
| `ignore` | Ignore diagnosis results | `--filter [CRITERIA ...]`, `--list` |
| `unignore` | Un-ignore diagnosis results | `--filter [CRITERIA ...]` |

**Prev:** [Log](22-log.md) · **Next:** [Storage](24-storage.md)
