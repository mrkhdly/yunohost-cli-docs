# Hook

```
yunohost hook {add,remove,info,list,callback,exec} ... [-h]
```

## Actions

| Command | Description | Key Options |
|---------|-------------|-------------|
| `add <app> <file>` | Store hook script to filesystem | — |
| `remove <app>` | Remove hook scripts | — |
| `info {action} <name>` | Get hook information | 18 action types available |
| `list {action}` | List available hooks for an action | `-l {name,priority,folder}`, `-i` (show-info) |
| `callback {action}` | Execute all scripts bound to an action | `-n HOOKS`, `-a ARGS`, `-d CHDIR` |
| `exec <path>` | Execute hook from a file | `-a ARGS`, `--raise-on-error`, `-d CHDIR` |

## Available Hook Actions

`post_user_create`, `post_user_delete`, `post_user_update`, `post_app_addaccess`, `post_app_removeaccess`, `post_domain_add`, `post_domain_remove`, `post_cert_update`, `custom_dns_rules`, `post_app_change_url`, `post_app_upgrade`, `post_app_install`, `post_app_remove`, `backup`, `restore`, `backup_method`, `post_iptable_rules`, `conf_regen`

**Prev:** [Migrations](20-tools-migrations.md) · **Next:** [Log](22-log.md)
