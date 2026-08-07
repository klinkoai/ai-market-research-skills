# Audience Finder

Use to decide which audience a product, service, or idea should investigate first.

- **Inputs:** offer, decision, geography, stage, adoption constraints, excluded audiences.
- **Run:** call `match_submit` with `scenario=product`; poll with `match_get`; use `circle_knowledge` only when the leading candidates need deeper evidence.
- **Decide by:** problem fit, demand, motivation, adoption context, reachability, and meaningful risk.
- **Return:** ranked audience shortlist, evidence, risk, and one validation test.
- **Boundary:** do not claim market size, willingness to pay, or causal impact unless returned evidence supports it.
