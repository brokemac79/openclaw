# OpenClaw PR 100472 Mantis Web UI Chat Docker Proof

Commit: e63393cdddd8af2d82daf9c55c5f16eac7091ea7
Container: mcr.microsoft.com/playwright:v1.60.0-noble
Docker Engine: 29.5.2
Result: pass

This proof was generated from git archive HEAD of PR branch codex/mantis-web-ui-proof in a clean Linux Playwright container. It proves the candidate browser chat proof and evidence-builder path. It does not prove the maintainer-only GitHub workflow_dispatch registration or qa-live-shared Mantis publish-secret boundary; those still require maintainer-owned workflow execution.

Generated binary artifacts are not included here, but their SHA256 hashes are listed in hashes.sha256:

- web-ui-chat.png screenshot
- web-ui-chat.webm browser recording

Text artifacts in this gist:

- mantis-report.md
- mantis-evidence.json
- web-ui-chat-proof.json
- vitest.log.txt
- hashes.sha256
