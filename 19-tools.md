# Tools

```
yunohost tools {rootpw,maindomain,postinstall,update_norefresh,update,upgrade,shell,basic-space-cleanup,shutdown,reboot,regen-conf,versions,migrations} ... [-h]
```

## Actions

| Command | Description | Key Options |
|---------|-------------|-------------|
| `rootpw` | Change root password | `-n NEW_PASSWORD` |
| `maindomain` | Check/change main domain | `-n NEW_MAIN_DOMAIN` |
| `postinstall` | YunoHost post-install | `-d DOMAIN`, `-u USERNAME`, `-F FULLNAME`, `-p PASSWORD`, `--ignore-dyndns`, `--dyndns-recovery-password`, `--force-diskspace`, `--i-have-read-terms-of-services` |
| `update_norefresh` | List updates (no cache refresh) | — |
| `update [TARGET]` | Update apps/system. TARGET: `apps`, `system`, `all` | `--no-refresh` |
| `upgrade [{apps,system}]` | Upgrade all apps or system packages | — |
| `shell` | Launch dev shell (Python) | `-c COMMAND` |
| `basic-space-cleanup` | Space cleanup (apt, logs, etc.) | — |
| `shutdown` | Shut down server | `-f` (force, skip confirmation) |
| `reboot` | Reboot server | `-f` (force, skip confirmation) |
| `regen-conf [NAME ...]` | Regenerate config files | `-d` (with diff), `-f` (force override), `-n` (dry-run), `-p` (list pending) |
| `versions` | Show YunoHost package versions | — |

**Next:** [Migrations](20-tools-migrations.md)
