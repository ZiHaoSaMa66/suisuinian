记录一些会用得上的字段

```json
"hasCompletedOnboarding": true
```

```
settings.json
```

```json
{
  "env": {
    "ANTHROPIC_AUTH_TOKEN": "",
    "ANTHROPIC_BASE_URL": "",
    "ANTHROPIC_DEFAULT_SONNET_MODEL": "cc2",
    "ANTHROPIC_DEFAULT_OPUS_MODEL": "cc3",
    "ANTHROPIC_DEFAULT_HAIKU_MODEL": "cc1",
    "CLAUDE_CODE_AUTO_COMPACT_WINDOW": "270000"
  },
  "includeCoAuthoredBy": false
}
```

```bash
export IS_SANDBOX=1
claude --permission-mode bypassPermissions
```