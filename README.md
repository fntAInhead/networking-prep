# Networking Prep

A reusable Codex skill for preparing for networking events, practicing conversations, and following through afterward.

It combines your supplied background and event goals with sourced attendee research to produce detailed briefs, quick reference cards, and hypothetical conversation rehearsals. It also keeps actual meeting notes and outstanding commitments, and drafts follow-up messages.

## Get started

Clone this private repository using your own GitHub account after the owner grants you access:

```powershell
git clone https://github.com/fntAInhead/networking-prep.git
cd networking-prep
```

In Codex, open the cloned folder and ask:

> Read and use the skill at `skills/networking-prep/SKILL.md` to prepare me for a networking event.

For a separate user profile, say `new user` (or start with `hello` / `what do you do`). The skill creates an isolated profile and asks for background, LinkedIn URL, and event details in separate prompts.

Later, say `share` or `share my info` to display a QR code for the active profile's LinkedIn page; it is shown locally and is not sent to anyone.

Provide your resume or a short background summary, the event details and goal, and attendee names. Employers, roles, and profile links help resolve ambiguous names. The skill asks for missing information and creates your local profile as needed.

For use across chats, ask Codex to install the `skills/networking-prep` folder in your personal skills directory. Configure `local-config.json` beside the installed `SKILL.md` with your own absolute local data directory, for example:

```json
{
  "data_root": "C:\\Projects\\networking-prep\\networking-data"
}
```

Replace the example path with your clone's `networking-data` directory or another local directory excluded from version control. The local configuration is machine-specific and is not included in this repository. When no configuration exists, the skill defaults to `networking-data` in the current project workspace. After installation, invoke it as `$networking-prep`.

## What to ask

- Prepare me for an event and prioritize whom to meet.
- Refresh a person's background and recent developments.
- Practice meeting someone, then give me feedback.
- Update my background, interests, or preferred introduction.
- Record what happened and what I promised after an event.
- Draft a follow-up based on my actual meeting notes.
- Draft brief thank-you emails to people I actually met; share what stood out and any genuine connection, or skip anyone I do not want to contact.

Research uses available web search and, when available, the computer-use skill for your existing logged-in LinkedIn session. Source access may require your own account or manual excerpts. LinkedIn prohibits third-party automation and profile views may be visible; the skill explains the limits and supports a supplied-material fallback. Rehearsal personas are explicitly hypothetical and do not establish a real person's private views or personality.

## Shared project and personal records

| Shared in Git | Kept local and ignored by Git |
| --- | --- |
| Skill instructions, UI metadata, and supporting references | `networking-data/`: resume summaries, profiles, contact research, event notes, and drafts |
| Fictional validation inputs and the validation summary | `skills/networking-prep/local-config.json`: your machine-local data path |
| This setup guide and `.gitignore` | `validation/runs/`: generated test artifacts |

Each teammate maintains their own profile, configuration, and event records. Do not force-add ignored files or paste personal records into shared issues or pull requests. Git exclusions do not provide encryption, and using the assistant or research tools involves their normal data processing.

## Contributing

Create a branch such as `codex/improve-event-intake`, make focused changes, and open a pull request. Keep changes in this repository's skill folder; a personal installed copy may need updating separately.

Use the [fictional sessions](validation/fixtures/networking-sessions.md) to check changes to identity resolution, personalization, research fallback, rehearsal boundaries, or event continuity. Run your installed skill-creator's `quick_validate.py` against `skills/networking-prep` for package validation. Store generated scenarios and test records under the ignored `validation/runs` folder.

See the [validation summary](validation/report.md) for checks already performed and their limitations. Live LinkedIn navigation and real resume ingestion have not been integration-tested in this project.
