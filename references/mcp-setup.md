# Connect Klinko MCP

Use the validated production endpoint `https://api.klinko.ai/mcp/` with the user's own Klinko API key as a Bearer token. Keep the key outside the Skill and every project repository.

## Store the key

Have the user enter the key in their own terminal, save it in `~/.klinko_mcp_key`, and set permission `600`. Never ask them to paste it into chat. Regenerating a key revokes the previous key everywhere.

## Codex

Preserve existing settings and add this user-level configuration to `~/.codex/config.toml`:

```toml
[mcp_servers.klinko]
url = "https://api.klinko.ai/mcp/"
bearer_token_env_var = "KLINKO_MCP_API_KEY"
```

Export `KLINKO_MCP_API_KEY` in the terminal that launches Codex CLI. For the macOS desktop app, use `launchctl setenv KLINKO_MCP_API_KEY "$(cat "$HOME/.klinko_mcp_key")"`, then fully restart Codex.

## Claude Code

Add the server at user scope, not project scope:

```bash
export KLINKO_MCP_API_KEY="$(cat "$HOME/.klinko_mcp_key")"
claude mcp add --transport http --scope user klinko \
  https://api.klinko.ai/mcp/ \
  -H "Authorization: Bearer $KLINKO_MCP_API_KEY"
```

Restart the client and confirm that all four Klinko tools are listed without running billable calls. Never print the key while troubleshooting.
