# Community Coordination V1 — operational policy

**Founder approval:** Speedlink3 AI Technologies · 2026-11-19  
**Policy coverage:** All public MIT-licensed repositories in `ChatGPT-GURU-Speedlink3-AI` must follow the same community governance when onboarded. **ALL private repositories are categorically excluded, without exception.**
**Current technical deployment:** The V1 workflow presently runs only for Issues in the public `ChatGPT-GURU-Speedlink3-AI/.github` governance repository; coverage of other public MIT repositories requires a separate reviewed per-repository workflow configuration. See [GOV-REPO-PRIVACY-001](REPOSITORY-PRIVACY-SCOPE.md).

This system is **coordination-only, not autonomous code development**. The workflow may update public Issue metadata (labels and a single evidence checklist comment) with `contents: read` and `issues: write`. It does not checkout source, modify repositories, publish releases, touch production WordPress, access private repositories or call external AI APIs.

## Supported automatic activity

Newly opened or reopened Issues are classified and given an evidence reminder. An authenticated repository OWNER, MEMBER or COLLABORATOR can ask to triage an existing Issue by adding a comment beginning `/triage`. The workflow is designed to avoid duplicate bot comments and automatic feedback loops.

**The deployed workflow currently applies ONLY to Issues in this public .github repository.** The same CGS3 AI community policy is mandatory for eligible public MIT repositories after onboarding. All private repositories are permanently excluded from public community workflows.

## Voluntary community participation

People worldwide—including beginner developers, experienced engineers, testers, translators, security researchers and independent thinkers—are invited to contribute. [Open the volunteer issue form](https://github.com/ChatGPT-GURU-Speedlink3-AI/.github/issues/new?template=community-volunteer.yml). No unsolicited mass messaging, scraping of private contact details, or fake tool acknowledgments.

## Evidence and acknowledgments

States: `REQUESTED → SEEN → REVIEWED → IMPLEMENTED → TESTED → APPROVED`.

Only a genuine contributor action or inspectable execution record advances a status. Automated comments/labels mean REQUESTED, not SEEN. Tests require a source version, environment, command, result and exit code; otherwise they remain NOT_RUN.

## Security boundaries

- Public Issues must not contain credentials, SQL dumps, private account details or sensitive unpublished vulnerability information.
- Human approval is required for source modifications, merges, deployments, secrets handling and production writes.
- No AI worker receives automatic execution rights merely by appearing in an Issue.
- Security vulnerabilities requiring confidentiality must be handled privately, not in public Issues.

## First test

Founder-authorized Issue [EMERGENCY-HOOK-002 #1](https://github.com/ChatGPT-GURU-Speedlink3-AI/.github/issues/1) is the first intended test. After the workflow exists on the default branch, a repository member may comment `/triage` and inspect the actual GitHub Actions run and issue comment.

**Known technical limits:** Governance coverage for public MIT repositories is organization-wide, but automation must be separately configured within each eligible public repository; there is no automatic cross-repository dispatch. ALL private repositories are excluded. There is no AI agent dispatch, external email campaign, scheduled outreach, or cross-platform acknowledgments. These require additional reviewed integrations that must obey the global privacy policy.

Independent project founded by Speedlink3 AI Technologies; platform and AI-tool mentions do not imply affiliation or endorsement.

## First GitHub Actions execution evidence (2026-11-19, Asia/Dhaka)

| Test | Trigger / Issue | Result | Evidence |
|---|---|---|---|
| V1-T01 | Authorized `/triage` issue comment on EMERGENCY-HOOK-002 #1 | **PASS** — run completed; labels `community-review`, `urgent-review`, `needs-evidence` and one bot evidence reminder verified | [Run 44420424572](https://github.com/ChatGPT-GURU-Speedlink3-AI/.github/actions/runs/44420424572), [issue #1](https://github.com/ChatGPT-GURU-Speedlink3-AI/.github/issues/1) |
| V1-T02 | New public invitation issue #2 opened | **PASS** — run completed; labels `community-review`, `welcome-contributor` and one bot evidence reminder verified | [Run 44420514896](https://github.com/ChatGPT-GURU-Speedlink3-AI/.github/actions/runs/44420514896), [issue #2](https://github.com/ChatGPT-GURU-Speedlink3-AI/.github/issues/2) |

Evidence method: Real GitHub Actions run statuses and issue labels/comments fetched from the connected GitHub repository. These tests do **not** prove automatic notification to external AI products, execution of PHP/MySQL tests, or WordPress production safety.

