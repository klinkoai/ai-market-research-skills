<img align="right" width="400" src="../assets/skills/audience-finder.webp" alt="Audience Finder market research visual">

# 🎯 Klinko Audience Finder

**Find and prioritize the audience segments most worth serving.**

[⬇️ Install Klinko Skills](https://github.com/klinkoai/ai-market-research-skills) · [🌐 Klinko](https://klinko.ai/en/) · [🚀 Start Market Research](https://home.klinko.ai)

<br clear="right">

## What is Klinko Audience Finder?

Klinko Audience Finder is an AI market research skill for identifying promising customer and community segments around a product, idea, category, or market. It turns a broad audience question into a prioritized shortlist, explains why each segment matters, and gives teams a clearer starting point for research, positioning, acquisition, and validation.

## What this skill helps you do

- Turn a broad market into specific audience segments
- Prioritize audiences by relevance, need, and practical opportunity
- Describe each segment's motivations, context, and likely demand
- Identify which audience deserves deeper validation first

## Questions you can ask

- “Who is the best target audience for my product?”
- “Which customer segments should we prioritize first?”
- “What audiences are most likely to need this solution?”
- “Find promising communities for a new B2B SaaS product.”

## What you receive

| Deliverable | Decision it supports |
|---|---|
| Prioritized audience list | Choose where to focus research and acquisition |
| Segment summaries | Understand who each audience is and why it matters |
| Needs and motivations | Shape product and messaging hypotheses |
| Opportunity signals | Decide which segments deserve validation |

## Example research process

1. Describe the product, idea, audience, or market you want to understand.
2. Add relevant public context such as geography, category, goals, or constraints.
3. Ask a clear decision question rather than requesting generic research.
4. Review the structured answer and use follow-up questions to refine the decision.

### Example prompt

> Find the most promising audiences for an AI meeting assistant built for remote teams in the United States. Prioritize segments that can adopt through self-serve onboarding.

### Example result structure

- A ranked shortlist of relevant audience segments
- Why each segment is a plausible fit
- The needs, motivations, and adoption context that matter
- Recommended next questions for validation

## How Audience Finder ranks a target audience

Audience Finder does not rank groups by online popularity alone. It treats audience selection as a market decision and compares candidates against evidence that can change what a team should do next.

| Decision criterion | What the skill examines | Why it matters |
|---|---|---|
| Problem fit | Whether the audience repeatedly encounters the problem the offer addresses | A visible community is not necessarily a relevant market |
| Demand and motivation | Observable needs, active solution-seeking, triggers, and desired outcomes | Interest is weaker than a reason to change behavior |
| Adoption context | Existing tools, workarounds, switching friction, and decision constraints | A good conceptual fit can still be hard to adopt |
| Reachability | Where the audience gathers, learns, compares, and asks for help | A segment must be practical to research and recruit |
| Evidence quality | Supporting signals, contradictory signals, and unresolved assumptions | The ranking should expose uncertainty, not hide it |

The result is a prioritized starting point. It answers “who deserves deeper validation first?” rather than declaring that one audience is permanently correct.

## Audience Finder compared with adjacent research

| Approach | Best used for | Key difference |
|---|---|---|
| Audience Finder | Choosing which broad audience to investigate first | Produces a ranked shortlist before detailed persona work |
| Customer Pain Point Analyst | Determining which recurring audience problem creates meaningful demand | Starts with problems rather than choosing the audience first |
| Market Opportunity Analyst | Comparing broader audience-problem-opportunity combinations | Ranks complete market directions rather than audience segments alone |
| Startup Idea Validator | Testing the riskiest assumptions behind one proposed offer | Starts with a defined idea and designs the next validation step |

## Evidence boundaries

Audience Finder uses public market signals to organize a decision. Public signals can reveal recurring language, needs, workarounds, communities, and alternatives, but they are not a representative census. The skill does not claim market size, willingness to pay, causal impact, or product-market fit unless available evidence directly supports the claim. Interviews, landing-page tests, commitments, and payment behavior remain necessary forms of validation.

## Audience Finder FAQ

### What information should I provide?

Provide the product or idea, geography, current stage, adoption constraints, excluded audiences, and the decision you need to make. A precise decision produces a more useful ranking than a general request for “target customers.”

### Can Audience Finder work before a product exists?

Yes. It can organize candidate audiences around a problem or proposed capability before launch. The output is a research priority and assumption map, not proof that the proposed offer will sell.

### Does the largest audience rank first?

No. Public discussion volume is not reliable market sizing. A smaller audience may rank higher when its need is more urgent, its context fits the offer, and it is easier to reach and validate.

### What should I do after receiving the shortlist?

Test the highest-impact uncertainty behind the leading candidate. That may mean interviewing people with a specific workaround, recruiting a small design-partner group, or testing whether the audience takes a costly action rather than merely expressing interest.

## Who this skill is for

- Founders
- Product marketers
- Growth teams
- Agencies

## Supported agent platforms

- [Codex](https://openai.com/codex/)
- [Claude Code](https://www.anthropic.com/claude-code)

## Install Klinko Skills

Copy this prompt into Codex or Claude Code:

```text
Install Klinko AI Market Research Skills from https://github.com/klinkoai/ai-market-research-skills. Preserve my existing Skills and MCP configuration, connect Klinko MCP with my own API key, verify the four Klinko tools, and report which research skills are available.
```

The installable package, MCP setup, and secure API key instructions live in the [main Klinko Skill repository](https://github.com/klinkoai/ai-market-research-skills).

## Klinko access

This skill uses the authenticated Klinko MCP runtime and returns decision-ready results in an agent-friendly format. Each user connects with their own Klinko API key. One active key works across Klinko market research skills in both validated clients; rotating it revokes the old key everywhere.

## Related Klinko skills

- [Customer Pain Point Analyst](./workflow-customer-pain-point-analyst.md)
- [Market Opportunity Analyst](./workflow-market-opportunity-analyst.md)
- [Startup Idea Validator](./workflow-startup-idea-validator.md)

## Research and editorial standard

This documentation is maintained by [Klinko Research](https://klinko.ai/en/about/). Recommendations separate observed evidence, interpretation, uncertainty, and the next validation step. Read the public [research methodology](https://klinko.ai/en/research-methodology/) for source handling, limitations, and editorial standards.

## About Klinko

[Klinko](https://klinko.ai/en/) is an AI market research tool and Audience Decision Engine for target audience analysis, customer research, market opportunity discovery, validation, positioning, and content strategy. Explore the complete [Klinko AI Market Research Skills](https://github.com/klinkoai/ai-market-research-skills).

---

Maintained by [Klinko](https://github.com/klinkoai) · Contact [business@klinko.ai](mailto:business@klinko.ai) · Last updated August 9, 2026
