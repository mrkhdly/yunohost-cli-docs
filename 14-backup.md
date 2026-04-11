# Backup

```
yunohost backup {create,restore,list,info,download,delete} ... [-h]
```

## Actions

| Command | Description | Key Options |
|---------|-------------|-------------|
| `create` | Create backup archive | `-n NAME`, `-d DESCRIPTION`, `-o OUTPUT_DIR`, `--methods` (copy/tar), `--system`, `--apps`, `--dry-run` |
| `restore <name>` | Restore from archive | `--system`, `--apps`, `--force`, `--no-remove-on-failure` |
| `list` | List backups | `-i` (with info), `-H` (human-readable) |
| `info <name>` | Backup details | `-d` (with details), `-H` (human-readable) |
| `download <name>` | Download archive (API only) | — |
| `delete <name>` | Delete archive | — |

**Prev:** [App Config](13-app-config.md) · **Next:** [Settings](15-settings.md)
