# App

```
yunohost app {catalog,search,manifest,list,info,map,install,remove,upgrade,change-url,setting,shell,register-url,makedefault,dismiss-notification,ssowatconf,change-label,action,config} ... [-h]
```

## Catalog & Discovery

| Command | Description | Options |
|---------|-------------|---------|
| `catalog` | Show installable apps | `-f` (full), `-c` (categories), `-a` (antifeatures) |
| `search <string>` | Search apps by name/description | — |
| `manifest <app>` | Fetch app manifest | `-s` (with screenshot, API only) |

## Management

| Command | Description | Key Options |
|---------|-------------|-------------|
| `list` | List installed apps | `-f` (full) |
| `info <app>` | App details | `-f` (full), `--with-pre-upgrade-notifications` |
| `map` | URL-to-app mapping | `-a APP`, `-r` (raw), `-u USER` |
| `install <app>` | Install app (name, path, or git URL) | `-l LABEL`, `-a ARGS`, `-n` (no-remove-on-failure), `-f` (force), `-i` (ignore-yunohost-version) |
| `remove <app>` | Remove app | `-p` (purge data) |
| `upgrade [app ...]` | Upgrade app(s), all if none specified | `-u URL`, `-f FILE`, `-F` (force), `-b` (no-backup), `-c` (continue-on-failure), `-i` |
| `change-url <app>` | Change app URL | `-d DOMAIN`, `-p PATH` |
| `change-label <app> <new_label>` | Change app label | — |

## Configuration & Misc

| Command | Description | Options |
|---------|-------------|---------|
| `setting <app> <key>` | Get/set app setting | `-v VALUE`, `-d` (delete) |
| `shell <app>` | Open interactive shell with app env | — |
| `register-url <app> <domain> <path>` | Register web path for app | — |
| `makedefault <app>` | Redirect domain root to app | `-d DOMAIN`, `-u` (undo) |
| `dismiss-notification <app> {post_install,post_upgrade}` | Dismiss notification | — |
| `ssowatconf` | Regenerate SSOwat config | — |

**Next:** [App Actions](12-app-actions.md) · [App Config](13-app-config.md)
