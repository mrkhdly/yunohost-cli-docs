# Domain

```
yunohost domain {list,info,add,remove,main-domain,url-available,action-run,dyndns,config,dns,cert} ... [-h]
```

## Actions

| Command | Description | Key Options |
|---------|-------------|-------------|
| `list` | List domains | `--exclude-subdomains`, `--tree`, `--features` |
| `info <domain>` | Get domain aggregated data | — |
| `add <domain>` | Create a custom domain | `--ignore-dyndns`, `--dyndns-recovery-password`, `--install-letsencrypt-cert` |
| `remove <domain>` | Delete domain | `-r` (remove apps), `-f` (force), `--ignore-dyndns`, `--dyndns-recovery-password` |
| `main-domain` | Check/change main domain | `-n NEW_MAIN_DOMAIN` |
| `maindomain` | Alias for `main-domain` (deprecated) | `-n NEW_MAIN_DOMAIN` |
| `url-available <domain> <path>` | Check web path availability | — |
| `action-run <domain> <action>` | Run domain action | `-a ARGS` |

**Next:** [DynDNS](07-domain-dyndns.md) · [Config](08-domain-config.md) · [DNS](09-domain-dns.md) · [Certificates](10-domain-certificates.md)
