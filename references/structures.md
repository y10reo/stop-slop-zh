# Structures

Chinese AI traces often live in structure rather than individual words. Fix structure before polishing words.

## Essay Skeleton

Avoid defaulting to:

```text
开篇定义/背景 -> 首先 -> 其次 -> 再次 -> 最后 -> 总结升华
```

Use one of these instead:

- Start with the actual claim.
- Start with a scene where the problem appears.
- Start with the surprising constraint.
- Start with the user's choice or tradeoff.
- Tell one story in time order.
- Explain one point deeply instead of listing three shallow points.

## Three-Part Balance

Patterns:

- 是...，是...，更是...
- 不仅是...，更是...
- 既要...，又要...，还要...
- 从...到...，从...到...
- 让...更...，让...更...，让...更...
- A、B、C 三个 nouns stacked to sound complete

Fix:

- Keep the one point that carries meaning.
- Split genuinely different claims into separate sentences.
- Use two items when both matter.
- Replace a list with one example.

Example:

> AI 不仅是工具，更是伙伴，更是未来生产力的入口。

Rewrite:

> 团队把 AI 当工具用：写测试、查日志、整理客服问题。

## Negative Contrast

Patterns:

- 不是 X，而是 Y
- 不只是 X，更是 Y
- 问题不在于 X，而在于 Y
- 真正重要的不是 X，而是 Y

Fix by stating Y directly unless the contrast carries real information.

## Abstract Subject Agency

Patterns:

- 时代呼唤...
- 科技改变...
- AI 赋能...
- 市场奖励...
- 行业推动...
- 数据告诉我们...
- 现实要求...

Fix:

- Name who acts.
- If the actor is unknowable, name the process.
- If the process is also vague, cut the sentence.

Example:

> 市场正在奖励更高效的团队。

Rewrite:

> 买家把预算给了能在两周内上线试点的团队。

## Nominalized Action Chains

Patterns:

- 对...进行...
- 为...提供...
- 通过...实现...
- 围绕...开展...
- 持续推进...建设
- 进一步加强...能力

Fix by finding the verb and object.

Example:

> 我们将围绕用户反馈开展产品体验优化工作。

Rewrite:

> 本周先改两个问题：登录慢，导出表格容易失败。

## Generic Meaning Inflation

Patterns:

- 标志着...
- 象征着...
- 体现了...
- 彰显了...
- 凸显了...
- 为...奠定基础
- 对...具有重要意义

Fix:

- If the sentence does not add factual information, delete it.
- If it has a real implication, name the implication.

## Evidence Leap

Patterns:

- Crowdfunding backers -> "market demand proven"
- Market-size report -> "this startup will grow"
- Product page promise -> "feature works"
- Theoretical model -> "final proof"
- Legal clause -> "risk eliminated"
- Media coverage -> "industry recognition"

Fix:

- State the evidence first.
- Name the narrow inference.
- Add the missing uncertainty if the original claim crosses the evidence boundary.

Example:

> 众筹 48.2 万美元成功验证了市场真实需求。

Rewrite:

> 众筹 48.2 万美元说明，早期支持者愿意提前付费。大众渠道转化、交付能力和留存还要单独验证。

## Vague Range

Patterns:

- 从个人到社会
- 从线上到线下
- 从认知到行动
- 覆盖工作、生活、学习的方方面面

Fix:

- Name the actual range.
- Use examples only when they are specific and relevant.

## Over-Formatted AI Output

Watch for:

- Every bullet starts with bold title + colon.
- Every section has "概念解释 -> 重要性 -> 做法 -> 小结".
- Emojis decorate headings.
- Tables are used to make thin ideas look structured.

Fix:

- Merge bullets into paragraphs when the items are not truly scan-worthy.
- Keep lists only for steps, options, requirements, or comparisons.
- Remove decorative emojis and mechanical bolding unless the user requested platform formatting.

## Repetition By Synonym

Chinese AI text often rotates synonyms to avoid repetition:

- 用户 / 消费者 / 受众 / 人群 / 客群
- 企业 / 组织 / 公司 / 平台 / 机构
- 问题 / 挑战 / 痛点 / 难题

Fix:

- Use one stable term when it refers to the same thing.
- Use different terms only when the distinction matters.

## Ending Patterns

Avoid ending every paragraph with a punchline, slogan, or value elevation. Let some paragraphs end on facts, examples, or a plain consequence.

Weak:

> 这就是长期主义的价值。

Better:

> 三个月后，续费率从 62% 回到 74%。
