# Klinko MCP Authentication

Klinko MCP uses Bearer authentication. One active key can be shared by Codex and Claude Code for the same account.

## Store the key locally

```bash
chmod 600 ~/.klinko_mcp_qa_key
export KLINKO_MCP_API_KEY="$(cat ~/.klinko_mcp_qa_key)"
```

Never place the key in `SKILL.md`, source files, examples, screenshots, logs, prompts, or Git history.

## Request header

```http
Authorization: Bearer YOUR_KLINKO_MCP_API_KEY
```

## Key rotation

Creating a replacement key immediately revokes the previous key. After rotation:

1. Replace the local key file.
2. Restart Codex with the updated environment variable.
3. Remove and re-add the Klinko server in Claude Code.
4. Verify all connected clients before deleting any secure handoff record.

## Access scope

The current MCP endpoint and key flow are intended for authorized development and QA users. Contact [business@klinko.ai](mailto:business@klinko.ai) for access questions.
