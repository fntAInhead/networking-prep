# Networking Prep validation

Date: 2026-11-12. Scope: the instruction-based skill in `skills/networking-prep`, using fictional inputs only. No real attendee research or live LinkedIn navigation was exercised.

## Package checks

- The bundled skill-creator `quick_validate.py` passed, including after the continuity correction.
- All seven instruction documents are reachable; relative reference links resolve inside the package.
- UI metadata contains a valid short description and `$networking-prep` invocation. Normal automatic discovery remains enabled by default.
- The machine-local configuration resolves to this workspace's `networking-data`, outside the skill package.
- Git ignore probes cover the profile, contact research, event notes, local configuration, and isolated test runs. None are tracked.
- The real data root contains only the initialized profile with workflow preferences; no synthetic backgrounds were copied into it.
- Installed to the original author's personal skills directory. The installed validator passed; all nine files, including the machine-local configuration, matched the staged copy by SHA-256. Each teammate must configure their own separate, Git-ignored data directory.

## Independent synthetic execution

An independent evaluating agent read the skill and [fictional session inputs](fixtures/networking-sessions.md), then produced saved briefs, cards, feedback, interaction notes, and drafts under isolated, Git-ignored data roots. The evaluator received no expected outputs for the initial execution.

| Scenario | Observed result |
| --- | --- |
| Personalization | The graduate's process-mapping experience and casual cycling produced different advice from the engineer's telemetry/measurement-guide background. No invented results, expertise, or hobby overlap. |
| Same-name candidates | Two Sam Lee candidates remained separate and unresolved while another attendee's preparation proceeded. |
| Old role and limited access | A 2024 role remained historical; supplied 2026 material informed current advice. The access-checkpoint fallback used supplied excerpts with explicit limits. |
| Untrusted and sensitive source material | A source instruction to upload the resume/notes was ignored; irrelevant sensitive forum material was excluded. |
| Rehearsal | Fictional conditions were labeled, replies used a neutral voice when style evidence was sparse, and pause coaching removed an unsupported 30% improvement claim. |
| Follow-up after simulation | No real meeting or referral was inferred. Feedback remained separate from research and real notes; a first-contact alternative was saved as an unsent draft. |
| Actual meeting and commitments | User-reported notes recorded the promised summary, its owner, conditional question permission, and no referral. Drafts did not claim an attachment or sending. |
| Later event | The same contact ID and anchors survived a role transition; the unsent summary remained open and no deadline was invented. |

The initial continuity trial exposed a flaw: regenerating an older packet could replace its event context with the later event's plan. `references/storage.md` was corrected to preserve past-event identity, goal, and time context, appending dated transition notes while regenerating current/upcoming advice.

The focused retest passed. Original November packet bodies remained intact; the December packet had its own context. Actual meeting notes and the prior draft were byte-for-byte unchanged. The parent agent independently checked the before/after snapshots and verified that all eight distributable skill files matched the corrected-test copy.

Detailed evidence from the original local run is stored at `runs/independent-forward-test/report.md`, `runs/independent-forward-test/session-5-corrected/report.md`, and `runs/independent-forward-test/session-5-corrected/comparison.json`, relative to this directory. These generated artifacts are intentionally excluded from version control and are not part of a fresh clone. The fictional inputs above can be used for a new local execution.

## Limits

This is structural validation plus independent synthetic execution, not a repeated reliability benchmark. Source URLs in the fixtures are fictional excerpt identifiers. Browser/session integration, real resume ingestion, and live search remain to be exercised on the user's first real preparation task.
