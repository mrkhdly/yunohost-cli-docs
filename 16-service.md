# Service

```
yunohost service {add,remove,start,stop,reload,restart,reload_or_restart,enable,disable,status,log} ... [-h]
```

## Actions

| Command | Description | Key Options |
|---------|-------------|-------------|
| `add <name>` | Add a service | `-d DESCRIPTION`, `-l LOG`, `--test_status`, `--test_conf`, `--needs_exposed_ports`, `-n` (need_lock) |
| `remove <name>` | Remove a service | — |
| `start <NAME> [...]` | Start service(s) | — |
| `stop <NAME> [...]` | Stop service(s) | — |
| `reload <NAME> [...]` | Reload service(s) | — |
| `restart <NAME> [...]` | Restart (starts if not running) | — |
| `reload_or_restart <NAME> [...]` | Reload if supported, else restart | — |
| `enable <NAME> [...]` | Enable service(s) | — |
| `disable <NAME> [...]` | Disable service(s) | — |
| `status [NAME ...]` | Show status (all by default) | — |
| `log <name>` | Show service log files | `-n NUMBER` (lines to display) |

**Prev:** [Settings](15-settings.md) · **Next:** [Firewall](17-firewall.md)
