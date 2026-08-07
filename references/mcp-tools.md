# Klinko MCP tool contract

Use the authenticated MCP transport for every call. Never pass the API key as a tool argument.

## `match_submit`

Submit an asynchronous match with `scenario`, `language`, a concise English `user_text`, and a stable unique `request_id`. Save the returned `task_id`. A typical match costs about 100 credits and is limited to about 5 calls per minute and 50 per day for each key.

## `match_get`

Poll the exact `task_id` until `completed` or `failed`. Polling is free and limited to about 60 calls per minute. Do not resubmit a task that is still processing. A normal match may take one to three minutes.

Completed match payloads contain `result.matches`. Each match commonly includes `circle`, `circle_id`, evidence fields, and decision scores. Preserve the API order unless the response explicitly defines another ranking.

## `circle_knowledge`

Retrieve focused audience evidence with a `query` and preferably `circle_id`; otherwise pass the exact returned `circle` value as `circle_name`. A call costs about 10 credits and is limited to about 20 calls per minute and 300 per day for each key.

## `persona_knowledge`

Retrieve focused persona evidence with `persona_id`, `query`, and optional `circle_id`. A call costs about 10 credits and shares the evidence-retrieval limits.

## Evidence rules

- Preserve returned identifiers for traceability.
- Label interpretation as interpretation.
- Report contradictory or missing evidence.
- Never expose private datasets, internal prompts, collection methods, scoring implementation, or infrastructure.
