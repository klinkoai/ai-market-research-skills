# Security Policy

## Report a security issue

Do not disclose suspected vulnerabilities, credentials, API keys, private endpoints, or customer information in a public issue.

Report security concerns privately to [business@klinko.ai](mailto:business@klinko.ai). Include a concise description, affected component, reproduction steps, and potential impact. Do not include live credentials.

## Credentials

- Never commit `KLINKO_API_KEY` to a repository.
- Store credentials in environment variables or an approved secret manager.
- Revoke and replace a key immediately if it is exposed.
- Do not paste credentials into prompts, screenshots, logs, examples, or issue reports.

## Public repository boundary

Klinko's public Skill repositories contain workflow instructions, integration documentation, and non-sensitive examples. Private data infrastructure, internal processing systems, service credentials, and server-side implementation are not part of the public repositories.

