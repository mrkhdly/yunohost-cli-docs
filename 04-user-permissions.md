# User - Permissions

```
yunohost user permission {list,info,update,add,remove,ldapsync} ... [-h]
```

## Actions

| Command | Description | Key Options |
|---------|-------------|-------------|
| `list [apps ...]` | List permissions | `-f` (full info including user lists) |
| `info <permission>` | Get permission info | — |
| `update <permission>` | Manage permissions | `-l LABEL`, `-s SHOW_TILE`, `-L LOGO`, `-d DESCRIPTION`, `-o ORDER`, `-H HIDE_FROM_PUBLIC` |
| `add <perm> [GROUP_OR_USER ...]` | Grant permission | — |
| `remove <perm> [GROUP_OR_USER ...]` | Revoke permission | — |
| `ldapsync` | Resync permissions to LDAP | Technical command only |

**Prev:** [Groups](03-user-groups.md) · **Next:** [SSH](05-user-ssh.md)
