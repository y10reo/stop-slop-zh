# stop-slop-zh

`stop-slop-zh` is a Codex skill for removing predictable AI writing patterns from Chinese prose while preserving meaning, facts, tone, and genre.

It is not a direct translation of English `stop-slop`. Chinese AI slop often shows up as essay-like structure, abstract subjects, slogan endings, nominalized verbs, false warmth, over-balanced phrasing, and evidence overclaiming.

## Use Cases

- Rewrite Chinese prose to sound less AI-generated.
- Review articles, reports, product copy, work messages, speeches, academic summaries, and official-style drafts.
- Tighten product, crowdfunding, and venture-analysis writing without overstating what the data proves.
- Preserve formal genre requirements when aggressive casual rewriting would be wrong.

## Install

Copy this folder into your Codex skills directory:

```powershell
Copy-Item -Recurse . "$env:USERPROFILE\.codex\skills\stop-slop-zh"
```

Then call it in Codex:

```text
Use $stop-slop-zh to rewrite this Chinese text.
```

## Structure

```text
stop-slop-zh/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── claim-boundaries.md
    ├── examples.md
    ├── phrases.md
    ├── scenarios.md
    └── structures.md
```

## Design Notes

The skill keeps the main instructions short and moves detailed phrase lists, genre guidance, examples, and evidence-boundary rules into `references/`. This follows progressive disclosure: load the core workflow first, then pull detailed references only when needed.

The current version draws inspiration from:

- hardikpandya/stop-slop
- a Chinese adaptation of humanizer-style AI writing cleanup rules

## License

MIT
