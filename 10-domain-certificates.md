# Domain - Certificates

```
yunohost domain cert {status,install,renew} ... [-h]
```

## Actions

| Command | Description | Options |
|---------|-------------|---------|
| `status [domain_list ...]` | List certificate status (all by default) | `--full` |
| `install [domain_list ...]` | Install Let's Encrypt certs | `--force`, `--no-checks` (not recommended), `--self-signed` |
| `renew [domain_list ...]` | Renew Let's Encrypt certs | `--force` (ignore 15-day threshold), `--email` (send log on failure), `--no-checks` |

**Prev:** [DNS](09-domain-dns.md) · **Next:** [App](11-app.md)
