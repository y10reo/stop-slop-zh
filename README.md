# stop-slop-zh

`stop-slop-zh` is a Codex skill for removing predictable AI writing patterns from Chinese prose while preserving meaning, facts, tone, and genre.

它不是把中文改得更口语，而是在不改事实、不乱降格的前提下，去掉中文 AI 写作里最常见的套话、八股结构、金句收尾和证据越界。

It is not a direct translation of English `stop-slop`. Chinese AI slop often shows up as essay-like structure, abstract subjects, slogan endings, nominalized verbs, false warmth, over-balanced phrasing, and evidence overclaiming.

## Quick Example

Before:

> 这一辉煌的众筹战绩成功验证了早期极客用户的买单意愿，并以极低的初期获客成本完成了品牌曝光。

After:

> FMB 先后在 Kickstarter 和 Indiegogo 众筹，合计获得 5,300 多名支持者和 56.6 万美元认购。这说明它在早期极客用户中有一定吸引力，也获得了初期曝光。它还不能证明大众市场需求、交付能力或主流渠道获客成本。

The rewrite keeps the useful data, removes marketing language, and stops the conclusion from outrunning the evidence.

## Use Cases

- Rewrite Chinese prose to sound less AI-generated.
- Review articles, reports, product copy, work messages, speeches, academic summaries, and official-style drafts.
- Tighten product, crowdfunding, and venture-analysis writing without overstating what the data proves.
- Preserve formal genre requirements when aggressive casual rewriting would be wrong.

## What It Catches

- 中文总分总八股：`首先 / 其次 / 综上所述`
- 排比三件套：`不仅是...更是...`、`是...是...更是...`
- 名词化动词：`进行优化`、`实现突破`、`提供保障`
- 抽象主语：`时代呼唤`、`科技赋能`、`市场选择`
- 金句收尾：`这就是...的力量`、`未来可期`
- 证据越界：众筹金额被写成市场验证，理论推演被写成最终证明

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
├── examples/
│   └── for-me-buds-due-diligence.md
└── references/
    ├── claim-boundaries.md
    ├── examples.md
    ├── phrases.md
    ├── scenarios.md
    └── structures.md
```

## Design Notes

The skill keeps the main instructions short and moves detailed phrase lists, genre guidance, examples, and evidence-boundary rules into `references/`. This follows progressive disclosure: load the core workflow first, then pull detailed references only when needed.

The included `examples/for-me-buds-due-diligence.md` comes from a real stress test on a Chinese venture-capital course report. The examples are excerpted and cleaned for demonstration.

The current version draws inspiration from:

- hardikpandya/stop-slop
- a Chinese adaptation of humanizer-style AI writing cleanup rules

## License

MIT
