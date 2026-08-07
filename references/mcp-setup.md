# Connect Klinko MCP

Use the validated endpoint `https://mcp-dev.klinko.ai/mcp/` with the user's own Klinko API key as a Bearer token. Keep the key outside the Skill and every project repository.

## Store the key

Have the user enter the key in their own terminal, save it in `~/.klinko_mcp_qa_key`, and set permission `600`. Never ask them to paste it into chat. Regenerating a key revokes the previous key everywhere.

## Codex

Preserve existing settings and add this user-level configuration to `~/.codex/config.toml`:

```toml
[mcp_servers.klinko]
url = "https://mcp-dev.klinko.ai/mcp/"
bearer_token_env_var = "KLINKO_MCP_API_KEY"
```

Export `KLINKO_MCP_API_KEY` in the terminal that launches Codex CLI. For the macOS desktop app, use `launchctl setenv KLINKO_MCP_API_KEY "$(cat "$HOME/.klinko_mcp_qa_key")"`, then fully restart Codex.

## Claude Code

Add the server at user scope, not project scope:

```bash
export KLINKO_MCP_API_KEY="$(cat "$HOME/.klinko_mcp_qa_key")"
claude mcp add --transport http --scope user klinko \
  https://mcp-dev.klinko.ai/mcp/ \
  -H "Authorization: Bearer $KLINKO_MCP_API_KEY"
```

Restart the client and verify all four Klinko tools. Never print the key while troubleshooting.
