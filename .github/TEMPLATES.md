# Pull request template

[`pull_request_template.md`](pull_request_template.md) is the default PR description for every repo in the organization.

## Repo-level templates take precedence

A repo's own PR template overrides this one. GitHub uses the repo's template instead of the org default if the repo has either of these:

- A `pull_request_template.md` in its root, `docs/` or `.github/` folder
- A `PULL_REQUEST_TEMPLATE/` folder with multiple templates

To use the org template in a repo, delete the repo's own template. To customize it for one repo, copy `pull_request_template.md` into that repo and edit the copy.

Changes to the template apply only to PRs opened after the change. Existing PR descriptions stay as they are.

## Writing a PR

- **Title:** `[FEATURE|BUGFIX|CHORE] [PROJ-XXXX]: Short summary in plain English`, where `PROJ-XXXX` is the Jira ticket.
- **Jira:** replace `PROJ-XXXX` with the ticket, e.g. `PROJ-1234`. No ticket? Delete the line.
- **Sections:** fill in what helps the reviewer and delete what doesn't apply.

| Section | What goes in it |
| --- | --- |
| Summary | What the PR does and why, in one or two sentences. |
| Changes | The main changes as a short list, and anything that needs a close look. |
| Testing | How you checked it works: tests, manual steps, queries or dev runs, and the results. |
| Risks & out of scope | Known limits, what the PR leaves out, and follow-up tickets. |
| Checklist | Title format, testing, docs, and no secrets or customer data. |
