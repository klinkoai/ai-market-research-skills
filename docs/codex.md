# Install Klinko Skills in Codex

Klinko Skills follow the open Agent Skills format. Each installable Skill is a directory containing a required `SKILL.md` file and optional references, assets, scripts, and `agents/openai.yaml` metadata.

## Availability

Individual Klinko Skill repositories are being prepared. Use the installation pattern below after a Skill repository is published.

## User installation

Install a Skill for use across repositories by copying its installable Skill directory into:

```text
$HOME/.agents/skills/<skill-name>/
```

## Repository installation

Install a Skill for everyone working in one repository by copying it into:

```text
<repository>/.agents/skills/<skill-name>/
```

## Invoke a Skill

In Codex CLI or the IDE extension, type `$` to mention the Skill or use `/skills` to browse available Skills. Codex can also select a Skill automatically when the request matches its description.

If a newly installed Skill does not appear, restart Codex.

## Authentication

Klinko Skills require `KLINKO_API_KEY` after the public API becomes available. See [Authentication](./authentication.md).

## Official reference

See OpenAI's [Build skills](https://learn.chatgpt.com/docs/build-skills) documentation.

