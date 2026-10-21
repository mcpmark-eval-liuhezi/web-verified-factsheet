# web-verified-factsheet

A small showcase repo demonstrating a full "research, commit, run, clean up" loop.

## What this repo contains

- **`FACTS.md`** — a fact sheet with two web-researched facts: the current stable version of Node.js and the current stable version of Python. Each fact lists the version exactly as stated by its source, together with the URL of that source.
- **`.github/workflows/verify.yml`** — a GitHub Actions workflow that is triggered **manually only** (`workflow_dispatch`) and runs a single job that prints the contents of `FACTS.md`.

## How to start the workflow manually

1. Open the repository on GitHub and go to the **Actions** tab.
2. In the left sidebar, select the **Verify** workflow.
3. Click the **Run workflow** button.
4. Choose the `main` branch and click **Run workflow** again.

The run will appear in the workflow's history; it simply checks out the repo and prints `FACTS.md`.

## History note

The workflow was triggered once, and that run's **logs were deleted** afterwards, so the run remains visible in the Actions history with no stored logs behind it.
