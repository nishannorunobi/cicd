# cicd

The workspace's self-hosted DevOps platform: **Forgejo** (git hosting + pull-request
review) and, in later releases, its **Actions runner** (CI/CD) — all in Docker, offline
after the images are pulled once, nothing installed on the host.

Tracked in Plane (`myportfolio` workspace, project `CICD`), following the DEMO Scrum
template. Product goal, requirements, architecture and contract are Plane pages there.

| Release | Goal |
|---|---|
| v1 (v0.1.0) | Forgejo running in Docker, repos mirrored from GitHub, pull-request review |
| v2 | CI: runner + automatic checks (secrets, lint, tests) on every push |
| v3 | CD: release packages, offline release tests, tags, artifacts; logs to Grafana |

Sprint 0 (make the workspace ready) is in progress; the Docker environment and the
`start.sh` / `stop.sh` / `status.sh` entry points come next.
