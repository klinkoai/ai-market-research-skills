# Connect Klinko MCP to Codex

Klinko's market research capabilities run on an authenticated remote MCP server. This setup has been validated with Codex CLI and the Codex desktop app.

## Access

The current endpoint is for authorized development and QA access:

```text
https://mcp-dev.klinko.ai/mcp/
```

The server requires a Bearer API key. Store the key locally and never commit it to a repository.

```bash
chmod 600 ~/.klinko_mcp_qa_key
export KLINKO_MCP_API_KEY="$(cat ~/.klinko_mcp_qa_key)"
```

Regenerating a Klinko MCP key immediately revokes the previous key. Codex and Claude Code may share one key, but both clients must be updated after rotation.

## Configure Codex

Add the following configuration to `~/.codex/config.toml`:

```toml
[mcp_servers.klinko]
url = "https://mcp-dev.klinko.ai/mcp/"
bearer_token_env_var = "KLINKO_MCP_API_KEY"
```

Restart Codex after changing the configuration.

### Codex CLI

Export the key in the terminal that launches Codex:

```bash
export KLINKO_MCP_API_KEY="$(cat ~/.klinko_mcp_qa_key)"
codex
```

### Codex desktop app on macOS

The desktop app does not inherit variables from an existing terminal. Inject the variable before reopening the app:

```bash
launchctl setenv KLINKO_MCP_API_KEY "$(cat ~/.klinko_mcp_qa_key)"
```

Completely quit and reopen Codex. The injected value must be set again after restarting macOS.

## Verify

Ask Codex to list the connected Klinko MCP tools. A successful connection exposes:

- `match_submit`
- `match_get`
- `circle_knowledge`
- `persona_knowledge`

## Security

- Never place the API key in `SKILL.md`, prompts, screenshots, logs, or Git history.
- Keep the local key file at mode `600`.
- Rotate the key immediately if it is exposed.
- Update every connected client after key rotation.
