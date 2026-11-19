# Event briefs and quick cards

Read the event, the user's current profile, and the confirmed attendee records. Tailor the plan to this event's goal, format, relationship stage, and time available. Every proposed personal bridge needs support from both sides: a sourced attendee finding and a user-provided background fact.

## Detailed person brief

Save a readable Markdown brief per confirmed attendee. Include:

1. **Identity and objective:** name, current role with verification status, identity anchor, event-specific reason to meet, and an achievable outcome.
2. **Useful background:** a short career summary, recent work or professional themes, relevant voluntarily shared interests, source links, and gaps.
3. **Personal bridges:** two or three real connections when available. For each, show the attendee evidence and the user's fact/story. Fewer genuine bridges are better than invented overlap.
4. **Three conversation starters:** natural spoken wording, why it fits, a follow-up question, and a transition to a relevant experience or another topic. Use a mix of event context, recent work, and genuine overlap as the evidence allows.
5. **Introduction and short story:** a tailored introduction in the user's tone and one relevant 20- to 40-second story from their experience. If no supported story exists, provide a truthful short introduction and ask for a useful example rather than fabricating one.
6. **Reciprocity and closing:** something the user could genuinely offer, an appropriate next-step request, and a graceful exit. Clearly distinguish a possible offer from a promise already made.
7. **Hypothetical practice simulation:** sourced background, observed communication tendencies with evidence and uncertainty, unknowns, and any fictional scenario conditions. Read the rehearsal reference when actually starting practice.
8. **Evidence and coverage:** usable source links and dates, user-background references, interpretations, last refresh, and access limitations. Keep uncertainty beside the affected advice rather than hiding it only in an appendix.

Use this compact format for topic recommendations:

```text
Topic: [specific, naturally discussable subject]
Say: [one conversational opener]
Why it fits: [attendee evidence] + [user evidence or goal]
Follow up: [open question that responds to their answer]
Bridge: [relevant true experience, or informed curiosity]
If it does not land: [gentle transition]
```

The three starters need not cover personal hobbies. When overlap is limited, ask about their work or experience in a way the user can honestly sustain. Reference the research at a natural level: a recent public talk is easier to bring up than an obscure old post.

Do not manufacture flattery or assume hiring, investment, referrals, friendship, or interest in the user. Scale requests to the relationship and event goal. Prepare a lower-pressure alternative if the other person seems busy.

## Quick cards

Save `quick-cards.md` as a compact event document, ordered by the user's priorities and the recommended approach order. Create two companion artifacts in the same event folder: a self-contained `event-brief.html` and a polished `event-brief.pdf`. The HTML should support navigation between attendee briefs and useful local interactions such as persistent suggested-action checkboxes; it must work when opened locally without a server or external assets. The PDF should have a clear, print-friendly attendee card for each person, styled with a person header, highlighted objective, conversation prompts, and follow-up/action area. Both companions must be based on the existing event, quick-card, person-brief, and contact Markdown records, preserve their identity caveats and provenance, and never claim a conversation occurred unless actual interaction notes say so. Do not edit Markdown files just to format or enrich a companion artifact. Render and inspect every PDF page and open the HTML locally to verify navigation and state persistence before delivery.

Keep the Markdown text and formatting unchanged when adding or regenerating these companions; if the user asks to change card content, update the Markdown deliberately and then regenerate affected companions from it.

Make each Markdown card easy to scan at a glance, following this hierarchy:

1. **Person header:** name, role/organization, and relevant event or relationship status. Include uncertainty where relevant.
2. **Objective of meeting:** one concise, tailored outcome in a visually distinct callout.
3. **Conversation opener (1 of N):** give 1–3 short, natural questions the user can ask this individual. Number them `1 of N`, etc., so the user can choose an idea. Prefer questions grounded in confirmed attendee information or event context; label a general curiosity question when identity or background is unresolved. Avoid presenting a multi-part interrogation as one question.
4. **Personal connection:** a real bridge grounded in the user's stated experience, or a clearly labeled curiosity angle when no connection is known.
5. **Useful next step:** one suitable, low-pressure action to take after the conversation.

Use clear section labels and whitespace so the visual structure reads like a compact meeting dashboard. Do not invent meeting history, action items, relationship details, or profile facts just to fill a section. Aim for roughly 100–150 words per confirmed-person card; sources and detailed reasoning belong in the linked person brief. Link each card to its saved brief and preserve unresolved identity warnings. Keep an unresolved attendee entry short, with the clarification needed, rather than a guessed conversation plan. The 1–3 conversation questions belong on every confirmed-person card; unresolved entries can only use neutral event-context questions if clearly marked as generic.

## Event overview and refresh

In `event.md`, retain the event goal, prioritized approach order with reasons, and the coverage or preparation-time tradeoff. Include a short general introduction and a fallback opener for unexpected attendees when useful.

In chat, provide the approach order, the strongest few opportunities, material gaps, and absolute links to the quick cards and detailed briefs. Offer a concrete practice entry, such as `Practice the conversation with [confirmed name]`, without starting a simulation until requested.

On refresh, update the affected topic, role, persona evidence, and card together. State which earlier findings changed and which parts remain unverified. Previously saved versions are preparation artifacts, not proof that a meeting occurred.
