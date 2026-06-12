# Skills

Reusable **skills** for writing and checking content for the WordPress open source project. Each one captures the WordPress.org brand voice, terminology, and editorial conventions so an AI agent can produce on-brand drafts for the project's marketing and communications work.

A *skill* is a self-contained capability an AI agent can load on demand. Each skill bundles everything it needs — its instructions, any brand reference material, and any helper scripts — in a single directory, so a skills-aware agent can discover it, decide when it applies, and run it.

These skills produce public-facing WordPress content. Treat anything they generate as a draft for human review before it is published under a contributor's name or posted to an official channel.

---

## What's here

| Skill | What it does |
|---|---|
| `wordpress-news-writing/` | Drafts posts for [WordPress.org/news](https://wordpress.org/news/) in the WordPress project voice, following the WordPress Marketing Style Guide and Brand Book (bundled in `references/`). The foundational writing skill the others build on. |
| `wordcamp-event-recap/` | Drafts a flagship WordCamp event recap for WordPress.org/news from real event notes and live event sources. Builds on `wordpress-news-writing`. |
| `wordpress-social-writer/` | Turns a single feed item (post title, URL, content) into ready-to-publish, per-platform social copy for X, Bluesky, Threads, Mastodon, Facebook, Instagram, LinkedIn, and Tumblr. |

Some skills build on another: `wordcamp-event-recap` follows the rules in `wordpress-news-writing`, so keep them together.

---

## How a skill is laid out

Each skill is a directory:

```
skill-name/
├── SKILL.md              Required. Frontmatter (name + description) and the instructions.
├── agents/openai.yaml    Interface metadata: display name, one-line summary, starter prompt.
├── references/           Optional. Bundled documents the skill reads at runtime.
└── scripts/              Optional. Helper scripts the skill can run.
```

The frontmatter `description` in `SKILL.md` is what a skills-aware runtime reads to decide *when* to trigger the skill, so it spells out the situations the skill is for. The body is the instruction set the agent follows.

---

## How to use them

**In a skills-aware agent (the intended path).** Point the agent at this directory, or install a skill into your agent platform. The agent loads each `SKILL.md`, matches the request against the `description`, and runs the skill that fits. `agents/openai.yaml` provides the display name and a `default_prompt` you can use to invoke a skill explicitly, for example:

> Use $wordpress-news-writing to draft a WordPress.org/news post in the WordPress project voice.

**By hand in any LLM client.** A skill is just Markdown. Open its `SKILL.md`, paste the body into your assistant of choice, attach anything it references (the bundled `references/` files, your event notes, the feed item), and supply the inputs it asks for.

Because these skills produce public WordPress content, always review and fact-check the output before publishing.

---

## Conventions

- **Keep skills self-contained.** Everything a skill needs at runtime travels with it: instructions in `SKILL.md`, reference docs under `references/`, helpers under `scripts/`. A skill should not depend on files outside its own directory.
- **Output is a draft.** Every skill here writes or assesses official WordPress content. A person reviews before anything ships.
