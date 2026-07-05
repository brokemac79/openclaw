# Mantis Web UI Chat Proof

Status: pass
Candidate ref: codex/mantis-web-ui-proof
Candidate SHA: e63393cdddd8af2d82daf9c55c5f16eac7091ea7

## Scenario

OpenClaw Control UI chat was loaded in a browser with the mocked Gateway harness. The proof sends a chat message through the GUI, verifies the `chat.send` request, emits a final Gateway reply, and waits for the reply to render in the web chat thread.

## Artifacts

- Screenshot: `web-ui-chat.png` (present)
- Recording: `web-ui-chat.webm` (present)
- Proof metadata: `web-ui-chat-proof.json` (present)
- Vitest log: `vitest.log` (present)
