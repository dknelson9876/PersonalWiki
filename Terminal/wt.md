# Windows Terminal

## Include SSH Profile

Add the following to `settings.json` inside the `list` property of `profiles`:

```json
{
    "name": "SSH Profile",
    "commandline": "ssh user@machine"
}
```

[Microsoft Documentation](https://learn.microsoft.com/en-us/windows/terminal/tutorials/ssh)