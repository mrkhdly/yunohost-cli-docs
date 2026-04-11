# Firewall

```
yunohost firewall {list,is-open,open,close,delete,allow,disallow,upnp,reload,stop} ... [-h]
```

## Actions

| Command | Description | Key Options |
|---------|-------------|-------------|
| `list` | List all rules | `-r` (raw YAML), `-p {tcp,udp}`, `-f` (forwarded/UPnP) |
| `is-open <port>` | Check if port is open | `-p {tcp,udp}` |
| `open <port> <comment>` | Allow connections | `-p {tcp,udp}`, `--upnp`, `--no-reload` |
| `close <port>` | Disallow connections | `-p {tcp,udp}`, `--upnp-only`, `--no-reload` |
| `delete <port>` | Unregister port from YunoHost | `-p {tcp,udp}`, `--no-reload` |
| `allow {TCP,UDP,Both} <port>` | Allow (fine-grained) | `-4` (IPv4 only), `-6` (IPv6 only), `--no-upnp`, `--no-reload` |
| `disallow {TCP,UDP,Both} <port>` | Disallow (fine-grained) | `-4`, `-6`, `--upnp-only`, `--no-reload` |
| `upnp [{enable,disable,status}]` | UPnP port forwarding | `--no-refresh` |
| `reload` | Reload all rules | `--skip-upnp` |
| `stop` | Remove all rules | — |

## Notes

- **`open`/`close` vs `allow`/`disallow`**: Two overlapping pairs. `open`/`close` are simpler (`-p {tcp,udp}`). `allow`/`disallow` use `{TCP,UDP,Both}` with per-protocol IPv4/IPv6 control for fine-grained rules.
- **`close`** removes the port and UPnP forwarding. **`delete`** unregisters the port from YunoHost entirely.

**Prev:** [Service](16-service.md) · **Next:** [DynDNS Deprecated](18-dyndns-deprecated.md)
