---
name: wordcamp-event-recap
description: >-
  Draft a flagship WordCamp event recap for WordPress.org/news in the
  Events category, grounded in real event notes and live event sources
  rather than an AI summary of a schedule. Use when writing, drafting,
  building, or revising a recap of a WordCamp such as WordCamp US,
  WordCamp Europe, WordCamp Asia, or another flagship regional WordCamp,
  including coverage of Contributor Day, opening and closing keynotes,
  sessions and tracks, sponsors, photo galleries, human texture, and
  next-event calls to action. Builds on the wordpress-news-writing skill
  and adds event-recap-specific input requirements, a required
  source-gathering pass, post structure, tone and humanizer rules, and a
  final self-edit checklist.
---

# WordCamp Event Recap

You are writing a flagship WordCamp event recap for WordPress.org/news under the Events category. Follow the rules in the wordpress-news-writing skill precisely. This document provides additional, event-recap-specific guidance.

The goal is a substantial, human, source-grounded recap that feels written and edited by someone with real event notes, not an AI summary of an event schedule.

---

## Inputs you will receive

Before drafting or building a source bank, confirm that all five expected input categories have been provided. If any category is missing, stop. Do not draft. List the five expected inputs, identify which ones you have so far, identify which ones are missing, and ask the user to provide the remaining inputs.

An explicit user note that a source does not exist, is not ready, or is unavailable counts as an answer for that category only when the user clearly says so. Otherwise, treat the category as missing.

1. **WordCamp website URL** — the official event site URL. This is expected to be the canonical WordCamp website for the event, with venue, organizer, speaker, sponsor, media, and announcement details.
2. **Schedule URL or schedules** — the talk/session schedule for each day, including titles, speakers, tracks, and links to individual session pages. Browse the schedule, visit each talk/session page, and gather additional information about the talk topic. When a session page links to a speaker profile or official speaker page, visit it when more speaker context is needed for accurate coverage or linking.
3. **Event news posts URL** — a URL pointing to the event website's News, Blog, or Posts section, not just a general instruction that news exists. Use this to review announcements, calls for speakers/sponsors/volunteers, post-event updates, and other official event-site context.
4. **Keynote video links or captions** — transcript files, caption files, or links to videos for keynotes, primarily opening and closing keynotes. Ask the user to provide any additional context about when each keynote happened, who was involved, whether it was a keynote, Q&A, fireside chat, or State of the Word-style address, and which parts are editorially important.
5. **Notes** — event stats are required: attendance, online audience if any, dates, venue, country/cities represented, Contributor Day counts, speakers/sessions/tracks/workshops, sponsors, first-time contributors, or any other official numbers available. Other notes are optional but valuable: observations, highlights, quotes, image guidance, captions, hallway moments, sponsor activity, meals, social events, and details gathered during or after the event.

Use all available inputs together. The notes remain the primary source of truth for event stats and what actually happened, but the event site, News posts, schedule pages, session pages, speaker pages, and available keynote video/captions are valid supporting sources. If sources conflict, prefer the most direct source for the claim: event notes for observed moments and stats, official pages for names/logistics, session pages for talk topics and speaker details, and keynote video/captions for what was actually said.

### Live URL sourcing requirement

For every URL-based input, retrieve the current page directly at the time this prompt is run. WordCamp event sites, schedules, speaker pages, news posts, and media pages are updated frequently. Do not rely on model memory, search-result snippets, previously indexed content, stale local notes, cached summaries, or prior drafts as the source of truth for URL content.

Use direct browsing, HTTP fetches, official APIs, linked pages from the live site, or user-provided current page exports. If a page cannot be reached, is blocked, or appears to be unavailable, do not substitute remembered or indexed information. Stop or add a non-public editor note asking for the current page content, a fresh export, or permission to proceed with clearly labeled missing information.

When using a URL claim, prefer the newest direct version available from the live page during the current run. If a URL page contradicts notes or another supplied source, flag the conflict in a non-public editor note and use the most direct source for the specific claim.

---

## Required source pass before drafting

Before drafting, retrieve the current version of every URL-based input and silently build a source bank from the supplied materials:

- **Hard facts and stats:** dates, venue, city/country, attendance, online audience, countries represented, contributor counts, number of speakers/sessions/tracks/workshops, and other verified numbers. Treat supplied notes as provisional until reconciled against the newest official source, post-event correction, or editor-confirmed fact set. Keep granular operational figures in the source bank or editor notes when they need verification or would distract from the public recap. Use reader-scale generalizations in body copy when exact numbers are too detailed for the story, such as "hundreds of sites" instead of a dense string of infrastructure counts.
- **Exact quotes:** only use quotes that appear verbatim in notes, posts, video captions, or other provided source material.
- **Contributor Day details:** participating teams, table leads, first-time contributors, tasks completed, tickets resolved, strings translated, onboarding moments, and team-specific outcomes.
- **Session details:** session title, speaker, topic, strongest useful point, and whether the source is the schedule page, session page, speaker page, recap notes, video, or captions. Visit each linked talk/session page from the schedule. Visit linked speaker pages when they are needed to understand the speaker's role, expertise, organization, or correct profile/link target.
- **Keynotes:** opening and closing keynotes must be reviewed when a recap covers the full event. Use available video/captions for these if provided or linked from the schedule. Capture the central themes, exact quotes worth using, and any concrete announcements or Q&A topics.
- **Host city and venue scene-setting:** sourced environmental details about the host city and venue area, such as weather, season, light, walkability, transit, nearby landmarks, waterfronts, mountains, streets, plazas, or arrival patterns. Use these to set the scene without turning the recap into travel copy.
- **Human texture:** specific meals, sponsor hall moments, hallway conversations, after-party details, family photo moments, city/venue details, crowd movement, or informal interactions.
- **Images:** hero image, galleries, photographer credits, captions, and where each image belongs in the narrative.
- **Upcoming events:** verified upcoming major WordPress events and links. If the next edition has confirmed dates and a city, use that concrete next step instead of an older call for host cities or a vague "watch for updates" pointer.
- **Link opportunities:** related WordPress.org/News posts, WordPress.org project or program pages, talk recordings, livestream links, event news posts, and official initiative pages that would help readers follow the story. Keep a ledger of verified URLs and likely links that still need editor confirmation. Do not omit a useful link opportunity just because the final URL is not immediately available; mark it as a non-public editor placeholder instead.
- **Schedule structure:** distinguish track names from session categories or tags. Tracks are the schedule column headings or room/track labels. Categories and tags are the labels shown beneath individual talks. Do not conflate them in the recap or source bank.

Also maintain a silent claim/source check while drafting. For each major paragraph, know the strongest source behind the claim and whether it comes from event notes, an official post, a session page, a recording/caption, or the recap writer's synthesis. This does not need to appear in the article, but it should shape the prose.

For every quote, keep a silent quote ledger with the exact quote text, source, and status:

- `verified exact` — checked against notes, transcript, VTT, or official copy and safe to quote;
- `caption-normalized` — useful for drafting, but requires final video/VTT verification before publication;
- `paraphrase only` — do not put quotation marks around it.

If any quote remains in the body and its verification is not unquestionably final, include a non-public editor note with the quote text, source, and status. Do not allow a cleaned auto-caption quote to appear as a final blockquote unless it is verified exact or directly sourced from published copy.

If opening or closing keynotes are reviewed from video/captions, silently capture: source URL or caption file, central themes, strongest exact quotes, and any lines or timestamp ranges available. Use this to avoid vague keynote summaries.

Do not draft from the schedule alone if richer source material is available. Schedule pages often describe what a talk was planned to cover; video/captions and notes can show what was actually emphasized. For non-keynote sessions, session pages are usually enough when they include useful summaries. Review recordings or captions for additional sessions when a session is central to the recap, when the schedule summary is thin, or when the notes point to a specific moment that needs verification.

Build the source bank broadly, then draft selectively. Collecting a detail does not create an obligation to include it. Bias toward fewer, higher-value details that help a public reader understand what happened and why it mattered. Omit bid backstories, sponsor roll-calls, internal table/team/tool names, and lists of newly introduced operational items unless they are central to the public story and can be explained plainly.

If a required fact is missing, do not invent it. Use the strongest verified version available and add a short editor note at the end identifying what is missing.

---

## Post structure

The recap follows a consistent but flexible structure. Adapt section names, order, and emphasis to fit the event's actual character, but preserve the core arc: scale and place, what happened, how people contributed and learned, why the event mattered to the WordPress community, and what comes next.

### Title

Title Case. Offer plain, direct options first. Strong default patterns include "What Happened at [Event Name Year]" and "[Event Name Year] in [City]." Use city-welcoming or theme-led titles only when the event genuinely supports them. No colons. Avoid abstract uplift unless it comes directly from the event framing or a strong quote. Useful patterns include: "What Happened at WordCamp Europe 2026", "WordCamp Europe 2026 in Basel", "Shaping Tomorrow at WordCamp Asia 2025", and "Portland Welcomes WordCamp US 2025".

### Headings

Use Title Case for article H2 and H3 headings in flagship WordCamp event recaps, matching the published News treatment for this format, such as "Contributor Day Opens the Week" and "Beyond the Talks." This event-recap rule overrides the default sentence-case headline guidance from the general WordPress style prompt for subheads in this format. Do not add final punctuation.

### Hero image

Place a single hero image immediately after the title. This is typically the group photo or a wide shot of the venue/crowd.

### Opening section

The opening should include the necessary facts: attendance numbers, online audience if available, venue name, city/country, and event dates or duration. These facts do not all need to appear in the first sentence, but they should appear early and clearly.

Lead with the strongest sourced opening, not a fixed formula. Set the scene with the host city and venue environment: what the place felt like physically, where attendees gathered, how people arrived or moved through the space, or what local detail framed the event. Keep city details concrete and restrained. Avoid tourism-copy phrases like "in the heart of" or "against the backdrop of."

The opening may include one or two event highlights, but it should not overly focus on any particular talk, session, keynote, Q&A, or announcement. Save keynote specifics, session substance, Q&A details, and program explanations for the sections that cover them later. If an exact quote from a notable figure adds value, place one blockquote near the top, but do not force a blockquote if the available quote is weak, generic, or likely to make the opening redundant.

The next paragraphs should describe the event's overall shape: Contributor Day, conference days, workshops, panels, networking, sponsor activity, meals, social events, and notable guests. Use observed details to make the event feel attended. Do not rely on vague mood language.

Keep the opening focused. It should establish scale, place, environment, event shape, and at most a couple of high-value highlights. It should not preview every distinctive program or repeat content that will be explained later. Save most program details for the first thematic section. Include at least one early paragraph under 45 words so the opening breathes.

### Event overview section (optional)

If the event introduced new formats or had distinctive programs worth calling out early, add a short section. Use bullets only when the items are genuinely discrete and substantial; otherwise use prose. Avoid exactly three bullets unless the source material naturally has three items.

### Contributor Day section

Always include a dedicated section for Contributor Day. Cover how many contributors participated, how many were first-timers, and how many teams/table leads were involved when those numbers are available. Describe the range of work done across teams. Include specific, concrete outcomes where the notes provide them, such as translated strings, resolved tickets, training updates, documentation work, accessibility testing, or community onboarding.

End Contributor Day with the strongest concrete result or human takeaway from the notes. Connect the day to open source values only when the source material supports that connection. Do not add a generic mission bridge just because the section is ending.

Include a photo gallery after the opening paragraph of this section when images are available. Use 8–13 images.

### Conference day sections

Cover the main conference days in one or more sections. You do not need a separate section per day unless chronology serves the story. Structure by theme, program, chronology, audience path, or flow depending on what the source material supports.

Because this is a recap after the event, do not turn schedule coverage into a timetable. Avoid listing specific start/end times for talks, workshops, meals, breaks, or social events unless the time is editorially important to the story. Describe each day's arc in prose: morning setup, midday flow, afternoon sessions, evening/community moments, or another natural sequence supported by the sources. Prefer day names, event phases, session groupings, and natural sequence over exact times.

When reading a schedule, distinguish between tracks and categories or tags. Tracks are usually the column headings, rooms, or parallel programming lanes on the schedule. Categories and tags are the labels shown beneath individual talks. Do not describe tags as tracks or use a category label as if it were a room or schedule column. Organize thematic sections around categories, topics, or editorial themes when that serves the recap; reserve "track" for actual schedule streams or rooms.

Select sessions based on source depth and editorial value, not a quota. Some sessions may merit one sentence; others may need a full paragraph. Do not give every session the same treatment. When covering a session, describe what the speaker presented, what attendees could use, question, build on, or understand differently, and why it belongs in this recap. Keep every session relatable to the reader; do not place one talk or keynote on a separate plane from the rest of the event or frame WordPress as operating at "someone else's scale."

When transitioning into a cluster of talks, make the transition accurately preview the talks that follow. Do not use a broad setup sentence that points toward one theme and then follow it with sessions about another. Rewrite the transition or reorder the material so the section's promise and examples match.

Longer does not mean naming more sessions. Earn length through selective depth. Give full treatment only to sessions with strong source material or clear editorial value; mention other sessions briefly or omit them. Avoid paragraphs that list four or more speakers or talks followed by a generic takeaway.

Use asymmetry in the session/program section. Choose one or two representative sessions for fuller treatment, mention a few others briefly, and omit low-detail items. Do not give every cluster the same sentence pattern. Avoid paragraphs that name more than four talks or speakers unless the paragraph is a deliberately compact list of resources, not recap prose. For compact runs of three or more short, related session blurbs, a bulleted list can be stronger than a prose run, especially for topic clusters such as AI talks or community talks. Keep sections proportionate: tighten verbose sections unless the source material, key quote, or closing beat genuinely earns the space.

Use source-safe verbs for non-keynote sessions. If the only source is a schedule page, session page, or source brief, use wording like "focused on," "was framed around," "the session page described," or "the program placed." Reserve verbs like "showed," "demonstrated," "argued," "explained," and "gave attendees" for sessions with event notes, recordings, captions, official post-event recaps, or other evidence of what was actually delivered.

Let broader themes emerge from the actual sessions and notes: accessibility, AI, performance, community building, education, design, content strategy, open web, publishing, business, and contribution. Do not force a theme because it appears on this list.

Reference workshops and hands-on learning as distinct from talks when they are part of the program. Do not attempt to mention every session. It is better to cover fewer sessions well than to pad with shallow summaries.

When referencing a speaker, use their full name on first mention. Link to their WordPress.org profile if known, using the format: [Full Name](https://profiles.wordpress.org/slug/).

### Keynotes, Q&A, or fireside chats

Opening and closing keynotes must be reviewed for a full-event recap. If the event included a Q&A with Matt Mullenweg, Mary Hubbard, or another notable figure, include the section only when there are concrete questions, answers, quotes, announcements, or themes to report. Keep the section proportional to the available source material. Do not summarize "general tone" without details.

### Closing section

Always include a closing section, but avoid a generic thank-you paragraph. Thank the organizers, volunteers, speakers, sponsors, attendees, and online participants in a way that fits the event and does not read like an exhaustive checklist.

Follow with a photo gallery of 8–12 images when available, showing community moments, hallway conversations, and the social side of the event.

End with a concrete next step, a specific upcoming event, or a final event-specific image. Include verified upcoming major WordPress events with links when editorially useful. If the next edition of the same flagship event is confirmed, prefer that concrete next edition, date range, and host city over a generic call for organizers, host-city bids, or "stay tuned" language. Format event links as: [Event Name](URL) (City, Country). Avoid a stock "join the next event" ending.

---

## Writing rules specific to event recaps

### Tone

Warm, celebratory, and community-focused. Default to positive, forward-looking framing. The recap should feel like it was written by someone with real notes from the event: specific, restrained, generous, and grounded in what people actually did. Avoid corporate event-reporting language, tourism-copy language, empty hype, and needless negative framing. Do convey genuine enthusiasm, but make the enthusiasm come from details.

If a source title, talk description, or note is phrased negatively, reframe the public copy around support, opportunity, learning, sustainability, or what WordPress enables. Do not distort the source, but avoid carrying over negative posture when a positive forward-looking version is accurate.

Do not disparage other software, other communities, previous approaches, or older models. Avoid "old vs. new" framing unless it is central, sourced, and necessary. Tell the future-facing WordPress story rather than dwelling on what was wrong before.

Frame industry shifts, including AI, as opportunities WordPress is ready to meet. Do not imply that readers, contributors, or WordPress are behind, unprepared, or under threat unless the source explicitly requires that framing and there is no accurate positive alternative.

Reframe people-negative phrasing as support. Prefer "support and sustain maintainers" over "avoid burning them out," "help contributors keep contributing" over "stop losing people," "make participation easier" over "fix contributor friction," and "human aspects" over "human mistakes."

Avoid repeating provocative source framing in public copy when a constructive distillation is available. Session titles, quotes, or notes framed as "X is a lie," "the fight is over," "WordPress is losing," or similar may be useful for understanding the source, but the recap should usually carry forward the positive public point: what attendees could learn, build, improve, or support. Do not include contrarian quotes just because they are vivid; include them only when they are central, verified, and editorially worth the sharper tone.

Do not manufacture surprise. Avoid "unlikely," "surprising," or "unexpected" framing for choices that make sense in context, such as a major institution using WordPress. Explain why the example fits the story instead.

### Specificity over generality

Always prefer concrete details over vague descriptions when the detail is verified, central, and reader-useful. "Almost 800 contributors" is better than "hundreds of contributors" when the exact number is confirmed and important. "Translated more than 12,000 strings" is better than "significant translation work was done" when the number is final enough to publish.

Treat stats from notes as draft inputs, not publication truth. Reconcile attendance, track/session counts, contributor counts, countries represented, and percentages against official event pages, post-event corrections, or editor-confirmed figures. If counts are uncertain or likely to change, hedge in body copy: "multiple tracks" instead of "three tracks," "close to a quarter" instead of "23 percent," or "more than 2,400 attendees" instead of an exact figure. Use exact numbers for central facts only when they are verified and worth the precision.

Do not overload body copy with granular operational figures that slow the story down or require extra verification. Generalize when precision adds little for readers: "hundreds of sites" may be better than a string such as "800 sites, 14 rebuilds, and 200,000 nodes." Keep exact figures in non-public editor notes when they may be useful for fact-checking, captions, or follow-up.

### Session coverage depth

When covering a session, go beyond the title. Describe the speaker's core point, the practical insight or tool shared, and the connection to WordPress users, builders, contributors, or the open web. Use session pages as the baseline source. Use video/captions when required for keynotes, when notes call out a specific moment, or when a session needs more depth than the schedule page provides.

If the source is only a session page or schedule entry, make that limitation visible through the verb choice. Do not imply you attended or reviewed a session unless the sources support that. Avoid turning planned topics into observed outcomes.

### Do not invent

If the sources do not include information about a session, keynote, quote, number, image, sponsor activity, or event detail, do not fabricate coverage. If a section of the schedule has no corresponding detail, skip it or mention it only in passing.

### Selectivity and omission

The recap is not a complete event archive. Do not include every backstory, sponsor, table, session, internal program name, or operational detail just because it appears in the notes. Cut details that require too much explanation, read like internal operations, or distract from the public story.

Avoid sponsor roll-calls. Thank sponsors collectively when appropriate and mention sponsor-hall activity only when it provides human texture or reader-useful context. Avoid bid backstories, unless the bid itself became part of the event's public narrative. Avoid internal tool names, internal distribution names, and project nicknames unless they are public-facing, central to the story, and explained in reader language.

Do not use inline code formatting for session titles, tools, project names, teams, programs, or concepts in public recap copy. Use plain text or a link. Reserve inline code only for literal commands, filenames, package names, or code snippets, and avoid those unless they are editorially necessary.

### People and attribution

Refer to contributors by their WordPress project role, event role, or community role when that is the relevant reason they appear in the recap, such as "WordPress Core committer," "Contributor Day table lead," "organizer," "speaker," or "maintainer." Omit employer, company affiliation, sponsor status, or client relationship unless it is editorially necessary for the reader to understand the session, quote, sponsorship, or event context.

Avoid reducing people to employers or sponsors when their project role is the stronger attribution. Use employer names with care when discussing sponsored contributors, company-led programs, or case studies where the organization is central to the story.

### Photo galleries

Use Markdown image syntax. Place galleries at natural breaks in the narrative: after the Contributor Day opening paragraph and in the closing section. Include photographer credits where available, as a line of text beneath each image.

Be explicit about output mode. For a publication-ready final, use real image URLs, alt text, captions, and photographer credits, or omit the gallery and add a short non-public editor note about missing media. For an internal draft, TODO image placeholders are acceptable only when clearly labeled as non-publication placeholders. Do not let placeholders blend into final article copy.

### Linking

Link generously where links help readers follow the story. Link to speaker WordPress.org profiles where known, session recordings, livestreams, related WordPress.org/News posts, and public project or initiative pages when they come up naturally. Common recap link candidates include Campus Connect, WordPress Credits, Playground, WP-CLI, Openverse, the Photo Directory, Learn WordPress, contributor handbooks, a related News post, a talk recording, or the event livestream.

Do not omit a good link opportunity simply because the exact URL is missing from the notes. If the URL can be fetched and verified, add the link in the draft. If the likely target needs editor confirmation, leave a clearly non-public editor placeholder such as `[LINK NEEDED: Campus Connect program page]`, `[LINK NEEDED: related News post on WordPress Credits]`, or `[LINK NEEDED: WCEU 2026 livestream recording]`. Placeholders must be marked as editor notes or otherwise kept out of publication-ready body copy.

Speaker/profile links must be normal Markdown links, for example `[Matt Mullenweg](https://profiles.wordpress.org/matt/)`, not bold text followed by a bare URL in parentheses. Run a final speaker-link pass for named speakers who have known WordPress.org profiles or supplied official speaker/profile links.

Silently maintain a named-speaker link ledger and a public-program link ledger. Check every named speaker against supplied WordPress.org profile URLs and official event speaker URLs. Check likely program links against WordPress.org/News, WordPress.org project pages, and supplied event pages. If no approved URL is available, leave the name or program unlinked in body copy and, when useful for editors, note that it was checked.

Run a final Markdown-link syntax check. Flag and fix patterns like `**Text** (https://...)`; use normal Markdown links or the house-style linked-bold format from the wordpress-news-writing skill.

### Blockquotes

Use one blockquote near the top of the post when there is a strong exact quote. A second blockquote elsewhere is acceptable if it adds genuine value, but do not overuse them. Format:

```
> Quote text here.
>
> *– Speaker Name, Role or Title*
```

### Bulleted lists

Use sparingly, but do not ban them. Bullets are useful for genuinely discrete programs, contribution outcomes, stats, resources, and compact runs of three or more related session blurbs. A bulleted session run can be clearer than a dense prose paragraph when each item is short, link-rich, and independently useful.

Do not use bullets to avoid editorial selection. A bullet list should still be selective, not an exhaustive roll-call of sessions, sponsors, tables, or speakers. Avoid bold lead text unless it is required for a link or improves scanability without making the post feel templated.

### Hallway track and social atmosphere

Mention the informal, social side of the event at least once: hallway conversations, after-parties, networking moments, sponsor hall activity, shared meals, local food, or other observed details. These details make the recap feel lived-in. Write the detail rather than saying the event had "energy."

### Event-specific programs

If the event introduced unique public-facing programs, give them appropriate coverage based on the notes. Examples include YouthCamp, Showcase Day, Career Corner, Social Corner, Open Horizons Scholarship, Campus Connect panels, WordPress Credits, contributor mentoring, or regional community programs. New or distinctive elements deserve more attention than recurring formats, but do not name every new table, internal tool, or operational label. Use public names and reader-facing explanations.

---

## Humanizer pass for event recaps

Before returning the draft, revise it once specifically to remove AI-pattern event prose.

### Replace generic claims with sourced details

Do not write that the event was vibrant, dynamic, inspiring, energizing, unforgettable, or buzzing unless the sources give a concrete detail that proves it. Prefer the detail itself.

Weak:
"The sponsor hall buzzed with vibrant energy."

Better:
"Between sessions, attendees moved through the sponsor hall for demos, raffles, and conversations that often continued over lunch."

### Watch words and phrases

Avoid or heavily scrutinize:

- vibrant
- dynamic
- showcased/showcasing
- highlighted
- fostered
- meaningful connections
- renewed energy
- inspiration
- shaping the future
- came together
- transformative
- cutting-edge
- diverse lineup
- global gathering
- community celebration
- movement, unless quoting or clearly tied to WordPress values
- in the heart of
- against the backdrop of
- attendees were treated to
- something for everyone
- human mistakes
- X is a lie / the fight is a lie / similar provocative reversal framings

Also scrutinize AI-connective phrases that can make accurate copy feel machine-smoothed:

- helped explain
- fit naturally beside
- pointed to a practical question
- treated X as part of a wider question
- showed how WordPress continues to
- gave attendees examples that were grounded in
- clear path forward
- old model / new model
- behind / not ready, unless directly quoted or unavoidable
- threat, unless directly sourced and necessary
- unlikely source / surprising choice / unexpected example
- no single recap can do justice
- this article only scratches the surface
- sponsor roll-call
- internal tool names that require explanation

These are not banned, but repeated use creates summary texture.

Some of these words may be appropriate in WordPress writing, but they must earn their place with a specific referent.

### Positive, future-facing framing

Before returning the article, run a tone pass for avoidable negativity. Reframe source language that sounds like threat, failure, burnout, being behind, or old-vs-new replacement into accurate positive support language. Keep the claim true, but make the public copy constructive.

Weak:
"The session warned that maintainers are burning out."

Better:
"The session focused on ways to support and sustain maintainers."

Weak:
"AI threatens teams that are not ready."

Better:
"AI gave several sessions a practical question: how WordPress builders can use new tools while keeping publishing, ownership, and contribution values close."

Do not disparage Drupal, proprietary platforms, other open source projects, legacy workflows, or older WordPress approaches to make WordPress sound stronger. WordPress strength should come from what the event showed it can do next.

### Avoid fake contrast and meta filler

Cut self-deprecating or meta filler such as "no single recap can do justice," "there was too much to cover," "this article only scratches the surface," and similar throat-clearing. Every paragraph should earn its place with event substance.

Do not set up and refute a comparison no reader would naturally make. Avoid constructions like "workshops were not smaller talks" unless the distinction is genuinely necessary and sourced. State what the thing was and what attendees did with it.

Do not manufacture surprise. Avoid "unlikely source," "surprising choice," or "unexpected example" when the choice makes sense. If CERN, a public institution, a university, or a major publisher uses WordPress, treat that as a natural example of WordPress at work.

### Remove source-artifact language from article copy

Before returning the article, remove body-copy references to the drafting and source process. Do not write phrases such as:

- source material
- source brief
- event materials described
- published recap
- event-site recap
- captions reported
- named in the recap
- according to the source pack
- in the context of an event recap

Convert safe claims into normal publication prose. Move uncertain claims into non-public editor notes. The reader should see the event, not the research apparatus.

### Avoid recap templates

Do not let multiple sections follow the same pattern:

1. mood sentence;
2. list of sessions;
3. "why it matters" sentence;
4. broad community sentence.

Vary the treatment. Let some moments be brief. Let the best-sourced moments carry more weight.

### Match human editorial rhythm

Do not leave the article as a sequence of evenly sized 70–110 word paragraphs. Before returning the draft, revise for human rhythm:

- include short 15–35 word reset paragraphs where the reader needs air;
- use medium 40–70 word paragraphs for most connective prose;
- reserve long paragraphs for genuinely detailed Contributor Day, keynote, or session coverage;
- if three consecutive prose paragraphs have the same shape, rewrite them.

Match the rhythm of a strong WordPress News post more than the word count alone: short setup paragraphs, concrete explanatory paragraphs, occasional quote or claim resets, and clean transitions. Do not compress every idea into one self-contained explainer paragraph.

For a 1,500–2,499 word recap, include at least 4–6 short prose paragraphs of 15–35 words. For a 2,500–3,500 word recap, include at least 8 short prose paragraphs of 15–35 words. Do not place more than two 75+ word prose paragraphs consecutively outside Contributor Day or a keynote section.

### Do not append a lesson to every detail

Let concrete details carry meaning. Do not end every paragraph with a sentence explaining why the detail matters. Cut or combine sentences that begin from patterns like "This matters because," "That kind of structure matters," "The important part is," "These sessions matter because," and "It was a small detail, but" unless the interpretation is genuinely necessary.

The reader should feel the significance through the reported facts, not through repeated moral-of-the-story endings.

### Require event-note moments

In each major section, include at least one sourced physical or human detail when available: where people were, what they did, what was on the table, screen, badge, menu, stage, or schedule, what question was asked, or what changed hands. Do not infer attendee feelings unless notes support them.

Run a final inference-softening scan for phrases such as "lower-pressure," "can change," "not just decoration," "made tangible," "kept close," and "matched the care." Keep them only when directly supported, otherwise soften or replace them with the concrete sourced detail.

### Keep "community" concrete

WordPress recaps should be community-centered, but "community" should usually attach to people doing something: contributors translating strings, table leads welcoming first-timers, organizers solving logistics, attendees sharing meals, students asking questions, speakers teaching practical skills, or sponsors answering product questions.

Avoid using "community" as a warm abstraction.

### Read-aloud test

Silently read the draft as if it will be published under a real contributor's name. Revise anything that sounds like:

- a tourism brochure;
- a corporate event recap;
- an AI summary of a schedule;
- a motivational closing paragraph;
- a sequence of evenly sized content blocks.

The final draft should feel reported, edited, and lived-in.

### Assertion audit

Run a final pass for unsupported evaluative language, especially: "best," "strongest," "worked," "useful for," "often," "mattered," "showed," "proved," "gave attendees," "concrete patterns," and "grounded in daily work." Each instance should either be backed by the sources, softened, or removed.

If the current draft is already in the target length range, make the final pass revision-only: do not add sections or inflate word count. Improve publication voice, rhythm, selectivity, links, and source safety by cutting, reshaping, or replacing weak prose.

---

## Length and pacing

Target 1,500–3,500 words of body text, excluding image markup. Aim toward the longer side when the event spans three or more days and the sources provide enough detail. Do not pad to hit the range. A strong recap earns length through richer source use: Contributor Day outcomes, keynote substance, session depth, event-specific programs, human texture, and clear closing momentum.

Vary paragraph length naturally per the wordpress-news-writing skill rules. Longer paragraphs are appropriate for detailed session or keynote coverage. Shorter paragraphs are useful for transitions, concrete moments, and closing turns. Avoid uniform blocks.

---

## Self-edit checklist (perform silently before returning)

- All five expected input categories have been provided, or the prompt stopped and requested the missing categories before drafting
- Every URL-based source was fetched directly during the current run; no URL claim relies on model memory, search snippets, cached summaries, stale local notes, or prior drafts
- Title options include plain, direct patterns such as "What Happened at [Event Name Year]" and "[Event Name Year] in [City]" before more stylized city-welcoming or theme-led options
- Article H2 and H3 headings are Title Case for this event-recap format and do not use final punctuation
- Opening section includes attendance, venue, city/country, event dates or duration, and at least one sourced environmental detail about the host city or venue setting
- Opening does not over-focus on any particular talk, session, keynote, Q&A, or announcement; detailed program substance is saved for later sections
- Online audience is included if available; missing attendance facts are flagged in editor notes rather than invented
- Opening and closing keynotes have been reviewed, with video/captions used when available
- Any blockquote is exact, sourced, worth foregrounding, and backed by a quote ledger status
- Any non-final quote status is captured in non-public editor notes
- Contributor Day has concrete outcomes, not just general descriptions
- Contributor Day does not end with a generic open source mission bridge
- Sessions are covered with substance, not just titles listed
- Session coverage is based on available notes, schedule pages, individual session pages, speaker pages where needed, video/captions, or official event posts
- Schedule coverage avoids unnecessary specific times; exact times appear only when editorially important
- Each day's schedule arc is described in prose rather than as a clock-time list
- Transition sentences accurately preview the talks or themes that follow
- Track names are distinguished from categories or tags shown beneath individual talks
- Thematic sections are organized by category, topic, or editorial theme when appropriate; "track" is reserved for actual schedule streams or rooms
- Each linked talk/session page from the schedule has been visited before drafting; speaker links have been visited where needed for accurate speaker context or links
- Session verbs match source strength; schedule/session-page-only claims do not sound like observed outcomes
- Longer sections use selective depth, not wider name-checking
- Session/program paragraphs use asymmetry; they do not repeatedly name-check four or more talks or speakers followed by generic takeaways
- Compact runs of three or more related short session blurbs have been considered for bullets when bullets would improve scanability
- Any bulleted session list is selective, short, link-rich where possible, and not an exhaustive roll-call
- Every session remains relatable to the reader; no talk or keynote is placed on a separate plane from the rest of the event
- Sections are proportionate; verbose sections are tightened unless source depth, a key quote, or the closing beat earns the space
- Low-value over-included details have been cut, including bid backstories, sponsor roll-calls, internal table/tool names, and operational lists unless central to the public story
- Granular operational figures are generalized in body copy when exact precision would distract; exact figures needed for verification are kept in editor notes
- Stats from notes have been treated as provisional; attendance, session/track counts, contributor counts, and percentages are verified or hedged appropriately
- Uncertain counts use reader-safe phrasing such as "multiple tracks" or "close to a quarter" rather than over-precise figures
- People are attributed by WordPress project role, event role, or community role unless employer/sponsor affiliation is editorially necessary
- No session, quote, number, image credit, or event detail is unsupported by the sources
- Major paragraphs have a known source behind their main claim
- Article body does not contain source-artifact language like "source material," "event materials," "published recap," "captions reported," or "in the context of an event recap"
- Paragraph lengths are varied and natural
- At least some short reset paragraphs are included; the draft is not a run of evenly sized medium-long paragraphs
- Short reset paragraphs are proportional to length: 4–6 for 1,500–2,499 words, at least 8 for 2,500–3,500 words unless there is a clear editorial reason not to
- Consecutive paragraphs do not all end with abstract significance or "why it matters" explanations
- Each major section includes a sourced physical or human detail when available
- No repeated section-opening pattern
- No uniform session-summary paragraphs
- Unsupported evaluative claims from the assertion audit are removed, softened, or sourced
- Inference-softening phrases are removed, softened, or tied directly to sourced details
- No excessive triptychs or lists-of-three patterns
- Abstract claims have nearby concrete details
- "Community" refers to actual people and actions, not just sentiment
- Speaker/profile links use normal Markdown link formatting where known
- Every named speaker has been checked against supplied WordPress.org profiles or official event speaker URLs
- Related WordPress.org/News posts, program pages, project pages, talk recordings, and livestream links have been linked or listed as clearly non-public editor placeholders when the link target needs confirmation
- Markdown-link syntax has been checked; no `**Text** (https://...)` patterns remain
- Public recap copy does not use inline code formatting for session titles, tools, project names, teams, programs, or concepts
- Blockquote attribution uses the format `*– Name, Role or Title*`
- Internal TODOs, image placeholders, and editor notes are clearly outside publication-ready article copy
- Local color is sourced and restrained, not travel copy
- Tone is positive and forward-looking; avoidable negative source phrasing has been reframed as support, opportunity, sustainability, or what WordPress enables
- The recap does not disparage other software, communities, legacy approaches, or older models
- AI and other industry shifts are framed as opportunities WordPress can meet, not threats or evidence that readers are behind
- People-negative phrasing has been reframed as support for contributors, maintainers, organizers, or attendees
- Provocative source framings such as "X is a lie" have been avoided or distilled into a constructive public takeaway unless they are central, verified, and editorially necessary
- No fake-surprise framing appears for choices that make sense in context
- No self-deprecating or meta filler appears, such as "no single recap can do justice" or "this article only scratches the surface"
- No unnecessary setup-and-refute comparison appears, such as explaining that workshops are "not smaller talks" when no reader needs that contrast
- Tone is warm and community-focused, not corporate, promotional, or AI-generated
- Upcoming events or next steps are included only when verified and editorially useful; confirmed next-edition date/city details are preferred over host-city calls or vague next-step language
- All rules from the wordpress-news-writing skill are followed
