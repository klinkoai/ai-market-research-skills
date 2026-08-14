# Connect Klinko MCP to Claude Code

Klinko's market research capabilities run on an authenticated remote MCP server. This setup has been validated with Claude Code.

## Access

The production endpoint is:

```text
https://api.klinko.ai/mcp/
```

Store the Bearer API key in a local file and do not commit it to a repository:

```bash
chmod 600 ~/.klinko_mcp_key
export KLINKO_MCP_API_KEY="$(cat ~/.klinko_mcp_key)"
```

Regenerating a Klinko MCP key immediately revokes the previous key. Codex and Claude Code may share one key, but both clients must be updated after rotation.

## Configure Claude Code

Add Klinko as a user-level HTTP MCP server:

```bash
export KLINKO_MCP_API_KEY="$(cat ~/.klinko_mcp_key)"
claude mcp add --transport http --scope user klinko \
  https://api.klinko.ai/mcp/ \
  -H "Authorization: Bearer $KLINKO_MCP_API_KEY"
```

Use user scope because a project-level `.mcp.json` can be committed accidentally with the key in plain text.

## Verify

```bash
claude mcp list
```

A successful connection reports `klinko (HTTP) - Connected` and exposes:

- `match_submit`
- `match_get`
- `circle_knowledge`
- `persona_knowledge`

Start a new session or use `/mcp` to reconnect after changing the configuration.

## Rotate or remove access

```bash
claude mcp remove klinko
```

After key rotation, remove and add the server again with the new key.

## Security

- The user-level configuration stores the authorization header locally. Protect `~/.claude.json` with appropriate file permissions.
- Never add the key to project-level `.mcp.json`, `SKILL.md`, prompts, screenshots, logs, or Git history.
- Rotate the key immediately if it is exposed.
- Update every connected client after key rotation.
