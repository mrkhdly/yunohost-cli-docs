# Global Options

Applies to all `yunohost` commands.

```
yunohost [-h] [--output-as {json,plain,none}] [--debug] [--quiet]
         [--version] [--timeout ==SUPPRESS==]
```

| Flag | Description |
|------|-------------|
| `-h, --help` | Show this help message and exit |
| `--output-as {json,plain,none}` | Output result in another format |
| `--debug` | Log and print debug messages |
| `--quiet` | Don't produce any output |
| `--version` | Display YunoHost packages versions (alias to `yunohost tools versions`) |
| `--timeout` | Seconds before timeout due to lock contention (default: no timeout) |
