# Template variables

This file lists common placeholders used across the template repository and where they should be replaced.

- `{{PROJECT_NAME}}` — human-friendly name; example: "My Project".
  Appears in `README.md`, badges, and documentation.
- `{{REPO_NAME}}` — repository name; example: `my-project`. Used in repository URLs and CI examples.
- `{{OWNER}}` — GitHub organization or owner; example: `example-org`.
- `{{YEAR}}` — copyright year; example: `2026`.
- `{{MAINTAINER_EMAIL}}` — primary contact for maintainer or team; example: `maintainer@example.com`.
- `{{SUPPORT_EMAIL}}` — support contact for users; example: `support@example.com`.
- `{{SECURITY_EMAIL}}` — security contact for private vulnerability reports; example: `security@example.com`.
- `{{PGP_KEY_URL}}` — optional PGP key URL for secure reporting (used by `SECURITY.md` examples).
- `{{PGP_KEY_ID}}` — optional PGP key ID (short or long form) used in `SECURITY.md`.
- `{{GITHUB_USERNAME}}` — default GitHub handle or team for `CODEOWNERS`.
  Example: `my-org/maintainers` or `my-user`.
- `{{REPO_NAME}}` and `{{OWNER}}` can be used to form Discussion URLs, for example:
  `https://github.com/{{OWNER}}/{{REPO_NAME}}/discussions`.

How to replace placeholders

- **Recommended**: Use the **GitHub Actions workflow** (Actions → Instantiate Template →
  Run workflow) to automatically replace all placeholders with your project values.
- **Alternative**: Run `python3 scripts/instantiate_template.py` locally with appropriate flags.
- For small edits, update `CITATION.cff`, `README.md`, and `LICENSE` manually.
- Set repository-level Actions variables in Settings when a value should be
  be configurable at the repo level rather than baked into files.
