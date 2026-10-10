# TWT QA release control

Proposed repository: `trainwithtariq/twt-qa-release-control` (public).

This repository is reserved for reviewed release-control code. The TWT application repository and application artifacts remain private. Application source, credentials, account identifiers, client data, screenshots and provider diagnostic output must not be committed here.

Initial contents are only this README and `.github/CODEOWNERS`. No workflow, schedule, deployment, credential or paid service is activated by this bootstrap.

Before any deployment credential is stored or used, independently verify effective protections on the default branch, require owner review for release-control changes, prevent bypass/force pushes/deletions, and verify the coding principal has no write or administrative access to this repository. A CODEOWNERS file alone does not enforce these rules.

Future release workflows require separate review. Candidate builds must run without deployment credentials. The trusted release stage must consume a pinned, verified artifact and independently controlled configuration; it must not run candidate scripts with credentials. It must reject stale candidates and unknown provider activity, permit only the approved isolated QA resources, serialize deployments, verify authenticated application health, and retain a compatible code rollback target.

There is currently no running release controller here. No TWT application deployment, unattended repair, production cutover, database recovery or spending authority is established by creating this repository.
