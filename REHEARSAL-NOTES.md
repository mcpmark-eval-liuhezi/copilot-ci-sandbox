# Rehearsal Notes — copilot-ci-sandbox

This sandbox records a full automated-release-checklist rehearsal loop:

1. **Repository** — `mcpmark-eval-liuhezi/copilot-ci-sandbox`, created with a README so it has a default branch.
2. **Issue** — "Set up CI checks": the repo has no CI yet and needs a workflow that runs on pushes and pull requests.
3. **Branch** — `add-ci-workflow`, carrying the workflow at `.github/workflows/ci.yml` plus this notes file.
4. **Workflow** — named "Sandbox CI", triggered on both `push` and `pull_request`, with a single job that echoes `sandbox-ci-marker` and then succeeds.
5. **Pull request** — `add-ci-workflow` → default branch, titled "Add Sandbox CI workflow", referencing the CI issue.
6. **Copilot** — assigned to the issue as its assignee, and asked to review the pull request.
7. **CI run** — the workflow run for the pull request, with its usage/billable figures and logs pulled afterward.
8. **Review comments** — read back from the pull request to see what Copilot (or anyone) said.
9. **Closure** — a summary comment left on the issue (PR number, run result, billable time), then the issue closed as completed. The pull request stays open.

## Purpose

The goal is to observe exactly how a ticket, a CI run, and the Copilot reviewer behave together, before pitching an automated release checklist to the team.
