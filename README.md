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

## Runbook

- **Re-run the workflow:** open the *Actions* tab, select the **CI build** workflow, pick the run you want, and use the **Re-run all jobs** button (or *Re-run failed jobs*). You can also re-run from a commit's checks view or the PR's *Checks* tab.
- **Where the build-log artifact shows up:** on a completed workflow run, open the run's summary page — the **Artifacts** section at the bottom lists `build-log`, downloadable as a ZIP containing `build.log`.
- **Ask Copilot to review a pull request:** on the PR page, use the **Reviewers** panel on the right and click the Copilot icon / select **Copilot** to request a review; Copilot then reads the diff and leaves feedback. (You can also mention @copilot in a comment on newer setups.)
