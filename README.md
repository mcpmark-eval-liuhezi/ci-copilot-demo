# ci-copilot-demo

A throwaway project for a live demo of **GitHub Actions + Copilot** at Thursday's lab meeting.

## What this repo contains

- A CI workflow at `.github/workflows/build.yml` that runs on every push.
- The workflow writes the line `demo build ok` to `build.log` and uploads it as a workflow artifact named `build-log`.
- A `feature/readme-tweak` branch with a README runbook, delivered via an open pull request with a Copilot review requested.

## Demo plan

1. Show the seed commit and the workflow file.
2. Watch the push-triggered workflow run finish and download the `build-log` artifact.
3. Walk through the open pull request and the requested Copilot review.
