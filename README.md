# YunoHost CLI — Complete Reference

> Generated from `yunohost --help` on **a YunoHost server**

---

## Quick Navigation

| # | Page | Description |
|---|------|-------------|
| 01 | [Global Options](01-global-options.md) | `--debug`, `--output-as`, `--timeout`, etc. |
| | | |
| | **User Management** | |
| 02 | [User](02-user.md) | list, create, delete, update, info, export, import |
| 03 | [Groups](03-user-groups.md) | list, create, delete, info, add, remove, mail aliases |
| 04 | [Permissions](04-user-permissions.md) | list, info, update, add, remove, ldapsync |
| 05 | [SSH](05-user-ssh.md) | list-keys, add-key, remove-key |
| | | |
| | **Domains** | |
| 06 | [Domain](06-domain.md) | list, info, add, remove, main-domain, url-available, action-run |
| 07 | [DynDNS](07-domain-dyndns.md) | subscribe, unsubscribe, set-recovery-password |
| 08 | [Config](08-domain-config.md) | get, set |
| 09 | [DNS](09-domain-dns.md) | suggest, push |
| 10 | [Certificates](10-domain-certificates.md) | status, install, renew (Let's Encrypt) |
| | | |
| | **Apps** | |
| 11 | [App](11-app.md) | catalog, search, install, remove, upgrade, map, etc. |
| 12 | [Actions](12-app-actions.md) | list, run |
| 13 | [Config](13-app-config.md) | get, set |
| | | |
| | **System** | |
| 14 | [Backup](14-backup.md) | create, restore, list, info, download, delete |
| 15 | [Settings](15-settings.md) | list, get, set, reset-all, reset |
| 16 | [Service](16-service.md) | add, remove, start, stop, reload, restart, enable, disable, status, log |
| 17 | [Firewall](17-firewall.md) | list, open, close, allow, disallow, upnp, reload, stop |
| 18 | [DynDNS Deprecated](18-dyndns-deprecated.md) | subscribe, update (use domain dyndns instead) |
| | | |
| | **Tools & Misc** | |
| 19 | [Tools](19-tools.md) | rootpw, postinstall, update, upgrade, shell, shutdown, reboot, regen-conf, versions |
| 20 | [Migrations](20-tools-migrations.md) | list, run, migrate, state |
| 21 | [Hook](21-hook.md) | add, remove, info, list, callback, exec |
| 22 | [Log](22-log.md) | list, show, display, share |
| 23 | [Diagnosis](23-diagnosis.md) | list, show, get, run, ignore, unignore |
| 24 | [Storage](24-storage.md) | disk list, disk info |

---

## Command Tree

```
yunohost
├── user ─── list, create, delete, update, info, export, import
│   ├── group ─── list, create, delete, info, add, remove, add-mailalias, remove-mailalias
│   ├── permission ─── list, info, update, add, remove, ldapsync
│   └── ssh ─── list-keys, add-key, remove-key
├── domain ─── list, info, add, remove, main-domain, url-available, action-run
│   ├── dyndns ─── subscribe, unsubscribe, set-recovery-password
│   ├── config ─── get, set
│   ├── dns ─── suggest, push
│   └── cert ─── status, install, renew
├── app ─── catalog, search, manifest, list, info, map, install, remove, upgrade,
│           change-url, change-label, setting, shell, register-url, makedefault,
│           dismiss-notification, ssowatconf
│   ├── action ─── list, run
│   └── config ─── get, set
├── backup ─── create, restore, list, info, download, delete
├── settings ─── list, get, set, reset-all, reset
├── service ─── add, remove, start, stop, reload, restart, reload_or_restart,
│               enable, disable, status, log
├── firewall ─── list, is-open, open, close, delete, allow, disallow, upnp, reload, stop
├── dyndns (deprecated) ─── subscribe, update
├── tools ─── rootpw, maindomain, postinstall, update_norefresh, update, upgrade,
│             shell, basic-space-cleanup, shutdown, reboot, regen-conf, versions
│   └── migrations ─── list, run, migrate, state
├── hook ─── add, remove, info, list, callback, exec
├── log ─── list, show, display, share
├── diagnosis ─── list, show, get, run, ignore, unignore
└── storage ─── disk ─── list, info
```

---

## Notes

- ⚠️ `yunohost dyndns` is **deprecated** — use `yunohost domain dyndns`
- ⚠️ `yunohost domain maindomain` is **deprecated** — use `yunohost domain main-domain`
- `log display` is an alias for `log show`
- `log share` is an alias for `log show --share`; `log show --share` itself is **deprecated**
- `migrations migrate` is an alias for `migrations run`
- Many commands have `--full` and `--export` flags for API usage
- Serialized arguments use the format: `"key1=value1&key2=value2"`
