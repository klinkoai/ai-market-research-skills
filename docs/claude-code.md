# Install Klinko Skills in Claude Code

Klinko Skills follow the Agent Skills open standard. Claude Code discovers a Skill from its directory and required `SKILL.md` file.

## Availability

Individual Klinko Skill repositories are being prepared. Use the installation pattern below after a Skill repository is published.

## Personal installation

Install a Skill for use across projects by copying its installable Skill directory into:

```text
$HOME/.claude/skills/<skill-name>/
```

## Project installation

Install a Skill for one project by copying it into:

```text
<project>/.claude/skills/<skill-name>/
```

## Invoke a Skill

Invoke a Skill directly with:

```text
/<skill-name>
```

Claude Code can also load a Skill automatically when the request matches its description. If a top-level skills directory is created after Claude Code starts and is not detected, restart Claude Code.

## Authentication

Klinko Skills require `KLINKO_API_KEY` after the public API becomes available. See [Authentication](./authentication.md).

## Official reference

See Anthropic's [Extend Claude with skills](https://code.claude.com/docs/en/slash-commands) documentation.

