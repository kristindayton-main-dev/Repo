# Tools

This repository contains small utilities and workflows used by kristindayton-main-dev.

Included files
- `rice_report.py` (example script to generate a RICE-prioritized issue report) — if present in repo root
- `.github/workflows/rice_report.yml` — scheduled GitHub Action to run the RICE report
- `requirements.txt` — Python dependencies

Getting started
1. Set up a Python environment (3.8+ recommended):

   python -m venv .venv
   source .venv/bin/activate
   pip install -r requirements.txt

2. If you have a personal access token, set it as an environment variable (recommended):

   export GITHUB_TOKEN="ghp_..."

3. Run the RICE report script (adjust path if needed):

   python rice_report.py --owner kristindayton-main-dev --repo Repo --token "$GITHUB_TOKEN" --top 20

If you want scheduled weekly reports, the workflow `.github/workflows/rice_report.yml` will run the script using the repository's GITHUB_TOKEN.

Contributing
- Please open issues or PRs with improvements. See CONTRIBUTING.md for guidelines.

License
- This repository is licensed under the MIT license (see LICENSE).