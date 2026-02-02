# GitHub Repo Starter

Generic repository starter providing CI and standard GitHub templates (issues, pull request
templates, CODE_OF_CONDUCT), plus common files such as README, LICENSE, and CONTRIBUTING.
Use this repository as a template to create consistently configured repositories across teams.

[![CI](https://img.shields.io/badge/ci-passing-brightgreen)](https://github.com/SamyRai/github-repo-starter/actions)
[![License](https://img.shields.io/badge/license-MIT-blue)](LICENSE)

## Create a repository from this template

- Web UI: open the template repo and click **Use this template** → **Create a new repository**.
- gh CLI example:

  ```bash
  gh repo create my-org/my-new-repo --template SamyRai/github-repo-starter --public --clone \
    --description "<repo description>" \
    --homepage "https://github.com/my-org/my-new-repo"
  ```

## Quick start

1. Clone: `git clone https://github.com/<owner>/<repo>.git`
2. **Replace placeholders**: Go to **Actions** → **Instantiate Template** → **Run workflow**
   and fill in your project details. The workflow will automatically replace all placeholders.
3. Install dependencies:
   - Node: `npm ci && npm test`
   - Python: `python -m venv .venv && source .venv/bin/activate && pip install -r requirements.txt`
4. Run tests: `npm test` or `pytest`
5. Follow the complete setup checklist in `SETUP.md`

See `TEMPLATE-VARS.md` for all available placeholders.

## What this repo contains

- Policy files: `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, `SECURITY.md`, `SUPPORT.md`

- Templates: issue and PR templates in `.github/` for consistent triage

- Automation examples: Dependabot and example CI workflows

## Maintainer status

This template is intended for general use. Replace contact emails, badges,
and placeholders with project-specific values when creating a new project
from this template.

## Community

See the project policies for contribution and support guidance:

- [CONTRIBUTING.md](CONTRIBUTING.md)
- [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)
- [SECURITY.md](SECURITY.md)
- [SUPPORT.md](SUPPORT.md)

For questions, open an issue or use the repository Discussions tab if
enabled.
