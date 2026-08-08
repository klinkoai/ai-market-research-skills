# Klinko MCP Runtime Overview

Klinko's six core AI market research skills use an authenticated remote MCP runtime. Codex and Claude Code are the validated clients.

## Current development endpoint

```text
https://mcp-dev.klinko.ai/mcp/
```

Authentication uses `Authorization: Bearer <api_key>`.

## Tools

| Tool | Purpose | Typical cost | Key-level limit |
| --- | --- | ---: | --- |
| `match_submit` | Submit an asynchronous audience match | about 100 credits | 5/minute, 50/day |
| `match_get` | Read match status and results | free | 60/minute |
| `circle_knowledge` | Retrieve evidence for a circle | about 10 credits | 20/minute, 300/day |
| `persona_knowledge` | Retrieve evidence for a persona | about 10 credits | 20/minute, 300/day |

Matching usually takes one to three minutes. A workflow should retain the returned `task_id`, poll with `match_get`, and carry returned `circle_id` or `persona_id` values into later evidence requests.

## Skill layer

The MCP server provides the evidence and execution layer for Klinko AI market research skills. Each skill defines its required inputs, tool sequence, evidence boundaries, decision criteria, and output structure. A skill must never invent evidence when an MCP tool returns no support.

## Public boundary

Public documentation describes only the four MCP tools and the decision-ready results required by Codex and Claude Code. It does not expose private datasets, internal storage, collection methods, scoring implementation, prompts, or infrastructure.
