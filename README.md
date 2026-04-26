# lucasbrandao-cc-plugins

> Personal Claude Code plugin marketplace by Lucas Brandão.

This repository is a [Claude Code marketplace](https://docs.claude.com/en/docs/claude-code/plugins) — a thin index that points to one or more plugins maintained by me. The plugins themselves live in their own repositories.

## Installation

In a Claude Code session:

```
/plugin marketplace add lucasbrandao4770/lucasbrandao-cc-plugins
/plugin install <plugin-name>@lucasbrandao-cc-plugins
```

The first command needs to be run once per machine. Subsequent installs of any plugin from this marketplace skip it.

### Private plugins

Some plugins listed here live in private GitHub repositories. To install them, the local machine must already be authenticated against GitHub with read access to the source repo. The cleanest setup:

```bash
gh auth login
```

Claude Code uses the local `git` / `gh` credentials at install time — there is no auth field inside `marketplace.json`.

## Plugins

| Plugin | Description | Status | Source |
|---|---|---|---|
| `pptx-workflow` | Generate `.pptx` presentations from user templates via a multi-agent workflow that preserves branding. | private, `v0.2.0` | [`lucasbrandao4770/pptx-workflow`](https://github.com/lucasbrandao4770/pptx-workflow) |

## Updating

```
/plugin update <plugin-name>@lucasbrandao-cc-plugins
```

## Status

Personal use, private during pre-release. Not accepting external contributions. Some listed plugins may be flipped to public (and licensed) once they stabilize.

## License

This index has no implied license. Each plugin retains its own license — see the linked plugin repositories.
