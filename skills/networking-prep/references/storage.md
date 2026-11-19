# Local records

## Resolve the root

Read `local-config.json` beside `SKILL.md` when present. It contains one machine-specific setting, `data_root`, which must be an absolute local directory. This installation points to the user's workspace `networking-data` directory. It contains no resume or contact research and should be omitted when sharing the skill.

If configuration is absent, use `networking-data` inside the current meaningful project workspace and report that choice. If there is no meaningful workspace, ask for a local directory and work in chat meanwhile. If a configured directory is inaccessible or the config is invalid, report the problem and work in chat without silently creating another profile. Resolve explicit configuration changes before moving or copying records; do not migrate data automatically.

Before saving personal data under a Git worktree, ensure the root directory is excluded from version control. Use an exact directory ignore entry; if records are already tracked, explain that ignoring them does not untrack them and do not remove them from history. Do not commit, publish, or upload personal records. Do not move a configured root into the reusable skill package.

## Organization

Create records as needed, not a tree of empty documents:

```text
networking-data/
  profile.md                 # existing/default user
  assets/                     # generated LinkedIn QR image when requested
  contacts/
    index.md
    person-0001.md
  events/
    2026-11-12-event-slug/
      event.md
      quick-cards.md
      quick-cards.pdf           # visually styled companion to quick-cards.md
      event-brief.html          # standalone interactive attendee brief
      event-brief.pdf           # print-friendly companion attendee cards
      briefs/person-0001.md
      practice/person-0001-feedback.md
      interactions.md
      interactions.html         # visual companion derived from interactions.md
      follow-ups.md
  profiles/
    index.md
    profile-0001/
      profile.md              # separate user
      contacts/
      events/
      assets/                 # generated LinkedIn QR image when requested
```

Treat `networking-data/profile.md` and its top-level contacts/events as the existing default user's records. Never overwrite or repurpose them for a different user. For each new user, create a separate `profiles/profile-NNNN/` directory with its own `profile.md`, `contacts/`, `events/`, and `assets/`; keep a `profiles/index.md` mapping generated profile IDs to paths and creation dates. Assign the next sequential ID without using a name, username, email, or other personal detail in the path. Create a minimal profile stub marked `intake pending` that includes `LinkedIn profile URL: Not supplied`, set that profile as active for the current conversation, and keep all of that user's later event and contact records inside the same profile directory. If multiple profiles exist and the active user is unclear, ask which profile to use before reading or writing personal records. Treat `Not supplied` as missing information. Never populate a profile from the computer's username, file paths, or illustrative examples.

Use the following records:

| Record | Required meaning |
| --- | --- |
| `profile.md` | Explicit user facts/preferences, LinkedIn profile URL and provenance, experience levels, story bank, separate coaching suggestions, and last update date |
| `contacts/index.md` | Stable local ID, display name, confirmed identity anchor, known profile URLs, and record path; pending matches remain explicitly unresolved |
| Contact record | Confirmed identity and anchors, reusable sourced findings, communication observations, evidence gaps, last research date |
| `event.md` | Event context, goal, format, date/time zone if supplied, preparation constraints, attendee IDs or unresolved candidates, user priority, approach order with reasons, research coverage |
| Person brief | Event-specific objective, evidence-linked topics and personal bridges, introduction/story, contribution, next-step request, hypothetical persona |
| Practice feedback | Event/contact IDs, scenario, useful coaching and retry suggestions, explicitly labeled simulation; no full transcript unless requested |
| `interactions.md` | User-reported real interactions, date if known, what was discussed, promises with owners, next steps, and uncertainty |
| `follow-ups.md` | Drafts, their actual-note basis, outstanding commitments, and status; default status is `draft, not sent` |

Dates should use ISO format; preserve source publication dates and access dates separately. For notes without a supplied meeting date, record the capture date and mark the meeting date unknown. Use the user's time zone for event interpretation. Do not invent precise event times or due dates.

## Identity and safe filenames

Allocate stable IDs such as `person-0001` after checking the index. A confirmed profile URL or reliable name/employer/professional context anchors identity; a name alone does not. Reuse the same ID after an employer change. Preserve previous anchors and dated corrections. Do not merge lookalikes automatically.

Use an event date and a short slug, or `undated-event-slug` when unknown. Restrict generated filename components to lowercase ASCII letters, digits, and hyphens. Check whether a matching event exists before reusing a directory; otherwise use a numeric suffix. Do not turn attendee names, source content, or arbitrary user text into paths without normalization. Resolve every generated write path inside the configured root.

## Evidence and updates

Use compact evidence IDs within each record, for example `S1`, `U1`, `I1`, and `SIM1`:

- **Sourced (`S`)**: claim, URL, source title/type, publication date or `unknown`, access date, and limitations. A claim without an inspected supporting source stays unverified.
- **User-reported (`U`)**: claim plus the user's provided resume/file reference or dated statement. Keep prior-interaction reports distinct from web research.
- **Interpretation (`I`)**: tentative conclusion, supporting evidence IDs, and limits or alternatives. Never silently upgrade it to a fact.
- **Simulation (`SIM`)**: fictional scenario or generated response, confined to the persona/practice record. Never use it as evidence for S/U findings or actual interactions.

User-provided screenshots or excerpts can support a finding: identify the supplied artifact and coverage, preserve its visible URL/date if present, and say the underlying page was not independently reviewed. Do not fabricate a source URL.

Before updating, read the current record. Preserve unrelated notes and provenance. Prefer targeted edits; never replace a populated profile with an intake template. Keep changed roles, disputed claims, and corrections dated.

Distinguish a later role transition from a correction of an earlier false finding. Preserve past-event packets as dated preparation with their original event identity, goal, and time context. Append a dated correction or transition note and a link to a new packet when useful; do not replace the old plan with another event's plan or rewrite a historically accurate role as if it were wrong then. Regenerate affected current/upcoming cards and briefs, and list which saved events were refreshed. Leave actual meeting notes as reported.

Save a concise profile summary and references to supplied files by default; do not duplicate full resumes or unrelated contact information. Store only relevant research excerpts or summaries. Full source dumps, screenshots, and practice transcripts require a concrete user need. A user's explicit request to stop retaining records overrides the default: work in chat and clarify which existing records, if any, they want removed.
