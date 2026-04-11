# User - Groups

```
yunohost user group {list,create,delete,info,add,remove,add-mailalias,remove-mailalias} ... [-h]
```

## Actions

| Command | Description | Options |
|---------|-------------|---------|
| `list` | List existing groups | `-f` (full info), `-p` (include primary groups) |
| `create <groupname>` | Create a group | — |
| `delete <groupname>` | Delete a group | — |
| `info <groupname>` | Get group information | — |
| `add <groupname> [USERNAME ...]` | Add users to group | — |
| `remove <groupname> [USERNAME ...]` | Remove users from group | — |
| `add-mailalias <groupname> <MAIL> [...]` | Add mail aliases to group | `--force` (ignore warnings) |
| `remove-mailalias <groupname> <MAIL> [...]` | Remove mail aliases from group | `--force` (ignore warnings) |

**Prev:** [User](02-user.md) · **Next:** [Permissions](04-user-permissions.md)
