# Audience Comparator

Use when the user already has two or more candidate audiences and must choose between them.

- **Inputs:** named audiences, offer, geography, decision constraints, and preferred criteria.
- **Run:** resolve each candidate to a `circle_id` from an existing match or a new `match_submit`; use equivalent `circle_knowledge` queries for every candidate.
- **Decide by:** demand, motivation, opportunity, reachability, competition, evidence quality, and risk.
- **Return:** comparison table, winner, trade-offs, disconfirming evidence, and next test.
- **Boundary:** use the same criteria and evidence depth for every candidate; do not manufacture precision with an unsupported score.
