# OpenClaw PR 100472 Mantis Web UI Chat Crabbox Proof

Commit: bd1f68ce0ddc11599afd85efd65f83d5c6229066
Provider: Crabbox local-container
Lease: cbx_61ddf3724d56
Image: mcr.microsoft.com/playwright:v1.60.0-noble
Docker Engine: 29.5.2
Result: pass

This proof was generated from the PR branch workspace in a Docker-backed Crabbox local-container run. It proves the current head's web UI chat parser regression, package artifact contract, browser chat proof, and evidence-builder path in Linux. It does not prove the maintainer-only GitHub workflow_dispatch registration, GitHub Actions artifact upload, or qa-live-shared Mantis publish-secret boundary; those still require maintainer-owned workflow execution or an explicit maintainer waiver.

Included artifacts:

- web-ui-chat.png screenshot
- web-ui-chat.webm browser recording
- mantis-report.md
- mantis-evidence.json
- web-ui-chat-proof.json
- vitest.log
- hashes.sha256

Crabbox commands/results covered:

- node scripts/run-vitest.mjs run --config test/vitest/vitest.tooling.config.ts test/scripts/mantis-web-ui-chat-proof-workflow.test.ts - passed, 1 test.
- node scripts/run-vitest.mjs run --config test/vitest/vitest.tooling.config.ts test/scripts/package-acceptance-workflow.test.ts -t "requires live proof evidence artifacts when proof jobs run" - passed, 1 selected test.
- node scripts/ensure-playwright-chromium.mjs - passed.
- OPENCLAW_MANTIS_WEB_UI_CHAT_OUTPUT_DIR=/tmp/mantis-web-ui-chat-proof node scripts/run-vitest.mjs run --config test/vitest/vitest.ui-e2e.config.ts --configLoader runner ui/src/e2e/mantis-chat-proof.e2e.test.ts - passed, 1 test.
- node scripts/mantis/build-web-ui-chat-evidence.mjs --output-dir /tmp/mantis-web-ui-chat-proof --candidate-ref codex/mantis-web-ui-proof --candidate-sha bd1f68ce0ddc11599afd85efd65f83d5c6229066 --status pass - passed.