---
name: klinko-market-research
description: "Run evidence-led market research with Klinko for audience finding, market opportunity analysis, startup idea validation, customer pain point analysis, positioning, content strategy, and related research decisions. Use when users need to decide who to serve, what market gap to pursue, what to validate, how to position an offer, what content to create, or how to turn public market signals into a ranked next action."
---

# Klinko Market Research

Route each market question to the focused research operation that best supports the decision over the authenticated Klinko MCP runtime.

## Preflight

1. Confirm that the `klinko` MCP connection exposes `match_submit`, `match_get`, `circle_knowledge`, and `persona_knowledge`.
2. If the tools are unavailable, stop before analysis and follow [references/mcp-setup.md](references/mcp-setup.md). Never ask the user to paste an API key into chat.
3. Read [references/mcp-tools.md](references/mcp-tools.md) before the first Klinko call in a session.
4. State approximate credit use before optional evidence calls. Treat an explicit request to run Klinko research as authorization for the required workflow calls.

## Route the request

Read only the workflow that matches the user's decision:

- Find or rank audiences: [Audience Finder](references/workflow-audience-finder.md)
- Discover overlooked niches: [Niche Audience Discovery](references/workflow-niche-audience-discovery.md)
- Compare named audiences: [Audience Comparator](references/workflow-audience-comparator.md)
- Rank market opportunities: [Market Opportunity Analyst](references/workflow-market-opportunity-analyst.md)
- Validate a startup idea: [Startup Idea Validator](references/workflow-startup-idea-validator.md)
- Identify likely first adopters: [Early Adopter Finder](references/workflow-early-adopter-finder.md)
- Build a buying-behavior persona: [Buyer Persona Builder](references/workflow-buyer-persona-builder.md)
- Analyze recurring unmet problems: [Customer Pain Point Analyst](references/workflow-customer-pain-point-analyst.md)
- Develop positioning and messaging: [Positioning Strategist](references/workflow-positioning-strategist.md)
- Prioritize content direction: [Content Strategy Builder](references/workflow-content-strategy-builder.md)
- Turn strategy into an execution brief: [Creative Brief Generator](references/workflow-creative-brief-generator.md)
- Analyze repeatable content mechanisms: [Viral Pattern Analyzer](references/workflow-viral-pattern-analyzer.md)

If a request spans multiple decisions, name the sequence and run only the first decision needed to unlock the next. Do not trigger several billable workflows when one answer is sufficient.

## Common execution rules

1. Collect or infer the minimum useful brief. Ask one concise question only when the product, audience, or decision is materially ambiguous.
2. Use a stable unique `request_id` for every new match and never resubmit while its `task_id` is processing.
3. Preserve Klinko's returned order unless the user supplies a different decision rule.
4. Use `circle_id` and `persona_id` from returned results for follow-up evidence.
5. Separate returned evidence, interpretation, uncertainty, and recommended tests.
6. Never invent support when a tool returns no evidence.

## Return the result

Answer in the user's language with:

1. **Decision** — the ranked answer and why it matters.
2. **Evidence** — the strongest supporting and contradictory signals.
3. **Uncertainty** — what the current evidence cannot establish.
4. **Next action** — one small validation step.
5. **Run details** — status, `task_id` when applicable, and approximate credit use; never expose credentials.

## Handle failures

- On `401` or `invalid_key`, stop and guide local key setup or rotation without requesting the key value.
- On `failed`, report the returned error and preserve the original `task_id`.
- On an extended processing state, keep polling before declaring failure.
- On insufficient evidence, narrow the question instead of filling gaps with general knowledge.
