# User

```
yunohost user {list,create,delete,update,info,export,import,group,permission,ssh} ... [-h]
```

## User Actions

### `yunohost user list`

List users

| Option | Description |
|--------|-------------|
| `--fields {username,fullname,mail,mail-alias,mail-forward,mailbox-quota,groups,shell,home-path} [...]` | Fields to fetch |

### `yunohost user create <username>`

Create a new user

| Option | Description |
|--------|-------------|
| `-F, --fullname FULLNAME` | The full name of the user. e.g. 'Camille Dupont' |
| `-p, --password PASSWORD` | User password |
| `-d, --domain DOMAIN` | Domain for the email address |
| `-q, --mailbox-quota {SIZE\|0}` | Mailbox size quota |
| `-s, --loginShell LOGINSHELL` | The login shell used |

### `yunohost user delete <username>`

Delete a user

| Option | Description |
|--------|-------------|
| `--purge` | Purge user's home and mail directories |
| `--force` | Force user deletion |

### `yunohost user update <username>`

Update user information

| Option | Description |
|--------|-------------|
| `-F, --fullname FULLNAME` | The full name of the user |
| `-m, --mail MAIL` | New email address |
| `-p, --change-password [PASSWORD]` | New password to set |
| `--add-mailforward [MAIL ...]` | Mailforward addresses to add |
| `--remove-mailforward [MAIL ...]` | Mailforward addresses to remove |
| `--add-mailalias [MAIL ...]` | Mail aliases to add |
| `--remove-mailalias [MAIL ...]` | Mail aliases to remove |
| `-q, --mailbox-quota {SIZE\|0}` | Mailbox size quota |
| `-s, --loginShell LOGINSHELL` | The login shell used |

### `yunohost user info <username>`

Get user information. Username or email can be used.

### `yunohost user export`

Export users into CSV.

### `yunohost user import <csvfile>`

Import several users from CSV. Columns: `username, firstname, lastname, password, mail, mailbox-quota, mail-alias, mail-forward, groups`

| Option | Description |
|--------|-------------|
| `-u, --update` | Update existing users in the CSV (default: ignore) |
| `-d, --delete` | Delete users not in the CSV (default: keep) |

**Next:** [Groups](03-user-groups.md) · [Permissions](04-user-permissions.md) · [SSH](05-user-ssh.md)
